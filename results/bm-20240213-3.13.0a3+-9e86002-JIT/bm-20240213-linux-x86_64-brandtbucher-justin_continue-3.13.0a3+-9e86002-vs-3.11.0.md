
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 9e86002
- commit date: 2024-02-13
- overall geometric mean: 1.05x faster \*
- HPT reliability: 98.24%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 273 ms: 1.03x slower                                                    |
| chameleon      | 6.70 ms                                                | 6.74 ms: 1.01x slower                                                   |
| docutils       | 2.66 sec                                               | 2.62 sec: 1.02x faster                                                  |
| tornado_http   | 98.1 ms                                                | 96.7 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.00x slower                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 438 ms: 1.21x faster                                                    |
| async_tree_memoization     | 639 ms                                                 | 563 ms: 1.14x faster                                                    |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.10x faster                                                    |
| async_tree_memoization_tg  | 626 ms                                                 | 573 ms: 1.09x faster                                                    |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                                    |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 720 ms: 1.06x faster                                                    |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                    |
| nbody          | 96.0 ms                                                | 99.1 ms: 1.03x slower                                                   |
| float          | 78.9 ms                                                | 84.2 ms: 1.07x slower                                                   |
| Geometric mean | (ref)                                                  | 1.02x slower                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 136 ms: 1.04x faster                                                    |
| regex_effbot   | 3.51 ms                                                | 3.68 ms: 1.05x slower                                                   |
| regex_dna      | 205 ms                                                 | 224 ms: 1.09x slower                                                    |
| regex_v8       | 22.9 ms                                                | 25.6 ms: 1.12x slower                                                   |
| Geometric mean | (ref)                                                  | 1.05x slower                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                   |
| pickle_pure_python   | 320 us                                                 | 293 us: 1.09x faster                                                    |
| unpickle_pure_python | 242 us                                                 | 223 us: 1.08x faster                                                    |
| tomli_loads          | 2.30 sec                                               | 2.14 sec: 1.07x faster                                                  |
| json_loads           | 29.2 us                                                | 27.5 us: 1.06x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                    |
| pickle_dict          | 34.6 us                                                | 33.2 us: 1.04x faster                                                   |
| unpickle_list        | 5.21 us                                                | 5.04 us: 1.03x faster                                                   |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                    |
| xml_etree_process    | 56.9 ms                                                | 57.3 ms: 1.01x slower                                                   |
| pickle               | 11.0 us                                                | 11.4 us: 1.04x slower                                                   |
| xml_etree_generate   | 81.1 ms                                                | 84.8 ms: 1.05x slower                                                   |
| pickle_list          | 4.59 us                                                | 4.91 us: 1.07x slower                                                   |
| unpickle             | 13.8 us                                                | 15.0 us: 1.08x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                            |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                   |
| python_startup_no_site | 6.01 ms                                                | 8.83 ms: 1.47x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.0 ms: 1.12x slower                                                   |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 108 us: 4.81x faster                                                    |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                                   |
| asyncio_tcp                | 875 ms                                                 | 492 ms: 1.78x faster                                                    |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                   |
| comprehensions             | 23.6 us                                                | 18.7 us: 1.26x faster                                                   |
| richards_super             | 61.9 ms                                                | 50.6 ms: 1.22x faster                                                   |
| async_tree_none            | 528 ms                                                 | 438 ms: 1.21x faster                                                    |
| coroutines                 | 27.0 ms                                                | 22.6 ms: 1.19x faster                                                   |
| deltablue                  | 3.92 ms                                                | 3.33 ms: 1.18x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.47 ms: 1.16x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 563 ms: 1.14x faster                                                    |
| sqlglot_parse              | 1.43 ms                                                | 1.27 ms: 1.13x faster                                                   |
| raytrace                   | 309 ms                                                 | 276 ms: 1.12x faster                                                    |
| logging_silent             | 111 ns                                                 | 99.4 ns: 1.12x faster                                                   |
| richards                   | 49.8 ms                                                | 44.8 ms: 1.11x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.10x faster                                                    |
| async_tree_memoization_tg  | 626 ms                                                 | 573 ms: 1.09x faster                                                    |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.60 ms: 1.09x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 293 us: 1.09x faster                                                    |
| logging_simple             | 6.22 us                                                | 5.71 us: 1.09x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 223 us: 1.08x faster                                                    |
| mdp                        | 2.77 sec                                               | 2.57 sec: 1.08x faster                                                  |
| deepcopy_memo              | 40.2 us                                                | 37.3 us: 1.08x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 157 ms: 1.07x faster                                                    |
| logging_format             | 6.81 us                                                | 6.34 us: 1.07x faster                                                   |
| tomli_loads                | 2.30 sec                                               | 2.14 sec: 1.07x faster                                                  |
| deepcopy                   | 365 us                                                 | 340 us: 1.07x faster                                                    |
| sympy_str                  | 297 ms                                                 | 279 ms: 1.06x faster                                                    |
| deepcopy_reduce            | 3.22 us                                                | 3.03 us: 1.06x faster                                                   |
| json_loads                 | 29.2 us                                                | 27.5 us: 1.06x faster                                                   |
| chaos                      | 71.9 ms                                                | 67.8 ms: 1.06x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                                    |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 720 ms: 1.06x faster                                                    |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                    |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.05x faster                                                    |
| pickle_dict                | 34.6 us                                                | 33.2 us: 1.04x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 20.7 ms: 1.04x faster                                                   |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                    |
| regex_compile              | 141 ms                                                 | 136 ms: 1.04x faster                                                    |
| unpickle_list              | 5.21 us                                                | 5.04 us: 1.03x faster                                                   |
| scimark_lu                 | 116 ms                                                 | 113 ms: 1.03x faster                                                    |
| sympy_expand               | 484 ms                                                 | 471 ms: 1.03x faster                                                    |
| json                       | 5.24 ms                                                | 5.10 ms: 1.03x faster                                                   |
| go                         | 149 ms                                                 | 146 ms: 1.02x faster                                                    |
| docutils                   | 2.66 sec                                               | 2.62 sec: 1.02x faster                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                    |
| tornado_http               | 98.1 ms                                                | 96.7 ms: 1.01x faster                                                   |
| dask                       | 365 ms                                                 | 361 ms: 1.01x faster                                                    |
| sqlglot_optimize           | 55.3 ms                                                | 54.8 ms: 1.01x faster                                                   |
| bench_thread_pool          | 834 us                                                 | 836 us: 1.00x slower                                                    |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                    |
| meteor_contest             | 109 ms                                                 | 110 ms: 1.01x slower                                                    |
| pprint_safe_repr           | 747 ms                                                 | 752 ms: 1.01x slower                                                    |
| chameleon                  | 6.70 ms                                                | 6.74 ms: 1.01x slower                                                   |
| xml_etree_process          | 56.9 ms                                                | 57.3 ms: 1.01x slower                                                   |
| crypto_pyaes               | 76.7 ms                                                | 77.7 ms: 1.01x slower                                                   |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 72.4 ms: 1.02x slower                                                   |
| scimark_sor                | 121 ms                                                 | 124 ms: 1.03x slower                                                    |
| nbody                      | 96.0 ms                                                | 99.1 ms: 1.03x slower                                                   |
| 2to3                       | 264 ms                                                 | 273 ms: 1.03x slower                                                    |
| fannkuch                   | 405 ms                                                 | 420 ms: 1.04x slower                                                    |
| pickle                     | 11.0 us                                                | 11.4 us: 1.04x slower                                                   |
| dulwich_log                | 64.6 ms                                                | 67.3 ms: 1.04x slower                                                   |
| xml_etree_generate         | 81.1 ms                                                | 84.8 ms: 1.05x slower                                                   |
| regex_effbot               | 3.51 ms                                                | 3.68 ms: 1.05x slower                                                   |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.34 ms: 1.06x slower                                                   |
| float                      | 78.9 ms                                                | 84.2 ms: 1.07x slower                                                   |
| pickle_list                | 4.59 us                                                | 4.91 us: 1.07x slower                                                   |
| scimark_fft                | 345 ms                                                 | 370 ms: 1.07x slower                                                    |
| sqlite_synth               | 2.57 us                                                | 2.78 us: 1.08x slower                                                   |
| unpickle                   | 13.8 us                                                | 15.0 us: 1.08x slower                                                   |
| hexiom                     | 6.89 ms                                                | 7.52 ms: 1.09x slower                                                   |
| regex_dna                  | 205 ms                                                 | 224 ms: 1.09x slower                                                    |
| regex_v8                   | 22.9 ms                                                | 25.6 ms: 1.12x slower                                                   |
| mako                       | 10.7 ms                                                | 12.0 ms: 1.12x slower                                                   |
| pyflate                    | 434 ms                                                 | 496 ms: 1.14x slower                                                    |
| unpack_sequence            | 43.5 ns                                                | 50.2 ns: 1.15x slower                                                   |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                   |
| coverage                   | 78.8 ms                                                | 94.0 ms: 1.19x slower                                                   |
| spectral_norm              | 108 ms                                                 | 131 ms: 1.21x slower                                                    |
| async_generators           | 374 ms                                                 | 461 ms: 1.23x slower                                                    |
| telco                      | 6.86 ms                                                | 8.52 ms: 1.24x slower                                                   |
| mypy2                      | 686 ms                                                 | 863 ms: 1.26x slower                                                    |
| python_startup_no_site     | 6.01 ms                                                | 8.83 ms: 1.47x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                            |

Benchmark hidden because not significant (4): pprint_pformat, nqueens, bench_mp_pool, pathlib
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 98.24% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x