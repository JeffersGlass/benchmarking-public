
# Results vs. 3.10.4

- fork: python
- ref: 5a1b5316af648ae79bb9
- machine: windows-x86
- commit hash: 5a1b531
- commit date: 2023-12-03
- overall geometric mean: 1.15x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 312 ms: 1.17x slower                                                            |
| chameleon      | 6.42 ms                                                         | 9.94 ms: 1.55x slower                                                           |
| docutils       | 1.95 sec                                                        | 2.15 sec: 1.10x slower                                                          |
| tornado_http   | 118 ms                                                          | 113 ms: 1.04x faster                                                            |
| Geometric mean | (ref)                                                           | 1.18x slower                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 592 ms: 1.56x faster                                                            |
| async_tree_io           | 940 ms                                                          | 782 ms: 1.20x faster                                                            |
| async_tree_none         | 394 ms                                                          | 330 ms: 1.19x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 412 ms: 1.13x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.26x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 200 ms: 2.51x faster                                                            |
| float          | 69.6 ms                                                         | 68.7 ms: 1.01x faster                                                           |
| nbody          | 79.1 ms                                                         | 98.2 ms: 1.24x slower                                                           |
| Geometric mean | (ref)                                                           | 1.27x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 123 ms: 1.06x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 17.2 ms: 1.09x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.94 ms: 1.17x slower                                                           |
| regex_compile  | 117 ms                                                          | 149 ms: 1.28x slower                                                            |
| Geometric mean | (ref)                                                           | 1.11x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 8.30 ms: 1.18x faster                                                           |
| unpickle_list        | 2.98 us                                                         | 2.71 us: 1.10x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 111 ms: 1.08x faster                                                            |
| json_loads           | 22.4 us                                                         | 21.0 us: 1.07x faster                                                           |
| pickle               | 7.83 us                                                         | 7.54 us: 1.04x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.17 us: 1.02x faster                                                           |
| unpickle             | 9.82 us                                                         | 9.71 us: 1.01x faster                                                           |
| pickle_dict          | 18.2 us                                                         | 19.8 us: 1.08x slower                                                           |
| xml_etree_iterparse  | 70.8 ms                                                         | 78.3 ms: 1.11x slower                                                           |
| tomli_loads          | 1.91 sec                                                        | 2.21 sec: 1.16x slower                                                          |
| xml_etree_process    | 48.1 ms                                                         | 64.6 ms: 1.34x slower                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 83.0 ms: 1.35x slower                                                           |
| pickle_pure_python   | 280 us                                                          | 385 us: 1.37x slower                                                            |
| unpickle_pure_python | 189 us                                                          | 304 us: 1.60x slower                                                            |
| Geometric mean       | (ref)                                                           | 1.09x slower                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup_no_site | 18.1 ms                                                         | 20.5 ms: 1.14x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.06x slower                                                                    |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 8.09 ms: 1.13x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 132 us: 3.00x faster                                                            |
| pidigits                 | 502 ms                                                          | 200 ms: 2.51x faster                                                            |
| sqlglot_normalize        | 230 ms                                                          | 120 ms: 1.91x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 592 ms: 1.56x faster                                                            |
| crypto_pyaes             | 81.3 ms                                                         | 66.0 ms: 1.23x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.89 us: 1.21x faster                                                           |
| async_tree_io            | 940 ms                                                          | 782 ms: 1.20x faster                                                            |
| async_tree_none          | 394 ms                                                          | 330 ms: 1.19x faster                                                            |
| json_dumps               | 9.82 ms                                                         | 8.30 ms: 1.18x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 412 ms: 1.13x faster                                                            |
| mako                     | 9.10 ms                                                         | 8.09 ms: 1.13x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 674 ms: 1.10x faster                                                            |
| unpickle_list            | 2.98 us                                                         | 2.71 us: 1.10x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 642 us: 1.08x faster                                                            |
| json                     | 4.76 ms                                                         | 4.41 ms: 1.08x faster                                                           |
| xml_etree_parse          | 120 ms                                                          | 111 ms: 1.08x faster                                                            |
| json_loads               | 22.4 us                                                         | 21.0 us: 1.07x faster                                                           |
| regex_dna                | 131 ms                                                          | 123 ms: 1.06x faster                                                            |
| tornado_http             | 118 ms                                                          | 113 ms: 1.04x faster                                                            |
| pickle                   | 7.83 us                                                         | 7.54 us: 1.04x faster                                                           |
| pickle_list              | 3.22 us                                                         | 3.17 us: 1.02x faster                                                           |
| float                    | 69.6 ms                                                         | 68.7 ms: 1.01x faster                                                           |
| unpickle                 | 9.82 us                                                         | 9.71 us: 1.01x faster                                                           |
| deltablue                | 4.04 ms                                                         | 4.01 ms: 1.01x faster                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.3 sec: 1.02x slower                                                          |
| dask                     | 341 ms                                                          | 353 ms: 1.03x slower                                                            |
| sympy_sum                | 122 ms                                                          | 127 ms: 1.04x slower                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.18 ms: 1.05x slower                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.45 ms: 1.06x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 19.8 us: 1.08x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.39 ms: 1.08x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 72.4 ms: 1.09x slower                                                           |
| scimark_fft              | 216 ms                                                          | 236 ms: 1.09x slower                                                            |
| regex_v8                 | 15.8 ms                                                         | 17.2 ms: 1.09x slower                                                           |
| docutils                 | 1.95 sec                                                        | 2.15 sec: 1.10x slower                                                          |
| pathlib                  | 81.2 ms                                                         | 89.6 ms: 1.10x slower                                                           |
| xml_etree_iterparse      | 70.8 ms                                                         | 78.3 ms: 1.11x slower                                                           |
| pycparser                | 1.04 sec                                                        | 1.15 sec: 1.11x slower                                                          |
| spectral_norm            | 80.2 ms                                                         | 89.8 ms: 1.12x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 20.5 ms: 1.14x slower                                                           |
| mdp                      | 1.83 sec                                                        | 2.08 sec: 1.14x slower                                                          |
| nqueens                  | 87.1 ms                                                         | 99.7 ms: 1.15x slower                                                           |
| sympy_str                | 229 ms                                                          | 264 ms: 1.15x slower                                                            |
| tomli_loads              | 1.91 sec                                                        | 2.21 sec: 1.16x slower                                                          |
| pyflate                  | 422 ms                                                          | 488 ms: 1.16x slower                                                            |
| sympy_integrate          | 16.6 ms                                                         | 19.4 ms: 1.16x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.94 ms: 1.17x slower                                                           |
| meteor_contest           | 80.0 ms                                                         | 93.7 ms: 1.17x slower                                                           |
| raytrace                 | 303 ms                                                          | 354 ms: 1.17x slower                                                            |
| 2to3                     | 265 ms                                                          | 312 ms: 1.17x slower                                                            |
| sympy_expand             | 391 ms                                                          | 463 ms: 1.18x slower                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 1.60 ms: 1.20x slower                                                           |
| hexiom                   | 6.13 ms                                                         | 7.45 ms: 1.21x slower                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.93 ms: 1.22x slower                                                           |
| nbody                    | 79.1 ms                                                         | 98.2 ms: 1.24x slower                                                           |
| fannkuch                 | 317 ms                                                          | 399 ms: 1.26x slower                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 56.6 ms: 1.27x slower                                                           |
| go                       | 146 ms                                                          | 185 ms: 1.27x slower                                                            |
| regex_compile            | 117 ms                                                          | 149 ms: 1.28x slower                                                            |
| scimark_monte_carlo      | 61.9 ms                                                         | 79.6 ms: 1.29x slower                                                           |
| xml_etree_process        | 48.1 ms                                                         | 64.6 ms: 1.34x slower                                                           |
| xml_etree_generate       | 61.6 ms                                                         | 83.0 ms: 1.35x slower                                                           |
| richards_super           | 49.9 ms                                                         | 67.7 ms: 1.36x slower                                                           |
| pickle_pure_python       | 280 us                                                          | 385 us: 1.37x slower                                                            |
| pprint_pformat           | 1.37 sec                                                        | 1.90 sec: 1.39x slower                                                          |
| pprint_safe_repr         | 658 ms                                                          | 936 ms: 1.42x slower                                                            |
| deepcopy                 | 310 us                                                          | 443 us: 1.43x slower                                                            |
| deepcopy_reduce          | 2.68 us                                                         | 3.89 us: 1.45x slower                                                           |
| logging_format           | 7.91 us                                                         | 11.5 us: 1.45x slower                                                           |
| telco                    | 4.83 ms                                                         | 7.09 ms: 1.47x slower                                                           |
| scimark_lu               | 89.8 ms                                                         | 133 ms: 1.48x slower                                                            |
| async_generators         | 241 ms                                                          | 357 ms: 1.48x slower                                                            |
| logging_simple           | 7.29 us                                                         | 10.8 us: 1.48x slower                                                           |
| richards                 | 40.3 ms                                                         | 61.5 ms: 1.53x slower                                                           |
| chameleon                | 6.42 ms                                                         | 9.94 ms: 1.55x slower                                                           |
| logging_silent           | 97.9 ns                                                         | 156 ns: 1.59x slower                                                            |
| unpickle_pure_python     | 189 us                                                          | 304 us: 1.60x slower                                                            |
| scimark_sor              | 115 ms                                                          | 186 ms: 1.62x slower                                                            |
| deepcopy_memo            | 29.6 us                                                         | 50.7 us: 1.71x slower                                                           |
| coroutines               | 17.9 ms                                                         | 31.9 ms: 1.78x slower                                                           |
| generators               | 31.6 ms                                                         | 56.9 ms: 1.80x slower                                                           |
| unpack_sequence          | 40.0 ns                                                         | 97.7 ns: 2.44x slower                                                           |
| coverage                 | 46.6 ms                                                         | 774 ms: 16.62x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.15x slower                                                                    |

Benchmark hidden because not significant (3): python_startup, chaos, comprehensions
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231203-3.13.0a2+-5a1b531-PYTHON_UOPS/bm-20231203-pythonperf1_win32-x86-python-5a1b5316af648ae79bb9-3.13.0a2+-5a1b531.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.10x
- 95% likely to have a slowdown of 1.09x
- 99% likely to have a slowdown of 1.07x


# Memory

- memory change: unknown