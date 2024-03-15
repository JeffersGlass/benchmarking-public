# Results vs. 3.10.4

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: windows-x86
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.33%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| chameleon      | 6.42 ms                                                         | 6.00 ms: 1.07x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.87 sec: 1.04x faster                                                          |
| html5lib       | 52.1 ms                                                         | 47.6 ms: 1.09x faster                                                           |
| tornado_http   | 118 ms                                                          | 99.9 ms: 1.18x faster                                                           |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                    |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 529 ms: 1.74x faster                                                            |
| async_tree_none         | 394 ms                                                          | 271 ms: 1.45x faster                                                            |
| async_tree_io           | 940 ms                                                          | 649 ms: 1.45x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 339 ms: 1.38x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.50x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.53x faster                                                            |
| float          | 69.6 ms                                                         | 56.4 ms: 1.23x faster                                                           |
| nbody          | 79.1 ms                                                         | 96.7 ms: 1.22x slower                                                           |
| Geometric mean | (ref)                                                           | 1.37x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 113 ms: 1.03x faster                                                            |
| regex_dna      | 131 ms                                                          | 130 ms: 1.01x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.1 ms: 1.02x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.96 ms: 1.18x slower                                                           |
| Geometric mean | (ref)                                                           | 1.04x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 7.10 ms: 1.38x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 228 us: 1.23x faster                                                            |
| xml_etree_process    | 48.1 ms                                                         | 42.8 ms: 1.12x faster                                                           |
| unpickle_pure_python | 189 us                                                          | 170 us: 1.11x faster                                                            |
| json_loads           | 22.4 us                                                         | 20.3 us: 1.10x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.77 sec: 1.08x faster                                                          |
| xml_etree_iterparse  | 70.8 ms                                                         | 68.3 ms: 1.04x faster                                                           |
| unpickle_list        | 2.98 us                                                         | 2.93 us: 1.02x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.28 us: 1.02x slower                                                           |
| unpickle             | 9.82 us                                                         | 10.1 us: 1.03x slower                                                           |
| pickle               | 7.83 us                                                         | 8.16 us: 1.04x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 20.0 us: 1.10x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.07x faster                                                                    |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 26.0 ms: 1.14x slower                                                           |
| python_startup_no_site | 18.1 ms                                                         | 24.0 ms: 1.33x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.23x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako            | 9.10 ms                                                         | 7.19 ms: 1.27x faster                                                           |
| django_template | 36.0 ms                                                         | 31.9 ms: 1.13x faster                                                           |
| genshi_xml      | 46.6 ms                                                         | 51.0 ms: 1.09x slower                                                           |
| genshi_text     | 21.0 ms                                                         | 23.9 ms: 1.14x slower                                                           |
| Geometric mean  | (ref)                                                           | 1.04x faster                                                                    |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 101 us: 3.93x faster                                                            |
| pidigits                 | 502 ms                                                          | 198 ms: 2.53x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 529 ms: 1.74x faster                                                            |
| pylint                   | 384 ms                                                          | 236 ms: 1.63x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.75 ms: 1.47x faster                                                           |
| async_tree_none          | 394 ms                                                          | 271 ms: 1.45x faster                                                            |
| async_tree_io            | 940 ms                                                          | 649 ms: 1.45x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 68.8 ns: 1.42x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 7.10 ms: 1.38x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 339 ms: 1.38x faster                                                            |
| crypto_pyaes             | 81.3 ms                                                         | 60.8 ms: 1.34x faster                                                           |
| sqlglot_parse            | 1.33 ms                                                         | 1.03 ms: 1.29x faster                                                           |
| mako                     | 9.10 ms                                                         | 7.19 ms: 1.27x faster                                                           |
| generators               | 31.6 ms                                                         | 25.0 ms: 1.26x faster                                                           |
| float                    | 69.6 ms                                                         | 56.4 ms: 1.23x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 228 us: 1.23x faster                                                            |
| sqlglot_transpile        | 1.58 ms                                                         | 1.30 ms: 1.22x faster                                                           |
| comprehensions           | 17.7 us                                                         | 14.6 us: 1.21x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.91 us: 1.20x faster                                                           |
| chaos                    | 74.4 ms                                                         | 62.4 ms: 1.19x faster                                                           |
| coroutines               | 17.9 ms                                                         | 15.2 ms: 1.18x faster                                                           |
| richards_super           | 49.9 ms                                                         | 42.3 ms: 1.18x faster                                                           |
| tornado_http             | 118 ms                                                          | 99.9 ms: 1.18x faster                                                           |
| pycparser                | 1.04 sec                                                        | 902 ms: 1.16x faster                                                            |
| django_template          | 36.0 ms                                                         | 31.9 ms: 1.13x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 659 ms: 1.13x faster                                                            |
| scimark_sor              | 115 ms                                                          | 102 ms: 1.13x faster                                                            |
| go                       | 146 ms                                                          | 130 ms: 1.12x faster                                                            |
| xml_etree_process        | 48.1 ms                                                         | 42.8 ms: 1.12x faster                                                           |
| unpickle_pure_python     | 189 us                                                          | 170 us: 1.11x faster                                                            |
| json                     | 4.76 ms                                                         | 4.28 ms: 1.11x faster                                                           |
| json_loads               | 22.4 us                                                         | 20.3 us: 1.10x faster                                                           |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                                            |
| sympy_sum                | 122 ms                                                          | 112 ms: 1.10x faster                                                            |
| pyflate                  | 422 ms                                                          | 385 ms: 1.10x faster                                                            |
| html5lib                 | 52.1 ms                                                         | 47.6 ms: 1.09x faster                                                           |
| spectral_norm            | 80.2 ms                                                         | 73.7 ms: 1.09x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.77 sec: 1.08x faster                                                          |
| chameleon                | 6.42 ms                                                         | 6.00 ms: 1.07x faster                                                           |
| raytrace                 | 303 ms                                                          | 284 ms: 1.07x faster                                                            |
| richards                 | 40.3 ms                                                         | 37.9 ms: 1.06x faster                                                           |
| deepcopy_memo            | 29.6 us                                                         | 28.0 us: 1.05x faster                                                           |
| bench_thread_pool        | 1.12 ms                                                         | 1.07 ms: 1.05x faster                                                           |
| deepcopy                 | 310 us                                                          | 296 us: 1.05x faster                                                            |
| sympy_str                | 229 ms                                                          | 219 ms: 1.04x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.87 sec: 1.04x faster                                                          |
| create_gc_cycles         | 694 us                                                          | 668 us: 1.04x faster                                                            |
| deepcopy_reduce          | 2.68 us                                                         | 2.59 us: 1.04x faster                                                           |
| xml_etree_iterparse      | 70.8 ms                                                         | 68.3 ms: 1.04x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 86.9 ms: 1.03x faster                                                           |
| mdp                      | 1.83 sec                                                        | 1.77 sec: 1.03x faster                                                          |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.14 ms: 1.03x faster                                                           |
| regex_compile            | 117 ms                                                          | 113 ms: 1.03x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 16.3 ms: 1.02x faster                                                           |
| unpickle_list            | 2.98 us                                                         | 2.93 us: 1.02x faster                                                           |
| sympy_expand             | 391 ms                                                          | 383 ms: 1.02x faster                                                            |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                                          |
| regex_dna                | 131 ms                                                          | 130 ms: 1.01x faster                                                            |
| pickle_list              | 3.22 us                                                         | 3.28 us: 1.02x slower                                                           |
| regex_v8                 | 15.8 ms                                                         | 16.1 ms: 1.02x slower                                                           |
| unpickle                 | 9.82 us                                                         | 10.1 us: 1.03x slower                                                           |
| pickle                   | 7.83 us                                                         | 8.16 us: 1.04x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 84.7 ms: 1.04x slower                                                           |
| hexiom                   | 6.13 ms                                                         | 6.40 ms: 1.04x slower                                                           |
| sqlglot_normalize        | 230 ms                                                          | 241 ms: 1.04x slower                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 47.8 ms: 1.07x slower                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 66.3 ms: 1.07x slower                                                           |
| meteor_contest           | 80.0 ms                                                         | 85.9 ms: 1.07x slower                                                           |
| nqueens                  | 87.1 ms                                                         | 94.7 ms: 1.09x slower                                                           |
| genshi_xml               | 46.6 ms                                                         | 51.0 ms: 1.09x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.40 ms: 1.09x slower                                                           |
| fannkuch                 | 317 ms                                                          | 347 ms: 1.09x slower                                                            |
| pickle_dict              | 18.2 us                                                         | 20.0 us: 1.10x slower                                                           |
| unpack_sequence          | 40.0 ns                                                         | 44.3 ns: 1.11x slower                                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.52 sec: 1.11x slower                                                          |
| scimark_fft              | 216 ms                                                          | 242 ms: 1.12x slower                                                            |
| bench_mp_pool            | 66.4 ms                                                         | 74.5 ms: 1.12x slower                                                           |
| pprint_safe_repr         | 658 ms                                                          | 745 ms: 1.13x slower                                                            |
| python_startup           | 22.9 ms                                                         | 26.0 ms: 1.14x slower                                                           |
| genshi_text              | 21.0 ms                                                         | 23.9 ms: 1.14x slower                                                           |
| logging_format           | 7.91 us                                                         | 9.07 us: 1.15x slower                                                           |
| logging_simple           | 7.29 us                                                         | 8.37 us: 1.15x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.96 ms: 1.18x slower                                                           |
| nbody                    | 79.1 ms                                                         | 96.7 ms: 1.22x slower                                                           |
| async_generators         | 241 ms                                                          | 307 ms: 1.27x slower                                                            |
| telco                    | 4.83 ms                                                         | 6.16 ms: 1.27x slower                                                           |
| dask                     | 341 ms                                                          | 439 ms: 1.29x slower                                                            |
| python_startup_no_site   | 18.1 ms                                                         | 24.0 ms: 1.33x slower                                                           |
| coverage                 | 46.6 ms                                                         | 497 ms: 10.68x slower                                                           |
| thrift                   | 902 us                                                          | 11.0 ms: 12.21x slower                                                          |
| Geometric mean           | (ref)                                                           | 1.02x faster                                                                    |

Benchmark hidden because not significant (2): xml_etree_generate, 2to3
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-pythonperf1_win32-x86-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.33% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown