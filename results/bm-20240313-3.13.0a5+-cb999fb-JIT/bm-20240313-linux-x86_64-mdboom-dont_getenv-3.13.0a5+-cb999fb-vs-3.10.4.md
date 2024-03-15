# Results vs. 3.10.4

- fork: mdboom
- ref: dont_getenv
- machine: linux-x86_64
- commit hash: cb999fb
- commit date: 2024-03-13
- overall geometric mean: 1.30x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.33x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 283 ms: 1.23x faster                                          |
| chameleon      | 9.68 ms                                                | 6.83 ms: 1.42x faster                                         |
| docutils       | 3.30 sec                                               | 2.78 sec: 1.19x faster                                        |
| html5lib       | 88.9 ms                                                | 68.8 ms: 1.29x faster                                         |
| tornado_http   | 136 ms                                                 | 98.6 ms: 1.38x faster                                         |
| Geometric mean | (ref)                                                  | 1.30x faster                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 447 ms: 1.63x faster                                          |
| async_tree_memoization  | 870 ms                                                 | 576 ms: 1.51x faster                                          |
| async_tree_io           | 1.77 sec                                               | 1.22 sec: 1.45x faster                                        |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 725 ms: 1.40x faster                                          |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 92.8 ms: 1.65x faster                                         |
| float          | 117 ms                                                 | 80.0 ms: 1.46x faster                                         |
| pidigits       | 191 ms                                                 | 190 ms: 1.01x faster                                          |
| Geometric mean | (ref)                                                  | 1.35x faster                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 143 ms: 1.32x faster                                          |
| regex_v8       | 27.8 ms                                                | 25.4 ms: 1.09x faster                                         |
| regex_dna      | 227 ms                                                 | 225 ms: 1.01x faster                                          |
| regex_effbot   | 3.63 ms                                                | 3.90 ms: 1.07x slower                                         |
| Geometric mean | (ref)                                                  | 1.08x faster                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 312 us: 1.55x faster                                          |
| tomli_loads          | 3.14 sec                                               | 2.08 sec: 1.51x faster                                        |
| unpickle_pure_python | 331 us                                                 | 239 us: 1.38x faster                                          |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                         |
| xml_etree_process    | 79.1 ms                                                | 59.7 ms: 1.33x faster                                         |
| xml_etree_generate   | 99.4 ms                                                | 86.7 ms: 1.15x faster                                         |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                         |
| unpickle_list        | 5.20 us                                                | 4.80 us: 1.08x faster                                         |
| xml_etree_iterparse  | 115 ms                                                 | 108 ms: 1.07x faster                                          |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                          |
| pickle_list          | 5.08 us                                                | 5.00 us: 1.02x faster                                         |
| unpickle             | 14.4 us                                                | 14.5 us: 1.01x slower                                         |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                         |
| pickle_dict          | 29.6 us                                                | 34.1 us: 1.15x slower                                         |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.6 ms: 1.16x faster                                         |
| python_startup_no_site | 5.93 ms                                                | 11.1 ms: 1.88x slower                                         |
| Geometric mean         | (ref)                                                  | 1.27x slower                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.8 ms: 1.51x faster                                         |
| django_template | 48.2 ms                                                | 34.7 ms: 1.39x faster                                         |
| genshi_text     | 31.8 ms                                                | 24.3 ms: 1.31x faster                                         |
| genshi_xml      | 66.0 ms                                                | 55.3 ms: 1.19x faster                                         |
| Geometric mean  | (ref)                                                  | 1.35x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.95x faster                                          |
| generators               | 80.1 ms                                                | 29.5 ms: 2.72x faster                                         |
| deltablue                | 7.91 ms                                                | 3.43 ms: 2.30x faster                                         |
| logging_silent           | 190 ns                                                 | 102 ns: 1.87x faster                                          |
| asyncio_tcp              | 922 ms                                                 | 505 ms: 1.82x faster                                          |
| chaos                    | 115 ms                                                 | 64.5 ms: 1.79x faster                                         |
| richards_super           | 94.7 ms                                                | 53.7 ms: 1.76x faster                                         |
| scimark_sor              | 220 ms                                                 | 128 ms: 1.71x faster                                          |
| raytrace                 | 507 ms                                                 | 297 ms: 1.71x faster                                          |
| pylint                   | 551 ms                                                 | 324 ms: 1.70x faster                                          |
| richards                 | 79.3 ms                                                | 47.0 ms: 1.69x faster                                         |
| crypto_pyaes             | 128 ms                                                 | 76.1 ms: 1.68x faster                                         |
| scimark_monte_carlo      | 118 ms                                                 | 70.5 ms: 1.68x faster                                         |
| comprehensions           | 28.8 us                                                | 17.3 us: 1.66x faster                                         |
| sqlglot_parse            | 2.17 ms                                                | 1.31 ms: 1.66x faster                                         |
| nbody                    | 154 ms                                                 | 92.8 ms: 1.65x faster                                         |
| async_tree_none          | 728 ms                                                 | 447 ms: 1.63x faster                                          |
| coroutines               | 35.1 ms                                                | 22.4 ms: 1.57x faster                                         |
| sqlglot_transpile        | 2.57 ms                                                | 1.65 ms: 1.56x faster                                         |
| pickle_pure_python       | 484 us                                                 | 312 us: 1.55x faster                                          |
| go                       | 240 ms                                                 | 156 ms: 1.53x faster                                          |
| mako                     | 16.3 ms                                                | 10.8 ms: 1.51x faster                                         |
| tomli_loads              | 3.14 sec                                               | 2.08 sec: 1.51x faster                                        |
| async_tree_memoization   | 870 ms                                                 | 576 ms: 1.51x faster                                          |
| spectral_norm            | 170 ms                                                 | 113 ms: 1.50x faster                                          |
| pyflate                  | 716 ms                                                 | 480 ms: 1.49x faster                                          |
| hexiom                   | 10.4 ms                                                | 7.03 ms: 1.48x faster                                         |
| deepcopy_memo            | 58.5 us                                                | 39.7 us: 1.47x faster                                         |
| float                    | 117 ms                                                 | 80.0 ms: 1.46x faster                                         |
| async_tree_io            | 1.77 sec                                               | 1.22 sec: 1.45x faster                                        |
| chameleon                | 9.68 ms                                                | 6.83 ms: 1.42x faster                                         |
| logging_simple           | 8.30 us                                                | 5.90 us: 1.41x faster                                         |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 725 ms: 1.40x faster                                          |
| logging_format           | 9.09 us                                                | 6.53 us: 1.39x faster                                         |
| django_template          | 48.2 ms                                                | 34.7 ms: 1.39x faster                                         |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.85 sec: 1.39x faster                                        |
| tornado_http             | 136 ms                                                 | 98.6 ms: 1.38x faster                                         |
| unpickle_pure_python     | 331 us                                                 | 239 us: 1.38x faster                                          |
| scimark_fft              | 466 ms                                                 | 339 ms: 1.37x faster                                          |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                         |
| scimark_lu               | 176 ms                                                 | 130 ms: 1.36x faster                                          |
| pprint_pformat           | 2.10 sec                                               | 1.55 sec: 1.36x faster                                        |
| deepcopy_reduce          | 4.17 us                                                | 3.08 us: 1.35x faster                                         |
| deepcopy                 | 479 us                                                 | 355 us: 1.35x faster                                          |
| thrift                   | 1.07 ms                                                | 795 us: 1.35x faster                                          |
| pprint_safe_repr         | 1.02 sec                                               | 756 ms: 1.35x faster                                          |
| fannkuch                 | 532 ms                                                 | 398 ms: 1.33x faster                                          |
| xml_etree_process        | 79.1 ms                                                | 59.7 ms: 1.33x faster                                         |
| regex_compile            | 188 ms                                                 | 143 ms: 1.32x faster                                          |
| genshi_text              | 31.8 ms                                                | 24.3 ms: 1.31x faster                                         |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.31x faster                                          |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.94 ms: 1.31x faster                                         |
| pycparser                | 1.58 sec                                               | 1.22 sec: 1.29x faster                                        |
| html5lib                 | 88.9 ms                                                | 68.8 ms: 1.29x faster                                         |
| djangocms                | 38.4 us                                                | 31.0 us: 1.24x faster                                         |
| 2to3                     | 348 ms                                                 | 283 ms: 1.23x faster                                          |
| sqlglot_optimize         | 69.2 ms                                                | 56.8 ms: 1.22x faster                                         |
| sympy_sum                | 196 ms                                                 | 162 ms: 1.21x faster                                          |
| sympy_integrate          | 25.8 ms                                                | 21.3 ms: 1.21x faster                                         |
| dulwich_log              | 84.3 ms                                                | 70.0 ms: 1.20x faster                                         |
| sympy_str                | 346 ms                                                 | 287 ms: 1.20x faster                                          |
| aiohttp                  | 1.44 ms                                                | 1.20 ms: 1.20x faster                                         |
| genshi_xml               | 66.0 ms                                                | 55.3 ms: 1.19x faster                                         |
| docutils                 | 3.30 sec                                               | 2.78 sec: 1.19x faster                                        |
| gunicorn                 | 1.53 ms                                                | 1.29 ms: 1.18x faster                                         |
| nqueens                  | 106 ms                                                 | 89.6 ms: 1.18x faster                                         |
| dask                     | 441 ms                                                 | 374 ms: 1.18x faster                                          |
| sympy_expand             | 566 ms                                                 | 487 ms: 1.16x faster                                          |
| python_startup           | 14.6 ms                                                | 12.6 ms: 1.16x faster                                         |
| xml_etree_generate       | 99.4 ms                                                | 86.7 ms: 1.15x faster                                         |
| bench_thread_pool        | 986 us                                                 | 863 us: 1.14x faster                                          |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                         |
| json                     | 5.69 ms                                                | 5.17 ms: 1.10x faster                                         |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                          |
| pathlib                  | 20.5 ms                                                | 18.7 ms: 1.09x faster                                         |
| regex_v8                 | 27.8 ms                                                | 25.4 ms: 1.09x faster                                         |
| unpickle_list            | 5.20 us                                                | 4.80 us: 1.08x faster                                         |
| mdp                      | 2.85 sec                                               | 2.63 sec: 1.08x faster                                        |
| xml_etree_iterparse      | 115 ms                                                 | 108 ms: 1.07x faster                                          |
| create_gc_cycles         | 1.62 ms                                                | 1.52 ms: 1.07x faster                                         |
| sqlite_synth             | 3.02 us                                                | 2.85 us: 1.06x faster                                         |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                          |
| pickle_list              | 5.08 us                                                | 5.00 us: 1.02x faster                                         |
| regex_dna                | 227 ms                                                 | 225 ms: 1.01x faster                                          |
| pidigits                 | 191 ms                                                 | 190 ms: 1.01x faster                                          |
| asyncio_websockets       | 559 ms                                                 | 563 ms: 1.01x slower                                          |
| unpickle                 | 14.4 us                                                | 14.5 us: 1.01x slower                                         |
| async_generators         | 444 ms                                                 | 469 ms: 1.06x slower                                          |
| regex_effbot             | 3.63 ms                                                | 3.90 ms: 1.07x slower                                         |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                         |
| bench_mp_pool            | 24.0 ms                                                | 26.4 ms: 1.10x slower                                         |
| gc_traversal             | 3.62 ms                                                | 4.09 ms: 1.13x slower                                         |
| pickle_dict              | 29.6 us                                                | 34.1 us: 1.15x slower                                         |
| telco                    | 7.27 ms                                                | 8.42 ms: 1.16x slower                                         |
| coverage                 | 79.4 ms                                                | 97.8 ms: 1.23x slower                                         |
| unpack_sequence          | 60.0 ns                                                | 88.3 ns: 1.47x slower                                         |
| python_startup_no_site   | 5.93 ms                                                | 11.1 ms: 1.88x slower                                         |
| Geometric mean           | (ref)                                                  | 1.30x faster                                                  |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240313-3.13.0a5+-cb999fb-JIT/bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.33x