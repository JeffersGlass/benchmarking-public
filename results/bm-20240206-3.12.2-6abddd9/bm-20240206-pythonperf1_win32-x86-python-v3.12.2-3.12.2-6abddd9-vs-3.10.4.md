
# Results vs. 3.10.4

- fork: python
- ref: v3.12.2
- machine: windows-x86
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.01x faster \*
- HPT reliability: 65.44%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 274 ms: 1.03x slower                                            |
| chameleon      | 6.42 ms                                                         | 7.50 ms: 1.17x slower                                           |
| docutils       | 1.95 sec                                                        | 1.93 sec: 1.01x faster                                          |
| tornado_http   | 118 ms                                                          | 104 ms: 1.13x faster                                            |
| Geometric mean | (ref)                                                           | 1.01x slower                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|-------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 555 ms: 1.66x faster                                            |
| async_tree_io           | 940 ms                                                          | 678 ms: 1.39x faster                                            |
| async_tree_none         | 394 ms                                                          | 299 ms: 1.32x faster                                            |
| async_tree_memoization  | 467 ms                                                          | 358 ms: 1.30x faster                                            |
| Geometric mean          | (ref)                                                           | 1.41x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.54x faster                                            |
| float          | 69.6 ms                                                         | 73.6 ms: 1.06x slower                                           |
| nbody          | 79.1 ms                                                         | 124 ms: 1.56x slower                                            |
| Geometric mean | (ref)                                                           | 1.16x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 120 ms: 1.09x faster                                            |
| regex_v8       | 15.8 ms                                                         | 15.4 ms: 1.02x faster                                           |
| regex_compile  | 117 ms                                                          | 126 ms: 1.08x slower                                            |
| regex_effbot   | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                           |
| Geometric mean | (ref)                                                           | 1.03x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 7.47 ms: 1.31x faster                                           |
| json_loads           | 22.4 us                                                         | 20.3 us: 1.10x faster                                           |
| xml_etree_parse      | 120 ms                                                          | 111 ms: 1.08x faster                                            |
| unpickle             | 9.82 us                                                         | 9.42 us: 1.04x faster                                           |
| unpickle_list        | 2.98 us                                                         | 2.96 us: 1.01x faster                                           |
| pickle_list          | 3.22 us                                                         | 3.26 us: 1.01x slower                                           |
| pickle_pure_python   | 280 us                                                          | 286 us: 1.02x slower                                            |
| unpickle_pure_python | 189 us                                                          | 205 us: 1.08x slower                                            |
| xml_etree_iterparse  | 70.8 ms                                                         | 77.1 ms: 1.09x slower                                           |
| pickle_dict          | 18.2 us                                                         | 20.1 us: 1.10x slower                                           |
| xml_etree_process    | 48.1 ms                                                         | 53.9 ms: 1.12x slower                                           |
| tomli_loads          | 1.91 sec                                                        | 2.17 sec: 1.14x slower                                          |
| xml_etree_generate   | 61.6 ms                                                         | 72.8 ms: 1.18x slower                                           |
| Geometric mean       | (ref)                                                           | 1.01x slower                                                    |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup | 22.9 ms                                                         | 21.3 ms: 1.07x faster                                           |
| Geometric mean | (ref)                                                           | 1.03x faster                                                    |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| mako           | 9.10 ms                                                         | 9.80 ms: 1.08x slower                                           |
| Geometric mean | (ref)                                                           | 1.04x slower                                                    |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9 |
|--------------------------|:---------------------------------------------------------------:|:---------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 113 us: 3.51x faster                                            |
| pidigits                 | 502 ms                                                          | 198 ms: 2.54x faster                                            |
| sqlglot_normalize        | 230 ms                                                          | 102 ms: 2.27x faster                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 555 ms: 1.66x faster                                            |
| async_tree_io            | 940 ms                                                          | 678 ms: 1.39x faster                                            |
| async_tree_none          | 394 ms                                                          | 299 ms: 1.32x faster                                            |
| json_dumps               | 9.82 ms                                                         | 7.47 ms: 1.31x faster                                           |
| async_tree_memoization   | 467 ms                                                          | 358 ms: 1.30x faster                                            |
| crypto_pyaes             | 81.3 ms                                                         | 68.5 ms: 1.19x faster                                           |
| asyncio_tcp              | 744 ms                                                          | 645 ms: 1.15x faster                                            |
| deltablue                | 4.04 ms                                                         | 3.52 ms: 1.15x faster                                           |
| tornado_http             | 118 ms                                                          | 104 ms: 1.13x faster                                            |
| json                     | 4.76 ms                                                         | 4.24 ms: 1.12x faster                                           |
| mypy2                    | 590 ms                                                          | 529 ms: 1.11x faster                                            |
| aiohttp                  | 1.13 ms                                                         | 1.02 ms: 1.11x faster                                           |
| json_loads               | 22.4 us                                                         | 20.3 us: 1.10x faster                                           |
| sqlalchemy_imperative    | 13.2 ms                                                         | 11.9 ms: 1.10x faster                                           |
| sqlite_synth             | 2.29 us                                                         | 2.09 us: 1.10x faster                                           |
| chaos                    | 74.4 ms                                                         | 68.0 ms: 1.09x faster                                           |
| pycparser                | 1.04 sec                                                        | 955 ms: 1.09x faster                                            |
| go                       | 146 ms                                                          | 134 ms: 1.09x faster                                            |
| regex_dna                | 131 ms                                                          | 120 ms: 1.09x faster                                            |
| create_gc_cycles         | 694 us                                                          | 641 us: 1.08x faster                                            |
| xml_etree_parse          | 120 ms                                                          | 111 ms: 1.08x faster                                            |
| python_startup           | 22.9 ms                                                         | 21.3 ms: 1.07x faster                                           |
| sqlglot_parse            | 1.33 ms                                                         | 1.24 ms: 1.07x faster                                           |
| dask                     | 341 ms                                                          | 321 ms: 1.06x faster                                            |
| richards_super           | 49.9 ms                                                         | 46.9 ms: 1.06x faster                                           |
| dulwich_log              | 58.5 ms                                                         | 55.7 ms: 1.05x faster                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.51 ms: 1.05x faster                                           |
| unpickle                 | 9.82 us                                                         | 9.42 us: 1.04x faster                                           |
| sqlalchemy_declarative   | 104 ms                                                          | 101 ms: 1.04x faster                                            |
| regex_v8                 | 15.8 ms                                                         | 15.4 ms: 1.02x faster                                           |
| sympy_sum                | 122 ms                                                          | 120 ms: 1.02x faster                                            |
| docutils                 | 1.95 sec                                                        | 1.93 sec: 1.01x faster                                          |
| pyflate                  | 422 ms                                                          | 417 ms: 1.01x faster                                            |
| unpickle_list            | 2.98 us                                                         | 2.96 us: 1.01x faster                                           |
| raytrace                 | 303 ms                                                          | 301 ms: 1.01x faster                                            |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.9 sec: 1.01x faster                                          |
| mdp                      | 1.83 sec                                                        | 1.83 sec: 1.00x slower                                          |
| sympy_expand             | 391 ms                                                          | 393 ms: 1.01x slower                                            |
| pickle_list              | 3.22 us                                                         | 3.26 us: 1.01x slower                                           |
| pickle_pure_python       | 280 us                                                          | 286 us: 1.02x slower                                            |
| logging_silent           | 97.9 ns                                                         | 101 ns: 1.03x slower                                            |
| sympy_integrate          | 16.6 ms                                                         | 17.2 ms: 1.03x slower                                           |
| coverage                 | 46.6 ms                                                         | 48.0 ms: 1.03x slower                                           |
| 2to3                     | 265 ms                                                          | 274 ms: 1.03x slower                                            |
| richards                 | 40.3 ms                                                         | 41.8 ms: 1.04x slower                                           |
| sympy_str                | 229 ms                                                          | 238 ms: 1.04x slower                                            |
| pathlib                  | 81.2 ms                                                         | 85.1 ms: 1.05x slower                                           |
| scimark_lu               | 89.8 ms                                                         | 94.0 ms: 1.05x slower                                           |
| float                    | 69.6 ms                                                         | 73.6 ms: 1.06x slower                                           |
| sqlglot_optimize         | 44.7 ms                                                         | 47.6 ms: 1.06x slower                                           |
| mako                     | 9.10 ms                                                         | 9.80 ms: 1.08x slower                                           |
| regex_compile            | 117 ms                                                          | 126 ms: 1.08x slower                                            |
| bench_mp_pool            | 66.4 ms                                                         | 71.6 ms: 1.08x slower                                           |
| telco                    | 4.83 ms                                                         | 5.22 ms: 1.08x slower                                           |
| unpickle_pure_python     | 189 us                                                          | 205 us: 1.08x slower                                            |
| meteor_contest           | 80.0 ms                                                         | 86.5 ms: 1.08x slower                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 67.3 ms: 1.09x slower                                           |
| xml_etree_iterparse      | 70.8 ms                                                         | 77.1 ms: 1.09x slower                                           |
| nqueens                  | 87.1 ms                                                         | 94.8 ms: 1.09x slower                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.50 sec: 1.09x slower                                          |
| gc_traversal             | 1.28 ms                                                         | 1.40 ms: 1.10x slower                                           |
| hexiom                   | 6.13 ms                                                         | 6.75 ms: 1.10x slower                                           |
| pickle_dict              | 18.2 us                                                         | 20.1 us: 1.10x slower                                           |
| comprehensions           | 17.7 us                                                         | 19.6 us: 1.10x slower                                           |
| pprint_safe_repr         | 658 ms                                                          | 728 ms: 1.11x slower                                            |
| xml_etree_process        | 48.1 ms                                                         | 53.9 ms: 1.12x slower                                           |
| scimark_sor              | 115 ms                                                          | 130 ms: 1.13x slower                                            |
| tomli_loads              | 1.91 sec                                                        | 2.17 sec: 1.14x slower                                          |
| regex_effbot             | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                           |
| coroutines               | 17.9 ms                                                         | 20.7 ms: 1.15x slower                                           |
| deepcopy                 | 310 us                                                          | 358 us: 1.15x slower                                            |
| fannkuch                 | 317 ms                                                          | 367 ms: 1.16x slower                                            |
| chameleon                | 6.42 ms                                                         | 7.50 ms: 1.17x slower                                           |
| xml_etree_generate       | 61.6 ms                                                         | 72.8 ms: 1.18x slower                                           |
| deepcopy_reduce          | 2.68 us                                                         | 3.24 us: 1.21x slower                                           |
| generators               | 31.6 ms                                                         | 38.1 ms: 1.21x slower                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.93 ms: 1.21x slower                                           |
| scimark_fft              | 216 ms                                                          | 269 ms: 1.25x slower                                            |
| async_generators         | 241 ms                                                          | 307 ms: 1.27x slower                                            |
| deepcopy_memo            | 29.6 us                                                         | 37.8 us: 1.28x slower                                           |
| spectral_norm            | 80.2 ms                                                         | 102 ms: 1.28x slower                                            |
| logging_format           | 7.91 us                                                         | 10.1 us: 1.28x slower                                           |
| logging_simple           | 7.29 us                                                         | 9.50 us: 1.30x slower                                           |
| unpack_sequence          | 40.0 ns                                                         | 62.1 ns: 1.55x slower                                           |
| nbody                    | 79.1 ms                                                         | 124 ms: 1.56x slower                                            |
| Geometric mean           | (ref)                                                           | 1.01x faster                                                    |

Benchmark hidden because not significant (4): bench_thread_pool, pickle, django_template, python_startup_no_site
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
Ignored benchmarks (4) of results/bm-20240206-3.12.2-6abddd9/bm-20240206-pythonperf1_win32-x86-python-v3.12.2-3.12.2-6abddd9.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 65.44% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown