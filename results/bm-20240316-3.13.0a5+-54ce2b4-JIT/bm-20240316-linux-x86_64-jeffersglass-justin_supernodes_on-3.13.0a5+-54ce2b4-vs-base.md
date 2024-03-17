# Results vs. base

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: 54ce2b4
- commit date: 2024-03-16
- overall geometric mean: 1.01x slower
- HPT reliability: 80.08%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 294 ms                                                                 | 304 ms: 1.03x slower                                                         |
| docutils       | 2.58 sec                                                               | 2.76 sec: 1.07x slower                                                       |
| tornado_http   | 143 ms                                                                 | 145 ms: 1.01x slower                                                         |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                                 |

Benchmark hidden because not significant (2): chameleon, html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 651 ms                                                                 | 682 ms: 1.05x slower                                                         |
| async_tree_io_tg           | 1.07 sec                                                               | 1.14 sec: 1.07x slower                                                       |
| async_tree_none_tg         | 409 ms                                                                 | 440 ms: 1.08x slower                                                         |
| async_tree_io              | 1.11 sec                                                               | 1.21 sec: 1.08x slower                                                       |
| async_tree_cpu_io_mixed    | 665 ms                                                                 | 728 ms: 1.10x slower                                                         |
| async_tree_memoization_tg  | 529 ms                                                                 | 590 ms: 1.12x slower                                                         |
| async_tree_none            | 420 ms                                                                 | 476 ms: 1.13x slower                                                         |
| async_tree_memoization     | 532 ms                                                                 | 607 ms: 1.14x slower                                                         |
| Geometric mean             | (ref)                                                                  | 1.10x slower                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 113 ms                                                                 | 107 ms: 1.06x faster                                                         |
| pidigits       | 188 ms                                                                 | 187 ms: 1.01x faster                                                         |
| float          | 77.2 ms                                                                | 79.8 ms: 1.03x slower                                                        |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 136 ms                                                                 | 134 ms: 1.02x faster                                                         |
| regex_effbot   | 3.34 ms                                                                | 3.42 ms: 1.02x slower                                                        |
| regex_v8       | 23.8 ms                                                                | 24.6 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle_pure_python | 232 us                                                                 | 223 us: 1.04x faster                                                         |
| pickle_pure_python   | 316 us                                                                 | 308 us: 1.03x faster                                                         |
| json_loads           | 24.6 us                                                                | 24.0 us: 1.02x faster                                                        |
| tomli_loads          | 2.00 sec                                                               | 1.98 sec: 1.01x faster                                                       |
| pickle_dict          | 28.6 us                                                                | 28.7 us: 1.00x slower                                                        |
| xml_etree_parse      | 147 ms                                                                 | 148 ms: 1.01x slower                                                         |
| unpickle_list        | 4.49 us                                                                | 4.56 us: 1.01x slower                                                        |
| unpickle             | 13.3 us                                                                | 13.7 us: 1.02x slower                                                        |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                                 |

Benchmark hidden because not significant (6): json_dumps, pickle_list, xml_etree_iterparse, pickle, xml_etree_generate, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 18.2 ms                                                                | 19.3 ms: 1.06x slower                                                        |
| python_startup_no_site | 16.7 ms                                                                | 17.8 ms: 1.06x slower                                                        |
| Geometric mean         | (ref)                                                                  | 1.06x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|-----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| django_template | 35.3 ms                                                                | 34.5 ms: 1.02x faster                                                        |
| genshi_text     | 25.1 ms                                                                | 24.7 ms: 1.01x faster                                                        |
| mako            | 10.1 ms                                                                | 10.1 ms: 1.01x slower                                                        |
| Geometric mean  | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (1): genshi_xml

All benchmarks:
===============

| Benchmark                  | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| scimark_sparse_mat_mult    | 4.45 ms                                                                | 4.19 ms: 1.06x faster                                                        |
| unpack_sequence            | 113 ns                                                                 | 107 ns: 1.06x faster                                                         |
| nbody                      | 113 ms                                                                 | 107 ms: 1.06x faster                                                         |
| scimark_lu                 | 122 ms                                                                 | 116 ms: 1.05x faster                                                         |
| unpickle_pure_python       | 232 us                                                                 | 223 us: 1.04x faster                                                         |
| coverage                   | 84.7 ms                                                                | 81.6 ms: 1.04x faster                                                        |
| spectral_norm              | 95.4 ms                                                                | 92.2 ms: 1.03x faster                                                        |
| nqueens                    | 89.1 ms                                                                | 86.2 ms: 1.03x faster                                                        |
| hexiom                     | 6.50 ms                                                                | 6.29 ms: 1.03x faster                                                        |
| pprint_safe_repr           | 780 ms                                                                 | 757 ms: 1.03x faster                                                         |
| scimark_sor                | 152 ms                                                                 | 148 ms: 1.03x faster                                                         |
| pickle_pure_python         | 316 us                                                                 | 308 us: 1.03x faster                                                         |
| richards_super             | 55.0 ms                                                                | 53.7 ms: 1.02x faster                                                        |
| comprehensions             | 17.1 us                                                                | 16.7 us: 1.02x faster                                                        |
| json_loads                 | 24.6 us                                                                | 24.0 us: 1.02x faster                                                        |
| pprint_pformat             | 1.59 sec                                                               | 1.55 sec: 1.02x faster                                                       |
| meteor_contest             | 101 ms                                                                 | 98.7 ms: 1.02x faster                                                        |
| django_template            | 35.3 ms                                                                | 34.5 ms: 1.02x faster                                                        |
| scimark_monte_carlo        | 73.1 ms                                                                | 71.6 ms: 1.02x faster                                                        |
| scimark_fft                | 317 ms                                                                 | 311 ms: 1.02x faster                                                         |
| regex_compile              | 136 ms                                                                 | 134 ms: 1.02x faster                                                         |
| crypto_pyaes               | 67.3 ms                                                                | 66.1 ms: 1.02x faster                                                        |
| go                         | 160 ms                                                                 | 158 ms: 1.02x faster                                                         |
| logging_simple             | 6.10 us                                                                | 6.00 us: 1.02x faster                                                        |
| raytrace                   | 297 ms                                                                 | 293 ms: 1.01x faster                                                         |
| dulwich_log                | 79.0 ms                                                                | 77.8 ms: 1.01x faster                                                        |
| genshi_text                | 25.1 ms                                                                | 24.7 ms: 1.01x faster                                                        |
| typing_runtime_protocols   | 108 us                                                                 | 107 us: 1.01x faster                                                         |
| tomli_loads                | 2.00 sec                                                               | 1.98 sec: 1.01x faster                                                       |
| json                       | 4.71 ms                                                                | 4.67 ms: 1.01x faster                                                        |
| pidigits                   | 188 ms                                                                 | 187 ms: 1.01x faster                                                         |
| logging_silent             | 101 ns                                                                 | 100.0 ns: 1.01x faster                                                       |
| coroutines                 | 25.2 ms                                                                | 25.0 ms: 1.01x faster                                                        |
| logging_format             | 6.69 us                                                                | 6.63 us: 1.01x faster                                                        |
| sqlglot_parse              | 1.32 ms                                                                | 1.31 ms: 1.01x faster                                                        |
| chaos                      | 63.4 ms                                                                | 63.0 ms: 1.01x faster                                                        |
| thrift                     | 772 us                                                                 | 766 us: 1.01x faster                                                         |
| sqlglot_normalize          | 109 ms                                                                 | 109 ms: 1.01x faster                                                         |
| pickle_dict                | 28.6 us                                                                | 28.7 us: 1.00x slower                                                        |
| mako                       | 10.1 ms                                                                | 10.1 ms: 1.01x slower                                                        |
| deepcopy_reduce            | 3.14 us                                                                | 3.16 us: 1.01x slower                                                        |
| sqlglot_transpile          | 1.64 ms                                                                | 1.66 ms: 1.01x slower                                                        |
| sympy_integrate            | 20.7 ms                                                                | 20.9 ms: 1.01x slower                                                        |
| tornado_http               | 143 ms                                                                 | 145 ms: 1.01x slower                                                         |
| xml_etree_parse            | 147 ms                                                                 | 148 ms: 1.01x slower                                                         |
| sqlite_synth               | 2.65 us                                                                | 2.68 us: 1.01x slower                                                        |
| pathlib                    | 23.8 ms                                                                | 24.1 ms: 1.01x slower                                                        |
| create_gc_cycles           | 1.09 ms                                                                | 1.11 ms: 1.01x slower                                                        |
| unpickle_list              | 4.49 us                                                                | 4.56 us: 1.01x slower                                                        |
| bench_thread_pool          | 1.50 ms                                                                | 1.52 ms: 1.02x slower                                                        |
| unpickle                   | 13.3 us                                                                | 13.7 us: 1.02x slower                                                        |
| regex_effbot               | 3.34 ms                                                                | 3.42 ms: 1.02x slower                                                        |
| 2to3                       | 294 ms                                                                 | 304 ms: 1.03x slower                                                         |
| float                      | 77.2 ms                                                                | 79.8 ms: 1.03x slower                                                        |
| asyncio_tcp_ssl            | 1.73 sec                                                               | 1.79 sec: 1.04x slower                                                       |
| regex_v8                   | 23.8 ms                                                                | 24.6 ms: 1.04x slower                                                        |
| pyflate                    | 478 ms                                                                 | 496 ms: 1.04x slower                                                         |
| bench_mp_pool              | 15.5 ms                                                                | 16.2 ms: 1.04x slower                                                        |
| pycparser                  | 1.27 sec                                                               | 1.32 sec: 1.04x slower                                                       |
| async_tree_cpu_io_mixed_tg | 651 ms                                                                 | 682 ms: 1.05x slower                                                         |
| dask                       | 472 ms                                                                 | 495 ms: 1.05x slower                                                         |
| python_startup             | 18.2 ms                                                                | 19.3 ms: 1.06x slower                                                        |
| asyncio_tcp                | 558 ms                                                                 | 591 ms: 1.06x slower                                                         |
| generators                 | 31.7 ms                                                                | 33.6 ms: 1.06x slower                                                        |
| python_startup_no_site     | 16.7 ms                                                                | 17.8 ms: 1.06x slower                                                        |
| docutils                   | 2.58 sec                                                               | 2.76 sec: 1.07x slower                                                       |
| async_tree_io_tg           | 1.07 sec                                                               | 1.14 sec: 1.07x slower                                                       |
| async_tree_none_tg         | 409 ms                                                                 | 440 ms: 1.08x slower                                                         |
| gc_traversal               | 3.18 ms                                                                | 3.44 ms: 1.08x slower                                                        |
| async_tree_io              | 1.11 sec                                                               | 1.21 sec: 1.08x slower                                                       |
| async_tree_cpu_io_mixed    | 665 ms                                                                 | 728 ms: 1.10x slower                                                         |
| async_tree_memoization_tg  | 529 ms                                                                 | 590 ms: 1.12x slower                                                         |
| mdp                        | 2.42 sec                                                               | 2.70 sec: 1.12x slower                                                       |
| async_tree_none            | 420 ms                                                                 | 476 ms: 1.13x slower                                                         |
| async_tree_memoization     | 532 ms                                                                 | 607 ms: 1.14x slower                                                         |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (24): richards, json_dumps, regex_dna, genshi_xml, pickle_list, deltablue, sqlglot_optimize, xml_etree_iterparse, pickle, xml_etree_generate, fannkuch, sympy_sum, deepcopy_memo, asyncio_websockets, deepcopy, xml_etree_process, chameleon, sympy_str, sympy_expand, telco, async_generators, html5lib, pylint, mypy2


# HPT report

- Reliability score: 80.08% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x