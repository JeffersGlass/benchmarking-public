# Results vs. 3.11.0

- fork: jeffersglass
- ref: justin_supernodes_on
- machine: linux-x86_64
- commit hash: f486338
- commit date: 2024-03-16
- overall geometric mean: 1.04x faster
- HPT reliability: 99.74%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.23x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 299 ms: 1.13x slower                                                         |
| chameleon      | 6.70 ms                                                | 7.13 ms: 1.06x slower                                                        |
| docutils       | 2.66 sec                                               | 2.64 sec: 1.01x faster                                                       |
| html5lib       | 64.8 ms                                                | 70.4 ms: 1.09x slower                                                        |
| tornado_http   | 98.1 ms                                                | 144 ms: 1.47x slower                                                         |
| Geometric mean | (ref)                                                  | 1.14x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.29 sec                                               | 1.13 sec: 1.15x faster                                                       |
| async_tree_none            | 528 ms                                                 | 467 ms: 1.13x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 445 ms: 1.10x faster                                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 699 ms: 1.09x faster                                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 584 ms: 1.07x faster                                                         |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                       |
| async_tree_memoization     | 639 ms                                                 | 610 ms: 1.05x faster                                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.03x faster                                                         |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 186 ms: 1.04x faster                                                         |
| nbody          | 96.0 ms                                                | 103 ms: 1.07x slower                                                         |
| Geometric mean | (ref)                                                  | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 133 ms: 1.06x faster                                                         |
| regex_dna      | 205 ms                                                 | 197 ms: 1.04x faster                                                         |
| regex_effbot   | 3.51 ms                                                | 3.42 ms: 1.02x faster                                                        |
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.08x slower                                                        |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.63 ms: 1.39x faster                                                        |
| pickle_dict          | 34.6 us                                                | 27.5 us: 1.26x faster                                                        |
| pickle_list          | 4.59 us                                                | 3.76 us: 1.22x faster                                                        |
| json_loads           | 29.2 us                                                | 24.1 us: 1.21x faster                                                        |
| tomli_loads          | 2.30 sec                                               | 1.93 sec: 1.19x faster                                                       |
| unpickle_list        | 5.21 us                                                | 4.49 us: 1.16x faster                                                        |
| pickle               | 11.0 us                                                | 9.69 us: 1.13x faster                                                        |
| xml_etree_iterparse  | 108 ms                                                 | 97.9 ms: 1.10x faster                                                        |
| unpickle_pure_python | 242 us                                                 | 223 us: 1.08x faster                                                         |
| xml_etree_parse      | 164 ms                                                 | 152 ms: 1.08x faster                                                         |
| unpickle             | 13.8 us                                                | 13.3 us: 1.04x faster                                                        |
| pickle_pure_python   | 320 us                                                 | 312 us: 1.03x faster                                                         |
| xml_etree_process    | 56.9 ms                                                | 58.6 ms: 1.03x slower                                                        |
| xml_etree_generate   | 81.1 ms                                                | 84.1 ms: 1.04x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 18.3 ms: 2.14x slower                                                        |
| python_startup_no_site | 6.01 ms                                                | 16.8 ms: 2.80x slower                                                        |
| Geometric mean         | (ref)                                                  | 2.45x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.84 ms: 1.08x faster                                                        |
| genshi_xml      | 53.4 ms                                                | 54.3 ms: 1.02x slower                                                        |
| django_template | 33.5 ms                                                | 34.5 ms: 1.03x slower                                                        |
| genshi_text     | 22.5 ms                                                | 25.0 ms: 1.11x slower                                                        |
| Geometric mean  | (ref)                                                  | 1.02x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240316-linux-x86_64-jeffersglass-justin_supernodes_on-3.13.0a5+-f486338 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 106 us: 4.90x faster                                                         |
| generators                 | 74.9 ms                                                | 31.6 ms: 2.37x faster                                                        |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.74 sec: 1.79x faster                                                       |
| bench_mp_pool              | 24.0 ms                                                | 15.6 ms: 1.54x faster                                                        |
| pylint                     | 476 ms                                                 | 309 ms: 1.54x faster                                                         |
| asyncio_tcp                | 875 ms                                                 | 584 ms: 1.50x faster                                                         |
| comprehensions             | 23.6 us                                                | 16.5 us: 1.43x faster                                                        |
| json_dumps                 | 13.3 ms                                                | 9.63 ms: 1.39x faster                                                        |
| create_gc_cycles           | 1.43 ms                                                | 1.10 ms: 1.30x faster                                                        |
| pickle_dict                | 34.6 us                                                | 27.5 us: 1.26x faster                                                        |
| pickle_list                | 4.59 us                                                | 3.76 us: 1.22x faster                                                        |
| json_loads                 | 29.2 us                                                | 24.1 us: 1.21x faster                                                        |
| tomli_loads                | 2.30 sec                                               | 1.93 sec: 1.19x faster                                                       |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.21 ms: 1.19x faster                                                        |
| spectral_norm              | 108 ms                                                 | 91.5 ms: 1.18x faster                                                        |
| richards_super             | 61.9 ms                                                | 52.7 ms: 1.17x faster                                                        |
| chaos                      | 71.9 ms                                                | 61.3 ms: 1.17x faster                                                        |
| crypto_pyaes               | 76.7 ms                                                | 65.4 ms: 1.17x faster                                                        |
| unpickle_list              | 5.21 us                                                | 4.49 us: 1.16x faster                                                        |
| fannkuch                   | 405 ms                                                 | 349 ms: 1.16x faster                                                         |
| mdp                        | 2.77 sec                                               | 2.39 sec: 1.16x faster                                                       |
| async_tree_io_tg           | 1.29 sec                                               | 1.13 sec: 1.15x faster                                                       |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                         |
| json                       | 5.24 ms                                                | 4.60 ms: 1.14x faster                                                        |
| scimark_fft                | 345 ms                                                 | 304 ms: 1.14x faster                                                         |
| pickle                     | 11.0 us                                                | 9.69 us: 1.13x faster                                                        |
| async_tree_none            | 528 ms                                                 | 467 ms: 1.13x faster                                                         |
| sympy_str                  | 297 ms                                                 | 269 ms: 1.11x faster                                                         |
| sqlglot_parse              | 1.43 ms                                                | 1.30 ms: 1.10x faster                                                        |
| hexiom                     | 6.89 ms                                                | 6.24 ms: 1.10x faster                                                        |
| xml_etree_iterparse        | 108 ms                                                 | 97.9 ms: 1.10x faster                                                        |
| raytrace                   | 309 ms                                                 | 280 ms: 1.10x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 445 ms: 1.10x faster                                                         |
| deepcopy_memo              | 40.2 us                                                | 36.6 us: 1.10x faster                                                        |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                                         |
| richards                   | 49.8 ms                                                | 45.6 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 699 ms: 1.09x faster                                                         |
| gc_traversal               | 4.01 ms                                                | 3.68 ms: 1.09x faster                                                        |
| mako                       | 10.7 ms                                                | 9.84 ms: 1.08x faster                                                        |
| unpickle_pure_python       | 242 us                                                 | 223 us: 1.08x faster                                                         |
| meteor_contest             | 109 ms                                                 | 101 ms: 1.08x faster                                                         |
| sqlglot_transpile          | 1.75 ms                                                | 1.62 ms: 1.08x faster                                                        |
| xml_etree_parse            | 164 ms                                                 | 152 ms: 1.08x faster                                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 584 ms: 1.07x faster                                                         |
| deepcopy                   | 365 us                                                 | 343 us: 1.07x faster                                                         |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                       |
| regex_compile              | 141 ms                                                 | 133 ms: 1.06x faster                                                         |
| sympy_expand               | 484 ms                                                 | 457 ms: 1.06x faster                                                         |
| deltablue                  | 3.92 ms                                                | 3.71 ms: 1.06x faster                                                        |
| async_tree_memoization     | 639 ms                                                 | 610 ms: 1.05x faster                                                         |
| sympy_integrate            | 21.5 ms                                                | 20.6 ms: 1.04x faster                                                        |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.04x faster                                                         |
| unpickle                   | 13.8 us                                                | 13.3 us: 1.04x faster                                                        |
| pidigits                   | 194 ms                                                 | 186 ms: 1.04x faster                                                         |
| regex_dna                  | 205 ms                                                 | 197 ms: 1.04x faster                                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.03x faster                                                         |
| coroutines                 | 27.0 ms                                                | 26.2 ms: 1.03x faster                                                        |
| scimark_monte_carlo        | 70.7 ms                                                | 68.5 ms: 1.03x faster                                                        |
| logging_simple             | 6.22 us                                                | 6.03 us: 1.03x faster                                                        |
| logging_format             | 6.81 us                                                | 6.62 us: 1.03x faster                                                        |
| pickle_pure_python         | 320 us                                                 | 312 us: 1.03x faster                                                         |
| regex_effbot               | 3.51 ms                                                | 3.42 ms: 1.02x faster                                                        |
| deepcopy_reduce            | 3.22 us                                                | 3.14 us: 1.02x faster                                                        |
| thrift                     | 784 us                                                 | 771 us: 1.02x faster                                                         |
| docutils                   | 2.66 sec                                               | 2.64 sec: 1.01x faster                                                       |
| pprint_pformat             | 1.55 sec                                               | 1.55 sec: 1.01x faster                                                       |
| sqlglot_optimize           | 55.3 ms                                                | 55.8 ms: 1.01x slower                                                        |
| genshi_xml                 | 53.4 ms                                                | 54.3 ms: 1.02x slower                                                        |
| scimark_lu                 | 116 ms                                                 | 119 ms: 1.02x slower                                                         |
| django_template            | 33.5 ms                                                | 34.5 ms: 1.03x slower                                                        |
| xml_etree_process          | 56.9 ms                                                | 58.6 ms: 1.03x slower                                                        |
| coverage                   | 78.8 ms                                                | 81.5 ms: 1.03x slower                                                        |
| pyflate                    | 434 ms                                                 | 449 ms: 1.04x slower                                                         |
| sqlite_synth               | 2.57 us                                                | 2.66 us: 1.04x slower                                                        |
| xml_etree_generate         | 81.1 ms                                                | 84.1 ms: 1.04x slower                                                        |
| pycparser                  | 1.19 sec                                               | 1.26 sec: 1.06x slower                                                       |
| chameleon                  | 6.70 ms                                                | 7.13 ms: 1.06x slower                                                        |
| go                         | 149 ms                                                 | 159 ms: 1.07x slower                                                         |
| nbody                      | 96.0 ms                                                | 103 ms: 1.07x slower                                                         |
| async_generators           | 374 ms                                                 | 400 ms: 1.07x slower                                                         |
| regex_v8                   | 22.9 ms                                                | 24.6 ms: 1.08x slower                                                        |
| html5lib                   | 64.8 ms                                                | 70.4 ms: 1.09x slower                                                        |
| genshi_text                | 22.5 ms                                                | 25.0 ms: 1.11x slower                                                        |
| telco                      | 6.86 ms                                                | 7.66 ms: 1.12x slower                                                        |
| 2to3                       | 264 ms                                                 | 299 ms: 1.13x slower                                                         |
| dulwich_log                | 64.6 ms                                                | 78.0 ms: 1.21x slower                                                        |
| scimark_sor                | 121 ms                                                 | 148 ms: 1.22x slower                                                         |
| mypy2                      | 686 ms                                                 | 861 ms: 1.26x slower                                                         |
| pathlib                    | 18.5 ms                                                | 23.9 ms: 1.29x slower                                                        |
| dask                       | 365 ms                                                 | 472 ms: 1.29x slower                                                         |
| asyncio_websockets         | 550 ms                                                 | 721 ms: 1.31x slower                                                         |
| tornado_http               | 98.1 ms                                                | 144 ms: 1.47x slower                                                         |
| bench_thread_pool          | 834 us                                                 | 1.49 ms: 1.79x slower                                                        |
| python_startup             | 8.56 ms                                                | 18.3 ms: 2.14x slower                                                        |
| unpack_sequence            | 43.5 ns                                                | 104 ns: 2.40x slower                                                         |
| python_startup_no_site     | 6.01 ms                                                | 16.8 ms: 2.80x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                                 |

Benchmark hidden because not significant (3): nqueens, pprint_safe_repr, float
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, djangocms, flaskblogging, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.74% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.23x