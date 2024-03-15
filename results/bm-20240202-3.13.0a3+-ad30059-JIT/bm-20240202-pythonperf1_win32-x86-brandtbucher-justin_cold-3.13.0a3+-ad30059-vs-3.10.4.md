
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_cold
- machine: windows-x86
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.10x faster \*
- HPT reliability: 99.96%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 251 ms: 1.06x faster                                                         |
| chameleon      | 6.42 ms                                                         | 5.97 ms: 1.08x faster                                                        |
| docutils       | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                       |
| tornado_http   | 118 ms                                                          | 97.1 ms: 1.21x faster                                                        |
| Geometric mean | (ref)                                                           | 1.10x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 524 ms: 1.76x faster                                                         |
| async_tree_none         | 394 ms                                                          | 262 ms: 1.50x faster                                                         |
| async_tree_io           | 940 ms                                                          | 637 ms: 1.48x faster                                                         |
| async_tree_memoization  | 467 ms                                                          | 328 ms: 1.42x faster                                                         |
| Geometric mean          | (ref)                                                           | 1.54x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 204 ms: 2.47x faster                                                         |
| float          | 69.6 ms                                                         | 56.2 ms: 1.24x faster                                                        |
| nbody          | 79.1 ms                                                         | 97.0 ms: 1.23x slower                                                        |
| Geometric mean | (ref)                                                           | 1.36x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 106 ms: 1.10x faster                                                         |
| regex_dna      | 131 ms                                                          | 121 ms: 1.08x faster                                                         |
| regex_v8       | 15.8 ms                                                         | 16.6 ms: 1.05x slower                                                        |
| regex_effbot   | 1.66 ms                                                         | 1.94 ms: 1.16x slower                                                        |
| Geometric mean | (ref)                                                           | 1.01x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.87 ms: 1.43x faster                                                        |
| pickle_pure_python   | 280 us                                                          | 210 us: 1.33x faster                                                         |
| unpickle_pure_python | 189 us                                                          | 151 us: 1.26x faster                                                         |
| tomli_loads          | 1.91 sec                                                        | 1.67 sec: 1.15x faster                                                       |
| xml_etree_process    | 48.1 ms                                                         | 42.2 ms: 1.14x faster                                                        |
| json_loads           | 22.4 us                                                         | 19.6 us: 1.14x faster                                                        |
| xml_etree_parse      | 120 ms                                                          | 111 ms: 1.08x faster                                                         |
| xml_etree_iterparse  | 70.8 ms                                                         | 69.9 ms: 1.01x faster                                                        |
| xml_etree_generate   | 61.6 ms                                                         | 61.3 ms: 1.01x faster                                                        |
| unpickle_list        | 2.98 us                                                         | 3.04 us: 1.02x slower                                                        |
| unpickle             | 9.82 us                                                         | 10.3 us: 1.05x slower                                                        |
| pickle               | 7.83 us                                                         | 8.28 us: 1.06x slower                                                        |
| pickle_dict          | 18.2 us                                                         | 19.8 us: 1.09x slower                                                        |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                 |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 23.1 ms: 1.01x slower                                                        |
| python_startup_no_site | 18.1 ms                                                         | 21.0 ms: 1.16x slower                                                        |
| Geometric mean         | (ref)                                                           | 1.08x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.97 ms: 1.14x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|--------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 97.9 us: 4.04x faster                                                        |
| pidigits                 | 502 ms                                                          | 204 ms: 2.47x faster                                                         |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 524 ms: 1.76x faster                                                         |
| deltablue                | 4.04 ms                                                         | 2.52 ms: 1.60x faster                                                        |
| logging_silent           | 97.9 ns                                                         | 61.6 ns: 1.59x faster                                                        |
| richards_super           | 49.9 ms                                                         | 33.1 ms: 1.51x faster                                                        |
| async_tree_none          | 394 ms                                                          | 262 ms: 1.50x faster                                                         |
| scimark_lu               | 89.8 ms                                                         | 60.6 ms: 1.48x faster                                                        |
| async_tree_io            | 940 ms                                                          | 637 ms: 1.48x faster                                                         |
| sqlglot_parse            | 1.33 ms                                                         | 918 us: 1.45x faster                                                         |
| json_dumps               | 9.82 ms                                                         | 6.87 ms: 1.43x faster                                                        |
| async_tree_memoization   | 467 ms                                                          | 328 ms: 1.42x faster                                                         |
| generators               | 31.6 ms                                                         | 22.7 ms: 1.39x faster                                                        |
| richards                 | 40.3 ms                                                         | 29.0 ms: 1.39x faster                                                        |
| scimark_sor              | 115 ms                                                          | 83.4 ms: 1.38x faster                                                        |
| sqlglot_transpile        | 1.58 ms                                                         | 1.18 ms: 1.34x faster                                                        |
| raytrace                 | 303 ms                                                          | 227 ms: 1.33x faster                                                         |
| pickle_pure_python       | 280 us                                                          | 210 us: 1.33x faster                                                         |
| crypto_pyaes             | 81.3 ms                                                         | 63.3 ms: 1.28x faster                                                        |
| deepcopy_memo            | 29.6 us                                                         | 23.2 us: 1.27x faster                                                        |
| unpickle_pure_python     | 189 us                                                          | 151 us: 1.26x faster                                                         |
| pycparser                | 1.04 sec                                                        | 830 ms: 1.26x faster                                                         |
| chaos                    | 74.4 ms                                                         | 59.5 ms: 1.25x faster                                                        |
| float                    | 69.6 ms                                                         | 56.2 ms: 1.24x faster                                                        |
| coroutines               | 17.9 ms                                                         | 14.5 ms: 1.24x faster                                                        |
| sqlite_synth             | 2.29 us                                                         | 1.87 us: 1.23x faster                                                        |
| go                       | 146 ms                                                          | 119 ms: 1.22x faster                                                         |
| tornado_http             | 118 ms                                                          | 97.1 ms: 1.21x faster                                                        |
| json                     | 4.76 ms                                                         | 4.07 ms: 1.17x faster                                                        |
| tomli_loads              | 1.91 sec                                                        | 1.67 sec: 1.15x faster                                                       |
| mako                     | 9.10 ms                                                         | 7.97 ms: 1.14x faster                                                        |
| xml_etree_process        | 48.1 ms                                                         | 42.2 ms: 1.14x faster                                                        |
| json_loads               | 22.4 us                                                         | 19.6 us: 1.14x faster                                                        |
| comprehensions           | 17.7 us                                                         | 15.7 us: 1.13x faster                                                        |
| asyncio_tcp              | 744 ms                                                          | 665 ms: 1.12x faster                                                         |
| deepcopy                 | 310 us                                                          | 278 us: 1.11x faster                                                         |
| pyflate                  | 422 ms                                                          | 383 ms: 1.10x faster                                                         |
| dask                     | 341 ms                                                          | 310 ms: 1.10x faster                                                         |
| regex_compile            | 117 ms                                                          | 106 ms: 1.10x faster                                                         |
| deepcopy_reduce          | 2.68 us                                                         | 2.45 us: 1.10x faster                                                        |
| sympy_sum                | 122 ms                                                          | 112 ms: 1.09x faster                                                         |
| regex_dna                | 131 ms                                                          | 121 ms: 1.08x faster                                                         |
| xml_etree_parse          | 120 ms                                                          | 111 ms: 1.08x faster                                                         |
| docutils                 | 1.95 sec                                                        | 1.81 sec: 1.08x faster                                                       |
| chameleon                | 6.42 ms                                                         | 5.97 ms: 1.08x faster                                                        |
| sympy_expand             | 391 ms                                                          | 369 ms: 1.06x faster                                                         |
| 2to3                     | 265 ms                                                          | 251 ms: 1.06x faster                                                         |
| sqlglot_optimize         | 44.7 ms                                                         | 42.5 ms: 1.05x faster                                                        |
| create_gc_cycles         | 694 us                                                          | 660 us: 1.05x faster                                                         |
| sympy_str                | 229 ms                                                          | 219 ms: 1.05x faster                                                         |
| sqlglot_normalize        | 230 ms                                                          | 221 ms: 1.04x faster                                                         |
| sympy_integrate          | 16.6 ms                                                         | 16.1 ms: 1.04x faster                                                        |
| bench_thread_pool        | 1.12 ms                                                         | 1.09 ms: 1.03x faster                                                        |
| spectral_norm            | 80.2 ms                                                         | 78.2 ms: 1.03x faster                                                        |
| fannkuch                 | 317 ms                                                          | 313 ms: 1.01x faster                                                         |
| xml_etree_iterparse      | 70.8 ms                                                         | 69.9 ms: 1.01x faster                                                        |
| unpack_sequence          | 40.0 ns                                                         | 39.7 ns: 1.01x faster                                                        |
| xml_etree_generate       | 61.6 ms                                                         | 61.3 ms: 1.01x faster                                                        |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.26 ms: 1.01x slower                                                        |
| python_startup           | 22.9 ms                                                         | 23.1 ms: 1.01x slower                                                        |
| unpickle_list            | 2.98 us                                                         | 3.04 us: 1.02x slower                                                        |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.7 sec: 1.04x slower                                                       |
| pprint_safe_repr         | 658 ms                                                          | 688 ms: 1.05x slower                                                         |
| pprint_pformat           | 1.37 sec                                                        | 1.43 sec: 1.05x slower                                                       |
| unpickle                 | 9.82 us                                                         | 10.3 us: 1.05x slower                                                        |
| regex_v8                 | 15.8 ms                                                         | 16.6 ms: 1.05x slower                                                        |
| mdp                      | 1.83 sec                                                        | 1.93 sec: 1.06x slower                                                       |
| pickle                   | 7.83 us                                                         | 8.28 us: 1.06x slower                                                        |
| pickle_dict              | 18.2 us                                                         | 19.8 us: 1.09x slower                                                        |
| meteor_contest           | 80.0 ms                                                         | 87.5 ms: 1.09x slower                                                        |
| pathlib                  | 81.2 ms                                                         | 88.8 ms: 1.09x slower                                                        |
| hexiom                   | 6.13 ms                                                         | 6.72 ms: 1.10x slower                                                        |
| logging_format           | 7.91 us                                                         | 8.71 us: 1.10x slower                                                        |
| gc_traversal             | 1.28 ms                                                         | 1.42 ms: 1.11x slower                                                        |
| scimark_monte_carlo      | 61.9 ms                                                         | 69.4 ms: 1.12x slower                                                        |
| logging_simple           | 7.29 us                                                         | 8.19 us: 1.12x slower                                                        |
| bench_mp_pool            | 66.4 ms                                                         | 75.7 ms: 1.14x slower                                                        |
| python_startup_no_site   | 18.1 ms                                                         | 21.0 ms: 1.16x slower                                                        |
| regex_effbot             | 1.66 ms                                                         | 1.94 ms: 1.16x slower                                                        |
| scimark_fft              | 216 ms                                                          | 254 ms: 1.17x slower                                                         |
| async_generators         | 241 ms                                                          | 294 ms: 1.22x slower                                                         |
| nbody                    | 79.1 ms                                                         | 97.0 ms: 1.23x slower                                                        |
| telco                    | 4.83 ms                                                         | 6.11 ms: 1.27x slower                                                        |
| coverage                 | 46.6 ms                                                         | 480 ms: 10.32x slower                                                        |
| Geometric mean           | (ref)                                                           | 1.10x faster                                                                 |

Benchmark hidden because not significant (2): nqueens, pickle_list
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240202-3.13.0a3+-ad30059-JIT/bm-20240202-pythonperf1_win32-x86-brandtbucher-justin_cold-3.13.0a3+-ad30059.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.96% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown