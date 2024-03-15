
# Results vs. 3.10.4

- fork: python
- ref: v3.11.8
- machine: windows-x86
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.06x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 277 ms: 1.04x slower                                            |
| chameleon      | 6.42 ms                                                         | 8.27 ms: 1.29x slower                                           |
| docutils       | 1.95 sec                                                        | 2.00 sec: 1.03x slower                                          |
| html5lib       | 52.1 ms                                                         | 54.3 ms: 1.04x slower                                           |
| tornado_http   | 118 ms                                                          | 114 ms: 1.03x faster                                            |
| Geometric mean | (ref)                                                           | 1.07x slower                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|-------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 600 ms: 1.54x faster                                            |
| async_tree_io           | 940 ms                                                          | 740 ms: 1.27x faster                                            |
| async_tree_none         | 394 ms                                                          | 329 ms: 1.20x faster                                            |
| async_tree_memoization  | 467 ms                                                          | 392 ms: 1.19x faster                                            |
| Geometric mean          | (ref)                                                           | 1.29x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 197 ms: 2.55x faster                                            |
| float          | 69.6 ms                                                         | 71.6 ms: 1.03x slower                                           |
| nbody          | 79.1 ms                                                         | 117 ms: 1.48x slower                                            |
| Geometric mean | (ref)                                                           | 1.19x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 117 ms: 1.12x faster                                            |
| regex_v8       | 15.8 ms                                                         | 15.3 ms: 1.03x faster                                           |
| regex_effbot   | 1.66 ms                                                         | 1.85 ms: 1.12x slower                                           |
| regex_compile  | 117 ms                                                          | 140 ms: 1.20x slower                                            |
| Geometric mean | (ref)                                                           | 1.04x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| unpickle_list        | 2.98 us                                                         | 2.57 us: 1.16x faster                                           |
| json_loads           | 22.4 us                                                         | 20.1 us: 1.11x faster                                           |
| unpickle             | 9.82 us                                                         | 9.04 us: 1.09x faster                                           |
| xml_etree_parse      | 120 ms                                                          | 114 ms: 1.06x faster                                            |
| pickle               | 7.83 us                                                         | 7.53 us: 1.04x faster                                           |
| pickle_list          | 3.22 us                                                         | 3.20 us: 1.00x faster                                           |
| xml_etree_iterparse  | 70.8 ms                                                         | 73.4 ms: 1.04x slower                                           |
| pickle_pure_python   | 280 us                                                          | 299 us: 1.07x slower                                            |
| xml_etree_process    | 48.1 ms                                                         | 52.1 ms: 1.08x slower                                           |
| pickle_dict          | 18.2 us                                                         | 20.0 us: 1.10x slower                                           |
| xml_etree_generate   | 61.6 ms                                                         | 68.5 ms: 1.11x slower                                           |
| tomli_loads          | 1.91 sec                                                        | 2.24 sec: 1.17x slower                                          |
| unpickle_pure_python | 189 us                                                          | 230 us: 1.22x slower                                            |
| Geometric mean       | (ref)                                                           | 1.02x slower                                                    |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 21.4 ms: 1.07x faster                                           |
| python_startup_no_site | 18.1 ms                                                         | 17.9 ms: 1.01x faster                                           |
| Geometric mean         | (ref)                                                           | 1.04x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| django_template | 36.0 ms                                                         | 37.6 ms: 1.05x slower                                           |
| mako            | 9.10 ms                                                         | 9.58 ms: 1.05x slower                                           |
| genshi_text     | 21.0 ms                                                         | 26.8 ms: 1.28x slower                                           |
| genshi_xml      | 46.6 ms                                                         | 59.5 ms: 1.28x slower                                           |
| Geometric mean  | (ref)                                                           | 1.16x slower                                                    |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51 |
|--------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits                 | 502 ms                                                          | 197 ms: 2.55x faster                                            |
| sqlglot_normalize        | 230 ms                                                          | 107 ms: 2.14x faster                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 600 ms: 1.54x faster                                            |
| async_tree_io            | 940 ms                                                          | 740 ms: 1.27x faster                                            |
| async_tree_none          | 394 ms                                                          | 329 ms: 1.20x faster                                            |
| async_tree_memoization   | 467 ms                                                          | 392 ms: 1.19x faster                                            |
| unpickle_list            | 2.98 us                                                         | 2.57 us: 1.16x faster                                           |
| create_gc_cycles         | 694 us                                                          | 605 us: 1.15x faster                                            |
| thrift                   | 902 us                                                          | 786 us: 1.15x faster                                            |
| regex_dna                | 131 ms                                                          | 117 ms: 1.12x faster                                            |
| json_loads               | 22.4 us                                                         | 20.1 us: 1.11x faster                                           |
| sqlite_synth             | 2.29 us                                                         | 2.06 us: 1.11x faster                                           |
| json                     | 4.76 ms                                                         | 4.29 ms: 1.11x faster                                           |
| crypto_pyaes             | 81.3 ms                                                         | 73.4 ms: 1.11x faster                                           |
| pathlib                  | 81.2 ms                                                         | 74.7 ms: 1.09x faster                                           |
| unpickle                 | 9.82 us                                                         | 9.04 us: 1.09x faster                                           |
| python_startup           | 22.9 ms                                                         | 21.4 ms: 1.07x faster                                           |
| xml_etree_parse          | 120 ms                                                          | 114 ms: 1.06x faster                                            |
| pickle                   | 7.83 us                                                         | 7.53 us: 1.04x faster                                           |
| aiohttp                  | 1.13 ms                                                         | 1.10 ms: 1.03x faster                                           |
| regex_v8                 | 15.8 ms                                                         | 15.3 ms: 1.03x faster                                           |
| tornado_http             | 118 ms                                                          | 114 ms: 1.03x faster                                            |
| deltablue                | 4.04 ms                                                         | 3.93 ms: 1.03x faster                                           |
| async_generators         | 241 ms                                                          | 238 ms: 1.01x faster                                            |
| python_startup_no_site   | 18.1 ms                                                         | 17.9 ms: 1.01x faster                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                          |
| pycparser                | 1.04 sec                                                        | 1.03 sec: 1.01x faster                                          |
| pickle_list              | 3.22 us                                                         | 3.20 us: 1.00x faster                                           |
| flaskblogging            | 2.03 sec                                                        | 2.03 sec: 1.00x slower                                          |
| dask                     | 341 ms                                                          | 345 ms: 1.01x slower                                            |
| pyflate                  | 422 ms                                                          | 426 ms: 1.01x slower                                            |
| docutils                 | 1.95 sec                                                        | 2.00 sec: 1.03x slower                                          |
| float                    | 69.6 ms                                                         | 71.6 ms: 1.03x slower                                           |
| go                       | 146 ms                                                          | 150 ms: 1.03x slower                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 73.4 ms: 1.04x slower                                           |
| dulwich_log              | 58.5 ms                                                         | 60.7 ms: 1.04x slower                                           |
| html5lib                 | 52.1 ms                                                         | 54.3 ms: 1.04x slower                                           |
| mypy2                    | 590 ms                                                          | 616 ms: 1.04x slower                                            |
| 2to3                     | 265 ms                                                          | 277 ms: 1.04x slower                                            |
| django_template          | 36.0 ms                                                         | 37.6 ms: 1.05x slower                                           |
| telco                    | 4.83 ms                                                         | 5.06 ms: 1.05x slower                                           |
| raytrace                 | 303 ms                                                          | 318 ms: 1.05x slower                                            |
| mako                     | 9.10 ms                                                         | 9.58 ms: 1.05x slower                                           |
| gc_traversal             | 1.28 ms                                                         | 1.35 ms: 1.06x slower                                           |
| pylint                   | 384 ms                                                          | 407 ms: 1.06x slower                                            |
| sqlalchemy_declarative   | 104 ms                                                          | 111 ms: 1.06x slower                                            |
| pickle_pure_python       | 280 us                                                          | 299 us: 1.07x slower                                            |
| sqlglot_transpile        | 1.58 ms                                                         | 1.71 ms: 1.08x slower                                           |
| sqlglot_parse            | 1.33 ms                                                         | 1.44 ms: 1.08x slower                                           |
| xml_etree_process        | 48.1 ms                                                         | 52.1 ms: 1.08x slower                                           |
| scimark_lu               | 89.8 ms                                                         | 97.6 ms: 1.09x slower                                           |
| pickle_dict              | 18.2 us                                                         | 20.0 us: 1.10x slower                                           |
| bench_mp_pool            | 66.4 ms                                                         | 72.8 ms: 1.10x slower                                           |
| scimark_sor              | 115 ms                                                          | 127 ms: 1.10x slower                                            |
| xml_etree_generate       | 61.6 ms                                                         | 68.5 ms: 1.11x slower                                           |
| regex_effbot             | 1.66 ms                                                         | 1.85 ms: 1.12x slower                                           |
| sqlglot_optimize         | 44.7 ms                                                         | 49.9 ms: 1.12x slower                                           |
| richards_super           | 49.9 ms                                                         | 56.2 ms: 1.13x slower                                           |
| sqlalchemy_imperative    | 13.2 ms                                                         | 14.9 ms: 1.13x slower                                           |
| richards                 | 40.3 ms                                                         | 45.5 ms: 1.13x slower                                           |
| chaos                    | 74.4 ms                                                         | 84.1 ms: 1.13x slower                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 70.1 ms: 1.13x slower                                           |
| meteor_contest           | 80.0 ms                                                         | 92.1 ms: 1.15x slower                                           |
| sympy_expand             | 391 ms                                                          | 455 ms: 1.17x slower                                            |
| sympy_integrate          | 16.6 ms                                                         | 19.4 ms: 1.17x slower                                           |
| logging_silent           | 97.9 ns                                                         | 114 ns: 1.17x slower                                            |
| tomli_loads              | 1.91 sec                                                        | 2.24 sec: 1.17x slower                                          |
| hexiom                   | 6.13 ms                                                         | 7.22 ms: 1.18x slower                                           |
| typing_runtime_protocols | 396 us                                                          | 469 us: 1.19x slower                                            |
| pprint_pformat           | 1.37 sec                                                        | 1.63 sec: 1.19x slower                                          |
| mdp                      | 1.83 sec                                                        | 2.18 sec: 1.19x slower                                          |
| sympy_sum                | 122 ms                                                          | 146 ms: 1.19x slower                                            |
| pprint_safe_repr         | 658 ms                                                          | 787 ms: 1.20x slower                                            |
| sympy_str                | 229 ms                                                          | 274 ms: 1.20x slower                                            |
| comprehensions           | 17.7 us                                                         | 21.3 us: 1.20x slower                                           |
| regex_compile            | 117 ms                                                          | 140 ms: 1.20x slower                                            |
| deepcopy                 | 310 us                                                          | 375 us: 1.21x slower                                            |
| unpickle_pure_python     | 189 us                                                          | 230 us: 1.22x slower                                            |
| deepcopy_reduce          | 2.68 us                                                         | 3.27 us: 1.22x slower                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 4.01 ms: 1.24x slower                                           |
| nqueens                  | 87.1 ms                                                         | 108 ms: 1.24x slower                                            |
| coverage                 | 46.6 ms                                                         | 59.0 ms: 1.27x slower                                           |
| genshi_text              | 21.0 ms                                                         | 26.8 ms: 1.28x slower                                           |
| genshi_xml               | 46.6 ms                                                         | 59.5 ms: 1.28x slower                                           |
| coroutines               | 17.9 ms                                                         | 22.9 ms: 1.28x slower                                           |
| chameleon                | 6.42 ms                                                         | 8.27 ms: 1.29x slower                                           |
| fannkuch                 | 317 ms                                                          | 413 ms: 1.30x slower                                            |
| deepcopy_memo            | 29.6 us                                                         | 38.7 us: 1.31x slower                                           |
| scimark_fft              | 216 ms                                                          | 288 ms: 1.33x slower                                            |
| logging_format           | 7.91 us                                                         | 11.1 us: 1.40x slower                                           |
| logging_simple           | 7.29 us                                                         | 10.5 us: 1.43x slower                                           |
| unpack_sequence          | 40.0 ns                                                         | 58.6 ns: 1.46x slower                                           |
| spectral_norm            | 80.2 ms                                                         | 118 ms: 1.48x slower                                            |
| nbody                    | 79.1 ms                                                         | 117 ms: 1.48x slower                                            |
| generators               | 31.6 ms                                                         | 49.4 ms: 1.56x slower                                           |
| Geometric mean           | (ref)                                                           | 1.06x slower                                                    |

Benchmark hidden because not significant (3): asyncio_tcp, json_dumps, bench_thread_pool
Ignored benchmarks (4) of results/bm-20240206-3.11.8-db85d51/bm-20240206-pythonperf1_win32-x86-python-v3.11.8-3.11.8-db85d51.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: unknown