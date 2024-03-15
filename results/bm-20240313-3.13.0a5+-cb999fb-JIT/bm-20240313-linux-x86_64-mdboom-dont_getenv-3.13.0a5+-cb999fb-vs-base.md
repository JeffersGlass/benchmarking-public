# Results vs. base

- fork: mdboom
- ref: dont_getenv
- machine: linux-x86_64
- commit hash: cb999fb
- commit date: 2024-03-13
- overall geometric mean: 1.00x faster
- HPT reliability: 89.19%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5+-61733a2 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| chameleon      | 6.93 ms                                                                | 6.83 ms: 1.01x faster                                         |
| html5lib       | 67.0 ms                                                                | 68.8 ms: 1.03x slower                                         |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                  |

Benchmark hidden because not significant (3): 2to3, docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark      | bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5+-61733a2 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_io  | 1.22 sec                                                               | 1.22 sec: 1.00x faster                                        |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                  |

Benchmark hidden because not significant (7): async_tree_none, async_tree_memoization, async_tree_io_tg, async_tree_none_tg, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5+-61733a2 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| float          | 81.1 ms                                                                | 80.0 ms: 1.01x faster                                         |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                  |

Benchmark hidden because not significant (2): nbody, pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5+-61733a2 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_v8       | 25.8 ms                                                                | 25.4 ms: 1.01x faster                                         |
| regex_compile  | 144 ms                                                                 | 143 ms: 1.01x faster                                          |
| regex_dna      | 225 ms                                                                 | 225 ms: 1.00x faster                                          |
| regex_effbot   | 3.73 ms                                                                | 3.90 ms: 1.04x slower                                         |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5+-61733a2 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|----------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| unpickle_list        | 4.91 us                                                                | 4.80 us: 1.02x faster                                         |
| xml_etree_generate   | 87.6 ms                                                                | 86.7 ms: 1.01x faster                                         |
| json_dumps           | 10.5 ms                                                                | 10.4 ms: 1.01x faster                                         |
| xml_etree_parse      | 160 ms                                                                 | 159 ms: 1.01x faster                                          |
| unpickle_pure_python | 240 us                                                                 | 239 us: 1.01x faster                                          |
| json_loads           | 28.1 us                                                                | 28.3 us: 1.01x slower                                         |
| pickle_pure_python   | 309 us                                                                 | 312 us: 1.01x slower                                          |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                  |

Benchmark hidden because not significant (7): xml_etree_process, xml_etree_iterparse, tomli_loads, pickle_list, pickle_dict, unpickle, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5+-61733a2 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup_no_site | 11.2 ms                                                                | 11.1 ms: 1.01x faster                                         |
| python_startup         | 12.6 ms                                                                | 12.6 ms: 1.00x faster                                         |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                  |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (4): genshi_xml, mako, django_template, genshi_text

All benchmarks:
===============

| Benchmark                | bm-20240313-linux-x86_64-python-61733a2fb9dc36d2246d-3.13.0a5+-61733a2 | bm-20240313-linux-x86_64-mdboom-dont_getenv-3.13.0a5+-cb999fb |
|--------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------:|
| unpack_sequence          | 92.4 ns                                                                | 88.3 ns: 1.05x faster                                         |
| djangocms                | 32.2 us                                                                | 31.0 us: 1.04x faster                                         |
| pycparser                | 1.26 sec                                                               | 1.22 sec: 1.03x faster                                        |
| typing_runtime_protocols | 113 us                                                                 | 110 us: 1.03x faster                                          |
| unpickle_list            | 4.91 us                                                                | 4.80 us: 1.02x faster                                         |
| create_gc_cycles         | 1.55 ms                                                                | 1.52 ms: 1.02x faster                                         |
| scimark_lu               | 132 ms                                                                 | 130 ms: 1.02x faster                                          |
| chameleon                | 6.93 ms                                                                | 6.83 ms: 1.01x faster                                         |
| scimark_fft              | 344 ms                                                                 | 339 ms: 1.01x faster                                          |
| sqlglot_parse            | 1.33 ms                                                                | 1.31 ms: 1.01x faster                                         |
| nqueens                  | 90.9 ms                                                                | 89.6 ms: 1.01x faster                                         |
| float                    | 81.1 ms                                                                | 80.0 ms: 1.01x faster                                         |
| sqlglot_transpile        | 1.67 ms                                                                | 1.65 ms: 1.01x faster                                         |
| regex_v8                 | 25.8 ms                                                                | 25.4 ms: 1.01x faster                                         |
| spectral_norm            | 115 ms                                                                 | 113 ms: 1.01x faster                                          |
| hexiom                   | 7.11 ms                                                                | 7.03 ms: 1.01x faster                                         |
| pyflate                  | 485 ms                                                                 | 480 ms: 1.01x faster                                          |
| xml_etree_generate       | 87.6 ms                                                                | 86.7 ms: 1.01x faster                                         |
| meteor_contest           | 110 ms                                                                 | 109 ms: 1.01x faster                                          |
| telco                    | 8.49 ms                                                                | 8.42 ms: 1.01x faster                                         |
| deltablue                | 3.46 ms                                                                | 3.43 ms: 1.01x faster                                         |
| aiohttp                  | 1.21 ms                                                                | 1.20 ms: 1.01x faster                                         |
| json_dumps               | 10.5 ms                                                                | 10.4 ms: 1.01x faster                                         |
| comprehensions           | 17.4 us                                                                | 17.3 us: 1.01x faster                                         |
| xml_etree_parse          | 160 ms                                                                 | 159 ms: 1.01x faster                                          |
| pathlib                  | 18.8 ms                                                                | 18.7 ms: 1.01x faster                                         |
| unpickle_pure_python     | 240 us                                                                 | 239 us: 1.01x faster                                          |
| regex_compile            | 144 ms                                                                 | 143 ms: 1.01x faster                                          |
| python_startup_no_site   | 11.2 ms                                                                | 11.1 ms: 1.01x faster                                         |
| python_startup           | 12.6 ms                                                                | 12.6 ms: 1.00x faster                                         |
| async_tree_io            | 1.22 sec                                                               | 1.22 sec: 1.00x faster                                        |
| regex_dna                | 225 ms                                                                 | 225 ms: 1.00x faster                                          |
| generators               | 29.6 ms                                                                | 29.5 ms: 1.00x faster                                         |
| sqlglot_optimize         | 56.6 ms                                                                | 56.8 ms: 1.00x slower                                         |
| sympy_integrate          | 21.2 ms                                                                | 21.3 ms: 1.00x slower                                         |
| go                       | 156 ms                                                                 | 156 ms: 1.00x slower                                          |
| mdp                      | 2.62 sec                                                               | 2.63 sec: 1.00x slower                                        |
| asyncio_tcp              | 503 ms                                                                 | 505 ms: 1.00x slower                                          |
| logging_simple           | 5.86 us                                                                | 5.90 us: 1.01x slower                                         |
| json_loads               | 28.1 us                                                                | 28.3 us: 1.01x slower                                         |
| sympy_str                | 285 ms                                                                 | 287 ms: 1.01x slower                                          |
| coverage                 | 97.0 ms                                                                | 97.8 ms: 1.01x slower                                         |
| deepcopy                 | 352 us                                                                 | 355 us: 1.01x slower                                          |
| fannkuch                 | 394 ms                                                                 | 398 ms: 1.01x slower                                          |
| pickle_pure_python       | 309 us                                                                 | 312 us: 1.01x slower                                          |
| crypto_pyaes             | 75.3 ms                                                                | 76.1 ms: 1.01x slower                                         |
| chaos                    | 63.7 ms                                                                | 64.5 ms: 1.01x slower                                         |
| richards_super           | 52.9 ms                                                                | 53.7 ms: 1.01x slower                                         |
| deepcopy_memo            | 39.0 us                                                                | 39.7 us: 1.02x slower                                         |
| logging_silent           | 99.8 ns                                                                | 102 ns: 1.02x slower                                          |
| html5lib                 | 67.0 ms                                                                | 68.8 ms: 1.03x slower                                         |
| gc_traversal             | 3.97 ms                                                                | 4.09 ms: 1.03x slower                                         |
| regex_effbot             | 3.73 ms                                                                | 3.90 ms: 1.04x slower                                         |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                  |

Benchmark hidden because not significant (49): pprint_safe_repr, async_tree_none, tornado_http, logging_format, xml_etree_process, json, thrift, coroutines, pprint_pformat, xml_etree_iterparse, gunicorn, tomli_loads, sqlite_synth, async_tree_memoization, scimark_sor, deepcopy_reduce, mypy2, pickle_list, pickle_dict, nbody, async_tree_io_tg, asyncio_websockets, dulwich_log, genshi_xml, async_generators, async_tree_none_tg, mako, pylint, bench_mp_pool, sympy_expand, django_template, asyncio_tcp_ssl, unpickle, genshi_text, dask, bench_thread_pool, async_tree_cpu_io_mixed, 2to3, scimark_sparse_mat_mult, sqlglot_normalize, docutils, sympy_sum, pidigits, richards, pickle, async_tree_cpu_io_mixed_tg, scimark_monte_carlo, raytrace, async_tree_memoization_tg


# HPT report

- Reliability score: 89.19% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x