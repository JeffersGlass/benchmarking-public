# Results vs. 3.11.0

- fork: python
- ref: fdb2d90a274158aee23b
- machine: linux-x86_64
- commit hash: fdb2d90
- commit date: 2024-03-08
- overall geometric mean: 1.06x slower
- HPT reliability: 99.96%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 322 ms: 1.13x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.57 ms: 1.05x faster                                                        |
| docutils       | 2.85 sec                                                     | 3.07 sec: 1.08x slower                                                       |
| html5lib       | 72.2 ms                                                      | 78.5 ms: 1.09x slower                                                        |
| tornado_http   | 124 ms                                                       | 129 ms: 1.03x slower                                                         |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 446 ms: 1.16x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 559 ms: 1.13x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 560 ms: 1.07x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 443 ms: 1.07x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 712 ms: 1.06x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.10 sec: 1.05x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 713 ms: 1.05x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 265 ms: 1.05x slower                                                         |
| float          | 74.9 ms                                                      | 105 ms: 1.40x slower                                                         |
| nbody          | 92.9 ms                                                      | 132 ms: 1.42x slower                                                         |
| Geometric mean | (ref)                                                        | 1.28x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.58 ms: 1.07x slower                                                        |
| regex_v8       | 24.4 ms                                                      | 26.4 ms: 1.08x slower                                                        |
| regex_dna      | 227 ms                                                       | 249 ms: 1.09x slower                                                         |
| regex_compile  | 156 ms                                                       | 203 ms: 1.30x slower                                                         |
| Geometric mean | (ref)                                                        | 1.13x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.5 ms: 1.26x faster                                                        |
| json_loads           | 28.9 us                                                      | 24.8 us: 1.17x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 145 ms: 1.07x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 32.8 us: 1.01x slower                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 113 ms: 1.06x slower                                                         |
| pickle               | 9.89 us                                                      | 10.8 us: 1.09x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 62.1 ms: 1.11x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.45 us: 1.13x slower                                                        |
| unpickle             | 13.3 us                                                      | 15.0 us: 1.13x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 90.6 ms: 1.14x slower                                                        |
| unpickle_pure_python | 238 us                                                       | 309 us: 1.30x slower                                                         |
| tomli_loads          | 2.25 sec                                                     | 2.99 sec: 1.33x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.05x slower                                                                 |

Benchmark hidden because not significant (2): pickle_pure_python, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.8 ms: 1.19x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.2 ms: 1.45x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.31x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|-----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| django_template | 39.3 ms                                                      | 39.6 ms: 1.01x slower                                                        |
| genshi_xml      | 57.1 ms                                                      | 62.8 ms: 1.10x slower                                                        |
| genshi_text     | 25.5 ms                                                      | 30.0 ms: 1.18x slower                                                        |
| mako            | 11.0 ms                                                      | 14.1 ms: 1.28x slower                                                        |
| Geometric mean  | (ref)                                                        | 1.14x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 123 us: 4.32x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 375 ms: 1.99x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                       |
| generators                 | 54.6 ms                                                      | 34.1 ms: 1.60x faster                                                        |
| pylint                     | 514 ms                                                       | 368 ms: 1.40x faster                                                         |
| json_dumps                 | 13.3 ms                                                      | 10.5 ms: 1.26x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.6 ms: 1.23x faster                                                        |
| json_loads                 | 28.9 us                                                      | 24.8 us: 1.17x faster                                                        |
| async_tree_none            | 518 ms                                                       | 446 ms: 1.16x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.61 ms: 1.15x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 559 ms: 1.13x faster                                                         |
| thrift                     | 931 us                                                       | 868 us: 1.07x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 560 ms: 1.07x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 443 ms: 1.07x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                                       |
| sympy_sum                  | 186 ms                                                       | 174 ms: 1.07x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 145 ms: 1.07x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 712 ms: 1.06x faster                                                         |
| logging_simple             | 7.24 us                                                      | 6.87 us: 1.05x faster                                                        |
| async_tree_io_tg           | 1.15 sec                                                     | 1.10 sec: 1.05x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 713 ms: 1.05x faster                                                         |
| chameleon                  | 7.92 ms                                                      | 7.57 ms: 1.05x faster                                                        |
| mdp                        | 2.77 sec                                                     | 2.68 sec: 1.04x faster                                                       |
| json                       | 5.58 ms                                                      | 5.41 ms: 1.03x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.51 us: 1.03x faster                                                        |
| sympy_integrate            | 25.8 ms                                                      | 25.3 ms: 1.02x faster                                                        |
| deepcopy                   | 391 us                                                       | 383 us: 1.02x faster                                                         |
| asyncio_websockets         | 390 ms                                                       | 387 ms: 1.01x faster                                                         |
| sqlglot_normalize          | 122 ms                                                       | 122 ms: 1.00x slower                                                         |
| django_template            | 39.3 ms                                                      | 39.6 ms: 1.01x slower                                                        |
| deepcopy_reduce            | 3.40 us                                                      | 3.42 us: 1.01x slower                                                        |
| logging_silent             | 100 ns                                                       | 101 ns: 1.01x slower                                                         |
| richards_super             | 63.6 ms                                                      | 64.6 ms: 1.01x slower                                                        |
| pickle_dict                | 32.3 us                                                      | 32.8 us: 1.01x slower                                                        |
| create_gc_cycles           | 1.58 ms                                                      | 1.61 ms: 1.02x slower                                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.55 ms: 1.03x slower                                                        |
| deltablue                  | 3.97 ms                                                      | 4.10 ms: 1.03x slower                                                        |
| tornado_http               | 124 ms                                                       | 129 ms: 1.03x slower                                                         |
| chaos                      | 74.9 ms                                                      | 77.6 ms: 1.03x slower                                                        |
| sympy_expand               | 553 ms                                                       | 573 ms: 1.04x slower                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.99 ms: 1.04x slower                                                        |
| pidigits                   | 251 ms                                                       | 265 ms: 1.05x slower                                                         |
| xml_etree_iterparse        | 107 ms                                                       | 113 ms: 1.06x slower                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 88.4 ms: 1.06x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 20.2 ms: 1.07x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.58 ms: 1.07x slower                                                        |
| docutils                   | 2.85 sec                                                     | 3.07 sec: 1.08x slower                                                       |
| regex_v8                   | 24.4 ms                                                      | 26.4 ms: 1.08x slower                                                        |
| html5lib                   | 72.2 ms                                                      | 78.5 ms: 1.09x slower                                                        |
| pickle                     | 9.89 us                                                      | 10.8 us: 1.09x slower                                                        |
| regex_dna                  | 227 ms                                                       | 249 ms: 1.09x slower                                                         |
| meteor_contest             | 131 ms                                                       | 143 ms: 1.10x slower                                                         |
| genshi_xml                 | 57.1 ms                                                      | 62.8 ms: 1.10x slower                                                        |
| pycparser                  | 1.31 sec                                                     | 1.45 sec: 1.11x slower                                                       |
| xml_etree_process          | 55.9 ms                                                      | 62.1 ms: 1.11x slower                                                        |
| dulwich_log                | 67.4 ms                                                      | 75.6 ms: 1.12x slower                                                        |
| gunicorn                   | 966 us                                                       | 1.09 ms: 1.12x slower                                                        |
| 2to3                       | 287 ms                                                       | 322 ms: 1.13x slower                                                         |
| deepcopy_memo              | 37.5 us                                                      | 42.3 us: 1.13x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.84 us: 1.13x slower                                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 66.5 ms: 1.13x slower                                                        |
| aiohttp                    | 986 us                                                       | 1.11 ms: 1.13x slower                                                        |
| pickle_list                | 3.94 us                                                      | 4.45 us: 1.13x slower                                                        |
| unpickle                   | 13.3 us                                                      | 15.0 us: 1.13x slower                                                        |
| nqueens                    | 103 ms                                                       | 117 ms: 1.14x slower                                                         |
| xml_etree_generate         | 79.7 ms                                                      | 90.6 ms: 1.14x slower                                                        |
| raytrace                   | 309 ms                                                       | 357 ms: 1.15x slower                                                         |
| richards                   | 49.7 ms                                                      | 58.4 ms: 1.18x slower                                                        |
| genshi_text                | 25.5 ms                                                      | 30.0 ms: 1.18x slower                                                        |
| python_startup             | 10.7 ms                                                      | 12.8 ms: 1.19x slower                                                        |
| pprint_pformat             | 1.67 sec                                                     | 2.02 sec: 1.21x slower                                                       |
| telco                      | 6.81 ms                                                      | 8.28 ms: 1.22x slower                                                        |
| async_generators           | 322 ms                                                       | 393 ms: 1.22x slower                                                         |
| pprint_safe_repr           | 805 ms                                                       | 982 ms: 1.22x slower                                                         |
| mypy2                      | 762 ms                                                       | 934 ms: 1.23x slower                                                         |
| scimark_lu                 | 114 ms                                                       | 140 ms: 1.23x slower                                                         |
| coverage                   | 66.1 ms                                                      | 82.4 ms: 1.25x slower                                                        |
| go                         | 158 ms                                                       | 200 ms: 1.27x slower                                                         |
| mako                       | 11.0 ms                                                      | 14.1 ms: 1.28x slower                                                        |
| unpickle_pure_python       | 238 us                                                       | 309 us: 1.30x slower                                                         |
| regex_compile              | 156 ms                                                       | 203 ms: 1.30x slower                                                         |
| fannkuch                   | 416 ms                                                       | 543 ms: 1.30x slower                                                         |
| tomli_loads                | 2.25 sec                                                     | 2.99 sec: 1.33x slower                                                       |
| float                      | 74.9 ms                                                      | 105 ms: 1.40x slower                                                         |
| nbody                      | 92.9 ms                                                      | 132 ms: 1.42x slower                                                         |
| unpack_sequence            | 45.7 ns                                                      | 65.7 ns: 1.44x slower                                                        |
| dask                       | 410 ms                                                       | 591 ms: 1.44x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.2 ms: 1.45x slower                                                        |
| scimark_sor                | 110 ms                                                       | 162 ms: 1.47x slower                                                         |
| scimark_monte_carlo        | 69.8 ms                                                      | 105 ms: 1.50x slower                                                         |
| hexiom                     | 6.98 ms                                                      | 10.7 ms: 1.53x slower                                                        |
| scimark_fft                | 281 ms                                                       | 430 ms: 1.53x slower                                                         |
| pyflate                    | 449 ms                                                       | 695 ms: 1.55x slower                                                         |
| spectral_norm              | 95.1 ms                                                      | 152 ms: 1.60x slower                                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.71 ms: 1.65x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.06x slower                                                                 |

Benchmark hidden because not significant (6): pickle_pure_python, unpickle_list, sympy_str, bench_thread_pool, comprehensions, bench_mp_pool
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.96% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.00x