# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_mprotect
- machine: windows-x86
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.09x faster \*
- HPT reliability: 99.97%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 260 ms: 1.02x faster                                                             |
| chameleon      | 6.42 ms                                                         | 5.66 ms: 1.13x faster                                                            |
| docutils       | 1.95 sec                                                        | 1.81 sec: 1.07x faster                                                           |
| tornado_http   | 118 ms                                                          | 96.7 ms: 1.22x faster                                                            |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 517 ms: 1.78x faster                                                             |
| async_tree_none         | 394 ms                                                          | 258 ms: 1.52x faster                                                             |
| async_tree_io           | 940 ms                                                          | 624 ms: 1.51x faster                                                             |
| async_tree_memoization  | 467 ms                                                          | 323 ms: 1.45x faster                                                             |
| Geometric mean          | (ref)                                                           | 1.56x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.54x faster                                                             |
| float          | 69.6 ms                                                         | 54.9 ms: 1.27x faster                                                            |
| nbody          | 79.1 ms                                                         | 96.4 ms: 1.22x slower                                                            |
| Geometric mean | (ref)                                                           | 1.38x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 121 ms: 1.08x faster                                                             |
| regex_compile  | 117 ms                                                          | 109 ms: 1.07x faster                                                             |
| regex_v8       | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                            |
| regex_effbot   | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                            |
| Geometric mean | (ref)                                                           | 1.00x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.86 ms: 1.43x faster                                                            |
| pickle_pure_python   | 280 us                                                          | 210 us: 1.33x faster                                                             |
| xml_etree_process    | 48.1 ms                                                         | 42.1 ms: 1.14x faster                                                            |
| json_loads           | 22.4 us                                                         | 20.1 us: 1.11x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.72 sec: 1.11x faster                                                           |
| unpickle_pure_python | 189 us                                                          | 171 us: 1.11x faster                                                             |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                                             |
| unpickle_list        | 2.98 us                                                         | 2.81 us: 1.06x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 67.3 ms: 1.05x faster                                                            |
| xml_etree_generate   | 61.6 ms                                                         | 59.6 ms: 1.03x faster                                                            |
| pickle_list          | 3.22 us                                                         | 3.17 us: 1.01x faster                                                            |
| pickle               | 7.83 us                                                         | 7.94 us: 1.01x slower                                                            |
| unpickle             | 9.82 us                                                         | 10.1 us: 1.02x slower                                                            |
| pickle_dict          | 18.2 us                                                         | 20.0 us: 1.10x slower                                                            |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 25.7 ms: 1.12x slower                                                            |
| python_startup_no_site | 18.1 ms                                                         | 23.6 ms: 1.31x slower                                                            |
| Geometric mean         | (ref)                                                           | 1.21x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.30 ms: 1.25x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|--------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 92.1 us: 4.30x faster                                                            |
| pidigits                 | 502 ms                                                          | 198 ms: 2.54x faster                                                             |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 517 ms: 1.78x faster                                                             |
| logging_silent           | 97.9 ns                                                         | 59.6 ns: 1.64x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.59 ms: 1.56x faster                                                            |
| async_tree_none          | 394 ms                                                          | 258 ms: 1.52x faster                                                             |
| async_tree_io            | 940 ms                                                          | 624 ms: 1.51x faster                                                             |
| async_tree_memoization   | 467 ms                                                          | 323 ms: 1.45x faster                                                             |
| json_dumps               | 9.82 ms                                                         | 6.86 ms: 1.43x faster                                                            |
| generators               | 31.6 ms                                                         | 23.0 ms: 1.37x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 979 us: 1.36x faster                                                             |
| crypto_pyaes             | 81.3 ms                                                         | 60.3 ms: 1.35x faster                                                            |
| pickle_pure_python       | 280 us                                                          | 210 us: 1.33x faster                                                             |
| sqlglot_transpile        | 1.58 ms                                                         | 1.23 ms: 1.29x faster                                                            |
| richards_super           | 49.9 ms                                                         | 39.2 ms: 1.27x faster                                                            |
| coroutines               | 17.9 ms                                                         | 14.1 ms: 1.27x faster                                                            |
| float                    | 69.6 ms                                                         | 54.9 ms: 1.27x faster                                                            |
| mako                     | 9.10 ms                                                         | 7.30 ms: 1.25x faster                                                            |
| chaos                    | 74.4 ms                                                         | 60.3 ms: 1.23x faster                                                            |
| deepcopy_memo            | 29.6 us                                                         | 24.3 us: 1.22x faster                                                            |
| tornado_http             | 118 ms                                                          | 96.7 ms: 1.22x faster                                                            |
| comprehensions           | 17.7 us                                                         | 14.6 us: 1.21x faster                                                            |
| pycparser                | 1.04 sec                                                        | 859 ms: 1.21x faster                                                             |
| go                       | 146 ms                                                          | 120 ms: 1.21x faster                                                             |
| sqlite_synth             | 2.29 us                                                         | 1.93 us: 1.19x faster                                                            |
| asyncio_tcp              | 744 ms                                                          | 638 ms: 1.17x faster                                                             |
| richards                 | 40.3 ms                                                         | 34.9 ms: 1.15x faster                                                            |
| scimark_sor              | 115 ms                                                          | 100 ms: 1.15x faster                                                             |
| sympy_sum                | 122 ms                                                          | 107 ms: 1.15x faster                                                             |
| xml_etree_process        | 48.1 ms                                                         | 42.1 ms: 1.14x faster                                                            |
| json                     | 4.76 ms                                                         | 4.19 ms: 1.14x faster                                                            |
| chameleon                | 6.42 ms                                                         | 5.66 ms: 1.13x faster                                                            |
| spectral_norm            | 80.2 ms                                                         | 71.2 ms: 1.13x faster                                                            |
| deepcopy                 | 310 us                                                          | 278 us: 1.11x faster                                                             |
| json_loads               | 22.4 us                                                         | 20.1 us: 1.11x faster                                                            |
| tomli_loads              | 1.91 sec                                                        | 1.72 sec: 1.11x faster                                                           |
| unpickle_pure_python     | 189 us                                                          | 171 us: 1.11x faster                                                             |
| pyflate                  | 422 ms                                                          | 382 ms: 1.10x faster                                                             |
| raytrace                 | 303 ms                                                          | 275 ms: 1.10x faster                                                             |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                                             |
| sympy_str                | 229 ms                                                          | 210 ms: 1.09x faster                                                             |
| bench_thread_pool        | 1.12 ms                                                         | 1.03 ms: 1.08x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 15.4 ms: 1.08x faster                                                            |
| regex_dna                | 131 ms                                                          | 121 ms: 1.08x faster                                                             |
| scimark_lu               | 89.8 ms                                                         | 83.5 ms: 1.08x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.81 sec: 1.07x faster                                                           |
| deepcopy_reduce          | 2.68 us                                                         | 2.51 us: 1.07x faster                                                            |
| sqlglot_normalize        | 230 ms                                                          | 216 ms: 1.07x faster                                                             |
| regex_compile            | 117 ms                                                          | 109 ms: 1.07x faster                                                             |
| unpickle_list            | 2.98 us                                                         | 2.81 us: 1.06x faster                                                            |
| sympy_expand             | 391 ms                                                          | 370 ms: 1.06x faster                                                             |
| xml_etree_iterparse      | 70.8 ms                                                         | 67.3 ms: 1.05x faster                                                            |
| mdp                      | 1.83 sec                                                        | 1.74 sec: 1.05x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 665 us: 1.04x faster                                                             |
| xml_etree_generate       | 61.6 ms                                                         | 59.6 ms: 1.03x faster                                                            |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.15 ms: 1.03x faster                                                            |
| 2to3                     | 265 ms                                                          | 260 ms: 1.02x faster                                                             |
| pickle_list              | 3.22 us                                                         | 3.17 us: 1.01x faster                                                            |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                                           |
| hexiom                   | 6.13 ms                                                         | 6.21 ms: 1.01x slower                                                            |
| pickle                   | 7.83 us                                                         | 7.94 us: 1.01x slower                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 45.3 ms: 1.01x slower                                                            |
| regex_v8                 | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                            |
| unpickle                 | 9.82 us                                                         | 10.1 us: 1.02x slower                                                            |
| meteor_contest           | 80.0 ms                                                         | 82.8 ms: 1.04x slower                                                            |
| pathlib                  | 81.2 ms                                                         | 84.2 ms: 1.04x slower                                                            |
| scimark_monte_carlo      | 61.9 ms                                                         | 64.9 ms: 1.05x slower                                                            |
| nqueens                  | 87.1 ms                                                         | 91.4 ms: 1.05x slower                                                            |
| unpack_sequence          | 40.0 ns                                                         | 43.1 ns: 1.08x slower                                                            |
| scimark_fft              | 216 ms                                                          | 233 ms: 1.08x slower                                                             |
| fannkuch                 | 317 ms                                                          | 344 ms: 1.09x slower                                                             |
| pickle_dict              | 18.2 us                                                         | 20.0 us: 1.10x slower                                                            |
| pprint_pformat           | 1.37 sec                                                        | 1.51 sec: 1.10x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.74 us: 1.11x slower                                                            |
| gc_traversal             | 1.28 ms                                                         | 1.42 ms: 1.11x slower                                                            |
| bench_mp_pool            | 66.4 ms                                                         | 73.9 ms: 1.11x slower                                                            |
| pprint_safe_repr         | 658 ms                                                          | 735 ms: 1.12x slower                                                             |
| logging_simple           | 7.29 us                                                         | 8.15 us: 1.12x slower                                                            |
| python_startup           | 22.9 ms                                                         | 25.7 ms: 1.12x slower                                                            |
| regex_effbot             | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                            |
| async_generators         | 241 ms                                                          | 292 ms: 1.21x slower                                                             |
| dask                     | 341 ms                                                          | 413 ms: 1.21x slower                                                             |
| nbody                    | 79.1 ms                                                         | 96.4 ms: 1.22x slower                                                            |
| python_startup_no_site   | 18.1 ms                                                         | 23.6 ms: 1.31x slower                                                            |
| telco                    | 4.83 ms                                                         | 6.43 ms: 1.33x slower                                                            |
| coverage                 | 46.6 ms                                                         | 477 ms: 10.24x slower                                                            |
| Geometric mean           | (ref)                                                           | 1.09x faster                                                                     |
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-84bbac4-JIT/bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.97% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown