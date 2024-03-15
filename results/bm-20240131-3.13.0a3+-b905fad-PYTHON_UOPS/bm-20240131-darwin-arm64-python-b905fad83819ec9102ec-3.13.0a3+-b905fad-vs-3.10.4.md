
# Results vs. 3.10.4

- fork: python
- ref: b905fad83819ec9102ec
- machine: darwin-arm64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 174 ms: 1.10x faster                                                   |
| chameleon      | 6.26 ms                                                | 4.95 ms: 1.26x faster                                                  |
| docutils       | 1.73 sec                                               | 1.50 sec: 1.16x faster                                                 |
| tornado_http   | 86.7 ms                                                | 69.7 ms: 1.24x faster                                                  |
| Geometric mean | (ref)                                                  | 1.19x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 258 ms: 1.50x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 333 ms: 1.42x faster                                                   |
| async_tree_io           | 980 ms                                                 | 706 ms: 1.39x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 525 ms: 1.24x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.38x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 85.3 ms: 1.09x faster                                                  |
| float          | 69.0 ms                                                | 68.3 ms: 1.01x faster                                                  |
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| Geometric mean | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 81.7 ms: 1.17x faster                                                  |
| regex_dna      | 174 ms                                                 | 152 ms: 1.15x faster                                                   |
| regex_effbot   | 2.46 ms                                                | 2.56 ms: 1.04x slower                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 198 us: 1.42x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.57 ms: 1.23x faster                                                  |
| unpickle_pure_python | 194 us                                                 | 163 us: 1.19x faster                                                   |
| xml_etree_process    | 46.5 ms                                                | 41.0 ms: 1.13x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.64 sec: 1.04x faster                                                 |
| json_loads           | 16.4 us                                                | 17.0 us: 1.03x slower                                                  |
| pickle               | 6.97 us                                                | 7.22 us: 1.04x slower                                                  |
| unpickle             | 8.80 us                                                | 9.11 us: 1.04x slower                                                  |
| pickle_dict          | 17.0 us                                                | 18.2 us: 1.07x slower                                                  |
| pickle_list          | 2.74 us                                                | 2.99 us: 1.09x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 58.8 ms: 1.10x slower                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 80.5 ms: 1.12x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.08 us: 1.15x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 13.2 ms: 1.21x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 11.8 ms: 1.49x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.34x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 9.66 ms: 1.02x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 73.2 us: 4.41x faster                                                  |
| logging_silent           | 117 ns                                                 | 71.3 ns: 1.64x faster                                                  |
| raytrace                 | 301 ms                                                 | 185 ms: 1.62x faster                                                   |
| richards_super           | 57.8 ms                                                | 37.0 ms: 1.56x faster                                                  |
| asyncio_tcp              | 659 ms                                                 | 427 ms: 1.54x faster                                                   |
| sqlglot_parse            | 1.24 ms                                                | 813 us: 1.53x faster                                                   |
| async_tree_none          | 388 ms                                                 | 258 ms: 1.50x faster                                                   |
| richards                 | 48.7 ms                                                | 33.0 ms: 1.48x faster                                                  |
| sqlglot_transpile        | 1.44 ms                                                | 998 us: 1.45x faster                                                   |
| chaos                    | 65.8 ms                                                | 45.9 ms: 1.43x faster                                                  |
| async_tree_memoization   | 474 ms                                                 | 333 ms: 1.42x faster                                                   |
| pickle_pure_python       | 281 us                                                 | 198 us: 1.42x faster                                                   |
| deltablue                | 4.91 ms                                                | 3.53 ms: 1.39x faster                                                  |
| async_tree_io            | 980 ms                                                 | 706 ms: 1.39x faster                                                   |
| go                       | 151 ms                                                 | 111 ms: 1.36x faster                                                   |
| unpack_sequence          | 39.0 ns                                                | 29.1 ns: 1.34x faster                                                  |
| scimark_lu               | 103 ms                                                 | 76.8 ms: 1.34x faster                                                  |
| crypto_pyaes             | 71.8 ms                                                | 54.0 ms: 1.33x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 26.7 us: 1.30x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.95 ms: 1.26x faster                                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.27 sec: 1.26x faster                                                 |
| logging_simple           | 4.45 us                                                | 3.56 us: 1.25x faster                                                  |
| pycparser                | 877 ms                                                 | 702 ms: 1.25x faster                                                   |
| tornado_http             | 86.7 ms                                                | 69.7 ms: 1.24x faster                                                  |
| logging_format           | 4.83 us                                                | 3.88 us: 1.24x faster                                                  |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 525 ms: 1.24x faster                                                   |
| json_dumps               | 8.11 ms                                                | 6.57 ms: 1.23x faster                                                  |
| create_gc_cycles         | 860 us                                                 | 704 us: 1.22x faster                                                   |
| scimark_sor              | 128 ms                                                 | 106 ms: 1.21x faster                                                   |
| deepcopy                 | 272 us                                                 | 227 us: 1.20x faster                                                   |
| unpickle_pure_python     | 194 us                                                 | 163 us: 1.19x faster                                                   |
| dulwich_log              | 35.3 ms                                                | 30.1 ms: 1.17x faster                                                  |
| scimark_monte_carlo      | 65.6 ms                                                | 56.0 ms: 1.17x faster                                                  |
| regex_compile            | 95.3 ms                                                | 81.7 ms: 1.17x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 79.1 ms: 1.17x faster                                                  |
| pyflate                  | 427 ms                                                 | 366 ms: 1.16x faster                                                   |
| deepcopy_reduce          | 2.33 us                                                | 2.00 us: 1.16x faster                                                  |
| mypy2                    | 607 ms                                                 | 524 ms: 1.16x faster                                                   |
| docutils                 | 1.73 sec                                               | 1.50 sec: 1.16x faster                                                 |
| regex_dna                | 174 ms                                                 | 152 ms: 1.15x faster                                                   |
| sympy_integrate          | 13.1 ms                                                | 11.5 ms: 1.14x faster                                                  |
| xml_etree_process        | 46.5 ms                                                | 41.0 ms: 1.13x faster                                                  |
| pprint_safe_repr         | 641 ms                                                 | 568 ms: 1.13x faster                                                   |
| dask                     | 253 ms                                                 | 224 ms: 1.13x faster                                                   |
| generators               | 32.3 ms                                                | 28.7 ms: 1.13x faster                                                  |
| sympy_str                | 165 ms                                                 | 147 ms: 1.12x faster                                                   |
| pprint_pformat           | 1.30 sec                                               | 1.16 sec: 1.12x faster                                                 |
| comprehensions           | 16.9 us                                                | 15.2 us: 1.11x faster                                                  |
| sympy_expand             | 269 ms                                                 | 244 ms: 1.10x faster                                                   |
| 2to3                     | 192 ms                                                 | 174 ms: 1.10x faster                                                   |
| nbody                    | 93.0 ms                                                | 85.3 ms: 1.09x faster                                                  |
| hexiom                   | 6.19 ms                                                | 5.85 ms: 1.06x faster                                                  |
| coroutines               | 20.7 ms                                                | 19.7 ms: 1.05x faster                                                  |
| json                     | 3.08 ms                                                | 2.94 ms: 1.05x faster                                                  |
| tomli_loads              | 1.71 sec                                               | 1.64 sec: 1.04x faster                                                 |
| bench_thread_pool        | 527 us                                                 | 511 us: 1.03x faster                                                   |
| sqlglot_optimize         | 36.8 ms                                                | 35.8 ms: 1.03x faster                                                  |
| mako                     | 9.87 ms                                                | 9.66 ms: 1.02x faster                                                  |
| float                    | 69.0 ms                                                | 68.3 ms: 1.01x faster                                                  |
| mdp                      | 1.63 sec                                               | 1.62 sec: 1.01x faster                                                 |
| meteor_contest           | 77.7 ms                                                | 77.2 ms: 1.01x faster                                                  |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.01x slower                                                  |
| json_loads               | 16.4 us                                                | 17.0 us: 1.03x slower                                                  |
| pickle                   | 6.97 us                                                | 7.22 us: 1.04x slower                                                  |
| unpickle                 | 8.80 us                                                | 9.11 us: 1.04x slower                                                  |
| regex_effbot             | 2.46 ms                                                | 2.56 ms: 1.04x slower                                                  |
| fannkuch                 | 303 ms                                                 | 319 ms: 1.05x slower                                                   |
| nqueens                  | 63.8 ms                                                | 67.9 ms: 1.06x slower                                                  |
| spectral_norm            | 94.8 ms                                                | 101 ms: 1.07x slower                                                   |
| pickle_dict              | 17.0 us                                                | 18.2 us: 1.07x slower                                                  |
| scimark_fft              | 224 ms                                                 | 244 ms: 1.09x slower                                                   |
| pickle_list              | 2.74 us                                                | 2.99 us: 1.09x slower                                                  |
| xml_etree_generate       | 53.5 ms                                                | 58.8 ms: 1.10x slower                                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 80.5 ms: 1.12x slower                                                  |
| sqlite_synth             | 1.46 us                                                | 1.64 us: 1.13x slower                                                  |
| coverage                 | 41.5 ms                                                | 47.1 ms: 1.14x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.08 us: 1.15x slower                                                  |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 4.09 ms: 1.20x slower                                                  |
| python_startup           | 10.9 ms                                                | 13.2 ms: 1.21x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 45.5 ms: 1.22x slower                                                  |
| async_generators         | 231 ms                                                 | 297 ms: 1.28x slower                                                   |
| telco                    | 3.49 ms                                                | 4.70 ms: 1.35x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 11.8 ms: 1.49x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.13x faster                                                           |

Benchmark hidden because not significant (5): xml_etree_parse, asyncio_websockets, regex_v8, sqlglot_normalize, pathlib
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: 1.11x