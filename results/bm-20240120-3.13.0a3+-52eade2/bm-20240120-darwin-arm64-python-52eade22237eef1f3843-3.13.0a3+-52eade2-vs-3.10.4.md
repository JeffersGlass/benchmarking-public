
# Results vs. 3.10.4

- fork: python
- ref: 52eade22237eef1f3843
- machine: darwin-arm64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.19x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 192 ms                                                 | 169 ms: 1.13x faster                                                   |
| chameleon      | 6.26 ms                                                | 4.89 ms: 1.28x faster                                                  |
| docutils       | 1.73 sec                                               | 1.46 sec: 1.18x faster                                                 |
| tornado_http   | 86.7 ms                                                | 68.7 ms: 1.26x faster                                                  |
| Geometric mean | (ref)                                                  | 1.21x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 388 ms                                                 | 252 ms: 1.54x faster                                                   |
| async_tree_memoization  | 474 ms                                                 | 331 ms: 1.43x faster                                                   |
| async_tree_io           | 980 ms                                                 | 704 ms: 1.39x faster                                                   |
| async_tree_cpu_io_mixed | 649 ms                                                 | 520 ms: 1.25x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.40x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 93.0 ms                                                | 75.5 ms: 1.23x faster                                                  |
| float          | 69.0 ms                                                | 56.9 ms: 1.21x faster                                                  |
| Geometric mean | (ref)                                                  | 1.14x faster                                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 95.3 ms                                                | 73.9 ms: 1.29x faster                                                  |
| regex_dna      | 174 ms                                                 | 155 ms: 1.12x faster                                                   |
| regex_v8       | 17.1 ms                                                | 17.8 ms: 1.04x slower                                                  |
| regex_effbot   | 2.46 ms                                                | 2.74 ms: 1.12x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 281 us                                                 | 197 us: 1.42x faster                                                   |
| unpickle_pure_python | 194 us                                                 | 154 us: 1.26x faster                                                   |
| json_dumps           | 8.11 ms                                                | 6.59 ms: 1.23x faster                                                  |
| xml_etree_process    | 46.5 ms                                                | 39.4 ms: 1.18x faster                                                  |
| tomli_loads          | 1.71 sec                                               | 1.55 sec: 1.10x faster                                                 |
| xml_etree_parse      | 108 ms                                                 | 107 ms: 1.01x faster                                                   |
| unpickle             | 8.80 us                                                | 9.17 us: 1.04x slower                                                  |
| json_loads           | 16.4 us                                                | 17.2 us: 1.04x slower                                                  |
| xml_etree_generate   | 53.5 ms                                                | 56.2 ms: 1.05x slower                                                  |
| xml_etree_iterparse  | 72.1 ms                                                | 75.8 ms: 1.05x slower                                                  |
| pickle               | 6.97 us                                                | 7.40 us: 1.06x slower                                                  |
| pickle_dict          | 17.0 us                                                | 18.1 us: 1.07x slower                                                  |
| pickle_list          | 2.74 us                                                | 2.94 us: 1.08x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.06 us: 1.14x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.9 ms                                                | 12.5 ms: 1.15x slower                                                  |
| python_startup_no_site | 7.91 ms                                                | 11.1 ms: 1.40x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.27x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 9.87 ms                                                | 7.62 ms: 1.30x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 323 us                                                 | 71.3 us: 4.53x faster                                                  |
| deltablue                | 4.91 ms                                                | 2.45 ms: 2.01x faster                                                  |
| raytrace                 | 301 ms                                                 | 171 ms: 1.76x faster                                                   |
| logging_silent           | 117 ns                                                 | 70.5 ns: 1.66x faster                                                  |
| chaos                    | 65.8 ms                                                | 39.9 ms: 1.65x faster                                                  |
| sqlglot_parse            | 1.24 ms                                                | 790 us: 1.57x faster                                                   |
| richards_super           | 57.8 ms                                                | 37.0 ms: 1.56x faster                                                  |
| asyncio_tcp              | 659 ms                                                 | 423 ms: 1.56x faster                                                   |
| async_tree_none          | 388 ms                                                 | 252 ms: 1.54x faster                                                   |
| sqlglot_transpile        | 1.44 ms                                                | 967 us: 1.49x faster                                                   |
| crypto_pyaes             | 71.8 ms                                                | 48.6 ms: 1.48x faster                                                  |
| richards                 | 48.7 ms                                                | 33.2 ms: 1.47x faster                                                  |
| async_tree_memoization   | 474 ms                                                 | 331 ms: 1.43x faster                                                   |
| go                       | 151 ms                                                 | 106 ms: 1.43x faster                                                   |
| pickle_pure_python       | 281 us                                                 | 197 us: 1.42x faster                                                   |
| comprehensions           | 16.9 us                                                | 12.1 us: 1.40x faster                                                  |
| async_tree_io            | 980 ms                                                 | 704 ms: 1.39x faster                                                   |
| scimark_monte_carlo      | 65.6 ms                                                | 47.2 ms: 1.39x faster                                                  |
| scimark_lu               | 103 ms                                                 | 74.2 ms: 1.39x faster                                                  |
| unpack_sequence          | 39.0 ns                                                | 28.4 ns: 1.38x faster                                                  |
| hexiom                   | 6.19 ms                                                | 4.53 ms: 1.37x faster                                                  |
| deepcopy_memo            | 34.7 us                                                | 25.7 us: 1.35x faster                                                  |
| mako                     | 9.87 ms                                                | 7.62 ms: 1.30x faster                                                  |
| logging_format           | 4.83 us                                                | 3.74 us: 1.29x faster                                                  |
| regex_compile            | 95.3 ms                                                | 73.9 ms: 1.29x faster                                                  |
| logging_simple           | 4.45 us                                                | 3.47 us: 1.28x faster                                                  |
| chameleon                | 6.26 ms                                                | 4.89 ms: 1.28x faster                                                  |
| sympy_sum                | 92.2 ms                                                | 72.6 ms: 1.27x faster                                                  |
| tornado_http             | 86.7 ms                                                | 68.7 ms: 1.26x faster                                                  |
| unpickle_pure_python     | 194 us                                                 | 154 us: 1.26x faster                                                   |
| pycparser                | 877 ms                                                 | 697 ms: 1.26x faster                                                   |
| spectral_norm            | 94.8 ms                                                | 75.9 ms: 1.25x faster                                                  |
| pyflate                  | 427 ms                                                 | 342 ms: 1.25x faster                                                   |
| async_tree_cpu_io_mixed  | 649 ms                                                 | 520 ms: 1.25x faster                                                   |
| pprint_pformat           | 1.30 sec                                               | 1.05 sec: 1.24x faster                                                 |
| pprint_safe_repr         | 641 ms                                                 | 517 ms: 1.24x faster                                                   |
| nbody                    | 93.0 ms                                                | 75.5 ms: 1.23x faster                                                  |
| json_dumps               | 8.11 ms                                                | 6.59 ms: 1.23x faster                                                  |
| sympy_integrate          | 13.1 ms                                                | 10.7 ms: 1.23x faster                                                  |
| asyncio_tcp_ssl          | 1.60 sec                                               | 1.31 sec: 1.23x faster                                                 |
| scimark_sor              | 128 ms                                                 | 105 ms: 1.22x faster                                                   |
| create_gc_cycles         | 860 us                                                 | 706 us: 1.22x faster                                                   |
| float                    | 69.0 ms                                                | 56.9 ms: 1.21x faster                                                  |
| deepcopy                 | 272 us                                                 | 225 us: 1.21x faster                                                   |
| dulwich_log              | 35.3 ms                                                | 29.6 ms: 1.20x faster                                                  |
| sympy_str                | 165 ms                                                 | 139 ms: 1.19x faster                                                   |
| docutils                 | 1.73 sec                                               | 1.46 sec: 1.18x faster                                                 |
| xml_etree_process        | 46.5 ms                                                | 39.4 ms: 1.18x faster                                                  |
| deepcopy_reduce          | 2.33 us                                                | 1.98 us: 1.18x faster                                                  |
| mypy2                    | 607 ms                                                 | 518 ms: 1.17x faster                                                   |
| generators               | 32.3 ms                                                | 28.5 ms: 1.13x faster                                                  |
| 2to3                     | 192 ms                                                 | 169 ms: 1.13x faster                                                   |
| dask                     | 253 ms                                                 | 224 ms: 1.13x faster                                                   |
| regex_dna                | 174 ms                                                 | 155 ms: 1.12x faster                                                   |
| sympy_expand             | 269 ms                                                 | 240 ms: 1.12x faster                                                   |
| coroutines               | 20.7 ms                                                | 18.7 ms: 1.11x faster                                                  |
| fannkuch                 | 303 ms                                                 | 273 ms: 1.11x faster                                                   |
| tomli_loads              | 1.71 sec                                               | 1.55 sec: 1.10x faster                                                 |
| scimark_sparse_mat_mult  | 3.42 ms                                                | 3.12 ms: 1.10x faster                                                  |
| scimark_fft              | 224 ms                                                 | 205 ms: 1.09x faster                                                   |
| sqlglot_optimize         | 36.8 ms                                                | 33.8 ms: 1.09x faster                                                  |
| meteor_contest           | 77.7 ms                                                | 72.3 ms: 1.08x faster                                                  |
| nqueens                  | 63.8 ms                                                | 60.3 ms: 1.06x faster                                                  |
| bench_thread_pool        | 527 us                                                 | 502 us: 1.05x faster                                                   |
| sqlglot_normalize        | 190 ms                                                 | 182 ms: 1.05x faster                                                   |
| mdp                      | 1.63 sec                                               | 1.56 sec: 1.04x faster                                                 |
| json                     | 3.08 ms                                                | 2.96 ms: 1.04x faster                                                  |
| xml_etree_parse          | 108 ms                                                 | 107 ms: 1.01x faster                                                   |
| gc_traversal             | 2.36 ms                                                | 2.40 ms: 1.02x slower                                                  |
| regex_v8                 | 17.1 ms                                                | 17.8 ms: 1.04x slower                                                  |
| pathlib                  | 24.5 ms                                                | 25.4 ms: 1.04x slower                                                  |
| unpickle                 | 8.80 us                                                | 9.17 us: 1.04x slower                                                  |
| json_loads               | 16.4 us                                                | 17.2 us: 1.04x slower                                                  |
| xml_etree_generate       | 53.5 ms                                                | 56.2 ms: 1.05x slower                                                  |
| xml_etree_iterparse      | 72.1 ms                                                | 75.8 ms: 1.05x slower                                                  |
| pickle                   | 6.97 us                                                | 7.40 us: 1.06x slower                                                  |
| pickle_dict              | 17.0 us                                                | 18.1 us: 1.07x slower                                                  |
| pickle_list              | 2.74 us                                                | 2.94 us: 1.08x slower                                                  |
| sqlite_synth             | 1.46 us                                                | 1.59 us: 1.09x slower                                                  |
| regex_effbot             | 2.46 ms                                                | 2.74 ms: 1.12x slower                                                  |
| unpickle_list            | 2.69 us                                                | 3.06 us: 1.14x slower                                                  |
| coverage                 | 41.5 ms                                                | 47.5 ms: 1.15x slower                                                  |
| python_startup           | 10.9 ms                                                | 12.5 ms: 1.15x slower                                                  |
| bench_mp_pool            | 37.4 ms                                                | 44.1 ms: 1.18x slower                                                  |
| async_generators         | 231 ms                                                 | 296 ms: 1.28x slower                                                   |
| telco                    | 3.49 ms                                                | 4.55 ms: 1.30x slower                                                  |
| python_startup_no_site   | 7.91 ms                                                | 11.1 ms: 1.40x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.19x faster                                                           |

Benchmark hidden because not significant (2): asyncio_websockets, pidigits
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-darwin-arm64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: 1.10x