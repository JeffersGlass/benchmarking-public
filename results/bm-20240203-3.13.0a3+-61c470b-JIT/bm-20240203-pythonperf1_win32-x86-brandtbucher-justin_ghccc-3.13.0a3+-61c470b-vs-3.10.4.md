
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_ghccc
- machine: windows-x86
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.17x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 247 ms: 1.08x faster                                                          |
| chameleon      | 6.42 ms                                                         | 5.72 ms: 1.12x faster                                                         |
| docutils       | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                        |
| tornado_http   | 118 ms                                                          | 99.1 ms: 1.19x faster                                                         |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 522 ms: 1.77x faster                                                          |
| async_tree_none         | 394 ms                                                          | 246 ms: 1.60x faster                                                          |
| async_tree_io           | 940 ms                                                          | 599 ms: 1.57x faster                                                          |
| async_tree_memoization  | 467 ms                                                          | 314 ms: 1.49x faster                                                          |
| Geometric mean          | (ref)                                                           | 1.60x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 202 ms: 2.48x faster                                                          |
| float          | 69.6 ms                                                         | 49.8 ms: 1.40x faster                                                         |
| nbody          | 79.1 ms                                                         | 61.4 ms: 1.29x faster                                                         |
| Geometric mean | (ref)                                                           | 1.65x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 99.2 ms: 1.18x faster                                                         |
| regex_dna      | 131 ms                                                          | 121 ms: 1.08x faster                                                          |
| regex_v8       | 15.8 ms                                                         | 16.4 ms: 1.04x slower                                                         |
| regex_effbot   | 1.66 ms                                                         | 1.93 ms: 1.16x slower                                                         |
| Geometric mean | (ref)                                                           | 1.01x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.66 ms: 1.47x faster                                                         |
| pickle_pure_python   | 280 us                                                          | 209 us: 1.34x faster                                                          |
| tomli_loads          | 1.91 sec                                                        | 1.46 sec: 1.31x faster                                                        |
| unpickle_pure_python | 189 us                                                          | 147 us: 1.28x faster                                                          |
| xml_etree_process    | 48.1 ms                                                         | 40.5 ms: 1.19x faster                                                         |
| json_loads           | 22.4 us                                                         | 20.3 us: 1.10x faster                                                         |
| xml_etree_parse      | 120 ms                                                          | 110 ms: 1.09x faster                                                          |
| xml_etree_iterparse  | 70.8 ms                                                         | 65.0 ms: 1.09x faster                                                         |
| xml_etree_generate   | 61.6 ms                                                         | 57.8 ms: 1.07x faster                                                         |
| pickle_list          | 3.22 us                                                         | 3.24 us: 1.01x slower                                                         |
| unpickle_list        | 2.98 us                                                         | 3.04 us: 1.02x slower                                                         |
| unpickle             | 9.82 us                                                         | 10.2 us: 1.04x slower                                                         |
| pickle               | 7.83 us                                                         | 8.11 us: 1.04x slower                                                         |
| pickle_dict          | 18.2 us                                                         | 19.8 us: 1.09x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.12x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.2 ms: 1.01x slower                                                         |
| python_startup_no_site | 18.1 ms                                                         | 21.1 ms: 1.17x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.09x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 6.37 ms: 1.43x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|--------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 98.0 us: 4.04x faster                                                         |
| pidigits                 | 502 ms                                                          | 202 ms: 2.48x faster                                                          |
| deltablue                | 4.04 ms                                                         | 2.18 ms: 1.85x faster                                                         |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 522 ms: 1.77x faster                                                          |
| async_tree_none          | 394 ms                                                          | 246 ms: 1.60x faster                                                          |
| logging_silent           | 97.9 ns                                                         | 61.2 ns: 1.60x faster                                                         |
| crypto_pyaes             | 81.3 ms                                                         | 51.1 ms: 1.59x faster                                                         |
| async_tree_io            | 940 ms                                                          | 599 ms: 1.57x faster                                                          |
| sqlglot_parse            | 1.33 ms                                                         | 884 us: 1.50x faster                                                          |
| richards_super           | 49.9 ms                                                         | 33.4 ms: 1.49x faster                                                         |
| async_tree_memoization   | 467 ms                                                          | 314 ms: 1.49x faster                                                          |
| scimark_lu               | 89.8 ms                                                         | 60.7 ms: 1.48x faster                                                         |
| json_dumps               | 9.82 ms                                                         | 6.66 ms: 1.47x faster                                                         |
| comprehensions           | 17.7 us                                                         | 12.1 us: 1.47x faster                                                         |
| chaos                    | 74.4 ms                                                         | 51.6 ms: 1.44x faster                                                         |
| mako                     | 9.10 ms                                                         | 6.37 ms: 1.43x faster                                                         |
| raytrace                 | 303 ms                                                          | 213 ms: 1.42x faster                                                          |
| generators               | 31.6 ms                                                         | 22.2 ms: 1.42x faster                                                         |
| sqlglot_transpile        | 1.58 ms                                                         | 1.12 ms: 1.41x faster                                                         |
| scimark_sor              | 115 ms                                                          | 82.3 ms: 1.40x faster                                                         |
| float                    | 69.6 ms                                                         | 49.8 ms: 1.40x faster                                                         |
| richards                 | 40.3 ms                                                         | 29.5 ms: 1.36x faster                                                         |
| pickle_pure_python       | 280 us                                                          | 209 us: 1.34x faster                                                          |
| tomli_loads              | 1.91 sec                                                        | 1.46 sec: 1.31x faster                                                        |
| pyflate                  | 422 ms                                                          | 325 ms: 1.30x faster                                                          |
| deepcopy_memo            | 29.6 us                                                         | 22.8 us: 1.30x faster                                                         |
| nbody                    | 79.1 ms                                                         | 61.4 ms: 1.29x faster                                                         |
| go                       | 146 ms                                                          | 113 ms: 1.29x faster                                                          |
| unpickle_pure_python     | 189 us                                                          | 147 us: 1.28x faster                                                          |
| spectral_norm            | 80.2 ms                                                         | 63.2 ms: 1.27x faster                                                         |
| pycparser                | 1.04 sec                                                        | 822 ms: 1.27x faster                                                          |
| sqlite_synth             | 2.29 us                                                         | 1.82 us: 1.26x faster                                                         |
| coroutines               | 17.9 ms                                                         | 14.6 ms: 1.23x faster                                                         |
| fannkuch                 | 317 ms                                                          | 263 ms: 1.21x faster                                                          |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 2.69 ms: 1.20x faster                                                         |
| xml_etree_process        | 48.1 ms                                                         | 40.5 ms: 1.19x faster                                                         |
| tornado_http             | 118 ms                                                          | 99.1 ms: 1.19x faster                                                         |
| nqueens                  | 87.1 ms                                                         | 73.7 ms: 1.18x faster                                                         |
| regex_compile            | 117 ms                                                          | 99.2 ms: 1.18x faster                                                         |
| deepcopy                 | 310 us                                                          | 266 us: 1.16x faster                                                          |
| sympy_sum                | 122 ms                                                          | 106 ms: 1.16x faster                                                          |
| asyncio_tcp              | 744 ms                                                          | 647 ms: 1.15x faster                                                          |
| sqlglot_normalize        | 230 ms                                                          | 203 ms: 1.13x faster                                                          |
| json                     | 4.76 ms                                                         | 4.22 ms: 1.13x faster                                                         |
| chameleon                | 6.42 ms                                                         | 5.72 ms: 1.12x faster                                                         |
| deepcopy_reduce          | 2.68 us                                                         | 2.40 us: 1.12x faster                                                         |
| sympy_str                | 229 ms                                                          | 205 ms: 1.12x faster                                                          |
| dask                     | 341 ms                                                          | 306 ms: 1.11x faster                                                          |
| sqlglot_optimize         | 44.7 ms                                                         | 40.2 ms: 1.11x faster                                                         |
| pprint_pformat           | 1.37 sec                                                        | 1.23 sec: 1.11x faster                                                        |
| pprint_safe_repr         | 658 ms                                                          | 593 ms: 1.11x faster                                                          |
| json_loads               | 22.4 us                                                         | 20.3 us: 1.10x faster                                                         |
| scimark_fft              | 216 ms                                                          | 197 ms: 1.10x faster                                                          |
| sympy_expand             | 391 ms                                                          | 357 ms: 1.09x faster                                                          |
| sympy_integrate          | 16.6 ms                                                         | 15.2 ms: 1.09x faster                                                         |
| xml_etree_parse          | 120 ms                                                          | 110 ms: 1.09x faster                                                          |
| xml_etree_iterparse      | 70.8 ms                                                         | 65.0 ms: 1.09x faster                                                         |
| regex_dna                | 131 ms                                                          | 121 ms: 1.08x faster                                                          |
| docutils                 | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                        |
| hexiom                   | 6.13 ms                                                         | 5.70 ms: 1.08x faster                                                         |
| 2to3                     | 265 ms                                                          | 247 ms: 1.08x faster                                                          |
| bench_thread_pool        | 1.12 ms                                                         | 1.05 ms: 1.07x faster                                                         |
| xml_etree_generate       | 61.6 ms                                                         | 57.8 ms: 1.07x faster                                                         |
| scimark_monte_carlo      | 61.9 ms                                                         | 58.6 ms: 1.06x faster                                                         |
| mdp                      | 1.83 sec                                                        | 1.75 sec: 1.04x faster                                                        |
| create_gc_cycles         | 694 us                                                          | 668 us: 1.04x faster                                                          |
| meteor_contest           | 80.0 ms                                                         | 79.4 ms: 1.01x faster                                                         |
| pickle_list              | 3.22 us                                                         | 3.24 us: 1.01x slower                                                         |
| python_startup           | 22.9 ms                                                         | 23.2 ms: 1.01x slower                                                         |
| unpickle_list            | 2.98 us                                                         | 3.04 us: 1.02x slower                                                         |
| unpickle                 | 9.82 us                                                         | 10.2 us: 1.04x slower                                                         |
| pickle                   | 7.83 us                                                         | 8.11 us: 1.04x slower                                                         |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.6 sec: 1.04x slower                                                        |
| regex_v8                 | 15.8 ms                                                         | 16.4 ms: 1.04x slower                                                         |
| logging_simple           | 7.29 us                                                         | 7.63 us: 1.05x slower                                                         |
| logging_format           | 7.91 us                                                         | 8.38 us: 1.06x slower                                                         |
| unpack_sequence          | 40.0 ns                                                         | 42.7 ns: 1.07x slower                                                         |
| pickle_dict              | 18.2 us                                                         | 19.8 us: 1.09x slower                                                         |
| pathlib                  | 81.2 ms                                                         | 88.8 ms: 1.09x slower                                                         |
| gc_traversal             | 1.28 ms                                                         | 1.40 ms: 1.10x slower                                                         |
| bench_mp_pool            | 66.4 ms                                                         | 74.4 ms: 1.12x slower                                                         |
| regex_effbot             | 1.66 ms                                                         | 1.93 ms: 1.16x slower                                                         |
| async_generators         | 241 ms                                                          | 282 ms: 1.17x slower                                                          |
| python_startup_no_site   | 18.1 ms                                                         | 21.1 ms: 1.17x slower                                                         |
| telco                    | 4.83 ms                                                         | 5.68 ms: 1.18x slower                                                         |
| coverage                 | 46.6 ms                                                         | 473 ms: 10.16x slower                                                         |
| Geometric mean           | (ref)                                                           | 1.17x faster                                                                  |
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240203-3.13.0a3+-61c470b-JIT/bm-20240203-pythonperf1_win32-x86-brandtbucher-justin_ghccc-3.13.0a3+-61c470b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown