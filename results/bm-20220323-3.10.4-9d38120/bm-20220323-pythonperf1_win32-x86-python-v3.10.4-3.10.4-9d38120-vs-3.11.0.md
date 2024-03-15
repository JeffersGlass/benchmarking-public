
# Results vs. 3.11.0

- fork: python
- ref: v3.10.4
- machine: windows-x86
- commit hash: 9d38120
- commit date: 2022-03-23
- overall geometric mean: 1.10x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 282 ms                                                          | 265 ms: 1.06x faster                                            |
| chameleon      | 8.08 ms                                                         | 6.42 ms: 1.26x faster                                           |
| docutils       | 2.10 sec                                                        | 1.95 sec: 1.08x faster                                          |
| html5lib       | 54.3 ms                                                         | 52.1 ms: 1.04x faster                                           |
| Geometric mean | (ref)                                                           | 1.09x faster                                                    |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 |
|-------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_memoization  | 408 ms                                                          | 467 ms: 1.14x slower                                            |
| async_tree_none         | 343 ms                                                          | 394 ms: 1.15x slower                                            |
| async_tree_io           | 754 ms                                                          | 940 ms: 1.25x slower                                            |
| async_tree_cpu_io_mixed | 590 ms                                                          | 922 ms: 1.56x slower                                            |
| Geometric mean          | (ref)                                                           | 1.26x slower                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 126 ms                                                          | 79.1 ms: 1.59x faster                                           |
| float          | 76.1 ms                                                         | 69.6 ms: 1.09x faster                                           |
| pidigits       | 203 ms                                                          | 502 ms: 2.48x slower                                            |
| Geometric mean | (ref)                                                           | 1.13x slower                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 148 ms                                                          | 117 ms: 1.26x faster                                            |
| regex_effbot   | 1.82 ms                                                         | 1.66 ms: 1.10x faster                                           |
| regex_v8       | 15.2 ms                                                         | 15.8 ms: 1.04x slower                                           |
| regex_dna      | 122 ms                                                          | 131 ms: 1.07x slower                                            |
| Geometric mean | (ref)                                                           | 1.06x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 |
|----------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| unpickle_pure_python | 231 us                                                          | 189 us: 1.22x faster                                            |
| tomli_loads          | 2.31 sec                                                        | 1.91 sec: 1.21x faster                                          |
| xml_etree_generate   | 71.6 ms                                                         | 61.6 ms: 1.16x faster                                           |
| xml_etree_process    | 55.0 ms                                                         | 48.1 ms: 1.14x faster                                           |
| pickle_pure_python   | 309 us                                                          | 280 us: 1.10x faster                                            |
| pickle_dict          | 20.1 us                                                         | 18.2 us: 1.10x faster                                           |
| unpickle_list        | 3.28 us                                                         | 2.98 us: 1.10x faster                                           |
| xml_etree_iterparse  | 75.6 ms                                                         | 70.8 ms: 1.07x faster                                           |
| pickle               | 7.99 us                                                         | 7.83 us: 1.02x faster                                           |
| pickle_list          | 3.27 us                                                         | 3.22 us: 1.02x faster                                           |
| xml_etree_parse      | 114 ms                                                          | 120 ms: 1.05x slower                                            |
| unpickle             | 9.23 us                                                         | 9.82 us: 1.06x slower                                           |
| json_loads           | 20.0 us                                                         | 22.4 us: 1.12x slower                                           |
| Geometric mean       | (ref)                                                           | 1.06x faster                                                    |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 |
|------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 18.8 ms                                                         | 18.1 ms: 1.04x faster                                           |
| python_startup         | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                           |
| Geometric mean         | (ref)                                                           | 1.00x slower                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 |
|-----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| genshi_xml      | 61.2 ms                                                         | 46.6 ms: 1.31x faster                                           |
| genshi_text     | 26.8 ms                                                         | 21.0 ms: 1.27x faster                                           |
| mako            | 10.3 ms                                                         | 9.10 ms: 1.13x faster                                           |
| django_template | 37.4 ms                                                         | 36.0 ms: 1.04x faster                                           |
| Geometric mean  | (ref)                                                           | 1.18x faster                                                    |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 |
|--------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| generators               | 52.2 ms                                                         | 31.6 ms: 1.65x faster                                           |
| unpack_sequence          | 65.2 ns                                                         | 40.0 ns: 1.63x faster                                           |
| nbody                    | 126 ms                                                          | 79.1 ms: 1.59x faster                                           |
| spectral_norm            | 122 ms                                                          | 80.2 ms: 1.52x faster                                           |
| logging_simple           | 10.8 us                                                         | 7.29 us: 1.48x faster                                           |
| logging_format           | 11.5 us                                                         | 7.91 us: 1.45x faster                                           |
| deepcopy_memo            | 40.0 us                                                         | 29.6 us: 1.35x faster                                           |
| scimark_fft              | 291 ms                                                          | 216 ms: 1.35x faster                                            |
| coroutines               | 23.7 ms                                                         | 17.9 ms: 1.32x faster                                           |
| genshi_xml               | 61.2 ms                                                         | 46.6 ms: 1.31x faster                                           |
| scimark_sparse_mat_mult  | 4.23 ms                                                         | 3.24 ms: 1.31x faster                                           |
| nqueens                  | 111 ms                                                          | 87.1 ms: 1.28x faster                                           |
| genshi_text              | 26.8 ms                                                         | 21.0 ms: 1.27x faster                                           |
| regex_compile            | 148 ms                                                          | 117 ms: 1.26x faster                                            |
| fannkuch                 | 399 ms                                                          | 317 ms: 1.26x faster                                            |
| chameleon                | 8.08 ms                                                         | 6.42 ms: 1.26x faster                                           |
| coverage                 | 58.0 ms                                                         | 46.6 ms: 1.25x faster                                           |
| pprint_safe_repr         | 819 ms                                                          | 658 ms: 1.24x faster                                            |
| comprehensions           | 22.1 us                                                         | 17.7 us: 1.24x faster                                           |
| pprint_pformat           | 1.70 sec                                                        | 1.37 sec: 1.24x faster                                          |
| sympy_str                | 283 ms                                                          | 229 ms: 1.24x faster                                            |
| deepcopy_reduce          | 3.32 us                                                         | 2.68 us: 1.24x faster                                           |
| deepcopy                 | 381 us                                                          | 310 us: 1.23x faster                                            |
| hexiom                   | 7.51 ms                                                         | 6.13 ms: 1.22x faster                                           |
| unpickle_pure_python     | 231 us                                                          | 189 us: 1.22x faster                                            |
| logging_silent           | 119 ns                                                          | 97.9 ns: 1.22x faster                                           |
| sympy_sum                | 149 ms                                                          | 122 ms: 1.22x faster                                            |
| richards                 | 48.8 ms                                                         | 40.3 ms: 1.21x faster                                           |
| tomli_loads              | 2.31 sec                                                        | 1.91 sec: 1.21x faster                                          |
| typing_runtime_protocols | 478 us                                                          | 396 us: 1.21x faster                                            |
| sympy_integrate          | 19.9 ms                                                         | 16.6 ms: 1.20x faster                                           |
| sympy_expand             | 462 ms                                                          | 391 ms: 1.18x faster                                            |
| richards_super           | 58.7 ms                                                         | 49.9 ms: 1.18x faster                                           |
| scimark_sor              | 135 ms                                                          | 115 ms: 1.18x faster                                            |
| sqlalchemy_imperative    | 15.4 ms                                                         | 13.2 ms: 1.17x faster                                           |
| xml_etree_generate       | 71.6 ms                                                         | 61.6 ms: 1.16x faster                                           |
| sqlglot_optimize         | 51.8 ms                                                         | 44.7 ms: 1.16x faster                                           |
| scimark_monte_carlo      | 70.8 ms                                                         | 61.9 ms: 1.14x faster                                           |
| xml_etree_process        | 55.0 ms                                                         | 48.1 ms: 1.14x faster                                           |
| scimark_lu               | 102 ms                                                          | 89.8 ms: 1.14x faster                                           |
| meteor_contest           | 90.9 ms                                                         | 80.0 ms: 1.14x faster                                           |
| chaos                    | 84.4 ms                                                         | 74.4 ms: 1.13x faster                                           |
| mdp                      | 2.07 sec                                                        | 1.83 sec: 1.13x faster                                          |
| mako                     | 10.3 ms                                                         | 9.10 ms: 1.13x faster                                           |
| sqlglot_transpile        | 1.78 ms                                                         | 1.58 ms: 1.13x faster                                           |
| sqlglot_parse            | 1.49 ms                                                         | 1.33 ms: 1.12x faster                                           |
| pyflate                  | 471 ms                                                          | 422 ms: 1.12x faster                                            |
| sqlalchemy_declarative   | 115 ms                                                          | 104 ms: 1.10x faster                                            |
| pickle_pure_python       | 309 us                                                          | 280 us: 1.10x faster                                            |
| pickle_dict              | 20.1 us                                                         | 18.2 us: 1.10x faster                                           |
| unpickle_list            | 3.28 us                                                         | 2.98 us: 1.10x faster                                           |
| regex_effbot             | 1.82 ms                                                         | 1.66 ms: 1.10x faster                                           |
| telco                    | 5.29 ms                                                         | 4.83 ms: 1.10x faster                                           |
| float                    | 76.1 ms                                                         | 69.6 ms: 1.09x faster                                           |
| pylint                   | 418 ms                                                          | 384 ms: 1.09x faster                                            |
| raytrace                 | 327 ms                                                          | 303 ms: 1.08x faster                                            |
| async_generators         | 260 ms                                                          | 241 ms: 1.08x faster                                            |
| docutils                 | 2.10 sec                                                        | 1.95 sec: 1.08x faster                                          |
| gc_traversal             | 1.38 ms                                                         | 1.28 ms: 1.07x faster                                           |
| dulwich_log              | 62.8 ms                                                         | 58.5 ms: 1.07x faster                                           |
| bench_mp_pool            | 70.9 ms                                                         | 66.4 ms: 1.07x faster                                           |
| xml_etree_iterparse      | 75.6 ms                                                         | 70.8 ms: 1.07x faster                                           |
| 2to3                     | 282 ms                                                          | 265 ms: 1.06x faster                                            |
| mypy2                    | 626 ms                                                          | 590 ms: 1.06x faster                                            |
| asyncio_tcp              | 787 ms                                                          | 744 ms: 1.06x faster                                            |
| html5lib                 | 54.3 ms                                                         | 52.1 ms: 1.04x faster                                           |
| python_startup_no_site   | 18.8 ms                                                         | 18.1 ms: 1.04x faster                                           |
| dask                     | 355 ms                                                          | 341 ms: 1.04x faster                                            |
| django_template          | 37.4 ms                                                         | 36.0 ms: 1.04x faster                                           |
| aiohttp                  | 1.17 ms                                                         | 1.13 ms: 1.03x faster                                           |
| pickle                   | 7.99 us                                                         | 7.83 us: 1.02x faster                                           |
| deltablue                | 4.10 ms                                                         | 4.04 ms: 1.02x faster                                           |
| pickle_list              | 3.27 us                                                         | 3.22 us: 1.02x faster                                           |
| go                       | 147 ms                                                          | 146 ms: 1.01x faster                                            |
| pathlib                  | 79.9 ms                                                         | 81.2 ms: 1.02x slower                                           |
| crypto_pyaes             | 79.4 ms                                                         | 81.3 ms: 1.02x slower                                           |
| regex_v8                 | 15.2 ms                                                         | 15.8 ms: 1.04x slower                                           |
| python_startup           | 22.0 ms                                                         | 22.9 ms: 1.04x slower                                           |
| xml_etree_parse          | 114 ms                                                          | 120 ms: 1.05x slower                                            |
| unpickle                 | 9.23 us                                                         | 9.82 us: 1.06x slower                                           |
| sqlite_synth             | 2.15 us                                                         | 2.29 us: 1.07x slower                                           |
| regex_dna                | 122 ms                                                          | 131 ms: 1.07x slower                                            |
| json_loads               | 20.0 us                                                         | 22.4 us: 1.12x slower                                           |
| create_gc_cycles         | 618 us                                                          | 694 us: 1.12x slower                                            |
| thrift                   | 801 us                                                          | 902 us: 1.13x slower                                            |
| async_tree_memoization   | 408 ms                                                          | 467 ms: 1.14x slower                                            |
| async_tree_none          | 343 ms                                                          | 394 ms: 1.15x slower                                            |
| async_tree_io            | 754 ms                                                          | 940 ms: 1.25x slower                                            |
| async_tree_cpu_io_mixed  | 590 ms                                                          | 922 ms: 1.56x slower                                            |
| sqlglot_normalize        | 113 ms                                                          | 230 ms: 2.04x slower                                            |
| pidigits                 | 203 ms                                                          | 502 ms: 2.48x slower                                            |
| Geometric mean           | (ref)                                                           | 1.10x faster                                                    |

Benchmark hidden because not significant (7): bench_thread_pool, tornado_http, asyncio_tcp_ssl, json, pycparser, flaskblogging, json_dumps
Ignored benchmarks (4) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.06x


# Memory

- memory change: unknown