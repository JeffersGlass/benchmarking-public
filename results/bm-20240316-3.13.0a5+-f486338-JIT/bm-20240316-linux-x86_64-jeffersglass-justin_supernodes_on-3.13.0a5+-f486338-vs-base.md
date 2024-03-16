# Results vs. base

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: f486338
- commit date: 2024-03-16
- overall geometric mean: 1.01x faster
- HPT reliability: 99.96%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 297 ms                                                                 | 299 ms: 1.01x slower                                                         |
| chameleon      | 7.27 ms                                                                | 7.13 ms: 1.02x faster                                                        |
| html5lib       | 75.3 ms                                                                | 70.4 ms: 1.07x faster                                                        |
| tornado_http   | 146 ms                                                                 | 144 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                                 |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.08 sec                                                               | 1.13 sec: 1.04x slower                                                       |
| async_tree_cpu_io_mixed_tg | 668 ms                                                                 | 699 ms: 1.05x slower                                                         |
| async_tree_io              | 1.14 sec                                                               | 1.21 sec: 1.06x slower                                                       |
| async_tree_cpu_io_mixed    | 681 ms                                                                 | 724 ms: 1.06x slower                                                         |
| async_tree_none_tg         | 416 ms                                                                 | 445 ms: 1.07x slower                                                         |
| async_tree_none            | 432 ms                                                                 | 467 ms: 1.08x slower                                                         |
| async_tree_memoization_tg  | 537 ms                                                                 | 584 ms: 1.09x slower                                                         |
| async_tree_memoization     | 549 ms                                                                 | 610 ms: 1.11x slower                                                         |
| Geometric mean             | (ref)                                                                  | 1.07x slower                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 111 ms                                                                 | 103 ms: 1.08x faster                                                         |
| pidigits       | 188 ms                                                                 | 186 ms: 1.01x faster                                                         |
| float          | 77.6 ms                                                                | 79.2 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.55 ms                                                                | 3.42 ms: 1.04x faster                                                        |
| regex_dna      | 202 ms                                                                 | 197 ms: 1.03x faster                                                         |
| regex_compile  | 136 ms                                                                 | 133 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                                 |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| xml_etree_iterparse  | 103 ms                                                                 | 97.9 ms: 1.05x faster                                                        |
| pickle_dict          | 28.7 us                                                                | 27.5 us: 1.04x faster                                                        |
| tomli_loads          | 2.00 sec                                                               | 1.93 sec: 1.04x faster                                                       |
| unpickle_list        | 4.61 us                                                                | 4.49 us: 1.03x faster                                                        |
| unpickle_pure_python | 229 us                                                                 | 223 us: 1.03x faster                                                         |
| pickle_list          | 3.84 us                                                                | 3.76 us: 1.02x faster                                                        |
| xml_etree_generate   | 85.9 ms                                                                | 84.1 ms: 1.02x faster                                                        |
| xml_etree_process    | 59.2 ms                                                                | 58.6 ms: 1.01x faster                                                        |
| pickle               | 9.79 us                                                                | 9.69 us: 1.01x faster                                                        |
| json_loads           | 23.9 us                                                                | 24.1 us: 1.01x slower                                                        |
| xml_etree_parse      | 148 ms                                                                 | 152 ms: 1.02x slower                                                         |
| pickle_pure_python   | 303 us                                                                 | 312 us: 1.03x slower                                                         |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (2): json_dumps, unpickle

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup, python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|-----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 10.1 ms                                                                | 9.84 ms: 1.02x faster                                                        |
| genshi_xml      | 54.9 ms                                                                | 54.3 ms: 1.01x faster                                                        |
| genshi_text     | 25.2 ms                                                                | 25.0 ms: 1.01x faster                                                        |
| django_template | 34.7 ms                                                                | 34.5 ms: 1.01x faster                                                        |
| Geometric mean  | (ref)                                                                  | 1.01x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpack_sequence            | 113 ns                                                                 | 104 ns: 1.09x faster                                                         |
| nbody                      | 111 ms                                                                 | 103 ms: 1.08x faster                                                         |
| pyflate                    | 483 ms                                                                 | 449 ms: 1.07x faster                                                         |
| scimark_monte_carlo        | 73.5 ms                                                                | 68.5 ms: 1.07x faster                                                        |
| richards_super             | 56.5 ms                                                                | 52.7 ms: 1.07x faster                                                        |
| html5lib                   | 75.3 ms                                                                | 70.4 ms: 1.07x faster                                                        |
| scimark_lu                 | 127 ms                                                                 | 119 ms: 1.07x faster                                                         |
| richards                   | 48.8 ms                                                                | 45.6 ms: 1.07x faster                                                        |
| raytrace                   | 298 ms                                                                 | 280 ms: 1.07x faster                                                         |
| hexiom                     | 6.59 ms                                                                | 6.24 ms: 1.06x faster                                                        |
| xml_etree_iterparse        | 103 ms                                                                 | 97.9 ms: 1.05x faster                                                        |
| scimark_sparse_mat_mult    | 4.41 ms                                                                | 4.21 ms: 1.05x faster                                                        |
| spectral_norm              | 95.7 ms                                                                | 91.5 ms: 1.05x faster                                                        |
| pickle_dict                | 28.7 us                                                                | 27.5 us: 1.04x faster                                                        |
| chaos                      | 63.8 ms                                                                | 61.3 ms: 1.04x faster                                                        |
| fannkuch                   | 363 ms                                                                 | 349 ms: 1.04x faster                                                         |
| sympy_str                  | 279 ms                                                                 | 269 ms: 1.04x faster                                                         |
| sympy_expand               | 474 ms                                                                 | 457 ms: 1.04x faster                                                         |
| pycparser                  | 1.30 sec                                                               | 1.26 sec: 1.04x faster                                                       |
| tomli_loads                | 2.00 sec                                                               | 1.93 sec: 1.04x faster                                                       |
| regex_effbot               | 3.55 ms                                                                | 3.42 ms: 1.04x faster                                                        |
| pprint_safe_repr           | 777 ms                                                                 | 750 ms: 1.04x faster                                                         |
| comprehensions             | 17.1 us                                                                | 16.5 us: 1.03x faster                                                        |
| typing_runtime_protocols   | 110 us                                                                 | 106 us: 1.03x faster                                                         |
| async_generators           | 413 ms                                                                 | 400 ms: 1.03x faster                                                         |
| deltablue                  | 3.82 ms                                                                | 3.71 ms: 1.03x faster                                                        |
| regex_dna                  | 202 ms                                                                 | 197 ms: 1.03x faster                                                         |
| pprint_pformat             | 1.59 sec                                                               | 1.55 sec: 1.03x faster                                                       |
| unpickle_list              | 4.61 us                                                                | 4.49 us: 1.03x faster                                                        |
| unpickle_pure_python       | 229 us                                                                 | 223 us: 1.03x faster                                                         |
| sqlglot_optimize           | 57.1 ms                                                                | 55.8 ms: 1.02x faster                                                        |
| crypto_pyaes               | 67.0 ms                                                                | 65.4 ms: 1.02x faster                                                        |
| scimark_fft                | 311 ms                                                                 | 304 ms: 1.02x faster                                                         |
| regex_compile              | 136 ms                                                                 | 133 ms: 1.02x faster                                                         |
| scimark_sor                | 151 ms                                                                 | 148 ms: 1.02x faster                                                         |
| mako                       | 10.1 ms                                                                | 9.84 ms: 1.02x faster                                                        |
| pickle_list                | 3.84 us                                                                | 3.76 us: 1.02x faster                                                        |
| xml_etree_generate         | 85.9 ms                                                                | 84.1 ms: 1.02x faster                                                        |
| go                         | 162 ms                                                                 | 159 ms: 1.02x faster                                                         |
| chameleon                  | 7.27 ms                                                                | 7.13 ms: 1.02x faster                                                        |
| sqlglot_transpile          | 1.65 ms                                                                | 1.62 ms: 1.02x faster                                                        |
| sqlglot_normalize          | 110 ms                                                                 | 108 ms: 1.02x faster                                                         |
| sympy_sum                  | 151 ms                                                                 | 148 ms: 1.02x faster                                                         |
| json                       | 4.66 ms                                                                | 4.60 ms: 1.01x faster                                                        |
| coverage                   | 82.6 ms                                                                | 81.5 ms: 1.01x faster                                                        |
| dulwich_log                | 79.0 ms                                                                | 78.0 ms: 1.01x faster                                                        |
| tornado_http               | 146 ms                                                                 | 144 ms: 1.01x faster                                                         |
| genshi_xml                 | 54.9 ms                                                                | 54.3 ms: 1.01x faster                                                        |
| xml_etree_process          | 59.2 ms                                                                | 58.6 ms: 1.01x faster                                                        |
| pathlib                    | 24.2 ms                                                                | 23.9 ms: 1.01x faster                                                        |
| nqueens                    | 88.5 ms                                                                | 87.6 ms: 1.01x faster                                                        |
| pickle                     | 9.79 us                                                                | 9.69 us: 1.01x faster                                                        |
| logging_format             | 6.69 us                                                                | 6.62 us: 1.01x faster                                                        |
| logging_simple             | 6.09 us                                                                | 6.03 us: 1.01x faster                                                        |
| genshi_text                | 25.2 ms                                                                | 25.0 ms: 1.01x faster                                                        |
| bench_thread_pool          | 1.51 ms                                                                | 1.49 ms: 1.01x faster                                                        |
| pidigits                   | 188 ms                                                                 | 186 ms: 1.01x faster                                                         |
| sympy_integrate            | 20.7 ms                                                                | 20.6 ms: 1.01x faster                                                        |
| django_template            | 34.7 ms                                                                | 34.5 ms: 1.01x faster                                                        |
| asyncio_tcp_ssl            | 1.75 sec                                                               | 1.74 sec: 1.01x faster                                                       |
| sqlglot_parse              | 1.30 ms                                                                | 1.30 ms: 1.01x faster                                                        |
| json_loads                 | 23.9 us                                                                | 24.1 us: 1.01x slower                                                        |
| thrift                     | 765 us                                                                 | 771 us: 1.01x slower                                                         |
| 2to3                       | 297 ms                                                                 | 299 ms: 1.01x slower                                                         |
| deepcopy_memo              | 36.3 us                                                                | 36.6 us: 1.01x slower                                                        |
| create_gc_cycles           | 1.09 ms                                                                | 1.10 ms: 1.02x slower                                                        |
| telco                      | 7.51 ms                                                                | 7.66 ms: 1.02x slower                                                        |
| float                      | 77.6 ms                                                                | 79.2 ms: 1.02x slower                                                        |
| xml_etree_parse            | 148 ms                                                                 | 152 ms: 1.02x slower                                                         |
| pickle_pure_python         | 303 us                                                                 | 312 us: 1.03x slower                                                         |
| generators                 | 30.5 ms                                                                | 31.6 ms: 1.04x slower                                                        |
| async_tree_io_tg           | 1.08 sec                                                               | 1.13 sec: 1.04x slower                                                       |
| coroutines                 | 25.0 ms                                                                | 26.2 ms: 1.05x slower                                                        |
| async_tree_cpu_io_mixed_tg | 668 ms                                                                 | 699 ms: 1.05x slower                                                         |
| asyncio_tcp                | 558 ms                                                                 | 584 ms: 1.05x slower                                                         |
| async_tree_io              | 1.14 sec                                                               | 1.21 sec: 1.06x slower                                                       |
| async_tree_cpu_io_mixed    | 681 ms                                                                 | 724 ms: 1.06x slower                                                         |
| async_tree_none_tg         | 416 ms                                                                 | 445 ms: 1.07x slower                                                         |
| async_tree_none            | 432 ms                                                                 | 467 ms: 1.08x slower                                                         |
| async_tree_memoization_tg  | 537 ms                                                                 | 584 ms: 1.09x slower                                                         |
| async_tree_memoization     | 549 ms                                                                 | 610 ms: 1.11x slower                                                         |
| gc_traversal               | 3.20 ms                                                                | 3.68 ms: 1.15x slower                                                        |
| Geometric mean             | (ref)                                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (17): mypy2, dask, pylint, mdp, json_dumps, logging_silent, sqlite_synth, deepcopy_reduce, asyncio_websockets, bench_mp_pool, python_startup, python_startup_no_site, meteor_contest, unpickle, deepcopy, docutils, regex_v8


# HPT report

- Reliability score: 99.96% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x