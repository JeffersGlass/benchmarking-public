
# Results vs. 3.10.4

- fork: python
- ref: b905fad83819ec9102ec
- machine: darwin-arm64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.19x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 170 ms: 1.13x faster                                                   |
| chameleon      | 6.26 ms                                                | 4.89 ms: 1.28x faster                                                  |
| docutils       | 1.73 sec                                               | 1.45 sec: 1.19x faster                                                 |
| tornado_http   | 86.7 ms                                                | 67.7 ms: 1.28x faster                                                  |
| Geometric mean | (ref)                                                  | 1.22x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 249 ms: 1.56x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 325 ms: 1.46x faster                                                   |
| async_tree_io           | 980 ms                                                 | 694 ms: 1.41x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 517 ms: 1.26x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.42x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 75.0 ms: 1.24x faster                                                  |
| float          | 69.0 ms                                                | 56.4 ms: 1.22x faster                                                  |
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| Geometric mean | (ref)                                                  | 1.15x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 73.1 ms: 1.30x faster                                                  |
| regex_dna      | 174 ms                                                 | 151 ms: 1.15x faster                                                   |
| regex_v8       | 17.1 ms                                                | 17.1 ms: 1.00x faster                                                  |
| regex_effbot   | 2.46 ms                                                | 2.56 ms: 1.04x slower                                                  |
| Geometric mean | (ref)                                                  | 1.10x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 196 us: 1.43x faster                                                   |
| unpickle_pure_python | 194 us                                                 | 153 us: 1.27x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.49 ms: 1.25x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 39.6 ms: 1.17x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.54 sec: 1.11x faster                                                 |
| xml_etree_parse      | 108 ms                                                 | 105 ms: 1.02x faster                                                   |
| json_loads           | 16.4 us                                                | 16.9 us: 1.03x slower                                                  |
| pickle               | 6.97 us                                                | 7.23 us: 1.04x slower                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 75.5 ms: 1.05x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 56.1 ms: 1.05x slower                                                  |
| unpickle             | 8.80 us                                                | 9.23 us: 1.05x slower                                                  |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                  |
| pickle_list          | 2.74 us                                                | 2.97 us: 1.09x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.09 us: 1.15x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.0 ms: 1.20x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 11.6 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.33x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.59 ms: 1.30x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 70.8 us: 4.56x faster                                                  |
| deltablue                | 4.91 ms                                                | 2.43 ms: 2.02x faster                                                  |
| raytrace                 | 301 ms                                                 | 170 ms: 1.77x faster                                                   |
| logging_silent           | 117 ns                                                 | 70.1 ns: 1.67x faster                                                  |
| chaos                    | 65.8 ms                                                | 39.5 ms: 1.67x faster                                                  |
| sqlglot_parse            | 1.24 ms                                                | 793 us: 1.57x faster                                                   |
| async_tree_none          | 388 ms                                                 | 249 ms: 1.56x faster                                                   |
| richards_super           | 57.8 ms                                                | 37.4 ms: 1.54x faster                                                  |
| asyncio_tcp              | 659 ms                                                 | 435 ms: 1.52x faster                                                   |
| crypto_pyaes             | 71.8 ms                                                | 48.3 ms: 1.49x faster                                                  |
| sqlglot_transpile        | 1.44 ms                                                | 971 us: 1.48x faster                                                   |
| async_tree_memoization   | 474 ms                                                 | 325 ms: 1.46x faster                                                   |
| richards                 | 48.7 ms                                                | 33.5 ms: 1.45x faster                                                  |
| go                       | 151 ms                                                 | 105 ms: 1.44x faster                                                   |
| pickle_pure_python       | 281 us                                                 | 196 us: 1.43x faster                                                   |
| comprehensions           | 16.9 us                                                | 11.9 us: 1.42x faster                                                  |
| async_tree_io            | 980 ms                                                 | 694 ms: 1.41x faster                                                   |
| scimark_monte_carlo      | 65.6 ms                                                | 47.2 ms: 1.39x faster                                                  |
| hexiom                   | 6.19 ms                                                | 4.47 ms: 1.38x faster                                                  |
| scimark_lu               | 103 ms                                                 | 74.7 ms: 1.38x faster                                                  |
| unpack_sequence          | 39.0 ns                                                | 28.4 ns: 1.37x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 25.7 us: 1.35x faster                                                  |
| regex_compile            | 95.3 ms                                                | 73.1 ms: 1.30x faster                                                  |
| mako                     | 9.87 ms                                                | 7.59 ms: 1.30x faster                                                  |
| logging_simple           | 4.45 us                                                | 3.45 us: 1.29x faster                                                  |
| logging_format           | 4.83 us                                                | 3.75 us: 1.29x faster                                                  |
| tornado_http             | 86.7 ms                                                | 67.7 ms: 1.28x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.89 ms: 1.28x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 72.1 ms: 1.28x faster                                                  |
| pyflate                  | 427 ms                                                 | 334 ms: 1.28x faster                                                   |
| pycparser                | 877 ms                                                 | 691 ms: 1.27x faster                                                   |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.26 sec: 1.27x faster                                                 |
| spectral_norm            | 94.8 ms                                                | 74.7 ms: 1.27x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 153 us: 1.27x faster                                                   |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 517 ms: 1.26x faster                                                   |
| pprint_pformat           | 1.30 sec                                               | 1.04 sec: 1.25x faster                                                 |
| pprint_safe_repr         | 641 ms                                                 | 513 ms: 1.25x faster                                                   |
| json_dumps               | 8.11 ms                                                | 6.49 ms: 1.25x faster                                                  |
| nbody                    | 93.0 ms                                                | 75.0 ms: 1.24x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 10.7 ms: 1.23x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 701 us: 1.23x faster                                                   |
| float                    | 69.0 ms                                                | 56.4 ms: 1.22x faster                                                  |
| scimark_sor              | 128 ms                                                 | 105 ms: 1.22x faster                                                   |
| deepcopy                 | 272 us                                                 | 224 us: 1.21x faster                                                   |
| dulwich_log              | 35.3 ms                                                | 29.5 ms: 1.20x faster                                                  |
| sympy_str                | 165 ms                                                 | 139 ms: 1.19x faster                                                   |
| docutils                 | 1.73 sec                                               | 1.45 sec: 1.19x faster                                                 |
| mypy2                    | 607 ms                                                 | 511 ms: 1.19x faster                                                   |
| xml_etree_process        | 46.5 ms                                                | 39.6 ms: 1.17x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 2.00 us: 1.17x faster                                                  |
| regex_dna                | 174 ms                                                 | 151 ms: 1.15x faster                                                   |
| dask                     | 253 ms                                                 | 222 ms: 1.14x faster                                                   |
| generators               | 32.3 ms                                                | 28.3 ms: 1.14x faster                                                  |
| sympy_expand             | 269 ms                                                 | 237 ms: 1.13x faster                                                   |
| 2to3                     | 192 ms                                                 | 170 ms: 1.13x faster                                                   |
| fannkuch                 | 303 ms                                                 | 271 ms: 1.12x faster                                                   |
| scimark_fft              | 224 ms                                                 | 203 ms: 1.11x faster                                                   |
| tomli_loads              | 1.71 sec                                               | 1.54 sec: 1.11x faster                                                 |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.11 ms: 1.10x faster                                                  |
| sqlglot_optimize         | 36.8 ms                                                | 33.7 ms: 1.09x faster                                                  |
| bench_thread_pool        | 527 us                                                 | 491 us: 1.07x faster                                                   |
| meteor_contest           | 77.7 ms                                                | 72.4 ms: 1.07x faster                                                  |
| coroutines               | 20.7 ms                                                | 19.5 ms: 1.06x faster                                                  |
| nqueens                  | 63.8 ms                                                | 60.1 ms: 1.06x faster                                                  |
| json                     | 3.08 ms                                                | 2.94 ms: 1.05x faster                                                  |
| sqlglot_normalize        | 190 ms                                                 | 182 ms: 1.05x faster                                                   |
| mdp                      | 1.63 sec                                               | 1.56 sec: 1.05x faster                                                 |
| xml_etree_parse          | 108 ms                                                 | 105 ms: 1.02x faster                                                   |
| regex_v8                 | 17.1 ms                                                | 17.1 ms: 1.00x faster                                                  |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.01x slower                                                  |
| json_loads               | 16.4 us                                                | 16.9 us: 1.03x slower                                                  |
| pickle                   | 6.97 us                                                | 7.23 us: 1.04x slower                                                  |
| regex_effbot             | 2.46 ms                                                | 2.56 ms: 1.04x slower                                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 75.5 ms: 1.05x slower                                                  |
| xml_etree_generate       | 53.5 ms                                                | 56.1 ms: 1.05x slower                                                  |
| unpickle                 | 8.80 us                                                | 9.23 us: 1.05x slower                                                  |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                  |
| sqlite_synth             | 1.46 us                                                | 1.58 us: 1.08x slower                                                  |
| pickle_list              | 2.74 us                                                | 2.97 us: 1.09x slower                                                  |
| coverage                 | 41.5 ms                                                | 47.6 ms: 1.15x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.09 us: 1.15x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 44.7 ms: 1.19x slower                                                  |
| python_startup           | 10.9 ms                                                | 13.0 ms: 1.20x slower                                                  |
| async_generators         | 231 ms                                                 | 294 ms: 1.27x slower                                                   |
| telco                    | 3.49 ms                                                | 4.46 ms: 1.28x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 11.6 ms: 1.47x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.19x faster                                                           |

Benchmark hidden because not significant (2): asyncio_websockets, pathlib
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: 1.11x