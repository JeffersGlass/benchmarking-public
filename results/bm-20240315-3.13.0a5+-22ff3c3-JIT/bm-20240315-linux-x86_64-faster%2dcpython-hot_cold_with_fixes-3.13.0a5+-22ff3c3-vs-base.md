# Results vs. base

- fork: faster-cpython
- ref: hot_cold_with_fixes
- machine: linux-x86_64
- commit hash: 22ff3c3
- commit date: 2024-03-15
- overall geometric mean: 1.00x faster
- HPT reliability: 70.05%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.92x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                                 | 281 ms: 1.00x faster                                                            |
| chameleon      | 6.96 ms                                                                | 7.17 ms: 1.03x slower                                                           |
| docutils       | 2.78 sec                                                               | 2.77 sec: 1.00x faster                                                          |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                    |

Benchmark hidden because not significant (2): html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|-------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 731 ms                                                                 | 722 ms: 1.01x faster                                                            |
| async_tree_none_tg      | 461 ms                                                                 | 458 ms: 1.01x faster                                                            |
| Geometric mean          | (ref)                                                                  | 1.00x faster                                                                    |

Benchmark hidden because not significant (6): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_io, async_tree_io_tg, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 189 ms                                                                 | 189 ms: 1.00x faster                                                            |
| float          | 80.0 ms                                                                | 80.7 ms: 1.01x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                    |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_v8       | 25.9 ms                                                                | 24.9 ms: 1.04x faster                                                           |
| regex_dna      | 234 ms                                                                 | 228 ms: 1.03x faster                                                            |
| regex_effbot   | 3.79 ms                                                                | 3.69 ms: 1.03x faster                                                           |
| regex_compile  | 143 ms                                                                 | 145 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|--------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pickle_dict        | 35.4 us                                                                | 34.7 us: 1.02x faster                                                           |
| json_dumps         | 10.6 ms                                                                | 10.4 ms: 1.01x faster                                                           |
| pickle_list        | 5.29 us                                                                | 5.26 us: 1.01x faster                                                           |
| xml_etree_process  | 60.6 ms                                                                | 61.1 ms: 1.01x slower                                                           |
| pickle             | 11.9 us                                                                | 12.1 us: 1.01x slower                                                           |
| unpickle_list      | 4.93 us                                                                | 4.99 us: 1.01x slower                                                           |
| pickle_pure_python | 308 us                                                                 | 312 us: 1.01x slower                                                            |
| json_loads         | 28.1 us                                                                | 28.9 us: 1.03x slower                                                           |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                                                    |

Benchmark hidden because not significant (6): xml_etree_iterparse, tomli_loads, unpickle_pure_python, xml_etree_parse, xml_etree_generate, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup_no_site | 11.2 ms                                                                | 9.93 ms: 1.12x faster                                                           |
| python_startup         | 12.6 ms                                                                | 11.3 ms: 1.11x faster                                                           |
| Geometric mean         | (ref)                                                                  | 1.12x faster                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| genshi_xml     | 54.6 ms                                                                | 56.8 ms: 1.04x slower                                                           |
| genshi_text    | 24.2 ms                                                                | 25.6 ms: 1.06x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                                    |

Benchmark hidden because not significant (2): django_template, mako

All benchmarks:
===============

| Benchmark                | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|--------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| gc_traversal             | 4.07 ms                                                                | 3.57 ms: 1.14x faster                                                           |
| python_startup_no_site   | 11.2 ms                                                                | 9.93 ms: 1.12x faster                                                           |
| python_startup           | 12.6 ms                                                                | 11.3 ms: 1.11x faster                                                           |
| bench_mp_pool            | 26.8 ms                                                                | 24.8 ms: 1.08x faster                                                           |
| regex_v8                 | 25.9 ms                                                                | 24.9 ms: 1.04x faster                                                           |
| crypto_pyaes             | 77.0 ms                                                                | 74.6 ms: 1.03x faster                                                           |
| unpack_sequence          | 87.8 ns                                                                | 85.2 ns: 1.03x faster                                                           |
| pycparser                | 1.26 sec                                                               | 1.22 sec: 1.03x faster                                                          |
| pyflate                  | 493 ms                                                                 | 479 ms: 1.03x faster                                                            |
| regex_dna                | 234 ms                                                                 | 228 ms: 1.03x faster                                                            |
| regex_effbot             | 3.79 ms                                                                | 3.69 ms: 1.03x faster                                                           |
| raytrace                 | 297 ms                                                                 | 290 ms: 1.02x faster                                                            |
| djangocms                | 32.3 us                                                                | 31.6 us: 1.02x faster                                                           |
| spectral_norm            | 115 ms                                                                 | 113 ms: 1.02x faster                                                            |
| pickle_dict              | 35.4 us                                                                | 34.7 us: 1.02x faster                                                           |
| logging_silent           | 102 ns                                                                 | 101 ns: 1.02x faster                                                            |
| coverage                 | 98.5 ms                                                                | 96.9 ms: 1.02x faster                                                           |
| scimark_monte_carlo      | 70.9 ms                                                                | 69.8 ms: 1.02x faster                                                           |
| pprint_safe_repr         | 770 ms                                                                 | 759 ms: 1.02x faster                                                            |
| json_dumps               | 10.6 ms                                                                | 10.4 ms: 1.01x faster                                                           |
| async_tree_cpu_io_mixed  | 731 ms                                                                 | 722 ms: 1.01x faster                                                            |
| scimark_fft              | 345 ms                                                                 | 342 ms: 1.01x faster                                                            |
| asyncio_tcp_ssl          | 1.85 sec                                                               | 1.84 sec: 1.01x faster                                                          |
| async_tree_none_tg       | 461 ms                                                                 | 458 ms: 1.01x faster                                                            |
| sqlite_synth             | 2.87 us                                                                | 2.86 us: 1.01x faster                                                           |
| pickle_list              | 5.29 us                                                                | 5.26 us: 1.01x faster                                                           |
| docutils                 | 2.78 sec                                                               | 2.77 sec: 1.00x faster                                                          |
| 2to3                     | 282 ms                                                                 | 281 ms: 1.00x faster                                                            |
| pidigits                 | 189 ms                                                                 | 189 ms: 1.00x faster                                                            |
| sympy_integrate          | 21.3 ms                                                                | 21.4 ms: 1.00x slower                                                           |
| bench_thread_pool        | 864 us                                                                 | 869 us: 1.01x slower                                                            |
| pathlib                  | 18.7 ms                                                                | 18.8 ms: 1.01x slower                                                           |
| deepcopy_memo            | 38.9 us                                                                | 39.1 us: 1.01x slower                                                           |
| sympy_expand             | 486 ms                                                                 | 489 ms: 1.01x slower                                                            |
| sqlglot_optimize         | 56.8 ms                                                                | 57.2 ms: 1.01x slower                                                           |
| sqlglot_transpile        | 1.66 ms                                                                | 1.67 ms: 1.01x slower                                                           |
| dulwich_log              | 70.0 ms                                                                | 70.5 ms: 1.01x slower                                                           |
| sympy_str                | 287 ms                                                                 | 289 ms: 1.01x slower                                                            |
| xml_etree_process        | 60.6 ms                                                                | 61.1 ms: 1.01x slower                                                           |
| float                    | 80.0 ms                                                                | 80.7 ms: 1.01x slower                                                           |
| richards                 | 46.5 ms                                                                | 46.9 ms: 1.01x slower                                                           |
| fannkuch                 | 399 ms                                                                 | 403 ms: 1.01x slower                                                            |
| pickle                   | 11.9 us                                                                | 12.1 us: 1.01x slower                                                           |
| nqueens                  | 90.0 ms                                                                | 91.1 ms: 1.01x slower                                                           |
| unpickle_list            | 4.93 us                                                                | 4.99 us: 1.01x slower                                                           |
| create_gc_cycles         | 1.51 ms                                                                | 1.53 ms: 1.01x slower                                                           |
| regex_compile            | 143 ms                                                                 | 145 ms: 1.01x slower                                                            |
| pickle_pure_python       | 308 us                                                                 | 312 us: 1.01x slower                                                            |
| async_generators         | 469 ms                                                                 | 475 ms: 1.01x slower                                                            |
| mdp                      | 2.61 sec                                                               | 2.64 sec: 1.01x slower                                                          |
| sqlglot_normalize        | 108 ms                                                                 | 110 ms: 1.02x slower                                                            |
| hexiom                   | 7.06 ms                                                                | 7.17 ms: 1.02x slower                                                           |
| go                       | 157 ms                                                                 | 160 ms: 1.02x slower                                                            |
| typing_runtime_protocols | 111 us                                                                 | 113 us: 1.02x slower                                                            |
| richards_super           | 53.1 ms                                                                | 54.0 ms: 1.02x slower                                                           |
| deepcopy                 | 351 us                                                                 | 358 us: 1.02x slower                                                            |
| comprehensions           | 17.5 us                                                                | 17.9 us: 1.02x slower                                                           |
| scimark_sparse_mat_mult  | 4.82 ms                                                                | 4.93 ms: 1.02x slower                                                           |
| deepcopy_reduce          | 3.06 us                                                                | 3.13 us: 1.02x slower                                                           |
| generators               | 29.5 ms                                                                | 30.3 ms: 1.03x slower                                                           |
| logging_format           | 6.42 us                                                                | 6.60 us: 1.03x slower                                                           |
| json_loads               | 28.1 us                                                                | 28.9 us: 1.03x slower                                                           |
| deltablue                | 3.42 ms                                                                | 3.52 ms: 1.03x slower                                                           |
| chameleon                | 6.96 ms                                                                | 7.17 ms: 1.03x slower                                                           |
| logging_simple           | 5.77 us                                                                | 5.95 us: 1.03x slower                                                           |
| scimark_lu               | 129 ms                                                                 | 133 ms: 1.03x slower                                                            |
| genshi_xml               | 54.6 ms                                                                | 56.8 ms: 1.04x slower                                                           |
| genshi_text              | 24.2 ms                                                                | 25.6 ms: 1.06x slower                                                           |
| scimark_sor              | 127 ms                                                                 | 135 ms: 1.06x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                                    |

Benchmark hidden because not significant (33): pprint_pformat, html5lib, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, chaos, xml_etree_iterparse, thrift, async_tree_none, tomli_loads, django_template, async_tree_io, unpickle_pure_python, sympy_sum, xml_etree_parse, async_tree_io_tg, aiohttp, asyncio_websockets, nbody, xml_etree_generate, gunicorn, asyncio_tcp, coroutines, meteor_contest, tornado_http, pylint, async_tree_memoization, telco, sqlglot_parse, unpickle, mypy2, mako, json, dask


# HPT report

- Reliability score: 70.05% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.92x