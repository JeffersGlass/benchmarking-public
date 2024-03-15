
# Results vs. 3.10.4

- fork: python
- ref: v3.11.0
- machine: windows-x86
- commit hash: deaf509
- commit date: 2022-10-24
- overall geometric mean: 1.10x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 282 ms: 1.06x slower                                            |
| chameleon      | 6.42 ms                                                         | 8.08 ms: 1.26x slower                                           |
| docutils       | 1.95 sec                                                        | 2.10 sec: 1.08x slower                                          |
| html5lib       | 52.1 ms                                                         | 54.3 ms: 1.04x slower                                           |
| Geometric mean | (ref)                                                           | 1.09x slower                                                    |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|-------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 590 ms: 1.56x faster                                            |
| async_tree_io           | 940 ms                                                          | 754 ms: 1.25x faster                                            |
| async_tree_none         | 394 ms                                                          | 343 ms: 1.15x faster                                            |
| async_tree_memoization  | 467 ms                                                          | 408 ms: 1.14x faster                                            |
| Geometric mean          | (ref)                                                           | 1.26x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 203 ms: 2.48x faster                                            |
| float          | 69.6 ms                                                         | 76.1 ms: 1.09x slower                                           |
| nbody          | 79.1 ms                                                         | 126 ms: 1.59x slower                                            |
| Geometric mean | (ref)                                                           | 1.13x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 122 ms: 1.07x faster                                            |
| regex_v8       | 15.8 ms                                                         | 15.2 ms: 1.04x faster                                           |
| regex_effbot   | 1.66 ms                                                         | 1.82 ms: 1.10x slower                                           |
| regex_compile  | 117 ms                                                          | 148 ms: 1.26x slower                                            |
| Geometric mean | (ref)                                                           | 1.06x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|----------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| json_loads           | 22.4 us                                                         | 20.0 us: 1.12x faster                                           |
| unpickle             | 9.82 us                                                         | 9.23 us: 1.06x faster                                           |
| xml_etree_parse      | 120 ms                                                          | 114 ms: 1.05x faster                                            |
| pickle_list          | 3.22 us                                                         | 3.27 us: 1.02x slower                                           |
| pickle               | 7.83 us                                                         | 7.99 us: 1.02x slower                                           |
| xml_etree_iterparse  | 70.8 ms                                                         | 75.6 ms: 1.07x slower                                           |
| unpickle_list        | 2.98 us                                                         | 3.28 us: 1.10x slower                                           |
| pickle_dict          | 18.2 us                                                         | 20.1 us: 1.10x slower                                           |
| pickle_pure_python   | 280 us                                                          | 309 us: 1.10x slower                                            |
| xml_etree_process    | 48.1 ms                                                         | 55.0 ms: 1.14x slower                                           |
| xml_etree_generate   | 61.6 ms                                                         | 71.6 ms: 1.16x slower                                           |
| tomli_loads          | 1.91 sec                                                        | 2.31 sec: 1.21x slower                                          |
| unpickle_pure_python | 189 us                                                          | 231 us: 1.22x slower                                            |
| Geometric mean       | (ref)                                                           | 1.06x slower                                                    |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 22.0 ms: 1.04x faster                                           |
| python_startup_no_site | 18.1 ms                                                         | 18.8 ms: 1.04x slower                                           |
| Geometric mean         | (ref)                                                           | 1.00x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|-----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| django_template | 36.0 ms                                                         | 37.4 ms: 1.04x slower                                           |
| mako            | 9.10 ms                                                         | 10.3 ms: 1.13x slower                                           |
| genshi_text     | 21.0 ms                                                         | 26.8 ms: 1.27x slower                                           |
| genshi_xml      | 46.6 ms                                                         | 61.2 ms: 1.31x slower                                           |
| Geometric mean  | (ref)                                                           | 1.18x slower                                                    |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509 |
|--------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits                 | 502 ms                                                          | 203 ms: 2.48x faster                                            |
| sqlglot_normalize        | 230 ms                                                          | 113 ms: 2.04x faster                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 590 ms: 1.56x faster                                            |
| async_tree_io            | 940 ms                                                          | 754 ms: 1.25x faster                                            |
| async_tree_none          | 394 ms                                                          | 343 ms: 1.15x faster                                            |
| async_tree_memoization   | 467 ms                                                          | 408 ms: 1.14x faster                                            |
| thrift                   | 902 us                                                          | 801 us: 1.13x faster                                            |
| create_gc_cycles         | 694 us                                                          | 618 us: 1.12x faster                                            |
| json_loads               | 22.4 us                                                         | 20.0 us: 1.12x faster                                           |
| regex_dna                | 131 ms                                                          | 122 ms: 1.07x faster                                            |
| sqlite_synth             | 2.29 us                                                         | 2.15 us: 1.07x faster                                           |
| unpickle                 | 9.82 us                                                         | 9.23 us: 1.06x faster                                           |
| xml_etree_parse          | 120 ms                                                          | 114 ms: 1.05x faster                                            |
| python_startup           | 22.9 ms                                                         | 22.0 ms: 1.04x faster                                           |
| regex_v8                 | 15.8 ms                                                         | 15.2 ms: 1.04x faster                                           |
| crypto_pyaes             | 81.3 ms                                                         | 79.4 ms: 1.02x faster                                           |
| pathlib                  | 81.2 ms                                                         | 79.9 ms: 1.02x faster                                           |
| go                       | 146 ms                                                          | 147 ms: 1.01x slower                                            |
| pickle_list              | 3.22 us                                                         | 3.27 us: 1.02x slower                                           |
| deltablue                | 4.04 ms                                                         | 4.10 ms: 1.02x slower                                           |
| pickle                   | 7.83 us                                                         | 7.99 us: 1.02x slower                                           |
| aiohttp                  | 1.13 ms                                                         | 1.17 ms: 1.03x slower                                           |
| django_template          | 36.0 ms                                                         | 37.4 ms: 1.04x slower                                           |
| dask                     | 341 ms                                                          | 355 ms: 1.04x slower                                            |
| python_startup_no_site   | 18.1 ms                                                         | 18.8 ms: 1.04x slower                                           |
| html5lib                 | 52.1 ms                                                         | 54.3 ms: 1.04x slower                                           |
| asyncio_tcp              | 744 ms                                                          | 787 ms: 1.06x slower                                            |
| mypy2                    | 590 ms                                                          | 626 ms: 1.06x slower                                            |
| 2to3                     | 265 ms                                                          | 282 ms: 1.06x slower                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 75.6 ms: 1.07x slower                                           |
| bench_mp_pool            | 66.4 ms                                                         | 70.9 ms: 1.07x slower                                           |
| dulwich_log              | 58.5 ms                                                         | 62.8 ms: 1.07x slower                                           |
| gc_traversal             | 1.28 ms                                                         | 1.38 ms: 1.07x slower                                           |
| docutils                 | 1.95 sec                                                        | 2.10 sec: 1.08x slower                                          |
| async_generators         | 241 ms                                                          | 260 ms: 1.08x slower                                            |
| raytrace                 | 303 ms                                                          | 327 ms: 1.08x slower                                            |
| pylint                   | 384 ms                                                          | 418 ms: 1.09x slower                                            |
| float                    | 69.6 ms                                                         | 76.1 ms: 1.09x slower                                           |
| telco                    | 4.83 ms                                                         | 5.29 ms: 1.10x slower                                           |
| regex_effbot             | 1.66 ms                                                         | 1.82 ms: 1.10x slower                                           |
| unpickle_list            | 2.98 us                                                         | 3.28 us: 1.10x slower                                           |
| pickle_dict              | 18.2 us                                                         | 20.1 us: 1.10x slower                                           |
| pickle_pure_python       | 280 us                                                          | 309 us: 1.10x slower                                            |
| sqlalchemy_declarative   | 104 ms                                                          | 115 ms: 1.10x slower                                            |
| pyflate                  | 422 ms                                                          | 471 ms: 1.12x slower                                            |
| sqlglot_parse            | 1.33 ms                                                         | 1.49 ms: 1.12x slower                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.78 ms: 1.13x slower                                           |
| mako                     | 9.10 ms                                                         | 10.3 ms: 1.13x slower                                           |
| mdp                      | 1.83 sec                                                        | 2.07 sec: 1.13x slower                                          |
| chaos                    | 74.4 ms                                                         | 84.4 ms: 1.13x slower                                           |
| meteor_contest           | 80.0 ms                                                         | 90.9 ms: 1.14x slower                                           |
| scimark_lu               | 89.8 ms                                                         | 102 ms: 1.14x slower                                            |
| xml_etree_process        | 48.1 ms                                                         | 55.0 ms: 1.14x slower                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 70.8 ms: 1.14x slower                                           |
| sqlglot_optimize         | 44.7 ms                                                         | 51.8 ms: 1.16x slower                                           |
| xml_etree_generate       | 61.6 ms                                                         | 71.6 ms: 1.16x slower                                           |
| sqlalchemy_imperative    | 13.2 ms                                                         | 15.4 ms: 1.17x slower                                           |
| scimark_sor              | 115 ms                                                          | 135 ms: 1.18x slower                                            |
| richards_super           | 49.9 ms                                                         | 58.7 ms: 1.18x slower                                           |
| sympy_expand             | 391 ms                                                          | 462 ms: 1.18x slower                                            |
| sympy_integrate          | 16.6 ms                                                         | 19.9 ms: 1.20x slower                                           |
| typing_runtime_protocols | 396 us                                                          | 478 us: 1.21x slower                                            |
| tomli_loads              | 1.91 sec                                                        | 2.31 sec: 1.21x slower                                          |
| richards                 | 40.3 ms                                                         | 48.8 ms: 1.21x slower                                           |
| sympy_sum                | 122 ms                                                          | 149 ms: 1.22x slower                                            |
| logging_silent           | 97.9 ns                                                         | 119 ns: 1.22x slower                                            |
| unpickle_pure_python     | 189 us                                                          | 231 us: 1.22x slower                                            |
| hexiom                   | 6.13 ms                                                         | 7.51 ms: 1.22x slower                                           |
| deepcopy                 | 310 us                                                          | 381 us: 1.23x slower                                            |
| deepcopy_reduce          | 2.68 us                                                         | 3.32 us: 1.24x slower                                           |
| sympy_str                | 229 ms                                                          | 283 ms: 1.24x slower                                            |
| pprint_pformat           | 1.37 sec                                                        | 1.70 sec: 1.24x slower                                          |
| comprehensions           | 17.7 us                                                         | 22.1 us: 1.24x slower                                           |
| pprint_safe_repr         | 658 ms                                                          | 819 ms: 1.24x slower                                            |
| coverage                 | 46.6 ms                                                         | 58.0 ms: 1.25x slower                                           |
| chameleon                | 6.42 ms                                                         | 8.08 ms: 1.26x slower                                           |
| fannkuch                 | 317 ms                                                          | 399 ms: 1.26x slower                                            |
| regex_compile            | 117 ms                                                          | 148 ms: 1.26x slower                                            |
| genshi_text              | 21.0 ms                                                         | 26.8 ms: 1.27x slower                                           |
| nqueens                  | 87.1 ms                                                         | 111 ms: 1.28x slower                                            |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 4.23 ms: 1.31x slower                                           |
| genshi_xml               | 46.6 ms                                                         | 61.2 ms: 1.31x slower                                           |
| coroutines               | 17.9 ms                                                         | 23.7 ms: 1.32x slower                                           |
| scimark_fft              | 216 ms                                                          | 291 ms: 1.35x slower                                            |
| deepcopy_memo            | 29.6 us                                                         | 40.0 us: 1.35x slower                                           |
| logging_format           | 7.91 us                                                         | 11.5 us: 1.45x slower                                           |
| logging_simple           | 7.29 us                                                         | 10.8 us: 1.48x slower                                           |
| spectral_norm            | 80.2 ms                                                         | 122 ms: 1.52x slower                                            |
| nbody                    | 79.1 ms                                                         | 126 ms: 1.59x slower                                            |
| unpack_sequence          | 40.0 ns                                                         | 65.2 ns: 1.63x slower                                           |
| generators               | 31.6 ms                                                         | 52.2 ms: 1.65x slower                                           |
| Geometric mean           | (ref)                                                           | 1.10x slower                                                    |

Benchmark hidden because not significant (7): json_dumps, flaskblogging, pycparser, json, asyncio_tcp_ssl, tornado_http, bench_thread_pool
Ignored benchmarks (4) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1_win32-x86-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.07x
- 95% likely to have a slowdown of 1.07x
- 99% likely to have a slowdown of 1.06x


# Memory

- memory change: unknown