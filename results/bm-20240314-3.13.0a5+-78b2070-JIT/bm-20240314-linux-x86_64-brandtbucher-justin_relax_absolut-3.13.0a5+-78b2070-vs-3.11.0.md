# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_relax_absolut
- machine: linux-x86_64
- commit hash: 78b2070
- commit date: 2024-03-14
- overall geometric mean: 1.02x faster
- HPT reliability: 55.11%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 284 ms: 1.07x slower                                                         |
| chameleon      | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                        |
| docutils       | 2.66 sec                                               | 2.78 sec: 1.04x slower                                                       |
| html5lib       | 64.8 ms                                                | 68.2 ms: 1.05x slower                                                        |
| tornado_http   | 98.1 ms                                                | 99.1 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                         |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                         |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 595 ms: 1.05x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.23 sec: 1.05x faster                                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 728 ms: 1.03x faster                                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 744 ms: 1.02x faster                                                         |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 92.6 ms: 1.04x faster                                                        |
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                                         |
| float          | 78.9 ms                                                | 81.3 ms: 1.03x slower                                                        |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 144 ms: 1.02x slower                                                         |
| regex_effbot   | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                        |
| regex_v8       | 22.9 ms                                                | 24.0 ms: 1.05x slower                                                        |
| regex_dna      | 205 ms                                                 | 225 ms: 1.10x slower                                                         |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                        |
| tomli_loads          | 2.30 sec                                               | 2.05 sec: 1.12x faster                                                       |
| unpickle_list        | 5.21 us                                                | 4.81 us: 1.08x faster                                                        |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                                         |
| json_loads           | 29.2 us                                                | 28.4 us: 1.03x faster                                                        |
| xml_etree_parse      | 164 ms                                                 | 161 ms: 1.02x faster                                                         |
| pickle_dict          | 34.6 us                                                | 34.9 us: 1.01x slower                                                        |
| xml_etree_iterparse  | 108 ms                                                 | 109 ms: 1.01x slower                                                         |
| unpickle_pure_python | 242 us                                                 | 245 us: 1.01x slower                                                         |
| pickle_list          | 4.59 us                                                | 4.81 us: 1.05x slower                                                        |
| xml_etree_process    | 56.9 ms                                                | 60.6 ms: 1.06x slower                                                        |
| pickle               | 11.0 us                                                | 11.8 us: 1.07x slower                                                        |
| xml_etree_generate   | 81.1 ms                                                | 88.1 ms: 1.09x slower                                                        |
| unpickle             | 13.8 us                                                | 15.7 us: 1.13x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.6 ms: 1.48x slower                                                        |
| python_startup_no_site | 6.01 ms                                                | 11.2 ms: 1.86x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.66x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 54.3 ms: 1.02x slower                                                        |
| django_template | 33.5 ms                                                | 34.2 ms: 1.02x slower                                                        |
| mako            | 10.7 ms                                                | 10.9 ms: 1.03x slower                                                        |
| genshi_text     | 22.5 ms                                                | 24.1 ms: 1.07x slower                                                        |
| Geometric mean  | (ref)                                                  | 1.03x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-brandtbucher-justin_relax_absolut-3.13.0a5+-78b2070 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 112 us: 4.64x faster                                                         |
| generators                 | 74.9 ms                                                | 29.7 ms: 2.52x faster                                                        |
| asyncio_tcp                | 875 ms                                                 | 495 ms: 1.77x faster                                                         |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.85 sec: 1.68x faster                                                       |
| pylint                     | 476 ms                                                 | 324 ms: 1.47x faster                                                         |
| comprehensions             | 23.6 us                                                | 17.9 us: 1.32x faster                                                        |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                        |
| coroutines                 | 27.0 ms                                                | 22.8 ms: 1.19x faster                                                        |
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                         |
| richards_super             | 61.9 ms                                                | 53.5 ms: 1.16x faster                                                        |
| deltablue                  | 3.92 ms                                                | 3.48 ms: 1.13x faster                                                        |
| tomli_loads                | 2.30 sec                                               | 2.05 sec: 1.12x faster                                                       |
| logging_silent             | 111 ns                                                 | 100 ns: 1.11x faster                                                         |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                                         |
| chaos                      | 71.9 ms                                                | 65.3 ms: 1.10x faster                                                        |
| sqlglot_parse              | 1.43 ms                                                | 1.31 ms: 1.09x faster                                                        |
| unpickle_list              | 5.21 us                                                | 4.81 us: 1.08x faster                                                        |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                         |
| logging_simple             | 6.22 us                                                | 5.83 us: 1.07x faster                                                        |
| djangocms                  | 33.5 us                                                | 31.4 us: 1.07x faster                                                        |
| logging_format             | 6.81 us                                                | 6.40 us: 1.06x faster                                                        |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                                         |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                       |
| sqlglot_transpile          | 1.75 ms                                                | 1.65 ms: 1.06x faster                                                        |
| deepcopy_reduce            | 3.22 us                                                | 3.04 us: 1.06x faster                                                        |
| async_tree_memoization_tg  | 626 ms                                                 | 595 ms: 1.05x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.23 sec: 1.05x faster                                                       |
| gc_traversal               | 4.01 ms                                                | 3.81 ms: 1.05x faster                                                        |
| mdp                        | 2.77 sec                                               | 2.65 sec: 1.05x faster                                                       |
| richards                   | 49.8 ms                                                | 47.7 ms: 1.04x faster                                                        |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                                         |
| sqlglot_normalize          | 113 ms                                                 | 109 ms: 1.04x faster                                                         |
| sympy_str                  | 297 ms                                                 | 287 ms: 1.04x faster                                                         |
| nbody                      | 96.0 ms                                                | 92.6 ms: 1.04x faster                                                        |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 728 ms: 1.03x faster                                                         |
| deepcopy                   | 365 us                                                 | 355 us: 1.03x faster                                                         |
| json_loads                 | 29.2 us                                                | 28.4 us: 1.03x faster                                                        |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.89 ms: 1.03x faster                                                        |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 744 ms: 1.02x faster                                                         |
| raytrace                   | 309 ms                                                 | 302 ms: 1.02x faster                                                         |
| xml_etree_parse            | 164 ms                                                 | 161 ms: 1.02x faster                                                         |
| pidigits                   | 194 ms                                                 | 190 ms: 1.02x faster                                                         |
| deepcopy_memo              | 40.2 us                                                | 39.4 us: 1.02x faster                                                        |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                                        |
| sympy_expand               | 484 ms                                                 | 487 ms: 1.00x slower                                                         |
| pprint_safe_repr           | 747 ms                                                 | 751 ms: 1.01x slower                                                         |
| crypto_pyaes               | 76.7 ms                                                | 77.3 ms: 1.01x slower                                                        |
| pickle_dict                | 34.6 us                                                | 34.9 us: 1.01x slower                                                        |
| xml_etree_iterparse        | 108 ms                                                 | 109 ms: 1.01x slower                                                         |
| tornado_http               | 98.1 ms                                                | 99.1 ms: 1.01x slower                                                        |
| unpickle_pure_python       | 242 us                                                 | 245 us: 1.01x slower                                                         |
| genshi_xml                 | 53.4 ms                                                | 54.3 ms: 1.02x slower                                                        |
| django_template            | 33.5 ms                                                | 34.2 ms: 1.02x slower                                                        |
| meteor_contest             | 109 ms                                                 | 111 ms: 1.02x slower                                                         |
| regex_compile              | 141 ms                                                 | 144 ms: 1.02x slower                                                         |
| dask                       | 365 ms                                                 | 373 ms: 1.02x slower                                                         |
| asyncio_websockets         | 550 ms                                                 | 562 ms: 1.02x slower                                                         |
| thrift                     | 784 us                                                 | 804 us: 1.03x slower                                                         |
| mako                       | 10.7 ms                                                | 10.9 ms: 1.03x slower                                                        |
| sqlglot_optimize           | 55.3 ms                                                | 56.8 ms: 1.03x slower                                                        |
| float                      | 78.9 ms                                                | 81.3 ms: 1.03x slower                                                        |
| bench_thread_pool          | 834 us                                                 | 860 us: 1.03x slower                                                         |
| pycparser                  | 1.19 sec                                               | 1.22 sec: 1.03x slower                                                       |
| nqueens                    | 87.9 ms                                                | 90.8 ms: 1.03x slower                                                        |
| scimark_monte_carlo        | 70.7 ms                                                | 73.1 ms: 1.03x slower                                                        |
| chameleon                  | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                        |
| regex_effbot               | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                        |
| docutils                   | 2.66 sec                                               | 2.78 sec: 1.04x slower                                                       |
| pickle_list                | 4.59 us                                                | 4.81 us: 1.05x slower                                                        |
| regex_v8                   | 22.9 ms                                                | 24.0 ms: 1.05x slower                                                        |
| html5lib                   | 64.8 ms                                                | 68.2 ms: 1.05x slower                                                        |
| hexiom                     | 6.89 ms                                                | 7.29 ms: 1.06x slower                                                        |
| xml_etree_process          | 56.9 ms                                                | 60.6 ms: 1.06x slower                                                        |
| go                         | 149 ms                                                 | 158 ms: 1.07x slower                                                         |
| genshi_text                | 22.5 ms                                                | 24.1 ms: 1.07x slower                                                        |
| pickle                     | 11.0 us                                                | 11.8 us: 1.07x slower                                                        |
| 2to3                       | 264 ms                                                 | 284 ms: 1.07x slower                                                         |
| scimark_sor                | 121 ms                                                 | 131 ms: 1.08x slower                                                         |
| aiohttp                    | 1.12 ms                                                | 1.20 ms: 1.08x slower                                                        |
| create_gc_cycles           | 1.43 ms                                                | 1.55 ms: 1.08x slower                                                        |
| gunicorn                   | 1.20 ms                                                | 1.30 ms: 1.08x slower                                                        |
| dulwich_log                | 64.6 ms                                                | 69.9 ms: 1.08x slower                                                        |
| xml_etree_generate         | 81.1 ms                                                | 88.1 ms: 1.09x slower                                                        |
| spectral_norm              | 108 ms                                                 | 118 ms: 1.09x slower                                                         |
| regex_dna                  | 205 ms                                                 | 225 ms: 1.10x slower                                                         |
| bench_mp_pool              | 24.0 ms                                                | 26.4 ms: 1.10x slower                                                        |
| sqlite_synth               | 2.57 us                                                | 2.84 us: 1.10x slower                                                        |
| unpickle                   | 13.8 us                                                | 15.7 us: 1.13x slower                                                        |
| scimark_lu                 | 116 ms                                                 | 134 ms: 1.15x slower                                                         |
| pyflate                    | 434 ms                                                 | 503 ms: 1.16x slower                                                         |
| telco                      | 6.86 ms                                                | 8.48 ms: 1.24x slower                                                        |
| coverage                   | 78.8 ms                                                | 97.4 ms: 1.24x slower                                                        |
| async_generators           | 374 ms                                                 | 471 ms: 1.26x slower                                                         |
| mypy2                      | 686 ms                                                 | 902 ms: 1.32x slower                                                         |
| python_startup             | 8.56 ms                                                | 12.6 ms: 1.48x slower                                                        |
| python_startup_no_site     | 6.01 ms                                                | 11.2 ms: 1.86x slower                                                        |
| unpack_sequence            | 43.5 ns                                                | 87.8 ns: 2.02x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                                 |

Benchmark hidden because not significant (5): json, fannkuch, pathlib, scimark_fft, pprint_pformat
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 55.11% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x