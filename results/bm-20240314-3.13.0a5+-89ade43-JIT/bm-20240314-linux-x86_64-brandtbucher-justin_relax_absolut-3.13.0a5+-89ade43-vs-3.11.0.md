# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_relax_absolut
- machine: linux-x86_64
- commit hash: 89ade43
- commit date: 2024-03-14
- overall geometric mean: 1.02x faster
- HPT reliability: 62.63%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.13x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 282 ms: 1.07x slower                                                         |
| chameleon      | 6.70 ms                                                | 6.89 ms: 1.03x slower                                                        |
| docutils       | 2.66 sec                                               | 2.79 sec: 1.05x slower                                                       |
| html5lib       | 64.8 ms                                                | 68.3 ms: 1.05x slower                                                        |
| tornado_http   | 98.1 ms                                                | 98.8 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 452 ms: 1.17x faster                                                         |
| async_tree_memoization     | 639 ms                                                 | 581 ms: 1.10x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 461 ms: 1.06x faster                                                         |
| async_tree_io              | 1.29 sec                                               | 1.22 sec: 1.05x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 600 ms: 1.04x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.25 sec: 1.04x faster                                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 728 ms: 1.03x faster                                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 744 ms: 1.02x faster                                                         |
| Geometric mean             | (ref)                                                  | 1.06x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 92.3 ms: 1.04x faster                                                        |
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                         |
| float          | 78.9 ms                                                | 82.7 ms: 1.05x slower                                                        |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 144 ms: 1.02x slower                                                         |
| regex_effbot   | 3.51 ms                                                | 3.74 ms: 1.07x slower                                                        |
| regex_dna      | 205 ms                                                 | 227 ms: 1.11x slower                                                         |
| regex_v8       | 22.9 ms                                                | 25.9 ms: 1.13x slower                                                        |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                        |
| tomli_loads          | 2.30 sec                                               | 2.07 sec: 1.11x faster                                                       |
| unpickle_list        | 5.21 us                                                | 4.83 us: 1.08x faster                                                        |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                                         |
| json_loads           | 29.2 us                                                | 28.4 us: 1.03x faster                                                        |
| xml_etree_parse      | 164 ms                                                 | 162 ms: 1.02x faster                                                         |
| xml_etree_iterparse  | 108 ms                                                 | 109 ms: 1.01x slower                                                         |
| unpickle_pure_python | 242 us                                                 | 244 us: 1.01x slower                                                         |
| pickle_dict          | 34.6 us                                                | 34.9 us: 1.01x slower                                                        |
| pickle               | 11.0 us                                                | 11.6 us: 1.05x slower                                                        |
| xml_etree_process    | 56.9 ms                                                | 60.2 ms: 1.06x slower                                                        |
| xml_etree_generate   | 81.1 ms                                                | 88.3 ms: 1.09x slower                                                        |
| pickle_list          | 4.59 us                                                | 5.08 us: 1.11x slower                                                        |
| unpickle             | 13.8 us                                                | 15.5 us: 1.12x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 11.5 ms: 1.34x slower                                                        |
| python_startup_no_site | 6.01 ms                                                | 10.1 ms: 1.68x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.50x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 10.7 ms                                                | 10.8 ms: 1.02x slower                                                        |
| django_template | 33.5 ms                                                | 34.3 ms: 1.02x slower                                                        |
| genshi_xml      | 53.4 ms                                                | 54.7 ms: 1.02x slower                                                        |
| genshi_text     | 22.5 ms                                                | 24.5 ms: 1.09x slower                                                        |
| Geometric mean  | (ref)                                                  | 1.04x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-89ade43 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.72x faster                                                         |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                                        |
| asyncio_tcp                | 875 ms                                                 | 505 ms: 1.73x faster                                                         |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.85 sec: 1.68x faster                                                       |
| pylint                     | 476 ms                                                 | 323 ms: 1.47x faster                                                         |
| comprehensions             | 23.6 us                                                | 17.9 us: 1.32x faster                                                        |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                        |
| richards_super             | 61.9 ms                                                | 52.5 ms: 1.18x faster                                                        |
| coroutines                 | 27.0 ms                                                | 23.0 ms: 1.18x faster                                                        |
| async_tree_none            | 528 ms                                                 | 452 ms: 1.17x faster                                                         |
| deltablue                  | 3.92 ms                                                | 3.49 ms: 1.12x faster                                                        |
| tomli_loads                | 2.30 sec                                               | 2.07 sec: 1.11x faster                                                       |
| async_tree_memoization     | 639 ms                                                 | 581 ms: 1.10x faster                                                         |
| logging_silent             | 111 ns                                                 | 101 ns: 1.10x faster                                                         |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                        |
| unpickle_list              | 5.21 us                                                | 4.83 us: 1.08x faster                                                        |
| chaos                      | 71.9 ms                                                | 66.8 ms: 1.08x faster                                                        |
| logging_simple             | 6.22 us                                                | 5.82 us: 1.07x faster                                                        |
| richards                   | 49.8 ms                                                | 46.7 ms: 1.07x faster                                                        |
| async_tree_none_tg         | 491 ms                                                 | 461 ms: 1.06x faster                                                         |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                                         |
| logging_format             | 6.81 us                                                | 6.43 us: 1.06x faster                                                        |
| async_tree_io              | 1.29 sec                                               | 1.22 sec: 1.05x faster                                                       |
| mdp                        | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                       |
| sqlglot_transpile          | 1.75 ms                                                | 1.67 ms: 1.05x faster                                                        |
| djangocms                  | 33.5 us                                                | 32.0 us: 1.05x faster                                                        |
| async_tree_memoization_tg  | 626 ms                                                 | 600 ms: 1.04x faster                                                         |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                                         |
| nbody                      | 96.0 ms                                                | 92.3 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 1.29 sec                                               | 1.25 sec: 1.04x faster                                                       |
| sqlglot_normalize          | 113 ms                                                 | 109 ms: 1.04x faster                                                         |
| deepcopy                   | 365 us                                                 | 353 us: 1.03x faster                                                         |
| sympy_str                  | 297 ms                                                 | 288 ms: 1.03x faster                                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 728 ms: 1.03x faster                                                         |
| deepcopy_reduce            | 3.22 us                                                | 3.13 us: 1.03x faster                                                        |
| json_loads                 | 29.2 us                                                | 28.4 us: 1.03x faster                                                        |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 744 ms: 1.02x faster                                                         |
| fannkuch                   | 405 ms                                                 | 397 ms: 1.02x faster                                                         |
| raytrace                   | 309 ms                                                 | 302 ms: 1.02x faster                                                         |
| gc_traversal               | 4.01 ms                                                | 3.93 ms: 1.02x faster                                                        |
| json                       | 5.24 ms                                                | 5.16 ms: 1.02x faster                                                        |
| xml_etree_parse            | 164 ms                                                 | 162 ms: 1.02x faster                                                         |
| deepcopy_memo              | 40.2 us                                                | 39.6 us: 1.01x faster                                                        |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                                        |
| sympy_expand               | 484 ms                                                 | 487 ms: 1.00x slower                                                         |
| crypto_pyaes               | 76.7 ms                                                | 77.2 ms: 1.01x slower                                                        |
| tornado_http               | 98.1 ms                                                | 98.8 ms: 1.01x slower                                                        |
| xml_etree_iterparse        | 108 ms                                                 | 109 ms: 1.01x slower                                                         |
| unpickle_pure_python       | 242 us                                                 | 244 us: 1.01x slower                                                         |
| pickle_dict                | 34.6 us                                                | 34.9 us: 1.01x slower                                                        |
| pprint_safe_repr           | 747 ms                                                 | 756 ms: 1.01x slower                                                         |
| pathlib                    | 18.5 ms                                                | 18.8 ms: 1.01x slower                                                        |
| mako                       | 10.7 ms                                                | 10.8 ms: 1.02x slower                                                        |
| scimark_fft                | 345 ms                                                 | 351 ms: 1.02x slower                                                         |
| regex_compile              | 141 ms                                                 | 144 ms: 1.02x slower                                                         |
| thrift                     | 784 us                                                 | 799 us: 1.02x slower                                                         |
| django_template            | 33.5 ms                                                | 34.3 ms: 1.02x slower                                                        |
| asyncio_websockets         | 550 ms                                                 | 562 ms: 1.02x slower                                                         |
| genshi_xml                 | 53.4 ms                                                | 54.7 ms: 1.02x slower                                                        |
| dask                       | 365 ms                                                 | 373 ms: 1.02x slower                                                         |
| meteor_contest             | 109 ms                                                 | 112 ms: 1.03x slower                                                         |
| bench_thread_pool          | 834 us                                                 | 858 us: 1.03x slower                                                         |
| chameleon                  | 6.70 ms                                                | 6.89 ms: 1.03x slower                                                        |
| sqlglot_optimize           | 55.3 ms                                                | 57.0 ms: 1.03x slower                                                        |
| scimark_monte_carlo        | 70.7 ms                                                | 73.4 ms: 1.04x slower                                                        |
| nqueens                    | 87.9 ms                                                | 91.6 ms: 1.04x slower                                                        |
| float                      | 78.9 ms                                                | 82.7 ms: 1.05x slower                                                        |
| docutils                   | 2.66 sec                                               | 2.79 sec: 1.05x slower                                                       |
| html5lib                   | 64.8 ms                                                | 68.3 ms: 1.05x slower                                                        |
| pickle                     | 11.0 us                                                | 11.6 us: 1.05x slower                                                        |
| xml_etree_process          | 56.9 ms                                                | 60.2 ms: 1.06x slower                                                        |
| pycparser                  | 1.19 sec                                               | 1.26 sec: 1.06x slower                                                       |
| regex_effbot               | 3.51 ms                                                | 3.74 ms: 1.07x slower                                                        |
| 2to3                       | 264 ms                                                 | 282 ms: 1.07x slower                                                         |
| hexiom                     | 6.89 ms                                                | 7.37 ms: 1.07x slower                                                        |
| create_gc_cycles           | 1.43 ms                                                | 1.54 ms: 1.07x slower                                                        |
| go                         | 149 ms                                                 | 160 ms: 1.08x slower                                                         |
| scimark_sor                | 121 ms                                                 | 131 ms: 1.08x slower                                                         |
| aiohttp                    | 1.12 ms                                                | 1.20 ms: 1.08x slower                                                        |
| dulwich_log                | 64.6 ms                                                | 70.0 ms: 1.08x slower                                                        |
| gunicorn                   | 1.20 ms                                                | 1.30 ms: 1.08x slower                                                        |
| genshi_text                | 22.5 ms                                                | 24.5 ms: 1.09x slower                                                        |
| xml_etree_generate         | 81.1 ms                                                | 88.3 ms: 1.09x slower                                                        |
| sqlite_synth               | 2.57 us                                                | 2.84 us: 1.11x slower                                                        |
| pickle_list                | 4.59 us                                                | 5.08 us: 1.11x slower                                                        |
| regex_dna                  | 205 ms                                                 | 227 ms: 1.11x slower                                                         |
| spectral_norm              | 108 ms                                                 | 120 ms: 1.11x slower                                                         |
| unpickle                   | 13.8 us                                                | 15.5 us: 1.12x slower                                                        |
| regex_v8                   | 22.9 ms                                                | 25.9 ms: 1.13x slower                                                        |
| pyflate                    | 434 ms                                                 | 497 ms: 1.15x slower                                                         |
| scimark_lu                 | 116 ms                                                 | 134 ms: 1.15x slower                                                         |
| telco                      | 6.86 ms                                                | 8.39 ms: 1.22x slower                                                        |
| coverage                   | 78.8 ms                                                | 96.6 ms: 1.23x slower                                                        |
| async_generators           | 374 ms                                                 | 470 ms: 1.26x slower                                                         |
| mypy2                      | 686 ms                                                 | 903 ms: 1.32x slower                                                         |
| python_startup             | 8.56 ms                                                | 11.5 ms: 1.34x slower                                                        |
| python_startup_no_site     | 6.01 ms                                                | 10.1 ms: 1.68x slower                                                        |
| unpack_sequence            | 43.5 ns                                                | 87.5 ns: 2.01x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                                 |

Benchmark hidden because not significant (3): pprint_pformat, bench_mp_pool, scimark_sparse_mat_mult
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 62.63% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.13x