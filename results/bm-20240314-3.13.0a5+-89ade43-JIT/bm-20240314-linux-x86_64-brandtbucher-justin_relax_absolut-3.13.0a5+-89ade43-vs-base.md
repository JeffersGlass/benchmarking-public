# Results vs. base

- fork: brandtbucher
- ref: justin_relax_absolut
- machine: linux-x86_64
- commit hash: 89ade43
- commit date: 2024-03-14
- overall geometric mean: 1.00x slower
- HPT reliability: 99.25%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.92x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| docutils       | 2.77 sec                                                               | 2.79 sec: 1.01x slower                                                       |
| html5lib       | 65.7 ms                                                                | 68.3 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (3): 2to3, chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|---------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none_tg        | 459 ms                                                                 | 461 ms: 1.00x slower                                                         |
| async_tree_io             | 1.22 sec                                                               | 1.22 sec: 1.01x slower                                                       |
| async_tree_io_tg          | 1.24 sec                                                               | 1.25 sec: 1.01x slower                                                       |
| async_tree_memoization_tg | 592 ms                                                                 | 600 ms: 1.01x slower                                                         |
| Geometric mean            | (ref)                                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 79.8 ms                                                                | 82.7 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (2): nbody, pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 238 ms                                                                 | 227 ms: 1.05x faster                                                         |
| regex_effbot   | 3.82 ms                                                                | 3.74 ms: 1.02x faster                                                        |
| regex_v8       | 25.4 ms                                                                | 25.9 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_list          | 5.31 us                                                                | 5.08 us: 1.04x faster                                                        |
| pickle               | 12.0 us                                                                | 11.6 us: 1.03x faster                                                        |
| unpickle_list        | 4.93 us                                                                | 4.83 us: 1.02x faster                                                        |
| pickle_dict          | 35.4 us                                                                | 34.9 us: 1.01x faster                                                        |
| pickle_pure_python   | 302 us                                                                 | 301 us: 1.00x faster                                                         |
| xml_etree_process    | 59.9 ms                                                                | 60.2 ms: 1.01x slower                                                        |
| json_dumps           | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                                        |
| xml_etree_parse      | 159 ms                                                                 | 162 ms: 1.01x slower                                                         |
| xml_etree_iterparse  | 107 ms                                                                 | 109 ms: 1.02x slower                                                         |
| xml_etree_generate   | 86.8 ms                                                                | 88.3 ms: 1.02x slower                                                        |
| json_loads           | 27.9 us                                                                | 28.4 us: 1.02x slower                                                        |
| unpickle_pure_python | 239 us                                                                 | 244 us: 1.02x slower                                                         |
| unpickle             | 15.1 us                                                                | 15.5 us: 1.02x slower                                                        |
| Geometric mean       | (ref)                                                                  | 1.00x slower                                                                 |

Benchmark hidden because not significant (1): tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup_no_site | 11.2 ms                                                                | 10.1 ms: 1.11x faster                                                        |
| python_startup         | 12.6 ms                                                                | 11.5 ms: 1.10x faster                                                        |
| Geometric mean         | (ref)                                                                  | 1.10x faster                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|-----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| django_template | 34.4 ms                                                                | 34.3 ms: 1.00x faster                                                        |
| mako            | 10.7 ms                                                                | 10.8 ms: 1.01x slower                                                        |
| Geometric mean  | (ref)                                                                  | 1.00x faster                                                                 |

Benchmark hidden because not significant (2): genshi_text, genshi_xml

All benchmarks:
===============

| Benchmark                 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|---------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup_no_site    | 11.2 ms                                                                | 10.1 ms: 1.11x faster                                                        |
| bench_mp_pool             | 26.4 ms                                                                | 24.0 ms: 1.10x faster                                                        |
| python_startup            | 12.6 ms                                                                | 11.5 ms: 1.10x faster                                                        |
| regex_dna                 | 238 ms                                                                 | 227 ms: 1.05x faster                                                         |
| pickle_list               | 5.31 us                                                                | 5.08 us: 1.04x faster                                                        |
| mdp                       | 2.75 sec                                                               | 2.64 sec: 1.04x faster                                                       |
| unpack_sequence           | 90.6 ns                                                                | 87.5 ns: 1.04x faster                                                        |
| pickle                    | 12.0 us                                                                | 11.6 us: 1.03x faster                                                        |
| pprint_safe_repr          | 779 ms                                                                 | 756 ms: 1.03x faster                                                         |
| regex_effbot              | 3.82 ms                                                                | 3.74 ms: 1.02x faster                                                        |
| pprint_pformat            | 1.58 sec                                                               | 1.55 sec: 1.02x faster                                                       |
| unpickle_list             | 4.93 us                                                                | 4.83 us: 1.02x faster                                                        |
| thrift                    | 811 us                                                                 | 799 us: 1.02x faster                                                         |
| pickle_dict               | 35.4 us                                                                | 34.9 us: 1.01x faster                                                        |
| coverage                  | 97.6 ms                                                                | 96.6 ms: 1.01x faster                                                        |
| sympy_sum                 | 163 ms                                                                 | 162 ms: 1.01x faster                                                         |
| dulwich_log               | 70.5 ms                                                                | 70.0 ms: 1.01x faster                                                        |
| gc_traversal              | 3.95 ms                                                                | 3.93 ms: 1.01x faster                                                        |
| logging_simple            | 5.86 us                                                                | 5.82 us: 1.01x faster                                                        |
| generators                | 29.7 ms                                                                | 29.6 ms: 1.00x faster                                                        |
| django_template           | 34.4 ms                                                                | 34.3 ms: 1.00x faster                                                        |
| pickle_pure_python        | 302 us                                                                 | 301 us: 1.00x faster                                                         |
| bench_thread_pool         | 862 us                                                                 | 858 us: 1.00x faster                                                         |
| asyncio_tcp_ssl           | 1.85 sec                                                               | 1.85 sec: 1.00x faster                                                       |
| deepcopy_memo             | 39.5 us                                                                | 39.6 us: 1.00x slower                                                        |
| asyncio_tcp               | 503 ms                                                                 | 505 ms: 1.00x slower                                                         |
| sqlglot_normalize         | 108 ms                                                                 | 109 ms: 1.00x slower                                                         |
| sqlite_synth              | 2.83 us                                                                | 2.84 us: 1.00x slower                                                        |
| async_tree_none_tg        | 459 ms                                                                 | 461 ms: 1.00x slower                                                         |
| fannkuch                  | 395 ms                                                                 | 397 ms: 1.00x slower                                                         |
| xml_etree_process         | 59.9 ms                                                                | 60.2 ms: 1.01x slower                                                        |
| richards_super            | 52.2 ms                                                                | 52.5 ms: 1.01x slower                                                        |
| sqlglot_optimize          | 56.6 ms                                                                | 57.0 ms: 1.01x slower                                                        |
| docutils                  | 2.77 sec                                                               | 2.79 sec: 1.01x slower                                                       |
| json_dumps                | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                                        |
| async_tree_io             | 1.22 sec                                                               | 1.22 sec: 1.01x slower                                                       |
| sqlglot_transpile         | 1.66 ms                                                                | 1.67 ms: 1.01x slower                                                        |
| coroutines                | 22.7 ms                                                                | 23.0 ms: 1.01x slower                                                        |
| async_tree_io_tg          | 1.24 sec                                                               | 1.25 sec: 1.01x slower                                                       |
| sqlglot_parse             | 1.31 ms                                                                | 1.33 ms: 1.01x slower                                                        |
| scimark_sor               | 130 ms                                                                 | 131 ms: 1.01x slower                                                         |
| mako                      | 10.7 ms                                                                | 10.8 ms: 1.01x slower                                                        |
| nqueens                   | 90.5 ms                                                                | 91.6 ms: 1.01x slower                                                        |
| create_gc_cycles          | 1.52 ms                                                                | 1.54 ms: 1.01x slower                                                        |
| async_tree_memoization_tg | 592 ms                                                                 | 600 ms: 1.01x slower                                                         |
| scimark_lu                | 132 ms                                                                 | 134 ms: 1.01x slower                                                         |
| deepcopy_reduce           | 3.09 us                                                                | 3.13 us: 1.01x slower                                                        |
| deltablue                 | 3.44 ms                                                                | 3.49 ms: 1.01x slower                                                        |
| xml_etree_parse           | 159 ms                                                                 | 162 ms: 1.01x slower                                                         |
| pyflate                   | 490 ms                                                                 | 497 ms: 1.01x slower                                                         |
| go                        | 158 ms                                                                 | 160 ms: 1.01x slower                                                         |
| xml_etree_iterparse       | 107 ms                                                                 | 109 ms: 1.02x slower                                                         |
| xml_etree_generate        | 86.8 ms                                                                | 88.3 ms: 1.02x slower                                                        |
| meteor_contest            | 110 ms                                                                 | 112 ms: 1.02x slower                                                         |
| regex_v8                  | 25.4 ms                                                                | 25.9 ms: 1.02x slower                                                        |
| json_loads                | 27.9 us                                                                | 28.4 us: 1.02x slower                                                        |
| unpickle_pure_python      | 239 us                                                                 | 244 us: 1.02x slower                                                         |
| crypto_pyaes              | 75.6 ms                                                                | 77.2 ms: 1.02x slower                                                        |
| scimark_fft               | 343 ms                                                                 | 351 ms: 1.02x slower                                                         |
| spectral_norm             | 118 ms                                                                 | 120 ms: 1.02x slower                                                         |
| unpickle                  | 15.1 us                                                                | 15.5 us: 1.02x slower                                                        |
| raytrace                  | 294 ms                                                                 | 302 ms: 1.03x slower                                                         |
| scimark_sparse_mat_mult   | 4.91 ms                                                                | 5.07 ms: 1.03x slower                                                        |
| comprehensions            | 17.3 us                                                                | 17.9 us: 1.04x slower                                                        |
| float                     | 79.8 ms                                                                | 82.7 ms: 1.04x slower                                                        |
| hexiom                    | 7.09 ms                                                                | 7.37 ms: 1.04x slower                                                        |
| html5lib                  | 65.7 ms                                                                | 68.3 ms: 1.04x slower                                                        |
| chaos                     | 64.1 ms                                                                | 66.8 ms: 1.04x slower                                                        |
| scimark_monte_carlo       | 70.1 ms                                                                | 73.4 ms: 1.05x slower                                                        |
| Geometric mean            | (ref)                                                                  | 1.00x slower                                                                 |

Benchmark hidden because not significant (33): genshi_text, logging_silent, genshi_xml, djangocms, logging_format, telco, typing_runtime_protocols, pylint, tomli_loads, chameleon, asyncio_websockets, dask, sympy_integrate, mypy2, json, sympy_expand, deepcopy, nbody, pidigits, 2to3, pathlib, tornado_http, sympy_str, async_generators, regex_compile, gunicorn, aiohttp, richards, pycparser, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_memoization, async_tree_cpu_io_mixed


# HPT report

- Reliability score: 99.25% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.92x