# Results vs. base

- fork: brandtbucher
- ref: justin_relax_absolut
- machine: linux-x86_64
- commit hash: 78b2070
- commit date: 2024-03-14
- overall geometric mean: 1.00x faster
- HPT reliability: 95.20%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                                 | 284 ms: 1.01x slower                                                         |
| chameleon      | 6.90 ms                                                                | 6.96 ms: 1.01x slower                                                        |
| html5lib       | 65.7 ms                                                                | 68.2 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io    | 1.22 sec                                                               | 1.21 sec: 1.00x faster                                                       |
| async_tree_io_tg | 1.24 sec                                                               | 1.23 sec: 1.00x faster                                                       |
| Geometric mean   | (ref)                                                                  | 1.00x slower                                                                 |

Benchmark hidden because not significant (6): async_tree_none, async_tree_memoization, async_tree_none_tg, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 189 ms                                                                 | 190 ms: 1.01x slower                                                         |
| float          | 79.8 ms                                                                | 81.3 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 238 ms                                                                 | 225 ms: 1.06x faster                                                         |
| regex_v8       | 25.4 ms                                                                | 24.0 ms: 1.06x faster                                                        |
| regex_effbot   | 3.82 ms                                                                | 3.65 ms: 1.05x faster                                                        |
| regex_compile  | 144 ms                                                                 | 144 ms: 1.00x slower                                                         |
| Geometric mean | (ref)                                                                  | 1.04x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_list          | 5.31 us                                                                | 4.81 us: 1.10x faster                                                        |
| unpickle_list        | 4.93 us                                                                | 4.81 us: 1.03x faster                                                        |
| pickle_dict          | 35.4 us                                                                | 34.9 us: 1.02x faster                                                        |
| pickle               | 12.0 us                                                                | 11.8 us: 1.01x faster                                                        |
| tomli_loads          | 2.08 sec                                                               | 2.05 sec: 1.01x faster                                                       |
| xml_etree_parse      | 159 ms                                                                 | 161 ms: 1.01x slower                                                         |
| xml_etree_process    | 59.9 ms                                                                | 60.6 ms: 1.01x slower                                                        |
| xml_etree_generate   | 86.8 ms                                                                | 88.1 ms: 1.01x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                                 | 109 ms: 1.02x slower                                                         |
| json_loads           | 27.9 us                                                                | 28.4 us: 1.02x slower                                                        |
| unpickle_pure_python | 239 us                                                                 | 245 us: 1.03x slower                                                         |
| unpickle             | 15.1 us                                                                | 15.7 us: 1.04x slower                                                        |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                                 |

Benchmark hidden because not significant (2): pickle_pure_python, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup_no_site | 11.2 ms                                                                | 11.2 ms: 1.00x slower                                                        |
| python_startup         | 12.6 ms                                                                | 12.6 ms: 1.00x slower                                                        |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|-----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| genshi_text     | 24.7 ms                                                                | 24.1 ms: 1.03x faster                                                        |
| genshi_xml      | 54.9 ms                                                                | 54.3 ms: 1.01x faster                                                        |
| django_template | 34.4 ms                                                                | 34.2 ms: 1.01x faster                                                        |
| mako            | 10.7 ms                                                                | 10.9 ms: 1.02x slower                                                        |
| Geometric mean  | (ref)                                                                  | 1.01x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|--------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_list              | 5.31 us                                                                | 4.81 us: 1.10x faster                                                        |
| regex_dna                | 238 ms                                                                 | 225 ms: 1.06x faster                                                         |
| regex_v8                 | 25.4 ms                                                                | 24.0 ms: 1.06x faster                                                        |
| regex_effbot             | 3.82 ms                                                                | 3.65 ms: 1.05x faster                                                        |
| mdp                      | 2.75 sec                                                               | 2.65 sec: 1.04x faster                                                       |
| pprint_safe_repr         | 779 ms                                                                 | 751 ms: 1.04x faster                                                         |
| gc_traversal             | 3.95 ms                                                                | 3.81 ms: 1.04x faster                                                        |
| unpack_sequence          | 90.6 ns                                                                | 87.8 ns: 1.03x faster                                                        |
| genshi_text              | 24.7 ms                                                                | 24.1 ms: 1.03x faster                                                        |
| pycparser                | 1.25 sec                                                               | 1.22 sec: 1.03x faster                                                       |
| unpickle_list            | 4.93 us                                                                | 4.81 us: 1.03x faster                                                        |
| djangocms                | 32.2 us                                                                | 31.4 us: 1.02x faster                                                        |
| asyncio_tcp              | 503 ms                                                                 | 495 ms: 1.02x faster                                                         |
| deepcopy_reduce          | 3.09 us                                                                | 3.04 us: 1.02x faster                                                        |
| pickle_dict              | 35.4 us                                                                | 34.9 us: 1.02x faster                                                        |
| logging_silent           | 102 ns                                                                 | 100 ns: 1.02x faster                                                         |
| pickle                   | 12.0 us                                                                | 11.8 us: 1.01x faster                                                        |
| pathlib                  | 18.8 ms                                                                | 18.5 ms: 1.01x faster                                                        |
| tomli_loads              | 2.08 sec                                                               | 2.05 sec: 1.01x faster                                                       |
| genshi_xml               | 54.9 ms                                                                | 54.3 ms: 1.01x faster                                                        |
| dulwich_log              | 70.5 ms                                                                | 69.9 ms: 1.01x faster                                                        |
| logging_format           | 6.46 us                                                                | 6.40 us: 1.01x faster                                                        |
| django_template          | 34.4 ms                                                                | 34.2 ms: 1.01x faster                                                        |
| scimark_sparse_mat_mult  | 4.91 ms                                                                | 4.89 ms: 1.01x faster                                                        |
| sympy_sum                | 163 ms                                                                 | 162 ms: 1.00x faster                                                         |
| async_tree_io            | 1.22 sec                                                               | 1.21 sec: 1.00x faster                                                       |
| async_tree_io_tg         | 1.24 sec                                                               | 1.23 sec: 1.00x faster                                                       |
| asyncio_tcp_ssl          | 1.85 sec                                                               | 1.85 sec: 1.00x faster                                                       |
| python_startup_no_site   | 11.2 ms                                                                | 11.2 ms: 1.00x slower                                                        |
| python_startup           | 12.6 ms                                                                | 12.6 ms: 1.00x slower                                                        |
| sqlglot_optimize         | 56.6 ms                                                                | 56.8 ms: 1.00x slower                                                        |
| regex_compile            | 144 ms                                                                 | 144 ms: 1.00x slower                                                         |
| go                       | 158 ms                                                                 | 158 ms: 1.00x slower                                                         |
| async_generators         | 469 ms                                                                 | 471 ms: 1.00x slower                                                         |
| pidigits                 | 189 ms                                                                 | 190 ms: 1.01x slower                                                         |
| 2to3                     | 282 ms                                                                 | 284 ms: 1.01x slower                                                         |
| xml_etree_parse          | 159 ms                                                                 | 161 ms: 1.01x slower                                                         |
| scimark_fft              | 343 ms                                                                 | 346 ms: 1.01x slower                                                         |
| chameleon                | 6.90 ms                                                                | 6.96 ms: 1.01x slower                                                        |
| scimark_sor              | 130 ms                                                                 | 131 ms: 1.01x slower                                                         |
| scimark_lu               | 132 ms                                                                 | 134 ms: 1.01x slower                                                         |
| deltablue                | 3.44 ms                                                                | 3.48 ms: 1.01x slower                                                        |
| meteor_contest           | 110 ms                                                                 | 111 ms: 1.01x slower                                                         |
| xml_etree_process        | 59.9 ms                                                                | 60.6 ms: 1.01x slower                                                        |
| xml_etree_generate       | 86.8 ms                                                                | 88.1 ms: 1.01x slower                                                        |
| typing_runtime_protocols | 110 us                                                                 | 112 us: 1.01x slower                                                         |
| xml_etree_iterparse      | 107 ms                                                                 | 109 ms: 1.02x slower                                                         |
| json_loads               | 27.9 us                                                                | 28.4 us: 1.02x slower                                                        |
| chaos                    | 64.1 ms                                                                | 65.3 ms: 1.02x slower                                                        |
| float                    | 79.8 ms                                                                | 81.3 ms: 1.02x slower                                                        |
| fannkuch                 | 395 ms                                                                 | 403 ms: 1.02x slower                                                         |
| create_gc_cycles         | 1.52 ms                                                                | 1.55 ms: 1.02x slower                                                        |
| mako                     | 10.7 ms                                                                | 10.9 ms: 1.02x slower                                                        |
| crypto_pyaes             | 75.6 ms                                                                | 77.3 ms: 1.02x slower                                                        |
| richards_super           | 52.2 ms                                                                | 53.5 ms: 1.03x slower                                                        |
| pyflate                  | 490 ms                                                                 | 503 ms: 1.03x slower                                                         |
| unpickle_pure_python     | 239 us                                                                 | 245 us: 1.03x slower                                                         |
| richards                 | 46.5 ms                                                                | 47.7 ms: 1.03x slower                                                        |
| raytrace                 | 294 ms                                                                 | 302 ms: 1.03x slower                                                         |
| hexiom                   | 7.09 ms                                                                | 7.29 ms: 1.03x slower                                                        |
| comprehensions           | 17.3 us                                                                | 17.9 us: 1.03x slower                                                        |
| unpickle                 | 15.1 us                                                                | 15.7 us: 1.04x slower                                                        |
| html5lib                 | 65.7 ms                                                                | 68.2 ms: 1.04x slower                                                        |
| scimark_monte_carlo      | 70.1 ms                                                                | 73.1 ms: 1.04x slower                                                        |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                                 |

Benchmark hidden because not significant (38): thrift, logging_simple, dask, pickle_pure_python, sympy_str, pprint_pformat, async_tree_none, bench_thread_pool, async_tree_memoization, coverage, deepcopy_memo, asyncio_websockets, mypy2, sqlglot_parse, sqlglot_transpile, spectral_norm, pylint, sympy_integrate, sympy_expand, async_tree_none_tg, docutils, generators, gunicorn, coroutines, bench_mp_pool, sqlite_synth, json_dumps, aiohttp, sqlglot_normalize, nbody, deepcopy, nqueens, async_tree_memoization_tg, tornado_http, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, telco, json


# HPT report

- Reliability score: 95.20% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x