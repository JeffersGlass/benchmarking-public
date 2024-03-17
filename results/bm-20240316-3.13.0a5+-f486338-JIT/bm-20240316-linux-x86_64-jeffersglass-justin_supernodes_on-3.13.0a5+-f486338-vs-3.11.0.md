# Results vs. 3.11.0

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: f486338
- commit date: 2024-03-16
- overall geometric mean: 1.04x faster
- HPT reliability: 99.80%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.23x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 297 ms: 1.12x slower                                                         |
| chameleon      | 6.70 ms                                                | 7.25 ms: 1.08x slower                                                        |
| html5lib       | 64.8 ms                                                | 71.7 ms: 1.11x slower                                                        |
| tornado_http   | 98.1 ms                                                | 147 ms: 1.50x slower                                                         |
| Geometric mean | (ref)                                                  | 1.15x slower                                                                 |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.29 sec                                               | 1.10 sec: 1.18x faster                                                       |
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 428 ms: 1.15x faster                                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 677 ms: 1.13x faster                                                         |
| async_tree_io              | 1.29 sec                                               | 1.16 sec: 1.11x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 566 ms: 1.11x faster                                                         |
| async_tree_memoization     | 639 ms                                                 | 581 ms: 1.10x faster                                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 698 ms: 1.07x faster                                                         |
| Geometric mean             | (ref)                                                  | 1.13x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                         |
| float          | 78.9 ms                                                | 78.5 ms: 1.01x faster                                                        |
| nbody          | 96.0 ms                                                | 103 ms: 1.07x slower                                                         |
| Geometric mean | (ref)                                                  | 1.01x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 205 ms                                                 | 191 ms: 1.07x faster                                                         |
| regex_compile  | 141 ms                                                 | 136 ms: 1.04x faster                                                         |
| regex_effbot   | 3.51 ms                                                | 3.37 ms: 1.04x faster                                                        |
| regex_v8       | 22.9 ms                                                | 23.8 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                  | 1.03x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.56 ms: 1.40x faster                                                        |
| pickle_dict          | 34.6 us                                                | 27.8 us: 1.24x faster                                                        |
| json_loads           | 29.2 us                                                | 23.9 us: 1.22x faster                                                        |
| pickle_list          | 4.59 us                                                | 3.76 us: 1.22x faster                                                        |
| tomli_loads          | 2.30 sec                                               | 1.93 sec: 1.19x faster                                                       |
| unpickle_list        | 5.21 us                                                | 4.43 us: 1.18x faster                                                        |
| pickle               | 11.0 us                                                | 9.75 us: 1.13x faster                                                        |
| xml_etree_parse      | 164 ms                                                 | 147 ms: 1.12x faster                                                         |
| unpickle_pure_python | 242 us                                                 | 223 us: 1.09x faster                                                         |
| xml_etree_iterparse  | 108 ms                                                 | 100 ms: 1.08x faster                                                         |
| pickle_pure_python   | 320 us                                                 | 304 us: 1.05x faster                                                         |
| unpickle             | 13.8 us                                                | 13.5 us: 1.02x faster                                                        |
| xml_etree_generate   | 81.1 ms                                                | 85.3 ms: 1.05x slower                                                        |
| xml_etree_process    | 56.9 ms                                                | 59.9 ms: 1.05x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 19.2 ms: 2.24x slower                                                        |
| python_startup_no_site | 6.01 ms                                                | 17.8 ms: 2.96x slower                                                        |
| Geometric mean         | (ref)                                                  | 2.57x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.85 ms: 1.08x faster                                                        |
| genshi_xml      | 53.4 ms                                                | 54.2 ms: 1.01x slower                                                        |
| django_template | 33.5 ms                                                | 34.6 ms: 1.03x slower                                                        |
| genshi_text     | 22.5 ms                                                | 24.7 ms: 1.10x slower                                                        |
| Geometric mean  | (ref)                                                  | 1.01x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.70x faster                                                         |
| generators                 | 74.9 ms                                                | 31.3 ms: 2.39x faster                                                        |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.76 sec: 1.77x faster                                                       |
| bench_mp_pool              | 24.0 ms                                                | 16.0 ms: 1.50x faster                                                        |
| asyncio_tcp                | 875 ms                                                 | 592 ms: 1.48x faster                                                         |
| pylint                     | 476 ms                                                 | 323 ms: 1.47x faster                                                         |
| comprehensions             | 23.6 us                                                | 16.4 us: 1.44x faster                                                        |
| json_dumps                 | 13.3 ms                                                | 9.56 ms: 1.40x faster                                                        |
| create_gc_cycles           | 1.43 ms                                                | 1.10 ms: 1.30x faster                                                        |
| pickle_dict                | 34.6 us                                                | 27.8 us: 1.24x faster                                                        |
| gc_traversal               | 4.01 ms                                                | 3.27 ms: 1.23x faster                                                        |
| json_loads                 | 29.2 us                                                | 23.9 us: 1.22x faster                                                        |
| pickle_list                | 4.59 us                                                | 3.76 us: 1.22x faster                                                        |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.16 ms: 1.21x faster                                                        |
| tomli_loads                | 2.30 sec                                               | 1.93 sec: 1.19x faster                                                       |
| fannkuch                   | 405 ms                                                 | 343 ms: 1.18x faster                                                         |
| unpickle_list              | 5.21 us                                                | 4.43 us: 1.18x faster                                                        |
| async_tree_io_tg           | 1.29 sec                                               | 1.10 sec: 1.18x faster                                                       |
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                         |
| chaos                      | 71.9 ms                                                | 61.3 ms: 1.17x faster                                                        |
| crypto_pyaes               | 76.7 ms                                                | 65.4 ms: 1.17x faster                                                        |
| spectral_norm              | 108 ms                                                 | 92.7 ms: 1.17x faster                                                        |
| async_tree_none_tg         | 491 ms                                                 | 428 ms: 1.15x faster                                                         |
| json                       | 5.24 ms                                                | 4.58 ms: 1.14x faster                                                        |
| scimark_fft                | 345 ms                                                 | 303 ms: 1.14x faster                                                         |
| richards_super             | 61.9 ms                                                | 54.3 ms: 1.14x faster                                                        |
| pickle                     | 11.0 us                                                | 9.75 us: 1.13x faster                                                        |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 677 ms: 1.13x faster                                                         |
| xml_etree_parse            | 164 ms                                                 | 147 ms: 1.12x faster                                                         |
| sympy_sum                  | 169 ms                                                 | 152 ms: 1.11x faster                                                         |
| async_tree_io              | 1.29 sec                                               | 1.16 sec: 1.11x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 566 ms: 1.11x faster                                                         |
| deepcopy_memo              | 40.2 us                                                | 36.3 us: 1.10x faster                                                        |
| hexiom                     | 6.89 ms                                                | 6.26 ms: 1.10x faster                                                        |
| async_tree_memoization     | 639 ms                                                 | 581 ms: 1.10x faster                                                         |
| sqlglot_parse              | 1.43 ms                                                | 1.30 ms: 1.10x faster                                                        |
| mdp                        | 2.77 sec                                               | 2.54 sec: 1.09x faster                                                       |
| unpickle_pure_python       | 242 us                                                 | 223 us: 1.09x faster                                                         |
| meteor_contest             | 109 ms                                                 | 101 ms: 1.08x faster                                                         |
| mako                       | 10.7 ms                                                | 9.85 ms: 1.08x faster                                                        |
| logging_silent             | 111 ns                                                 | 103 ns: 1.08x faster                                                         |
| sympy_str                  | 297 ms                                                 | 276 ms: 1.08x faster                                                         |
| xml_etree_iterparse        | 108 ms                                                 | 100 ms: 1.08x faster                                                         |
| raytrace                   | 309 ms                                                 | 287 ms: 1.08x faster                                                         |
| deepcopy                   | 365 us                                                 | 340 us: 1.07x faster                                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 698 ms: 1.07x faster                                                         |
| regex_dna                  | 205 ms                                                 | 191 ms: 1.07x faster                                                         |
| coroutines                 | 27.0 ms                                                | 25.4 ms: 1.06x faster                                                        |
| sqlglot_transpile          | 1.75 ms                                                | 1.65 ms: 1.06x faster                                                        |
| richards                   | 49.8 ms                                                | 46.8 ms: 1.06x faster                                                        |
| pickle_pure_python         | 320 us                                                 | 304 us: 1.05x faster                                                         |
| deltablue                  | 3.92 ms                                                | 3.75 ms: 1.05x faster                                                        |
| regex_compile              | 141 ms                                                 | 136 ms: 1.04x faster                                                         |
| regex_effbot               | 3.51 ms                                                | 3.37 ms: 1.04x faster                                                        |
| sympy_expand               | 484 ms                                                 | 469 ms: 1.03x faster                                                         |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                         |
| sqlglot_normalize          | 113 ms                                                 | 109 ms: 1.03x faster                                                         |
| deepcopy_reduce            | 3.22 us                                                | 3.13 us: 1.03x faster                                                        |
| logging_format             | 6.81 us                                                | 6.64 us: 1.03x faster                                                        |
| sympy_integrate            | 21.5 ms                                                | 21.0 ms: 1.02x faster                                                        |
| unpickle                   | 13.8 us                                                | 13.5 us: 1.02x faster                                                        |
| logging_simple             | 6.22 us                                                | 6.09 us: 1.02x faster                                                        |
| nqueens                    | 87.9 ms                                                | 86.3 ms: 1.02x faster                                                        |
| thrift                     | 784 us                                                 | 774 us: 1.01x faster                                                         |
| float                      | 78.9 ms                                                | 78.5 ms: 1.01x faster                                                        |
| genshi_xml                 | 53.4 ms                                                | 54.2 ms: 1.01x slower                                                        |
| scimark_lu                 | 116 ms                                                 | 118 ms: 1.02x slower                                                         |
| sqlglot_optimize           | 55.3 ms                                                | 56.9 ms: 1.03x slower                                                        |
| django_template            | 33.5 ms                                                | 34.6 ms: 1.03x slower                                                        |
| regex_v8                   | 22.9 ms                                                | 23.8 ms: 1.04x slower                                                        |
| sqlite_synth               | 2.57 us                                                | 2.69 us: 1.04x slower                                                        |
| xml_etree_generate         | 81.1 ms                                                | 85.3 ms: 1.05x slower                                                        |
| xml_etree_process          | 56.9 ms                                                | 59.9 ms: 1.05x slower                                                        |
| go                         | 149 ms                                                 | 159 ms: 1.07x slower                                                         |
| nbody                      | 96.0 ms                                                | 103 ms: 1.07x slower                                                         |
| chameleon                  | 6.70 ms                                                | 7.25 ms: 1.08x slower                                                        |
| async_generators           | 374 ms                                                 | 405 ms: 1.08x slower                                                         |
| genshi_text                | 22.5 ms                                                | 24.7 ms: 1.10x slower                                                        |
| pycparser                  | 1.19 sec                                               | 1.31 sec: 1.11x slower                                                       |
| html5lib                   | 64.8 ms                                                | 71.7 ms: 1.11x slower                                                        |
| telco                      | 6.86 ms                                                | 7.63 ms: 1.11x slower                                                        |
| 2to3                       | 264 ms                                                 | 297 ms: 1.12x slower                                                         |
| pyflate                    | 434 ms                                                 | 489 ms: 1.13x slower                                                         |
| scimark_sor                | 121 ms                                                 | 146 ms: 1.20x slower                                                         |
| dulwich_log                | 64.6 ms                                                | 78.2 ms: 1.21x slower                                                        |
| pathlib                    | 18.5 ms                                                | 24.2 ms: 1.31x slower                                                        |
| asyncio_websockets         | 550 ms                                                 | 721 ms: 1.31x slower                                                         |
| dask                       | 365 ms                                                 | 483 ms: 1.32x slower                                                         |
| mypy2                      | 686 ms                                                 | 928 ms: 1.35x slower                                                         |
| tornado_http               | 98.1 ms                                                | 147 ms: 1.50x slower                                                         |
| bench_thread_pool          | 834 us                                                 | 1.51 ms: 1.81x slower                                                        |
| python_startup             | 8.56 ms                                                | 19.2 ms: 2.24x slower                                                        |
| unpack_sequence            | 43.5 ns                                                | 110 ns: 2.54x slower                                                         |
| python_startup_no_site     | 6.01 ms                                                | 17.8 ms: 2.96x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                                 |

Benchmark hidden because not significant (5): scimark_monte_carlo, pprint_pformat, coverage, docutils, pprint_safe_repr
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.80% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.23x