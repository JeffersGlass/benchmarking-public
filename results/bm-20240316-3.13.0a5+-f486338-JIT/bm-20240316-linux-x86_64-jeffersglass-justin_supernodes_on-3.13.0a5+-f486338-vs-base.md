# Results vs. base

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: f486338
- commit date: 2024-03-16
- overall geometric mean: 1.00x faster
- HPT reliability: 73.05%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| chameleon      | 7.07 ms                                                                | 7.25 ms: 1.02x slower                                                        |
| docutils       | 2.62 sec                                                               | 2.67 sec: 1.02x slower                                                       |
| tornado_http   | 145 ms                                                                 | 147 ms: 1.02x slower                                                         |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (2): 2to3, html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 674 ms                                                                 | 698 ms: 1.03x slower                                                         |
| async_tree_cpu_io_mixed_tg | 654 ms                                                                 | 677 ms: 1.04x slower                                                         |
| async_tree_io              | 1.12 sec                                                               | 1.16 sec: 1.04x slower                                                       |
| async_tree_none            | 427 ms                                                                 | 449 ms: 1.05x slower                                                         |
| Geometric mean             | (ref)                                                                  | 1.02x slower                                                                 |

Benchmark hidden because not significant (4): async_tree_io_tg, async_tree_none_tg, async_tree_memoization, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 112 ms                                                                 | 103 ms: 1.09x faster                                                         |
| float          | 78.0 ms                                                                | 78.5 ms: 1.01x slower                                                        |
| pidigits       | 187 ms                                                                 | 188 ms: 1.01x slower                                                         |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_v8       | 25.3 ms                                                                | 23.8 ms: 1.06x faster                                                        |
| regex_dna      | 195 ms                                                                 | 191 ms: 1.02x faster                                                         |
| regex_effbot   | 3.45 ms                                                                | 3.37 ms: 1.02x faster                                                        |
| regex_compile  | 138 ms                                                                 | 136 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                                  | 1.03x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle_list        | 4.64 us                                                                | 4.43 us: 1.05x faster                                                        |
| tomli_loads          | 2.02 sec                                                               | 1.93 sec: 1.04x faster                                                       |
| pickle_list          | 3.89 us                                                                | 3.76 us: 1.04x faster                                                        |
| pickle_dict          | 28.8 us                                                                | 27.8 us: 1.03x faster                                                        |
| xml_etree_parse      | 150 ms                                                                 | 147 ms: 1.02x faster                                                         |
| unpickle_pure_python | 226 us                                                                 | 223 us: 1.02x faster                                                         |
| xml_etree_iterparse  | 102 ms                                                                 | 100 ms: 1.01x faster                                                         |
| pickle_pure_python   | 307 us                                                                 | 304 us: 1.01x faster                                                         |
| pickle               | 9.83 us                                                                | 9.75 us: 1.01x faster                                                        |
| json_dumps           | 9.49 ms                                                                | 9.56 ms: 1.01x slower                                                        |
| xml_etree_generate   | 84.1 ms                                                                | 85.3 ms: 1.01x slower                                                        |
| xml_etree_process    | 58.8 ms                                                                | 59.9 ms: 1.02x slower                                                        |
| unpickle             | 13.0 us                                                                | 13.5 us: 1.04x slower                                                        |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 18.2 ms                                                                | 19.2 ms: 1.06x slower                                                        |
| python_startup_no_site | 16.7 ms                                                                | 17.8 ms: 1.06x slower                                                        |
| Geometric mean         | (ref)                                                                  | 1.06x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|-----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 10.0 ms                                                                | 9.85 ms: 1.02x faster                                                        |
| genshi_text     | 25.1 ms                                                                | 24.7 ms: 1.02x faster                                                        |
| django_template | 35.0 ms                                                                | 34.6 ms: 1.01x faster                                                        |
| genshi_xml      | 54.7 ms                                                                | 54.2 ms: 1.01x faster                                                        |
| Geometric mean  | (ref)                                                                  | 1.01x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody                      | 112 ms                                                                 | 103 ms: 1.09x faster                                                         |
| scimark_sparse_mat_mult    | 4.44 ms                                                                | 4.16 ms: 1.07x faster                                                        |
| regex_v8                   | 25.3 ms                                                                | 23.8 ms: 1.06x faster                                                        |
| scimark_monte_carlo        | 73.7 ms                                                                | 69.6 ms: 1.06x faster                                                        |
| unpack_sequence            | 117 ns                                                                 | 110 ns: 1.06x faster                                                         |
| coverage                   | 83.2 ms                                                                | 78.8 ms: 1.06x faster                                                        |
| fannkuch                   | 361 ms                                                                 | 343 ms: 1.05x faster                                                         |
| unpickle_list              | 4.64 us                                                                | 4.43 us: 1.05x faster                                                        |
| tomli_loads                | 2.02 sec                                                               | 1.93 sec: 1.04x faster                                                       |
| comprehensions             | 17.1 us                                                                | 16.4 us: 1.04x faster                                                        |
| raytrace                   | 299 ms                                                                 | 287 ms: 1.04x faster                                                         |
| richards                   | 48.8 ms                                                                | 46.8 ms: 1.04x faster                                                        |
| richards_super             | 56.3 ms                                                                | 54.3 ms: 1.04x faster                                                        |
| gc_traversal               | 3.39 ms                                                                | 3.27 ms: 1.04x faster                                                        |
| pprint_safe_repr           | 777 ms                                                                 | 750 ms: 1.04x faster                                                         |
| hexiom                     | 6.49 ms                                                                | 6.26 ms: 1.04x faster                                                        |
| nqueens                    | 89.4 ms                                                                | 86.3 ms: 1.04x faster                                                        |
| pickle_list                | 3.89 us                                                                | 3.76 us: 1.04x faster                                                        |
| scimark_lu                 | 122 ms                                                                 | 118 ms: 1.04x faster                                                         |
| pickle_dict                | 28.8 us                                                                | 27.8 us: 1.03x faster                                                        |
| chaos                      | 63.4 ms                                                                | 61.3 ms: 1.03x faster                                                        |
| scimark_fft                | 312 ms                                                                 | 303 ms: 1.03x faster                                                         |
| spectral_norm              | 95.1 ms                                                                | 92.7 ms: 1.03x faster                                                        |
| pprint_pformat             | 1.58 sec                                                               | 1.55 sec: 1.02x faster                                                       |
| regex_dna                  | 195 ms                                                                 | 191 ms: 1.02x faster                                                         |
| regex_effbot               | 3.45 ms                                                                | 3.37 ms: 1.02x faster                                                        |
| regex_compile              | 138 ms                                                                 | 136 ms: 1.02x faster                                                         |
| scimark_sor                | 149 ms                                                                 | 146 ms: 1.02x faster                                                         |
| xml_etree_parse            | 150 ms                                                                 | 147 ms: 1.02x faster                                                         |
| crypto_pyaes               | 66.7 ms                                                                | 65.4 ms: 1.02x faster                                                        |
| mako                       | 10.0 ms                                                                | 9.85 ms: 1.02x faster                                                        |
| sympy_expand               | 477 ms                                                                 | 469 ms: 1.02x faster                                                         |
| sqlite_synth               | 2.73 us                                                                | 2.69 us: 1.02x faster                                                        |
| unpickle_pure_python       | 226 us                                                                 | 223 us: 1.02x faster                                                         |
| json                       | 4.66 ms                                                                | 4.58 ms: 1.02x faster                                                        |
| genshi_text                | 25.1 ms                                                                | 24.7 ms: 1.02x faster                                                        |
| xml_etree_iterparse        | 102 ms                                                                 | 100 ms: 1.01x faster                                                         |
| deltablue                  | 3.79 ms                                                                | 3.75 ms: 1.01x faster                                                        |
| pickle_pure_python         | 307 us                                                                 | 304 us: 1.01x faster                                                         |
| dulwich_log                | 79.2 ms                                                                | 78.2 ms: 1.01x faster                                                        |
| meteor_contest             | 102 ms                                                                 | 101 ms: 1.01x faster                                                         |
| django_template            | 35.0 ms                                                                | 34.6 ms: 1.01x faster                                                        |
| go                         | 161 ms                                                                 | 159 ms: 1.01x faster                                                         |
| genshi_xml                 | 54.7 ms                                                                | 54.2 ms: 1.01x faster                                                        |
| pickle                     | 9.83 us                                                                | 9.75 us: 1.01x faster                                                        |
| sqlglot_normalize          | 110 ms                                                                 | 109 ms: 1.01x faster                                                         |
| float                      | 78.0 ms                                                                | 78.5 ms: 1.01x slower                                                        |
| telco                      | 7.58 ms                                                                | 7.63 ms: 1.01x slower                                                        |
| json_dumps                 | 9.49 ms                                                                | 9.56 ms: 1.01x slower                                                        |
| pidigits                   | 187 ms                                                                 | 188 ms: 1.01x slower                                                         |
| create_gc_cycles           | 1.09 ms                                                                | 1.10 ms: 1.01x slower                                                        |
| logging_simple             | 6.04 us                                                                | 6.09 us: 1.01x slower                                                        |
| thrift                     | 765 us                                                                 | 774 us: 1.01x slower                                                         |
| pathlib                    | 23.9 ms                                                                | 24.2 ms: 1.01x slower                                                        |
| bench_thread_pool          | 1.49 ms                                                                | 1.51 ms: 1.01x slower                                                        |
| generators                 | 30.9 ms                                                                | 31.3 ms: 1.01x slower                                                        |
| xml_etree_generate         | 84.1 ms                                                                | 85.3 ms: 1.01x slower                                                        |
| xml_etree_process          | 58.8 ms                                                                | 59.9 ms: 1.02x slower                                                        |
| async_generators           | 398 ms                                                                 | 405 ms: 1.02x slower                                                         |
| docutils                   | 2.62 sec                                                               | 2.67 sec: 1.02x slower                                                       |
| tornado_http               | 145 ms                                                                 | 147 ms: 1.02x slower                                                         |
| asyncio_tcp_ssl            | 1.73 sec                                                               | 1.76 sec: 1.02x slower                                                       |
| chameleon                  | 7.07 ms                                                                | 7.25 ms: 1.02x slower                                                        |
| dask                       | 471 ms                                                                 | 483 ms: 1.02x slower                                                         |
| coroutines                 | 24.7 ms                                                                | 25.4 ms: 1.03x slower                                                        |
| pycparser                  | 1.27 sec                                                               | 1.31 sec: 1.03x slower                                                       |
| async_tree_cpu_io_mixed    | 674 ms                                                                 | 698 ms: 1.03x slower                                                         |
| async_tree_cpu_io_mixed_tg | 654 ms                                                                 | 677 ms: 1.04x slower                                                         |
| async_tree_io              | 1.12 sec                                                               | 1.16 sec: 1.04x slower                                                       |
| bench_mp_pool              | 15.4 ms                                                                | 16.0 ms: 1.04x slower                                                        |
| unpickle                   | 13.0 us                                                                | 13.5 us: 1.04x slower                                                        |
| pyflate                    | 468 ms                                                                 | 489 ms: 1.05x slower                                                         |
| mdp                        | 2.42 sec                                                               | 2.54 sec: 1.05x slower                                                       |
| async_tree_none            | 427 ms                                                                 | 449 ms: 1.05x slower                                                         |
| python_startup             | 18.2 ms                                                                | 19.2 ms: 1.06x slower                                                        |
| python_startup_no_site     | 16.7 ms                                                                | 17.8 ms: 1.06x slower                                                        |
| asyncio_tcp                | 555 ms                                                                 | 592 ms: 1.07x slower                                                         |
| Geometric mean             | (ref)                                                                  | 1.00x faster                                                                 |

Benchmark hidden because not significant (22): typing_runtime_protocols, html5lib, json_loads, sqlglot_optimize, sympy_str, logging_silent, sympy_integrate, 2to3, async_tree_io_tg, logging_format, asyncio_websockets, deepcopy_memo, deepcopy, sqlglot_parse, async_tree_none_tg, sympy_sum, sqlglot_transpile, async_tree_memoization, deepcopy_reduce, async_tree_memoization_tg, pylint, mypy2


# HPT report

- Reliability score: 73.05% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x