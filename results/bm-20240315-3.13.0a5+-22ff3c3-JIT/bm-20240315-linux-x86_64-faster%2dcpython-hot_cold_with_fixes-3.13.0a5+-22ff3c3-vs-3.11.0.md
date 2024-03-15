# Results vs. 3.11.0

- fork: faster-cpython
- ref: hot_cold_with_fixes
- machine: linux-x86_64
- commit hash: 22ff3c3
- commit date: 2024-03-15
- overall geometric mean: 1.02x faster
- HPT reliability: 62.76%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.14x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 281 ms: 1.06x slower                                                            |
| chameleon      | 6.70 ms                                                | 7.17 ms: 1.07x slower                                                           |
| docutils       | 2.66 sec                                               | 2.77 sec: 1.04x slower                                                          |
| html5lib       | 64.8 ms                                                | 66.1 ms: 1.02x slower                                                           |
| tornado_http   | 98.1 ms                                                | 99.3 ms: 1.01x slower                                                           |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 446 ms: 1.18x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.10x faster                                                            |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                          |
| async_tree_memoization_tg  | 626 ms                                                 | 592 ms: 1.06x faster                                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.24 sec: 1.04x faster                                                          |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 722 ms: 1.04x faster                                                            |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 738 ms: 1.03x faster                                                            |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 92.7 ms: 1.04x faster                                                           |
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                            |
| float          | 78.9 ms                                                | 80.7 ms: 1.02x slower                                                           |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 145 ms: 1.03x slower                                                            |
| regex_effbot   | 3.51 ms                                                | 3.69 ms: 1.05x slower                                                           |
| regex_v8       | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                           |
| regex_dna      | 205 ms                                                 | 228 ms: 1.11x slower                                                            |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                           |
| tomli_loads          | 2.30 sec                                               | 2.07 sec: 1.11x faster                                                          |
| unpickle_list        | 5.21 us                                                | 4.99 us: 1.04x faster                                                           |
| xml_etree_parse      | 164 ms                                                 | 160 ms: 1.03x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 312 us: 1.02x faster                                                            |
| unpickle_pure_python | 242 us                                                 | 238 us: 1.01x faster                                                            |
| json_loads           | 29.2 us                                                | 28.9 us: 1.01x faster                                                           |
| pickle_dict          | 34.6 us                                                | 34.7 us: 1.00x slower                                                           |
| xml_etree_process    | 56.9 ms                                                | 61.1 ms: 1.07x slower                                                           |
| xml_etree_generate   | 81.1 ms                                                | 88.6 ms: 1.09x slower                                                           |
| pickle               | 11.0 us                                                | 12.1 us: 1.10x slower                                                           |
| unpickle             | 13.8 us                                                | 15.4 us: 1.11x slower                                                           |
| pickle_list          | 4.59 us                                                | 5.26 us: 1.15x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                                    |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 11.3 ms: 1.33x slower                                                           |
| python_startup_no_site | 6.01 ms                                                | 9.93 ms: 1.65x slower                                                           |
| Geometric mean         | (ref)                                                  | 1.48x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| django_template | 33.5 ms                                                | 34.6 ms: 1.03x slower                                                           |
| mako            | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                           |
| genshi_xml      | 53.4 ms                                                | 56.8 ms: 1.06x slower                                                           |
| genshi_text     | 22.5 ms                                                | 25.6 ms: 1.14x slower                                                           |
| Geometric mean  | (ref)                                                  | 1.07x slower                                                                    |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240315-linux-x86_64-faster%2dcpython-hot_cold_with_fixes-3.13.0a5+-22ff3c3 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 113 us: 4.61x faster                                                            |
| generators                 | 74.9 ms                                                | 30.3 ms: 2.47x faster                                                           |
| asyncio_tcp                | 875 ms                                                 | 506 ms: 1.73x faster                                                            |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.84 sec: 1.69x faster                                                          |
| pylint                     | 476 ms                                                 | 326 ms: 1.46x faster                                                            |
| comprehensions             | 23.6 us                                                | 17.9 us: 1.32x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                           |
| coroutines                 | 27.0 ms                                                | 22.5 ms: 1.20x faster                                                           |
| async_tree_none            | 528 ms                                                 | 446 ms: 1.18x faster                                                            |
| richards_super             | 61.9 ms                                                | 54.0 ms: 1.14x faster                                                           |
| chaos                      | 71.9 ms                                                | 63.6 ms: 1.13x faster                                                           |
| gc_traversal               | 4.01 ms                                                | 3.57 ms: 1.12x faster                                                           |
| deltablue                  | 3.92 ms                                                | 3.52 ms: 1.12x faster                                                           |
| tomli_loads                | 2.30 sec                                               | 2.07 sec: 1.11x faster                                                          |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.10x faster                                                            |
| logging_silent             | 111 ns                                                 | 101 ns: 1.10x faster                                                            |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                                            |
| raytrace                   | 309 ms                                                 | 290 ms: 1.06x faster                                                            |
| richards                   | 49.8 ms                                                | 46.9 ms: 1.06x faster                                                           |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                          |
| djangocms                  | 33.5 us                                                | 31.6 us: 1.06x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 592 ms: 1.06x faster                                                            |
| mdp                        | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                          |
| sympy_sum                  | 169 ms                                                 | 161 ms: 1.05x faster                                                            |
| logging_simple             | 6.22 us                                                | 5.95 us: 1.05x faster                                                           |
| sqlglot_transpile          | 1.75 ms                                                | 1.67 ms: 1.05x faster                                                           |
| unpickle_list              | 5.21 us                                                | 4.99 us: 1.04x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.24 sec: 1.04x faster                                                          |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 722 ms: 1.04x faster                                                            |
| nbody                      | 96.0 ms                                                | 92.7 ms: 1.04x faster                                                           |
| logging_format             | 6.81 us                                                | 6.60 us: 1.03x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 738 ms: 1.03x faster                                                            |
| sympy_str                  | 297 ms                                                 | 289 ms: 1.03x faster                                                            |
| sqlglot_normalize          | 113 ms                                                 | 110 ms: 1.03x faster                                                            |
| crypto_pyaes               | 76.7 ms                                                | 74.6 ms: 1.03x faster                                                           |
| deepcopy_reduce            | 3.22 us                                                | 3.13 us: 1.03x faster                                                           |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                            |
| deepcopy_memo              | 40.2 us                                                | 39.1 us: 1.03x faster                                                           |
| xml_etree_parse            | 164 ms                                                 | 160 ms: 1.03x faster                                                            |
| pickle_pure_python         | 320 us                                                 | 312 us: 1.02x faster                                                            |
| deepcopy                   | 365 us                                                 | 358 us: 1.02x faster                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.93 ms: 1.02x faster                                                           |
| unpickle_pure_python       | 242 us                                                 | 238 us: 1.01x faster                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 69.8 ms: 1.01x faster                                                           |
| scimark_fft                | 345 ms                                                 | 342 ms: 1.01x faster                                                            |
| json_loads                 | 29.2 us                                                | 28.9 us: 1.01x faster                                                           |
| sympy_integrate            | 21.5 ms                                                | 21.4 ms: 1.00x faster                                                           |
| pickle_dict                | 34.6 us                                                | 34.7 us: 1.00x slower                                                           |
| sympy_expand               | 484 ms                                                 | 489 ms: 1.01x slower                                                            |
| tornado_http               | 98.1 ms                                                | 99.3 ms: 1.01x slower                                                           |
| pprint_safe_repr           | 747 ms                                                 | 759 ms: 1.02x slower                                                            |
| pathlib                    | 18.5 ms                                                | 18.8 ms: 1.02x slower                                                           |
| html5lib                   | 64.8 ms                                                | 66.1 ms: 1.02x slower                                                           |
| thrift                     | 784 us                                                 | 801 us: 1.02x slower                                                            |
| float                      | 78.9 ms                                                | 80.7 ms: 1.02x slower                                                           |
| meteor_contest             | 109 ms                                                 | 111 ms: 1.02x slower                                                            |
| asyncio_websockets         | 550 ms                                                 | 564 ms: 1.02x slower                                                            |
| regex_compile              | 141 ms                                                 | 145 ms: 1.03x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.22 sec: 1.03x slower                                                          |
| dask                       | 365 ms                                                 | 376 ms: 1.03x slower                                                            |
| django_template            | 33.5 ms                                                | 34.6 ms: 1.03x slower                                                           |
| bench_mp_pool              | 24.0 ms                                                | 24.8 ms: 1.03x slower                                                           |
| sqlglot_optimize           | 55.3 ms                                                | 57.2 ms: 1.04x slower                                                           |
| nqueens                    | 87.9 ms                                                | 91.1 ms: 1.04x slower                                                           |
| docutils                   | 2.66 sec                                               | 2.77 sec: 1.04x slower                                                          |
| hexiom                     | 6.89 ms                                                | 7.17 ms: 1.04x slower                                                           |
| bench_thread_pool          | 834 us                                                 | 869 us: 1.04x slower                                                            |
| spectral_norm              | 108 ms                                                 | 113 ms: 1.04x slower                                                            |
| mako                       | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                           |
| regex_effbot               | 3.51 ms                                                | 3.69 ms: 1.05x slower                                                           |
| genshi_xml                 | 53.4 ms                                                | 56.8 ms: 1.06x slower                                                           |
| 2to3                       | 264 ms                                                 | 281 ms: 1.06x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.53 ms: 1.07x slower                                                           |
| chameleon                  | 6.70 ms                                                | 7.17 ms: 1.07x slower                                                           |
| xml_etree_process          | 56.9 ms                                                | 61.1 ms: 1.07x slower                                                           |
| go                         | 149 ms                                                 | 160 ms: 1.08x slower                                                            |
| aiohttp                    | 1.12 ms                                                | 1.20 ms: 1.08x slower                                                           |
| gunicorn                   | 1.20 ms                                                | 1.30 ms: 1.09x slower                                                           |
| regex_v8                   | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                           |
| dulwich_log                | 64.6 ms                                                | 70.5 ms: 1.09x slower                                                           |
| xml_etree_generate         | 81.1 ms                                                | 88.6 ms: 1.09x slower                                                           |
| pickle                     | 11.0 us                                                | 12.1 us: 1.10x slower                                                           |
| pyflate                    | 434 ms                                                 | 479 ms: 1.10x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.86 us: 1.11x slower                                                           |
| regex_dna                  | 205 ms                                                 | 228 ms: 1.11x slower                                                            |
| unpickle                   | 13.8 us                                                | 15.4 us: 1.11x slower                                                           |
| scimark_sor                | 121 ms                                                 | 135 ms: 1.11x slower                                                            |
| genshi_text                | 22.5 ms                                                | 25.6 ms: 1.14x slower                                                           |
| scimark_lu                 | 116 ms                                                 | 133 ms: 1.15x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.26 us: 1.15x slower                                                           |
| coverage                   | 78.8 ms                                                | 96.9 ms: 1.23x slower                                                           |
| telco                      | 6.86 ms                                                | 8.47 ms: 1.23x slower                                                           |
| async_generators           | 374 ms                                                 | 475 ms: 1.27x slower                                                            |
| python_startup             | 8.56 ms                                                | 11.3 ms: 1.33x slower                                                           |
| mypy2                      | 686 ms                                                 | 911 ms: 1.33x slower                                                            |
| python_startup_no_site     | 6.01 ms                                                | 9.93 ms: 1.65x slower                                                           |
| unpack_sequence            | 43.5 ns                                                | 85.2 ns: 1.96x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                                    |

Benchmark hidden because not significant (4): fannkuch, xml_etree_iterparse, json, pprint_pformat
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 62.76% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.14x