# Results vs. 3.10.4

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: windows-x86
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 255 ms: 1.04x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.77 ms: 1.11x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.82 sec: 1.07x faster                                                          |
| tornado_http   | 118 ms                                                          | 95.2 ms: 1.23x faster                                                           |
| Geometric mean | (ref)                                                           | 1.11x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 523 ms: 1.76x faster                                                            |
| async_tree_io           | 940 ms                                                          | 612 ms: 1.54x faster                                                            |
| async_tree_none         | 394 ms                                                          | 257 ms: 1.53x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 318 ms: 1.47x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.57x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 201 ms: 2.50x faster                                                            |
| float          | 69.6 ms                                                         | 54.7 ms: 1.27x faster                                                           |
| nbody          | 79.1 ms                                                         | 93.7 ms: 1.18x slower                                                           |
| Geometric mean | (ref)                                                           | 1.39x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 111 ms: 1.05x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.0 ms: 1.01x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.97 ms: 1.18x slower                                                           |
| Geometric mean | (ref)                                                           | 1.03x slower                                                                    |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.80 ms: 1.45x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 214 us: 1.31x faster                                                            |
| xml_etree_process    | 48.1 ms                                                         | 41.9 ms: 1.15x faster                                                           |
| tomli_loads          | 1.91 sec                                                        | 1.66 sec: 1.15x faster                                                          |
| unpickle_pure_python | 189 us                                                          | 167 us: 1.14x faster                                                            |
| unpickle_list        | 2.98 us                                                         | 2.65 us: 1.12x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 107 ms: 1.12x faster                                                            |
| json_loads           | 22.4 us                                                         | 20.5 us: 1.09x faster                                                           |
| xml_etree_iterparse  | 70.8 ms                                                         | 66.6 ms: 1.06x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 60.4 ms: 1.02x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.25 us: 1.01x slower                                                           |
| pickle               | 7.83 us                                                         | 8.02 us: 1.02x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 20.3 us: 1.11x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.10x faster                                                                    |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 26.2 ms: 1.14x slower                                                           |
| python_startup_no_site | 18.1 ms                                                         | 23.6 ms: 1.30x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.22x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.22 ms: 1.26x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 94.5 us: 4.19x faster                                                           |
| pidigits                 | 502 ms                                                          | 201 ms: 2.50x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 523 ms: 1.76x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 60.2 ns: 1.63x faster                                                           |
| deltablue                | 4.04 ms                                                         | 2.51 ms: 1.61x faster                                                           |
| async_tree_io            | 940 ms                                                          | 612 ms: 1.54x faster                                                            |
| async_tree_none          | 394 ms                                                          | 257 ms: 1.53x faster                                                            |
| async_tree_memoization   | 467 ms                                                          | 318 ms: 1.47x faster                                                            |
| generators               | 31.6 ms                                                         | 21.6 ms: 1.46x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.80 ms: 1.45x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 58.5 ms: 1.39x faster                                                           |
| sqlglot_parse            | 1.33 ms                                                         | 958 us: 1.39x faster                                                            |
| sqlglot_transpile        | 1.58 ms                                                         | 1.20 ms: 1.32x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 214 us: 1.31x faster                                                            |
| float                    | 69.6 ms                                                         | 54.7 ms: 1.27x faster                                                           |
| chaos                    | 74.4 ms                                                         | 58.6 ms: 1.27x faster                                                           |
| coroutines               | 17.9 ms                                                         | 14.1 ms: 1.27x faster                                                           |
| mako                     | 9.10 ms                                                         | 7.22 ms: 1.26x faster                                                           |
| comprehensions           | 17.7 us                                                         | 14.1 us: 1.26x faster                                                           |
| tornado_http             | 118 ms                                                          | 95.2 ms: 1.23x faster                                                           |
| pycparser                | 1.04 sec                                                        | 850 ms: 1.23x faster                                                            |
| deepcopy_memo            | 29.6 us                                                         | 24.2 us: 1.22x faster                                                           |
| go                       | 146 ms                                                          | 119 ms: 1.22x faster                                                            |
| sqlite_synth             | 2.29 us                                                         | 1.90 us: 1.20x faster                                                           |
| richards_super           | 49.9 ms                                                         | 41.6 ms: 1.20x faster                                                           |
| scimark_sor              | 115 ms                                                          | 98.4 ms: 1.17x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 641 ms: 1.16x faster                                                            |
| raytrace                 | 303 ms                                                          | 261 ms: 1.16x faster                                                            |
| deepcopy                 | 310 us                                                          | 268 us: 1.16x faster                                                            |
| xml_etree_process        | 48.1 ms                                                         | 41.9 ms: 1.15x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.66 sec: 1.15x faster                                                          |
| sympy_sum                | 122 ms                                                          | 107 ms: 1.15x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 167 us: 1.14x faster                                                            |
| spectral_norm            | 80.2 ms                                                         | 71.1 ms: 1.13x faster                                                           |
| unpickle_list            | 2.98 us                                                         | 2.65 us: 1.12x faster                                                           |
| richards                 | 40.3 ms                                                         | 35.8 ms: 1.12x faster                                                           |
| pyflate                  | 422 ms                                                          | 376 ms: 1.12x faster                                                            |
| xml_etree_parse          | 120 ms                                                          | 107 ms: 1.12x faster                                                            |
| json                     | 4.76 ms                                                         | 4.25 ms: 1.12x faster                                                           |
| deepcopy_reduce          | 2.68 us                                                         | 2.40 us: 1.12x faster                                                           |
| chameleon                | 6.42 ms                                                         | 5.77 ms: 1.11x faster                                                           |
| sympy_str                | 229 ms                                                          | 208 ms: 1.10x faster                                                            |
| json_loads               | 22.4 us                                                         | 20.5 us: 1.09x faster                                                           |
| bench_thread_pool        | 1.12 ms                                                         | 1.03 ms: 1.09x faster                                                           |
| sympy_integrate          | 16.6 ms                                                         | 15.3 ms: 1.09x faster                                                           |
| sympy_expand             | 391 ms                                                          | 362 ms: 1.08x faster                                                            |
| mdp                      | 1.83 sec                                                        | 1.70 sec: 1.07x faster                                                          |
| docutils                 | 1.95 sec                                                        | 1.82 sec: 1.07x faster                                                          |
| xml_etree_iterparse      | 70.8 ms                                                         | 66.6 ms: 1.06x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 656 us: 1.06x faster                                                            |
| sqlglot_normalize        | 230 ms                                                          | 218 ms: 1.06x faster                                                            |
| regex_compile            | 117 ms                                                          | 111 ms: 1.05x faster                                                            |
| 2to3                     | 265 ms                                                          | 255 ms: 1.04x faster                                                            |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.16 ms: 1.03x faster                                                           |
| xml_etree_generate       | 61.6 ms                                                         | 60.4 ms: 1.02x faster                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                                          |
| scimark_lu               | 89.8 ms                                                         | 89.2 ms: 1.01x faster                                                           |
| meteor_contest           | 80.0 ms                                                         | 79.7 ms: 1.00x faster                                                           |
| pickle_list              | 3.22 us                                                         | 3.25 us: 1.01x slower                                                           |
| regex_v8                 | 15.8 ms                                                         | 16.0 ms: 1.01x slower                                                           |
| pickle                   | 7.83 us                                                         | 8.02 us: 1.02x slower                                                           |
| nqueens                  | 87.1 ms                                                         | 89.2 ms: 1.02x slower                                                           |
| fannkuch                 | 317 ms                                                          | 325 ms: 1.03x slower                                                            |
| hexiom                   | 6.13 ms                                                         | 6.35 ms: 1.03x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 84.6 ms: 1.04x slower                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 65.4 ms: 1.06x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.39 ms: 1.09x slower                                                           |
| scimark_fft              | 216 ms                                                          | 236 ms: 1.09x slower                                                            |
| pprint_pformat           | 1.37 sec                                                        | 1.51 sec: 1.10x slower                                                          |
| logging_format           | 7.91 us                                                         | 8.76 us: 1.11x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 20.3 us: 1.11x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 73.7 ms: 1.11x slower                                                           |
| pprint_safe_repr         | 658 ms                                                          | 735 ms: 1.12x slower                                                            |
| logging_simple           | 7.29 us                                                         | 8.23 us: 1.13x slower                                                           |
| python_startup           | 22.9 ms                                                         | 26.2 ms: 1.14x slower                                                           |
| async_generators         | 241 ms                                                          | 278 ms: 1.15x slower                                                            |
| regex_effbot             | 1.66 ms                                                         | 1.97 ms: 1.18x slower                                                           |
| nbody                    | 79.1 ms                                                         | 93.7 ms: 1.18x slower                                                           |
| telco                    | 4.83 ms                                                         | 6.26 ms: 1.30x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 23.6 ms: 1.30x slower                                                           |
| unpack_sequence          | 40.0 ns                                                         | 61.0 ns: 1.52x slower                                                           |
| coverage                 | 46.6 ms                                                         | 301 ms: 6.47x slower                                                            |
| Geometric mean           | (ref)                                                           | 1.10x faster                                                                    |

Benchmark hidden because not significant (3): regex_dna, sqlglot_optimize, unpickle
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-f0df35e-JIT/bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown