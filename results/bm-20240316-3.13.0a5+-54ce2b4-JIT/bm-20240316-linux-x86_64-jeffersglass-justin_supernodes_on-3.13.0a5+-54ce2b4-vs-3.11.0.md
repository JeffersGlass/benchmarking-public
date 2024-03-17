# Results vs. 3.11.0

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: 54ce2b4
- commit date: 2024-03-16
- overall geometric mean: 1.12x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: 1.22x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 273 ms: 1.03x slower                                                         |
| chameleon      | 6.70 ms                                                | 6.76 ms: 1.01x slower                                                        |
| docutils       | 2.66 sec                                               | 2.38 sec: 1.12x faster                                                       |
| html5lib       | 64.8 ms                                                | 67.5 ms: 1.04x slower                                                        |
| tornado_http   | 98.1 ms                                                | 137 ms: 1.40x slower                                                         |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 389 ms: 1.36x faster                                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 482 ms: 1.30x faster                                                         |
| async_tree_memoization     | 639 ms                                                 | 494 ms: 1.29x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 380 ms: 1.29x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.01 sec: 1.28x faster                                                       |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 606 ms: 1.26x faster                                                         |
| async_tree_io              | 1.29 sec                                               | 1.04 sec: 1.24x faster                                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 611 ms: 1.23x faster                                                         |
| Geometric mean             | (ref)                                                  | 1.28x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 174 ms: 1.11x faster                                                         |
| float          | 78.9 ms                                                | 73.3 ms: 1.08x faster                                                        |
| nbody          | 96.0 ms                                                | 99.6 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                  | 1.05x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 205 ms                                                 | 174 ms: 1.18x faster                                                         |
| regex_effbot   | 3.51 ms                                                | 3.07 ms: 1.14x faster                                                        |
| regex_compile  | 141 ms                                                 | 125 ms: 1.13x faster                                                         |
| Geometric mean | (ref)                                                  | 1.11x faster                                                                 |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 8.95 ms: 1.49x faster                                                        |
| pickle_dict          | 34.6 us                                                | 26.2 us: 1.32x faster                                                        |
| json_loads           | 29.2 us                                                | 22.4 us: 1.30x faster                                                        |
| pickle_list          | 4.59 us                                                | 3.57 us: 1.29x faster                                                        |
| tomli_loads          | 2.30 sec                                               | 1.85 sec: 1.25x faster                                                       |
| unpickle_list        | 5.21 us                                                | 4.22 us: 1.24x faster                                                        |
| pickle               | 11.0 us                                                | 8.98 us: 1.22x faster                                                        |
| xml_etree_parse      | 164 ms                                                 | 134 ms: 1.22x faster                                                         |
| xml_etree_iterparse  | 108 ms                                                 | 89.7 ms: 1.20x faster                                                        |
| unpickle_pure_python | 242 us                                                 | 207 us: 1.17x faster                                                         |
| pickle_pure_python   | 320 us                                                 | 288 us: 1.11x faster                                                         |
| unpickle             | 13.8 us                                                | 12.5 us: 1.11x faster                                                        |
| xml_etree_process    | 56.9 ms                                                | 55.3 ms: 1.03x faster                                                        |
| xml_etree_generate   | 81.1 ms                                                | 79.0 ms: 1.03x faster                                                        |
| Geometric mean       | (ref)                                                  | 1.21x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 17.2 ms: 2.01x slower                                                        |
| python_startup_no_site | 6.01 ms                                                | 15.9 ms: 2.64x slower                                                        |
| Geometric mean         | (ref)                                                  | 2.30x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.10 ms: 1.17x faster                                                        |
| genshi_xml      | 53.4 ms                                                | 50.1 ms: 1.07x faster                                                        |
| django_template | 33.5 ms                                                | 32.1 ms: 1.05x faster                                                        |
| genshi_text     | 22.5 ms                                                | 23.1 ms: 1.03x slower                                                        |
| Geometric mean  | (ref)                                                  | 1.06x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 103 us: 5.03x faster                                                         |
| generators                 | 74.9 ms                                                | 28.3 ms: 2.64x faster                                                        |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.61 sec: 1.93x faster                                                       |
| asyncio_tcp                | 875 ms                                                 | 514 ms: 1.70x faster                                                         |
| pylint                     | 476 ms                                                 | 287 ms: 1.66x faster                                                         |
| bench_mp_pool              | 24.0 ms                                                | 14.5 ms: 1.66x faster                                                        |
| comprehensions             | 23.6 us                                                | 15.3 us: 1.54x faster                                                        |
| json_dumps                 | 13.3 ms                                                | 8.95 ms: 1.49x faster                                                        |
| create_gc_cycles           | 1.43 ms                                                | 1.02 ms: 1.41x faster                                                        |
| async_tree_none            | 528 ms                                                 | 389 ms: 1.36x faster                                                         |
| gc_traversal               | 4.01 ms                                                | 2.97 ms: 1.35x faster                                                        |
| pickle_dict                | 34.6 us                                                | 26.2 us: 1.32x faster                                                        |
| json_loads                 | 29.2 us                                                | 22.4 us: 1.30x faster                                                        |
| async_tree_memoization_tg  | 626 ms                                                 | 482 ms: 1.30x faster                                                         |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 3.89 ms: 1.29x faster                                                        |
| async_tree_memoization     | 639 ms                                                 | 494 ms: 1.29x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 380 ms: 1.29x faster                                                         |
| pickle_list                | 4.59 us                                                | 3.57 us: 1.29x faster                                                        |
| async_tree_io_tg           | 1.29 sec                                               | 1.01 sec: 1.28x faster                                                       |
| fannkuch                   | 405 ms                                                 | 321 ms: 1.26x faster                                                         |
| mdp                        | 2.77 sec                                               | 2.21 sec: 1.26x faster                                                       |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 606 ms: 1.26x faster                                                         |
| tomli_loads                | 2.30 sec                                               | 1.85 sec: 1.25x faster                                                       |
| crypto_pyaes               | 76.7 ms                                                | 61.9 ms: 1.24x faster                                                        |
| async_tree_io              | 1.29 sec                                               | 1.04 sec: 1.24x faster                                                       |
| unpickle_list              | 5.21 us                                                | 4.22 us: 1.24x faster                                                        |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 611 ms: 1.23x faster                                                         |
| json                       | 5.24 ms                                                | 4.28 ms: 1.22x faster                                                        |
| pickle                     | 11.0 us                                                | 8.98 us: 1.22x faster                                                        |
| xml_etree_parse            | 164 ms                                                 | 134 ms: 1.22x faster                                                         |
| sympy_sum                  | 169 ms                                                 | 139 ms: 1.22x faster                                                         |
| chaos                      | 71.9 ms                                                | 59.2 ms: 1.21x faster                                                        |
| deepcopy_memo              | 40.2 us                                                | 33.1 us: 1.21x faster                                                        |
| spectral_norm              | 108 ms                                                 | 89.6 ms: 1.21x faster                                                        |
| xml_etree_iterparse        | 108 ms                                                 | 89.7 ms: 1.20x faster                                                        |
| richards_super             | 61.9 ms                                                | 51.5 ms: 1.20x faster                                                        |
| scimark_fft                | 345 ms                                                 | 289 ms: 1.19x faster                                                         |
| meteor_contest             | 109 ms                                                 | 91.5 ms: 1.19x faster                                                        |
| sympy_str                  | 297 ms                                                 | 251 ms: 1.18x faster                                                         |
| logging_silent             | 111 ns                                                 | 94.5 ns: 1.18x faster                                                        |
| regex_dna                  | 205 ms                                                 | 174 ms: 1.18x faster                                                         |
| mako                       | 10.7 ms                                                | 9.10 ms: 1.17x faster                                                        |
| unpickle_pure_python       | 242 us                                                 | 207 us: 1.17x faster                                                         |
| sqlglot_transpile          | 1.75 ms                                                | 1.50 ms: 1.17x faster                                                        |
| sqlglot_parse              | 1.43 ms                                                | 1.23 ms: 1.17x faster                                                        |
| hexiom                     | 6.89 ms                                                | 5.96 ms: 1.16x faster                                                        |
| deepcopy                   | 365 us                                                 | 316 us: 1.15x faster                                                         |
| regex_effbot               | 3.51 ms                                                | 3.07 ms: 1.14x faster                                                        |
| coroutines                 | 27.0 ms                                                | 23.7 ms: 1.14x faster                                                        |
| sympy_expand               | 484 ms                                                 | 427 ms: 1.13x faster                                                         |
| raytrace                   | 309 ms                                                 | 273 ms: 1.13x faster                                                         |
| regex_compile              | 141 ms                                                 | 125 ms: 1.13x faster                                                         |
| richards                   | 49.8 ms                                                | 44.3 ms: 1.12x faster                                                        |
| sympy_integrate            | 21.5 ms                                                | 19.1 ms: 1.12x faster                                                        |
| docutils                   | 2.66 sec                                               | 2.38 sec: 1.12x faster                                                       |
| deltablue                  | 3.92 ms                                                | 3.51 ms: 1.12x faster                                                        |
| pidigits                   | 194 ms                                                 | 174 ms: 1.11x faster                                                         |
| pickle_pure_python         | 320 us                                                 | 288 us: 1.11x faster                                                         |
| unpickle                   | 13.8 us                                                | 12.5 us: 1.11x faster                                                        |
| deepcopy_reduce            | 3.22 us                                                | 2.93 us: 1.10x faster                                                        |
| logging_simple             | 6.22 us                                                | 5.66 us: 1.10x faster                                                        |
| thrift                     | 784 us                                                 | 717 us: 1.09x faster                                                         |
| logging_format             | 6.81 us                                                | 6.25 us: 1.09x faster                                                        |
| pprint_pformat             | 1.55 sec                                               | 1.43 sec: 1.09x faster                                                       |
| nqueens                    | 87.9 ms                                                | 81.4 ms: 1.08x faster                                                        |
| float                      | 78.9 ms                                                | 73.3 ms: 1.08x faster                                                        |
| pprint_safe_repr           | 747 ms                                                 | 697 ms: 1.07x faster                                                         |
| sqlglot_optimize           | 55.3 ms                                                | 51.7 ms: 1.07x faster                                                        |
| scimark_monte_carlo        | 70.7 ms                                                | 66.2 ms: 1.07x faster                                                        |
| scimark_lu                 | 116 ms                                                 | 109 ms: 1.07x faster                                                         |
| genshi_xml                 | 53.4 ms                                                | 50.1 ms: 1.07x faster                                                        |
| django_template            | 33.5 ms                                                | 32.1 ms: 1.05x faster                                                        |
| coverage                   | 78.8 ms                                                | 76.0 ms: 1.04x faster                                                        |
| xml_etree_process          | 56.9 ms                                                | 55.3 ms: 1.03x faster                                                        |
| xml_etree_generate         | 81.1 ms                                                | 79.0 ms: 1.03x faster                                                        |
| async_generators           | 374 ms                                                 | 364 ms: 1.03x faster                                                         |
| pycparser                  | 1.19 sec                                               | 1.16 sec: 1.02x faster                                                       |
| sqlite_synth               | 2.57 us                                                | 2.54 us: 1.01x faster                                                        |
| go                         | 149 ms                                                 | 147 ms: 1.01x faster                                                         |
| chameleon                  | 6.70 ms                                                | 6.76 ms: 1.01x slower                                                        |
| pyflate                    | 434 ms                                                 | 439 ms: 1.01x slower                                                         |
| telco                      | 6.86 ms                                                | 7.00 ms: 1.02x slower                                                        |
| genshi_text                | 22.5 ms                                                | 23.1 ms: 1.03x slower                                                        |
| 2to3                       | 264 ms                                                 | 273 ms: 1.03x slower                                                         |
| nbody                      | 96.0 ms                                                | 99.6 ms: 1.04x slower                                                        |
| html5lib                   | 64.8 ms                                                | 67.5 ms: 1.04x slower                                                        |
| dulwich_log                | 64.6 ms                                                | 73.5 ms: 1.14x slower                                                        |
| mypy2                      | 686 ms                                                 | 788 ms: 1.15x slower                                                         |
| scimark_sor                | 121 ms                                                 | 140 ms: 1.15x slower                                                         |
| pathlib                    | 18.5 ms                                                | 22.4 ms: 1.21x slower                                                        |
| dask                       | 365 ms                                                 | 441 ms: 1.21x slower                                                         |
| asyncio_websockets         | 550 ms                                                 | 669 ms: 1.22x slower                                                         |
| tornado_http               | 98.1 ms                                                | 137 ms: 1.40x slower                                                         |
| bench_thread_pool          | 834 us                                                 | 1.41 ms: 1.69x slower                                                        |
| python_startup             | 8.56 ms                                                | 17.2 ms: 2.01x slower                                                        |
| unpack_sequence            | 43.5 ns                                                | 99.0 ns: 2.28x slower                                                        |
| sqlglot_normalize          | 113 ms                                                 | 269 ms: 2.38x slower                                                         |
| python_startup_no_site     | 6.01 ms                                                | 15.9 ms: 2.64x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.12x faster                                                                 |

Benchmark hidden because not significant (1): regex_v8
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.11x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: 1.22x