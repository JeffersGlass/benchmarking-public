# Results vs. base

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: 54ce2b4
- commit date: 2024-03-16
- overall geometric mean: 1.08x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 296 ms                                                                 | 273 ms: 1.09x faster                                                         |
| chameleon      | 7.07 ms                                                                | 6.76 ms: 1.05x faster                                                        |
| docutils       | 2.62 sec                                                               | 2.38 sec: 1.10x faster                                                       |
| html5lib       | 72.5 ms                                                                | 67.5 ms: 1.07x faster                                                        |
| tornado_http   | 145 ms                                                                 | 137 ms: 1.05x faster                                                         |
| Geometric mean | (ref)                                                                  | 1.07x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_memoization     | 578 ms                                                                 | 494 ms: 1.17x faster                                                         |
| async_tree_memoization_tg  | 557 ms                                                                 | 482 ms: 1.16x faster                                                         |
| async_tree_none_tg         | 427 ms                                                                 | 380 ms: 1.12x faster                                                         |
| async_tree_cpu_io_mixed    | 674 ms                                                                 | 611 ms: 1.10x faster                                                         |
| async_tree_none            | 427 ms                                                                 | 389 ms: 1.10x faster                                                         |
| async_tree_io_tg           | 1.10 sec                                                               | 1.01 sec: 1.09x faster                                                       |
| async_tree_io              | 1.12 sec                                                               | 1.04 sec: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 654 ms                                                                 | 606 ms: 1.08x faster                                                         |
| Geometric mean             | (ref)                                                                  | 1.11x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 112 ms                                                                 | 99.6 ms: 1.12x faster                                                        |
| pidigits       | 187 ms                                                                 | 174 ms: 1.07x faster                                                         |
| float          | 78.0 ms                                                                | 73.3 ms: 1.06x faster                                                        |
| Geometric mean | (ref)                                                                  | 1.09x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.45 ms                                                                | 3.07 ms: 1.12x faster                                                        |
| regex_dna      | 195 ms                                                                 | 174 ms: 1.12x faster                                                         |
| regex_v8       | 25.3 ms                                                                | 22.7 ms: 1.12x faster                                                        |
| regex_compile  | 138 ms                                                                 | 125 ms: 1.10x faster                                                         |
| Geometric mean | (ref)                                                                  | 1.12x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| xml_etree_iterparse  | 102 ms                                                                 | 89.7 ms: 1.13x faster                                                        |
| xml_etree_parse      | 150 ms                                                                 | 134 ms: 1.12x faster                                                         |
| unpickle_list        | 4.64 us                                                                | 4.22 us: 1.10x faster                                                        |
| pickle_dict          | 28.8 us                                                                | 26.2 us: 1.10x faster                                                        |
| unpickle_pure_python | 226 us                                                                 | 207 us: 1.10x faster                                                         |
| pickle               | 9.83 us                                                                | 8.98 us: 1.10x faster                                                        |
| tomli_loads          | 2.02 sec                                                               | 1.85 sec: 1.09x faster                                                       |
| pickle_list          | 3.89 us                                                                | 3.57 us: 1.09x faster                                                        |
| json_loads           | 24.0 us                                                                | 22.4 us: 1.07x faster                                                        |
| pickle_pure_python   | 307 us                                                                 | 288 us: 1.07x faster                                                         |
| xml_etree_process    | 58.8 ms                                                                | 55.3 ms: 1.06x faster                                                        |
| xml_etree_generate   | 84.1 ms                                                                | 79.0 ms: 1.06x faster                                                        |
| json_dumps           | 9.49 ms                                                                | 8.95 ms: 1.06x faster                                                        |
| unpickle             | 13.0 us                                                                | 12.5 us: 1.04x faster                                                        |
| Geometric mean       | (ref)                                                                  | 1.08x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup_no_site | 16.7 ms                                                                | 15.9 ms: 1.05x faster                                                        |
| python_startup         | 18.2 ms                                                                | 17.2 ms: 1.05x faster                                                        |
| Geometric mean         | (ref)                                                                  | 1.05x faster                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|-----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 10.0 ms                                                                | 9.10 ms: 1.10x faster                                                        |
| genshi_xml      | 54.7 ms                                                                | 50.1 ms: 1.09x faster                                                        |
| django_template | 35.0 ms                                                                | 32.1 ms: 1.09x faster                                                        |
| genshi_text     | 25.1 ms                                                                | 23.1 ms: 1.08x faster                                                        |
| Geometric mean  | (ref)                                                                  | 1.09x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20240315-linux-x86_64-python-1904f0a2245f500aa85f-3.13.0a5+-1904f0a | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpack_sequence            | 117 ns                                                                 | 99.0 ns: 1.18x faster                                                        |
| async_tree_memoization     | 578 ms                                                                 | 494 ms: 1.17x faster                                                         |
| async_tree_memoization_tg  | 557 ms                                                                 | 482 ms: 1.16x faster                                                         |
| scimark_sparse_mat_mult    | 4.44 ms                                                                | 3.89 ms: 1.14x faster                                                        |
| gc_traversal               | 3.39 ms                                                                | 2.97 ms: 1.14x faster                                                        |
| xml_etree_iterparse        | 102 ms                                                                 | 89.7 ms: 1.13x faster                                                        |
| fannkuch                   | 361 ms                                                                 | 321 ms: 1.13x faster                                                         |
| nbody                      | 112 ms                                                                 | 99.6 ms: 1.12x faster                                                        |
| scimark_lu                 | 122 ms                                                                 | 109 ms: 1.12x faster                                                         |
| regex_effbot               | 3.45 ms                                                                | 3.07 ms: 1.12x faster                                                        |
| async_tree_none_tg         | 427 ms                                                                 | 380 ms: 1.12x faster                                                         |
| regex_dna                  | 195 ms                                                                 | 174 ms: 1.12x faster                                                         |
| sympy_expand               | 477 ms                                                                 | 427 ms: 1.12x faster                                                         |
| comprehensions             | 17.1 us                                                                | 15.3 us: 1.12x faster                                                        |
| xml_etree_parse            | 150 ms                                                                 | 134 ms: 1.12x faster                                                         |
| regex_v8                   | 25.3 ms                                                                | 22.7 ms: 1.12x faster                                                        |
| pprint_safe_repr           | 777 ms                                                                 | 697 ms: 1.11x faster                                                         |
| scimark_monte_carlo        | 73.7 ms                                                                | 66.2 ms: 1.11x faster                                                        |
| meteor_contest             | 102 ms                                                                 | 91.5 ms: 1.11x faster                                                        |
| pprint_pformat             | 1.58 sec                                                               | 1.43 sec: 1.11x faster                                                       |
| regex_compile              | 138 ms                                                                 | 125 ms: 1.10x faster                                                         |
| async_tree_cpu_io_mixed    | 674 ms                                                                 | 611 ms: 1.10x faster                                                         |
| richards                   | 48.8 ms                                                                | 44.3 ms: 1.10x faster                                                        |
| mako                       | 10.0 ms                                                                | 9.10 ms: 1.10x faster                                                        |
| sqlglot_optimize           | 56.9 ms                                                                | 51.7 ms: 1.10x faster                                                        |
| docutils                   | 2.62 sec                                                               | 2.38 sec: 1.10x faster                                                       |
| unpickle_list              | 4.64 us                                                                | 4.22 us: 1.10x faster                                                        |
| async_tree_none            | 427 ms                                                                 | 389 ms: 1.10x faster                                                         |
| sympy_str                  | 276 ms                                                                 | 251 ms: 1.10x faster                                                         |
| nqueens                    | 89.4 ms                                                                | 81.4 ms: 1.10x faster                                                        |
| pickle_dict                | 28.8 us                                                                | 26.2 us: 1.10x faster                                                        |
| mdp                        | 2.42 sec                                                               | 2.21 sec: 1.10x faster                                                       |
| deepcopy_memo              | 36.3 us                                                                | 33.1 us: 1.10x faster                                                        |
| unpickle_pure_python       | 226 us                                                                 | 207 us: 1.10x faster                                                         |
| pickle                     | 9.83 us                                                                | 8.98 us: 1.10x faster                                                        |
| sympy_integrate            | 20.9 ms                                                                | 19.1 ms: 1.10x faster                                                        |
| coverage                   | 83.2 ms                                                                | 76.0 ms: 1.09x faster                                                        |
| richards_super             | 56.3 ms                                                                | 51.5 ms: 1.09x faster                                                        |
| raytrace                   | 299 ms                                                                 | 273 ms: 1.09x faster                                                         |
| sqlglot_transpile          | 1.64 ms                                                                | 1.50 ms: 1.09x faster                                                        |
| async_generators           | 398 ms                                                                 | 364 ms: 1.09x faster                                                         |
| genshi_xml                 | 54.7 ms                                                                | 50.1 ms: 1.09x faster                                                        |
| generators                 | 30.9 ms                                                                | 28.3 ms: 1.09x faster                                                        |
| tomli_loads                | 2.02 sec                                                               | 1.85 sec: 1.09x faster                                                       |
| go                         | 161 ms                                                                 | 147 ms: 1.09x faster                                                         |
| django_template            | 35.0 ms                                                                | 32.1 ms: 1.09x faster                                                        |
| pickle_list                | 3.89 us                                                                | 3.57 us: 1.09x faster                                                        |
| sympy_sum                  | 151 ms                                                                 | 139 ms: 1.09x faster                                                         |
| pycparser                  | 1.27 sec                                                               | 1.16 sec: 1.09x faster                                                       |
| hexiom                     | 6.49 ms                                                                | 5.96 ms: 1.09x faster                                                        |
| json                       | 4.66 ms                                                                | 4.28 ms: 1.09x faster                                                        |
| typing_runtime_protocols   | 112 us                                                                 | 103 us: 1.09x faster                                                         |
| async_tree_io_tg           | 1.10 sec                                                               | 1.01 sec: 1.09x faster                                                       |
| logging_silent             | 103 ns                                                                 | 94.5 ns: 1.09x faster                                                        |
| 2to3                       | 296 ms                                                                 | 273 ms: 1.09x faster                                                         |
| genshi_text                | 25.1 ms                                                                | 23.1 ms: 1.08x faster                                                        |
| telco                      | 7.58 ms                                                                | 7.00 ms: 1.08x faster                                                        |
| deltablue                  | 3.79 ms                                                                | 3.51 ms: 1.08x faster                                                        |
| async_tree_io              | 1.12 sec                                                               | 1.04 sec: 1.08x faster                                                       |
| asyncio_tcp                | 555 ms                                                                 | 514 ms: 1.08x faster                                                         |
| pylint                     | 310 ms                                                                 | 287 ms: 1.08x faster                                                         |
| crypto_pyaes               | 66.7 ms                                                                | 61.9 ms: 1.08x faster                                                        |
| scimark_fft                | 312 ms                                                                 | 289 ms: 1.08x faster                                                         |
| dulwich_log                | 79.2 ms                                                                | 73.5 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 654 ms                                                                 | 606 ms: 1.08x faster                                                         |
| create_gc_cycles           | 1.09 ms                                                                | 1.02 ms: 1.08x faster                                                        |
| sqlite_synth               | 2.73 us                                                                | 2.54 us: 1.08x faster                                                        |
| asyncio_websockets         | 720 ms                                                                 | 669 ms: 1.08x faster                                                         |
| html5lib                   | 72.5 ms                                                                | 67.5 ms: 1.07x faster                                                        |
| deepcopy                   | 339 us                                                                 | 316 us: 1.07x faster                                                         |
| chaos                      | 63.4 ms                                                                | 59.2 ms: 1.07x faster                                                        |
| pidigits                   | 187 ms                                                                 | 174 ms: 1.07x faster                                                         |
| asyncio_tcp_ssl            | 1.73 sec                                                               | 1.61 sec: 1.07x faster                                                       |
| pathlib                    | 23.9 ms                                                                | 22.4 ms: 1.07x faster                                                        |
| json_loads                 | 24.0 us                                                                | 22.4 us: 1.07x faster                                                        |
| pickle_pure_python         | 307 us                                                                 | 288 us: 1.07x faster                                                         |
| thrift                     | 765 us                                                                 | 717 us: 1.07x faster                                                         |
| dask                       | 471 ms                                                                 | 441 ms: 1.07x faster                                                         |
| pyflate                    | 468 ms                                                                 | 439 ms: 1.07x faster                                                         |
| logging_simple             | 6.04 us                                                                | 5.66 us: 1.07x faster                                                        |
| bench_mp_pool              | 15.4 ms                                                                | 14.5 ms: 1.07x faster                                                        |
| xml_etree_process          | 58.8 ms                                                                | 55.3 ms: 1.06x faster                                                        |
| xml_etree_generate         | 84.1 ms                                                                | 79.0 ms: 1.06x faster                                                        |
| float                      | 78.0 ms                                                                | 73.3 ms: 1.06x faster                                                        |
| scimark_sor                | 149 ms                                                                 | 140 ms: 1.06x faster                                                         |
| deepcopy_reduce            | 3.11 us                                                                | 2.93 us: 1.06x faster                                                        |
| logging_format             | 6.64 us                                                                | 6.25 us: 1.06x faster                                                        |
| spectral_norm              | 95.1 ms                                                                | 89.6 ms: 1.06x faster                                                        |
| json_dumps                 | 9.49 ms                                                                | 8.95 ms: 1.06x faster                                                        |
| bench_thread_pool          | 1.49 ms                                                                | 1.41 ms: 1.06x faster                                                        |
| sqlglot_parse              | 1.30 ms                                                                | 1.23 ms: 1.06x faster                                                        |
| tornado_http               | 145 ms                                                                 | 137 ms: 1.05x faster                                                         |
| python_startup_no_site     | 16.7 ms                                                                | 15.9 ms: 1.05x faster                                                        |
| python_startup             | 18.2 ms                                                                | 17.2 ms: 1.05x faster                                                        |
| chameleon                  | 7.07 ms                                                                | 6.76 ms: 1.05x faster                                                        |
| unpickle                   | 13.0 us                                                                | 12.5 us: 1.04x faster                                                        |
| coroutines                 | 24.7 ms                                                                | 23.7 ms: 1.04x faster                                                        |
| sqlglot_normalize          | 110 ms                                                                 | 269 ms: 2.44x slower                                                         |
| Geometric mean             | (ref)                                                                  | 1.08x faster                                                                 |

Benchmark hidden because not significant (1): mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: 1.01x