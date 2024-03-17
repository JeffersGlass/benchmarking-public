# Results vs. 3.11.0

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: 54ce2b4
- commit date: 2024-03-16
- overall geometric mean: 1.03x faster
- HPT reliability: 98.01%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.22x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 304 ms: 1.15x slower                                                         |
| chameleon      | 6.70 ms                                                | 7.35 ms: 1.10x slower                                                        |
| docutils       | 2.66 sec                                               | 2.76 sec: 1.04x slower                                                       |
| html5lib       | 64.8 ms                                                | 73.5 ms: 1.13x slower                                                        |
| tornado_http   | 98.1 ms                                                | 145 ms: 1.48x slower                                                         |
| Geometric mean | (ref)                                                  | 1.17x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.29 sec                                               | 1.14 sec: 1.13x faster                                                       |
| async_tree_none_tg         | 491 ms                                                 | 440 ms: 1.12x faster                                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 682 ms: 1.12x faster                                                         |
| async_tree_none            | 528 ms                                                 | 476 ms: 1.11x faster                                                         |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 590 ms: 1.06x faster                                                         |
| async_tree_memoization     | 639 ms                                                 | 607 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 728 ms: 1.03x faster                                                         |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                         |
| float          | 78.9 ms                                                | 79.8 ms: 1.01x slower                                                        |
| nbody          | 96.0 ms                                                | 107 ms: 1.11x slower                                                         |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 205 ms                                                 | 188 ms: 1.09x faster                                                         |
| regex_compile  | 141 ms                                                 | 134 ms: 1.06x faster                                                         |
| regex_effbot   | 3.51 ms                                                | 3.42 ms: 1.03x faster                                                        |
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.08x slower                                                        |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.57 ms: 1.39x faster                                                        |
| json_loads           | 29.2 us                                                | 24.0 us: 1.22x faster                                                        |
| pickle_dict          | 34.6 us                                                | 28.7 us: 1.21x faster                                                        |
| pickle_list          | 4.59 us                                                | 3.83 us: 1.20x faster                                                        |
| tomli_loads          | 2.30 sec                                               | 1.98 sec: 1.16x faster                                                       |
| unpickle_list        | 5.21 us                                                | 4.56 us: 1.14x faster                                                        |
| pickle               | 11.0 us                                                | 9.82 us: 1.12x faster                                                        |
| xml_etree_parse      | 164 ms                                                 | 148 ms: 1.11x faster                                                         |
| unpickle_pure_python | 242 us                                                 | 223 us: 1.08x faster                                                         |
| xml_etree_iterparse  | 108 ms                                                 | 101 ms: 1.07x faster                                                         |
| pickle_pure_python   | 320 us                                                 | 308 us: 1.04x faster                                                         |
| unpickle             | 13.8 us                                                | 13.7 us: 1.01x faster                                                        |
| xml_etree_process    | 56.9 ms                                                | 59.3 ms: 1.04x slower                                                        |
| xml_etree_generate   | 81.1 ms                                                | 85.2 ms: 1.05x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 19.3 ms: 2.25x slower                                                        |
| python_startup_no_site | 6.01 ms                                                | 17.8 ms: 2.96x slower                                                        |
| Geometric mean         | (ref)                                                  | 2.58x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 10.7 ms                                                | 10.1 ms: 1.05x faster                                                        |
| genshi_xml      | 53.4 ms                                                | 55.0 ms: 1.03x slower                                                        |
| django_template | 33.5 ms                                                | 34.5 ms: 1.03x slower                                                        |
| genshi_text     | 22.5 ms                                                | 24.7 ms: 1.10x slower                                                        |
| Geometric mean  | (ref)                                                  | 1.03x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-54ce2b4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 107 us: 4.86x faster                                                         |
| generators                 | 74.9 ms                                                | 33.6 ms: 2.23x faster                                                        |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.73x faster                                                       |
| bench_mp_pool              | 24.0 ms                                                | 16.2 ms: 1.49x faster                                                        |
| pylint                     | 476 ms                                                 | 321 ms: 1.48x faster                                                         |
| asyncio_tcp                | 875 ms                                                 | 591 ms: 1.48x faster                                                         |
| comprehensions             | 23.6 us                                                | 16.7 us: 1.41x faster                                                        |
| json_dumps                 | 13.3 ms                                                | 9.57 ms: 1.39x faster                                                        |
| create_gc_cycles           | 1.43 ms                                                | 1.11 ms: 1.30x faster                                                        |
| json_loads                 | 29.2 us                                                | 24.0 us: 1.22x faster                                                        |
| pickle_dict                | 34.6 us                                                | 28.7 us: 1.21x faster                                                        |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.19 ms: 1.20x faster                                                        |
| pickle_list                | 4.59 us                                                | 3.83 us: 1.20x faster                                                        |
| spectral_norm              | 108 ms                                                 | 92.2 ms: 1.17x faster                                                        |
| gc_traversal               | 4.01 ms                                                | 3.44 ms: 1.17x faster                                                        |
| tomli_loads                | 2.30 sec                                               | 1.98 sec: 1.16x faster                                                       |
| crypto_pyaes               | 76.7 ms                                                | 66.1 ms: 1.16x faster                                                        |
| richards_super             | 61.9 ms                                                | 53.7 ms: 1.15x faster                                                        |
| unpickle_list              | 5.21 us                                                | 4.56 us: 1.14x faster                                                        |
| chaos                      | 71.9 ms                                                | 63.0 ms: 1.14x faster                                                        |
| async_tree_io_tg           | 1.29 sec                                               | 1.14 sec: 1.13x faster                                                       |
| fannkuch                   | 405 ms                                                 | 358 ms: 1.13x faster                                                         |
| json                       | 5.24 ms                                                | 4.67 ms: 1.12x faster                                                        |
| pickle                     | 11.0 us                                                | 9.82 us: 1.12x faster                                                        |
| sympy_sum                  | 169 ms                                                 | 151 ms: 1.12x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 440 ms: 1.12x faster                                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 682 ms: 1.12x faster                                                         |
| scimark_fft                | 345 ms                                                 | 311 ms: 1.11x faster                                                         |
| logging_silent             | 111 ns                                                 | 100.0 ns: 1.11x faster                                                       |
| async_tree_none            | 528 ms                                                 | 476 ms: 1.11x faster                                                         |
| xml_etree_parse            | 164 ms                                                 | 148 ms: 1.11x faster                                                         |
| meteor_contest             | 109 ms                                                 | 98.7 ms: 1.10x faster                                                        |
| deepcopy_memo              | 40.2 us                                                | 36.6 us: 1.10x faster                                                        |
| sqlglot_parse              | 1.43 ms                                                | 1.31 ms: 1.09x faster                                                        |
| hexiom                     | 6.89 ms                                                | 6.29 ms: 1.09x faster                                                        |
| regex_dna                  | 205 ms                                                 | 188 ms: 1.09x faster                                                         |
| unpickle_pure_python       | 242 us                                                 | 223 us: 1.08x faster                                                         |
| coroutines                 | 27.0 ms                                                | 25.0 ms: 1.08x faster                                                        |
| sympy_str                  | 297 ms                                                 | 276 ms: 1.08x faster                                                         |
| xml_etree_iterparse        | 108 ms                                                 | 101 ms: 1.07x faster                                                         |
| richards                   | 49.8 ms                                                | 46.7 ms: 1.07x faster                                                        |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 590 ms: 1.06x faster                                                         |
| regex_compile              | 141 ms                                                 | 134 ms: 1.06x faster                                                         |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.06x faster                                                        |
| raytrace                   | 309 ms                                                 | 293 ms: 1.05x faster                                                         |
| async_tree_memoization     | 639 ms                                                 | 607 ms: 1.05x faster                                                         |
| deepcopy                   | 365 us                                                 | 347 us: 1.05x faster                                                         |
| mako                       | 10.7 ms                                                | 10.1 ms: 1.05x faster                                                        |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                         |
| pickle_pure_python         | 320 us                                                 | 308 us: 1.04x faster                                                         |
| logging_simple             | 6.22 us                                                | 6.00 us: 1.04x faster                                                        |
| sqlglot_normalize          | 113 ms                                                 | 109 ms: 1.04x faster                                                         |
| deltablue                  | 3.92 ms                                                | 3.80 ms: 1.03x faster                                                        |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 728 ms: 1.03x faster                                                         |
| sympy_integrate            | 21.5 ms                                                | 20.9 ms: 1.03x faster                                                        |
| logging_format             | 6.81 us                                                | 6.63 us: 1.03x faster                                                        |
| mdp                        | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                       |
| regex_effbot               | 3.51 ms                                                | 3.42 ms: 1.03x faster                                                        |
| sympy_expand               | 484 ms                                                 | 473 ms: 1.02x faster                                                         |
| thrift                     | 784 us                                                 | 766 us: 1.02x faster                                                         |
| nqueens                    | 87.9 ms                                                | 86.2 ms: 1.02x faster                                                        |
| deepcopy_reduce            | 3.22 us                                                | 3.16 us: 1.02x faster                                                        |
| unpickle                   | 13.8 us                                                | 13.7 us: 1.01x faster                                                        |
| float                      | 78.9 ms                                                | 79.8 ms: 1.01x slower                                                        |
| scimark_monte_carlo        | 70.7 ms                                                | 71.6 ms: 1.01x slower                                                        |
| pprint_safe_repr           | 747 ms                                                 | 757 ms: 1.01x slower                                                         |
| sqlglot_optimize           | 55.3 ms                                                | 56.7 ms: 1.02x slower                                                        |
| genshi_xml                 | 53.4 ms                                                | 55.0 ms: 1.03x slower                                                        |
| django_template            | 33.5 ms                                                | 34.5 ms: 1.03x slower                                                        |
| coverage                   | 78.8 ms                                                | 81.6 ms: 1.04x slower                                                        |
| docutils                   | 2.66 sec                                               | 2.76 sec: 1.04x slower                                                       |
| sqlite_synth               | 2.57 us                                                | 2.68 us: 1.04x slower                                                        |
| xml_etree_process          | 56.9 ms                                                | 59.3 ms: 1.04x slower                                                        |
| xml_etree_generate         | 81.1 ms                                                | 85.2 ms: 1.05x slower                                                        |
| go                         | 149 ms                                                 | 158 ms: 1.06x slower                                                         |
| regex_v8                   | 22.9 ms                                                | 24.6 ms: 1.08x slower                                                        |
| async_generators           | 374 ms                                                 | 406 ms: 1.09x slower                                                         |
| chameleon                  | 6.70 ms                                                | 7.35 ms: 1.10x slower                                                        |
| genshi_text                | 22.5 ms                                                | 24.7 ms: 1.10x slower                                                        |
| nbody                      | 96.0 ms                                                | 107 ms: 1.11x slower                                                         |
| pycparser                  | 1.19 sec                                               | 1.32 sec: 1.12x slower                                                       |
| telco                      | 6.86 ms                                                | 7.68 ms: 1.12x slower                                                        |
| html5lib                   | 64.8 ms                                                | 73.5 ms: 1.13x slower                                                        |
| pyflate                    | 434 ms                                                 | 496 ms: 1.14x slower                                                         |
| 2to3                       | 264 ms                                                 | 304 ms: 1.15x slower                                                         |
| dulwich_log                | 64.6 ms                                                | 77.8 ms: 1.21x slower                                                        |
| scimark_sor                | 121 ms                                                 | 148 ms: 1.22x slower                                                         |
| pathlib                    | 18.5 ms                                                | 24.1 ms: 1.30x slower                                                        |
| asyncio_websockets         | 550 ms                                                 | 720 ms: 1.31x slower                                                         |
| dask                       | 365 ms                                                 | 495 ms: 1.36x slower                                                         |
| mypy2                      | 686 ms                                                 | 940 ms: 1.37x slower                                                         |
| tornado_http               | 98.1 ms                                                | 145 ms: 1.48x slower                                                         |
| bench_thread_pool          | 834 us                                                 | 1.52 ms: 1.82x slower                                                        |
| python_startup             | 8.56 ms                                                | 19.3 ms: 2.25x slower                                                        |
| unpack_sequence            | 43.5 ns                                                | 107 ns: 2.47x slower                                                         |
| python_startup_no_site     | 6.01 ms                                                | 17.8 ms: 2.96x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                                 |

Benchmark hidden because not significant (2): scimark_lu, pprint_pformat
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 98.01% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.22x