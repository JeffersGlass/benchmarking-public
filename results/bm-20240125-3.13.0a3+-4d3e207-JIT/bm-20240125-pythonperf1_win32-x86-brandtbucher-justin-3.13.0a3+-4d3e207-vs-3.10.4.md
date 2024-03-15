
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin
- machine: windows-x86
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.11x faster
- HPT reliability: 99.99%
- HPT 99th percentile: 1.04x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 255 ms: 1.04x faster                                                    |
| chameleon      | 6.42 ms                                                         | 6.09 ms: 1.05x faster                                                   |
| docutils       | 1.95 sec                                                        | 1.82 sec: 1.07x faster                                                  |
| tornado_http   | 118 ms                                                          | 98.2 ms: 1.20x faster                                                   |
| Geometric mean | (ref)                                                           | 1.09x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 520 ms: 1.77x faster                                                    |
| async_tree_none         | 394 ms                                                          | 257 ms: 1.53x faster                                                    |
| async_tree_io           | 940 ms                                                          | 617 ms: 1.52x faster                                                    |
| async_tree_memoization  | 467 ms                                                          | 324 ms: 1.44x faster                                                    |
| Geometric mean          | (ref)                                                           | 1.56x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 204 ms: 2.46x faster                                                    |
| float          | 69.6 ms                                                         | 55.9 ms: 1.25x faster                                                   |
| nbody          | 79.1 ms                                                         | 93.0 ms: 1.18x slower                                                   |
| Geometric mean | (ref)                                                           | 1.38x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 106 ms: 1.10x faster                                                    |
| regex_dna      | 131 ms                                                          | 120 ms: 1.09x faster                                                    |
| regex_v8       | 15.8 ms                                                         | 16.4 ms: 1.04x slower                                                   |
| regex_effbot   | 1.66 ms                                                         | 1.92 ms: 1.15x slower                                                   |
| Geometric mean | (ref)                                                           | 1.00x slower                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.78 ms: 1.45x faster                                                   |
| pickle_pure_python   | 280 us                                                          | 205 us: 1.37x faster                                                    |
| unpickle_pure_python | 189 us                                                          | 150 us: 1.26x faster                                                    |
| xml_etree_process    | 48.1 ms                                                         | 41.2 ms: 1.17x faster                                                   |
| tomli_loads          | 1.91 sec                                                        | 1.64 sec: 1.16x faster                                                  |
| json_loads           | 22.4 us                                                         | 20.1 us: 1.12x faster                                                   |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                                    |
| xml_etree_generate   | 61.6 ms                                                         | 59.2 ms: 1.04x faster                                                   |
| xml_etree_iterparse  | 70.8 ms                                                         | 68.5 ms: 1.03x faster                                                   |
| pickle_list          | 3.22 us                                                         | 3.26 us: 1.01x slower                                                   |
| unpickle             | 9.82 us                                                         | 10.2 us: 1.04x slower                                                   |
| pickle               | 7.83 us                                                         | 8.23 us: 1.05x slower                                                   |
| unpickle_list        | 2.98 us                                                         | 3.23 us: 1.08x slower                                                   |
| pickle_dict          | 18.2 us                                                         | 20.0 us: 1.10x slower                                                   |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                            |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup_no_site | 18.1 ms                                                         | 20.7 ms: 1.14x slower                                                   |
| Geometric mean         | (ref)                                                           | 1.07x slower                                                            |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.75 ms: 1.17x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207 |
|--------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 95.7 us: 4.13x faster                                                   |
| pidigits                 | 502 ms                                                          | 204 ms: 2.46x faster                                                    |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 520 ms: 1.77x faster                                                    |
| deltablue                | 4.04 ms                                                         | 2.47 ms: 1.63x faster                                                   |
| logging_silent           | 97.9 ns                                                         | 60.0 ns: 1.63x faster                                                   |
| richards_super           | 49.9 ms                                                         | 31.7 ms: 1.58x faster                                                   |
| async_tree_none          | 394 ms                                                          | 257 ms: 1.53x faster                                                    |
| async_tree_io            | 940 ms                                                          | 617 ms: 1.52x faster                                                    |
| sqlglot_parse            | 1.33 ms                                                         | 902 us: 1.48x faster                                                    |
| scimark_lu               | 89.8 ms                                                         | 61.4 ms: 1.46x faster                                                   |
| json_dumps               | 9.82 ms                                                         | 6.78 ms: 1.45x faster                                                   |
| async_tree_memoization   | 467 ms                                                          | 324 ms: 1.44x faster                                                    |
| richards                 | 40.3 ms                                                         | 28.1 ms: 1.43x faster                                                   |
| scimark_sor              | 115 ms                                                          | 82.3 ms: 1.40x faster                                                   |
| sqlglot_transpile        | 1.58 ms                                                         | 1.15 ms: 1.38x faster                                                   |
| pickle_pure_python       | 280 us                                                          | 205 us: 1.37x faster                                                    |
| generators               | 31.6 ms                                                         | 23.2 ms: 1.36x faster                                                   |
| raytrace                 | 303 ms                                                          | 225 ms: 1.34x faster                                                    |
| crypto_pyaes             | 81.3 ms                                                         | 62.5 ms: 1.30x faster                                                   |
| deepcopy_memo            | 29.6 us                                                         | 22.9 us: 1.29x faster                                                   |
| chaos                    | 74.4 ms                                                         | 58.8 ms: 1.27x faster                                                   |
| unpickle_pure_python     | 189 us                                                          | 150 us: 1.26x faster                                                    |
| pycparser                | 1.04 sec                                                        | 826 ms: 1.26x faster                                                    |
| go                       | 146 ms                                                          | 117 ms: 1.25x faster                                                    |
| float                    | 69.6 ms                                                         | 55.9 ms: 1.25x faster                                                   |
| coroutines               | 17.9 ms                                                         | 14.4 ms: 1.24x faster                                                   |
| sqlite_synth             | 2.29 us                                                         | 1.88 us: 1.22x faster                                                   |
| tornado_http             | 118 ms                                                          | 98.2 ms: 1.20x faster                                                   |
| mako                     | 9.10 ms                                                         | 7.75 ms: 1.17x faster                                                   |
| comprehensions           | 17.7 us                                                         | 15.1 us: 1.17x faster                                                   |
| xml_etree_process        | 48.1 ms                                                         | 41.2 ms: 1.17x faster                                                   |
| tomli_loads              | 1.91 sec                                                        | 1.64 sec: 1.16x faster                                                  |
| deepcopy                 | 310 us                                                          | 268 us: 1.16x faster                                                    |
| pyflate                  | 422 ms                                                          | 366 ms: 1.15x faster                                                    |
| json                     | 4.76 ms                                                         | 4.18 ms: 1.14x faster                                                   |
| asyncio_tcp              | 744 ms                                                          | 654 ms: 1.14x faster                                                    |
| dask                     | 341 ms                                                          | 303 ms: 1.13x faster                                                    |
| deepcopy_reduce          | 2.68 us                                                         | 2.39 us: 1.12x faster                                                   |
| json_loads               | 22.4 us                                                         | 20.1 us: 1.12x faster                                                   |
| sympy_sum                | 122 ms                                                          | 110 ms: 1.12x faster                                                    |
| bench_thread_pool        | 1.12 ms                                                         | 1.01 ms: 1.11x faster                                                   |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                                    |
| regex_compile            | 117 ms                                                          | 106 ms: 1.10x faster                                                    |
| regex_dna                | 131 ms                                                          | 120 ms: 1.09x faster                                                    |
| sympy_expand             | 391 ms                                                          | 362 ms: 1.08x faster                                                    |
| sympy_str                | 229 ms                                                          | 214 ms: 1.07x faster                                                    |
| docutils                 | 1.95 sec                                                        | 1.82 sec: 1.07x faster                                                  |
| sympy_integrate          | 16.6 ms                                                         | 15.7 ms: 1.06x faster                                                   |
| chameleon                | 6.42 ms                                                         | 6.09 ms: 1.05x faster                                                   |
| sqlglot_normalize        | 230 ms                                                          | 219 ms: 1.05x faster                                                    |
| fannkuch                 | 317 ms                                                          | 302 ms: 1.05x faster                                                    |
| create_gc_cycles         | 694 us                                                          | 662 us: 1.05x faster                                                    |
| sqlglot_optimize         | 44.7 ms                                                         | 42.7 ms: 1.05x faster                                                   |
| xml_etree_generate       | 61.6 ms                                                         | 59.2 ms: 1.04x faster                                                   |
| 2to3                     | 265 ms                                                          | 255 ms: 1.04x faster                                                    |
| xml_etree_iterparse      | 70.8 ms                                                         | 68.5 ms: 1.03x faster                                                   |
| spectral_norm            | 80.2 ms                                                         | 78.1 ms: 1.03x faster                                                   |
| nqueens                  | 87.1 ms                                                         | 86.6 ms: 1.01x faster                                                   |
| mdp                      | 1.83 sec                                                        | 1.84 sec: 1.01x slower                                                  |
| pickle_list              | 3.22 us                                                         | 3.26 us: 1.01x slower                                                   |
| pprint_pformat           | 1.37 sec                                                        | 1.40 sec: 1.03x slower                                                  |
| pprint_safe_repr         | 658 ms                                                          | 676 ms: 1.03x slower                                                    |
| unpickle                 | 9.82 us                                                         | 10.2 us: 1.04x slower                                                   |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.7 sec: 1.04x slower                                                  |
| regex_v8                 | 15.8 ms                                                         | 16.4 ms: 1.04x slower                                                   |
| pickle                   | 7.83 us                                                         | 8.23 us: 1.05x slower                                                   |
| hexiom                   | 6.13 ms                                                         | 6.45 ms: 1.05x slower                                                   |
| meteor_contest           | 80.0 ms                                                         | 84.3 ms: 1.05x slower                                                   |
| unpickle_list            | 2.98 us                                                         | 3.23 us: 1.08x slower                                                   |
| logging_simple           | 7.29 us                                                         | 7.90 us: 1.08x slower                                                   |
| logging_format           | 7.91 us                                                         | 8.61 us: 1.09x slower                                                   |
| pathlib                  | 81.2 ms                                                         | 89.0 ms: 1.10x slower                                                   |
| pickle_dict              | 18.2 us                                                         | 20.0 us: 1.10x slower                                                   |
| bench_mp_pool            | 66.4 ms                                                         | 73.8 ms: 1.11x slower                                                   |
| gc_traversal             | 1.28 ms                                                         | 1.44 ms: 1.12x slower                                                   |
| python_startup_no_site   | 18.1 ms                                                         | 20.7 ms: 1.14x slower                                                   |
| scimark_monte_carlo      | 61.9 ms                                                         | 70.8 ms: 1.14x slower                                                   |
| scimark_fft              | 216 ms                                                          | 249 ms: 1.15x slower                                                    |
| regex_effbot             | 1.66 ms                                                         | 1.92 ms: 1.15x slower                                                   |
| nbody                    | 79.1 ms                                                         | 93.0 ms: 1.18x slower                                                   |
| async_generators         | 241 ms                                                          | 295 ms: 1.22x slower                                                    |
| telco                    | 4.83 ms                                                         | 5.94 ms: 1.23x slower                                                   |
| coverage                 | 46.6 ms                                                         | 499 ms: 10.72x slower                                                   |
| Geometric mean           | (ref)                                                           | 1.11x faster                                                            |

Benchmark hidden because not significant (3): scimark_sparse_mat_mult, unpack_sequence, python_startup
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240125-3.13.0a3+-4d3e207-JIT/bm-20240125-pythonperf1_win32-x86-brandtbucher-justin-3.13.0a3+-4d3e207.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: unknown