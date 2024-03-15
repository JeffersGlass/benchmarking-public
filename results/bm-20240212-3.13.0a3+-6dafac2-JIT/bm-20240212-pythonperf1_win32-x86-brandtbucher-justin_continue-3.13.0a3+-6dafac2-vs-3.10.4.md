
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_continue
- machine: windows-x86
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.12x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 247 ms: 1.07x faster                                                             |
| chameleon      | 6.42 ms                                                         | 5.91 ms: 1.09x faster                                                            |
| docutils       | 1.95 sec                                                        | 1.77 sec: 1.10x faster                                                           |
| tornado_http   | 118 ms                                                          | 96.4 ms: 1.22x faster                                                            |
| Geometric mean | (ref)                                                           | 1.12x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 510 ms: 1.81x faster                                                             |
| async_tree_none         | 394 ms                                                          | 250 ms: 1.57x faster                                                             |
| async_tree_io           | 940 ms                                                          | 601 ms: 1.56x faster                                                             |
| async_tree_memoization  | 467 ms                                                          | 313 ms: 1.49x faster                                                             |
| Geometric mean          | (ref)                                                           | 1.60x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 201 ms: 2.51x faster                                                             |
| float          | 69.6 ms                                                         | 53.8 ms: 1.29x faster                                                            |
| nbody          | 79.1 ms                                                         | 93.5 ms: 1.18x slower                                                            |
| Geometric mean | (ref)                                                           | 1.40x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 103 ms: 1.13x faster                                                             |
| regex_dna      | 131 ms                                                          | 123 ms: 1.06x faster                                                             |
| regex_v8       | 15.8 ms                                                         | 16.1 ms: 1.02x slower                                                            |
| regex_effbot   | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                            |
| Geometric mean | (ref)                                                           | 1.00x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.84 ms: 1.44x faster                                                            |
| pickle_pure_python   | 280 us                                                          | 210 us: 1.34x faster                                                             |
| unpickle_pure_python | 189 us                                                          | 155 us: 1.23x faster                                                             |
| tomli_loads          | 1.91 sec                                                        | 1.60 sec: 1.20x faster                                                           |
| xml_etree_process    | 48.1 ms                                                         | 41.5 ms: 1.16x faster                                                            |
| json_loads           | 22.4 us                                                         | 20.1 us: 1.11x faster                                                            |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.11x faster                                                             |
| unpickle_list        | 2.98 us                                                         | 2.82 us: 1.06x faster                                                            |
| xml_etree_generate   | 61.6 ms                                                         | 58.4 ms: 1.06x faster                                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 67.8 ms: 1.04x faster                                                            |
| pickle               | 7.83 us                                                         | 8.00 us: 1.02x slower                                                            |
| unpickle             | 9.82 us                                                         | 10.1 us: 1.03x slower                                                            |
| pickle_list          | 3.22 us                                                         | 3.37 us: 1.05x slower                                                            |
| pickle_dict          | 18.2 us                                                         | 19.7 us: 1.08x slower                                                            |
| Geometric mean       | (ref)                                                           | 1.10x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 22.3 ms: 1.03x faster                                                            |
| python_startup_no_site | 18.1 ms                                                         | 20.2 ms: 1.12x slower                                                            |
| Geometric mean         | (ref)                                                           | 1.04x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.60 ms: 1.20x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|--------------------------|:---------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 94.9 us: 4.17x faster                                                            |
| pidigits                 | 502 ms                                                          | 201 ms: 2.51x faster                                                             |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 510 ms: 1.81x faster                                                             |
| deltablue                | 4.04 ms                                                         | 2.37 ms: 1.70x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 61.0 ns: 1.61x faster                                                            |
| async_tree_none          | 394 ms                                                          | 250 ms: 1.57x faster                                                             |
| async_tree_io            | 940 ms                                                          | 601 ms: 1.56x faster                                                             |
| async_tree_memoization   | 467 ms                                                          | 313 ms: 1.49x faster                                                             |
| richards_super           | 49.9 ms                                                         | 33.5 ms: 1.49x faster                                                            |
| scimark_lu               | 89.8 ms                                                         | 60.5 ms: 1.48x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 920 us: 1.44x faster                                                             |
| json_dumps               | 9.82 ms                                                         | 6.84 ms: 1.44x faster                                                            |
| richards                 | 40.3 ms                                                         | 28.5 ms: 1.41x faster                                                            |
| generators               | 31.6 ms                                                         | 22.5 ms: 1.40x faster                                                            |
| scimark_sor              | 115 ms                                                          | 83.5 ms: 1.38x faster                                                            |
| sqlglot_transpile        | 1.58 ms                                                         | 1.16 ms: 1.37x faster                                                            |
| raytrace                 | 303 ms                                                          | 224 ms: 1.35x faster                                                             |
| pickle_pure_python       | 280 us                                                          | 210 us: 1.34x faster                                                             |
| crypto_pyaes             | 81.3 ms                                                         | 61.4 ms: 1.32x faster                                                            |
| float                    | 69.6 ms                                                         | 53.8 ms: 1.29x faster                                                            |
| chaos                    | 74.4 ms                                                         | 58.5 ms: 1.27x faster                                                            |
| pycparser                | 1.04 sec                                                        | 821 ms: 1.27x faster                                                             |
| go                       | 146 ms                                                          | 116 ms: 1.26x faster                                                             |
| deepcopy_memo            | 29.6 us                                                         | 23.6 us: 1.26x faster                                                            |
| coroutines               | 17.9 ms                                                         | 14.4 ms: 1.24x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 155 us: 1.23x faster                                                             |
| tornado_http             | 118 ms                                                          | 96.4 ms: 1.22x faster                                                            |
| sqlite_synth             | 2.29 us                                                         | 1.89 us: 1.21x faster                                                            |
| mako                     | 9.10 ms                                                         | 7.60 ms: 1.20x faster                                                            |
| tomli_loads              | 1.91 sec                                                        | 1.60 sec: 1.20x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 627 ms: 1.19x faster                                                             |
| comprehensions           | 17.7 us                                                         | 15.0 us: 1.19x faster                                                            |
| xml_etree_process        | 48.1 ms                                                         | 41.5 ms: 1.16x faster                                                            |
| dask                     | 341 ms                                                          | 296 ms: 1.15x faster                                                             |
| json                     | 4.76 ms                                                         | 4.19 ms: 1.14x faster                                                            |
| pyflate                  | 422 ms                                                          | 372 ms: 1.14x faster                                                             |
| regex_compile            | 117 ms                                                          | 103 ms: 1.13x faster                                                             |
| deepcopy                 | 310 us                                                          | 277 us: 1.12x faster                                                             |
| sympy_sum                | 122 ms                                                          | 110 ms: 1.11x faster                                                             |
| json_loads               | 22.4 us                                                         | 20.1 us: 1.11x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.01 ms: 1.11x faster                                                            |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.11x faster                                                             |
| deepcopy_reduce          | 2.68 us                                                         | 2.43 us: 1.10x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.77 sec: 1.10x faster                                                           |
| chameleon                | 6.42 ms                                                         | 5.91 ms: 1.09x faster                                                            |
| create_gc_cycles         | 694 us                                                          | 646 us: 1.07x faster                                                             |
| 2to3                     | 265 ms                                                          | 247 ms: 1.07x faster                                                             |
| sympy_str                | 229 ms                                                          | 213 ms: 1.07x faster                                                             |
| sqlglot_normalize        | 230 ms                                                          | 215 ms: 1.07x faster                                                             |
| sympy_expand             | 391 ms                                                          | 366 ms: 1.07x faster                                                             |
| sympy_integrate          | 16.6 ms                                                         | 15.6 ms: 1.06x faster                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 42.1 ms: 1.06x faster                                                            |
| spectral_norm            | 80.2 ms                                                         | 75.5 ms: 1.06x faster                                                            |
| regex_dna                | 131 ms                                                          | 123 ms: 1.06x faster                                                             |
| unpickle_list            | 2.98 us                                                         | 2.82 us: 1.06x faster                                                            |
| xml_etree_generate       | 61.6 ms                                                         | 58.4 ms: 1.06x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 67.8 ms: 1.04x faster                                                            |
| python_startup           | 22.9 ms                                                         | 22.3 ms: 1.03x faster                                                            |
| fannkuch                 | 317 ms                                                          | 315 ms: 1.01x faster                                                             |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.22 ms: 1.01x faster                                                            |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.9 sec: 1.01x faster                                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.39 sec: 1.01x slower                                                           |
| pprint_safe_repr         | 658 ms                                                          | 670 ms: 1.02x slower                                                             |
| mdp                      | 1.83 sec                                                        | 1.86 sec: 1.02x slower                                                           |
| pickle                   | 7.83 us                                                         | 8.00 us: 1.02x slower                                                            |
| regex_v8                 | 15.8 ms                                                         | 16.1 ms: 1.02x slower                                                            |
| meteor_contest           | 80.0 ms                                                         | 82.0 ms: 1.03x slower                                                            |
| hexiom                   | 6.13 ms                                                         | 6.30 ms: 1.03x slower                                                            |
| unpack_sequence          | 40.0 ns                                                         | 41.3 ns: 1.03x slower                                                            |
| unpickle                 | 9.82 us                                                         | 10.1 us: 1.03x slower                                                            |
| pathlib                  | 81.2 ms                                                         | 84.1 ms: 1.04x slower                                                            |
| pickle_list              | 3.22 us                                                         | 3.37 us: 1.05x slower                                                            |
| nqueens                  | 87.1 ms                                                         | 91.6 ms: 1.05x slower                                                            |
| bench_mp_pool            | 66.4 ms                                                         | 70.7 ms: 1.07x slower                                                            |
| gc_traversal             | 1.28 ms                                                         | 1.38 ms: 1.08x slower                                                            |
| pickle_dict              | 18.2 us                                                         | 19.7 us: 1.08x slower                                                            |
| logging_format           | 7.91 us                                                         | 8.60 us: 1.09x slower                                                            |
| logging_simple           | 7.29 us                                                         | 8.01 us: 1.10x slower                                                            |
| scimark_monte_carlo      | 61.9 ms                                                         | 68.3 ms: 1.10x slower                                                            |
| python_startup_no_site   | 18.1 ms                                                         | 20.2 ms: 1.12x slower                                                            |
| async_generators         | 241 ms                                                          | 277 ms: 1.15x slower                                                             |
| regex_effbot             | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                            |
| scimark_fft              | 216 ms                                                          | 251 ms: 1.16x slower                                                             |
| nbody                    | 79.1 ms                                                         | 93.5 ms: 1.18x slower                                                            |
| telco                    | 4.83 ms                                                         | 6.56 ms: 1.36x slower                                                            |
| coverage                 | 46.6 ms                                                         | 467 ms: 10.03x slower                                                            |
| Geometric mean           | (ref)                                                           | 1.12x faster                                                                     |
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240212-3.13.0a3+-6dafac2-JIT/bm-20240212-pythonperf1_win32-x86-brandtbucher-justin_continue-3.13.0a3+-6dafac2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.06x


# Memory

- memory change: unknown