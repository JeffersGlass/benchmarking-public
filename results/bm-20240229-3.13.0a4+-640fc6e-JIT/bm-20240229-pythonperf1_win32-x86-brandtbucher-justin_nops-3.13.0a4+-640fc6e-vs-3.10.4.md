# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_nops
- machine: windows-x86
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.95%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 259 ms: 1.03x faster                                                         |
| chameleon      | 6.42 ms                                                         | 5.58 ms: 1.15x faster                                                        |
| docutils       | 1.95 sec                                                        | 1.79 sec: 1.09x faster                                                       |
| html5lib       | 52.1 ms                                                         | 44.4 ms: 1.17x faster                                                        |
| tornado_http   | 118 ms                                                          | 96.1 ms: 1.22x faster                                                        |
| Geometric mean | (ref)                                                           | 1.13x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 525 ms: 1.76x faster                                                         |
| async_tree_none         | 394 ms                                                          | 261 ms: 1.51x faster                                                         |
| async_tree_io           | 940 ms                                                          | 630 ms: 1.49x faster                                                         |
| async_tree_memoization  | 467 ms                                                          | 324 ms: 1.44x faster                                                         |
| Geometric mean          | (ref)                                                           | 1.55x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.54x faster                                                         |
| float          | 69.6 ms                                                         | 55.0 ms: 1.27x faster                                                        |
| nbody          | 79.1 ms                                                         | 92.6 ms: 1.17x slower                                                        |
| Geometric mean | (ref)                                                           | 1.40x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 118 ms: 1.11x faster                                                         |
| regex_compile  | 117 ms                                                          | 107 ms: 1.09x faster                                                         |
| regex_v8       | 15.8 ms                                                         | 15.9 ms: 1.01x slower                                                        |
| regex_effbot   | 1.66 ms                                                         | 1.87 ms: 1.13x slower                                                        |
| Geometric mean | (ref)                                                           | 1.01x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 7.05 ms: 1.39x faster                                                        |
| pickle_pure_python   | 280 us                                                          | 208 us: 1.35x faster                                                         |
| tomli_loads          | 1.91 sec                                                        | 1.68 sec: 1.14x faster                                                       |
| xml_etree_process    | 48.1 ms                                                         | 42.5 ms: 1.13x faster                                                        |
| unpickle_pure_python | 189 us                                                          | 168 us: 1.13x faster                                                         |
| json_loads           | 22.4 us                                                         | 19.9 us: 1.12x faster                                                        |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                                         |
| xml_etree_iterparse  | 70.8 ms                                                         | 67.2 ms: 1.05x faster                                                        |
| unpickle_list        | 2.98 us                                                         | 2.91 us: 1.03x faster                                                        |
| pickle               | 7.83 us                                                         | 7.91 us: 1.01x slower                                                        |
| unpickle             | 9.82 us                                                         | 10.1 us: 1.02x slower                                                        |
| pickle_dict          | 18.2 us                                                         | 20.4 us: 1.12x slower                                                        |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                 |

Benchmark hidden because not significant (2): xml_etree_generate, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 26.9 ms: 1.17x slower                                                        |
| python_startup_no_site | 18.1 ms                                                         | 24.4 ms: 1.35x slower                                                        |
| Geometric mean         | (ref)                                                           | 1.26x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 9.10 ms                                                         | 7.19 ms: 1.27x faster                                                        |
| django_template | 36.0 ms                                                         | 30.2 ms: 1.19x faster                                                        |
| genshi_xml      | 46.6 ms                                                         | 49.5 ms: 1.06x slower                                                        |
| genshi_text     | 21.0 ms                                                         | 23.4 ms: 1.12x slower                                                        |
| Geometric mean  | (ref)                                                           | 1.06x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|--------------------------|:---------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 94.0 us: 4.21x faster                                                        |
| pidigits                 | 502 ms                                                          | 198 ms: 2.54x faster                                                         |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 525 ms: 1.76x faster                                                         |
| pylint                   | 384 ms                                                          | 227 ms: 1.69x faster                                                         |
| logging_silent           | 97.9 ns                                                         | 59.6 ns: 1.64x faster                                                        |
| deltablue                | 4.04 ms                                                         | 2.55 ms: 1.58x faster                                                        |
| async_tree_none          | 394 ms                                                          | 261 ms: 1.51x faster                                                         |
| async_tree_io            | 940 ms                                                          | 630 ms: 1.49x faster                                                         |
| async_tree_memoization   | 467 ms                                                          | 324 ms: 1.44x faster                                                         |
| generators               | 31.6 ms                                                         | 22.2 ms: 1.42x faster                                                        |
| json_dumps               | 9.82 ms                                                         | 7.05 ms: 1.39x faster                                                        |
| crypto_pyaes             | 81.3 ms                                                         | 58.6 ms: 1.39x faster                                                        |
| sqlglot_parse            | 1.33 ms                                                         | 976 us: 1.36x faster                                                         |
| pickle_pure_python       | 280 us                                                          | 208 us: 1.35x faster                                                         |
| sqlglot_transpile        | 1.58 ms                                                         | 1.21 ms: 1.30x faster                                                        |
| mako                     | 9.10 ms                                                         | 7.19 ms: 1.27x faster                                                        |
| float                    | 69.6 ms                                                         | 55.0 ms: 1.27x faster                                                        |
| chaos                    | 74.4 ms                                                         | 58.8 ms: 1.26x faster                                                        |
| coroutines               | 17.9 ms                                                         | 14.2 ms: 1.26x faster                                                        |
| comprehensions           | 17.7 us                                                         | 14.1 us: 1.26x faster                                                        |
| deepcopy_memo            | 29.6 us                                                         | 23.8 us: 1.24x faster                                                        |
| richards_super           | 49.9 ms                                                         | 40.3 ms: 1.24x faster                                                        |
| tornado_http             | 118 ms                                                          | 96.1 ms: 1.22x faster                                                        |
| pycparser                | 1.04 sec                                                        | 857 ms: 1.22x faster                                                         |
| go                       | 146 ms                                                          | 120 ms: 1.21x faster                                                         |
| django_template          | 36.0 ms                                                         | 30.2 ms: 1.19x faster                                                        |
| html5lib                 | 52.1 ms                                                         | 44.4 ms: 1.17x faster                                                        |
| asyncio_tcp              | 744 ms                                                          | 639 ms: 1.16x faster                                                         |
| sqlite_synth             | 2.29 us                                                         | 1.97 us: 1.16x faster                                                        |
| chameleon                | 6.42 ms                                                         | 5.58 ms: 1.15x faster                                                        |
| raytrace                 | 303 ms                                                          | 263 ms: 1.15x faster                                                         |
| scimark_sor              | 115 ms                                                          | 100 ms: 1.15x faster                                                         |
| sympy_sum                | 122 ms                                                          | 107 ms: 1.15x faster                                                         |
| tomli_loads              | 1.91 sec                                                        | 1.68 sec: 1.14x faster                                                       |
| json                     | 4.76 ms                                                         | 4.19 ms: 1.14x faster                                                        |
| xml_etree_process        | 48.1 ms                                                         | 42.5 ms: 1.13x faster                                                        |
| unpickle_pure_python     | 189 us                                                          | 168 us: 1.13x faster                                                         |
| deepcopy_reduce          | 2.68 us                                                         | 2.38 us: 1.13x faster                                                        |
| richards                 | 40.3 ms                                                         | 35.8 ms: 1.12x faster                                                        |
| json_loads               | 22.4 us                                                         | 19.9 us: 1.12x faster                                                        |
| deepcopy                 | 310 us                                                          | 277 us: 1.12x faster                                                         |
| regex_dna                | 131 ms                                                          | 118 ms: 1.11x faster                                                         |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                                         |
| pyflate                  | 422 ms                                                          | 383 ms: 1.10x faster                                                         |
| sympy_str                | 229 ms                                                          | 209 ms: 1.10x faster                                                         |
| scimark_lu               | 89.8 ms                                                         | 82.3 ms: 1.09x faster                                                        |
| bench_thread_pool        | 1.12 ms                                                         | 1.03 ms: 1.09x faster                                                        |
| regex_compile            | 117 ms                                                          | 107 ms: 1.09x faster                                                         |
| docutils                 | 1.95 sec                                                        | 1.79 sec: 1.09x faster                                                       |
| sympy_integrate          | 16.6 ms                                                         | 15.4 ms: 1.08x faster                                                        |
| sympy_expand             | 391 ms                                                          | 364 ms: 1.07x faster                                                         |
| xml_etree_iterparse      | 70.8 ms                                                         | 67.2 ms: 1.05x faster                                                        |
| mdp                      | 1.83 sec                                                        | 1.74 sec: 1.05x faster                                                       |
| create_gc_cycles         | 694 us                                                          | 663 us: 1.05x faster                                                         |
| spectral_norm            | 80.2 ms                                                         | 77.2 ms: 1.04x faster                                                        |
| sqlglot_normalize        | 230 ms                                                          | 223 ms: 1.03x faster                                                         |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.14 ms: 1.03x faster                                                        |
| unpickle_list            | 2.98 us                                                         | 2.91 us: 1.03x faster                                                        |
| 2to3                     | 265 ms                                                          | 259 ms: 1.03x faster                                                         |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                                       |
| pickle                   | 7.83 us                                                         | 7.91 us: 1.01x slower                                                        |
| hexiom                   | 6.13 ms                                                         | 6.20 ms: 1.01x slower                                                        |
| regex_v8                 | 15.8 ms                                                         | 15.9 ms: 1.01x slower                                                        |
| sqlglot_optimize         | 44.7 ms                                                         | 45.5 ms: 1.02x slower                                                        |
| unpickle                 | 9.82 us                                                         | 10.1 us: 1.02x slower                                                        |
| pathlib                  | 81.2 ms                                                         | 84.2 ms: 1.04x slower                                                        |
| scimark_monte_carlo      | 61.9 ms                                                         | 65.1 ms: 1.05x slower                                                        |
| nqueens                  | 87.1 ms                                                         | 91.9 ms: 1.05x slower                                                        |
| meteor_contest           | 80.0 ms                                                         | 84.5 ms: 1.06x slower                                                        |
| genshi_xml               | 46.6 ms                                                         | 49.5 ms: 1.06x slower                                                        |
| fannkuch                 | 317 ms                                                          | 339 ms: 1.07x slower                                                         |
| scimark_fft              | 216 ms                                                          | 235 ms: 1.09x slower                                                         |
| pprint_pformat           | 1.37 sec                                                        | 1.49 sec: 1.09x slower                                                       |
| logging_format           | 7.91 us                                                         | 8.63 us: 1.09x slower                                                        |
| unpack_sequence          | 40.0 ns                                                         | 43.7 ns: 1.09x slower                                                        |
| gc_traversal             | 1.28 ms                                                         | 1.41 ms: 1.10x slower                                                        |
| logging_simple           | 7.29 us                                                         | 8.07 us: 1.11x slower                                                        |
| pprint_safe_repr         | 658 ms                                                          | 733 ms: 1.11x slower                                                         |
| genshi_text              | 21.0 ms                                                         | 23.4 ms: 1.12x slower                                                        |
| pickle_dict              | 18.2 us                                                         | 20.4 us: 1.12x slower                                                        |
| regex_effbot             | 1.66 ms                                                         | 1.87 ms: 1.13x slower                                                        |
| bench_mp_pool            | 66.4 ms                                                         | 77.5 ms: 1.17x slower                                                        |
| nbody                    | 79.1 ms                                                         | 92.6 ms: 1.17x slower                                                        |
| python_startup           | 22.9 ms                                                         | 26.9 ms: 1.17x slower                                                        |
| async_generators         | 241 ms                                                          | 283 ms: 1.18x slower                                                         |
| dask                     | 341 ms                                                          | 418 ms: 1.23x slower                                                         |
| telco                    | 4.83 ms                                                         | 6.34 ms: 1.31x slower                                                        |
| python_startup_no_site   | 18.1 ms                                                         | 24.4 ms: 1.35x slower                                                        |
| coverage                 | 46.6 ms                                                         | 490 ms: 10.52x slower                                                        |
| thrift                   | 902 us                                                          | 10.7 ms: 11.85x slower                                                       |
| Geometric mean           | (ref)                                                           | 1.06x faster                                                                 |

Benchmark hidden because not significant (2): xml_etree_generate, pickle_list
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-640fc6e-JIT/bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_nops-3.13.0a4+-640fc6e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.95% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown