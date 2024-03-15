
# Results vs. 3.11.0

- fork: faster-cpython
- ref: split_on_oparg_1
- machine: linux-x86_64
- commit hash: d879778
- commit date: 2024-02-14
- overall geometric mean: 1.01x faster \*
- HPT reliability: 89.45%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 284 ms: 1.07x slower                                                         |
| chameleon      | 6.70 ms                                                | 7.01 ms: 1.05x slower                                                        |
| docutils       | 2.66 sec                                               | 2.68 sec: 1.01x slower                                                       |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                         |
| async_tree_memoization     | 639 ms                                                 | 569 ms: 1.12x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 584 ms: 1.07x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                       |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 718 ms: 1.04x faster                                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 733 ms: 1.04x faster                                                         |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                         |
| float          | 78.9 ms                                                | 93.5 ms: 1.18x slower                                                        |
| nbody          | 96.0 ms                                                | 121 ms: 1.26x slower                                                         |
| Geometric mean | (ref)                                                  | 1.13x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 150 ms: 1.06x slower                                                         |
| regex_effbot   | 3.51 ms                                                | 3.75 ms: 1.07x slower                                                        |
| regex_dna      | 205 ms                                                 | 228 ms: 1.11x slower                                                         |
| regex_v8       | 22.9 ms                                                | 26.3 ms: 1.15x slower                                                        |
| Geometric mean | (ref)                                                  | 1.10x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                        |
| pickle_pure_python   | 320 us                                                 | 299 us: 1.07x faster                                                         |
| json_loads           | 29.2 us                                                | 27.5 us: 1.06x faster                                                        |
| unpickle_list        | 5.21 us                                                | 4.97 us: 1.05x faster                                                        |
| unpickle_pure_python | 242 us                                                 | 232 us: 1.04x faster                                                         |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                         |
| pickle_dict          | 34.6 us                                                | 34.8 us: 1.01x slower                                                        |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.02x slower                                                         |
| xml_etree_process    | 56.9 ms                                                | 60.6 ms: 1.06x slower                                                        |
| pickle               | 11.0 us                                                | 12.0 us: 1.09x slower                                                        |
| xml_etree_generate   | 81.1 ms                                                | 88.8 ms: 1.10x slower                                                        |
| unpickle             | 13.8 us                                                | 15.4 us: 1.11x slower                                                        |
| tomli_loads          | 2.30 sec                                               | 2.61 sec: 1.13x slower                                                       |
| pickle_list          | 4.59 us                                                | 5.23 us: 1.14x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.3 ms: 1.20x slower                                                        |
| python_startup_no_site | 6.01 ms                                                | 8.88 ms: 1.48x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.33x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.9 ms: 1.30x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 115 us: 4.52x faster                                                         |
| generators                 | 74.9 ms                                                | 29.1 ms: 2.57x faster                                                        |
| asyncio_tcp                | 875 ms                                                 | 491 ms: 1.78x faster                                                         |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                       |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                        |
| coroutines                 | 27.0 ms                                                | 22.9 ms: 1.18x faster                                                        |
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                         |
| comprehensions             | 23.6 us                                                | 20.3 us: 1.16x faster                                                        |
| richards_super             | 61.9 ms                                                | 53.9 ms: 1.15x faster                                                        |
| async_tree_memoization     | 639 ms                                                 | 569 ms: 1.12x faster                                                         |
| deltablue                  | 3.92 ms                                                | 3.50 ms: 1.12x faster                                                        |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                                         |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                                         |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                        |
| async_tree_memoization_tg  | 626 ms                                                 | 584 ms: 1.07x faster                                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                       |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                       |
| pickle_pure_python         | 320 us                                                 | 299 us: 1.07x faster                                                         |
| sympy_sum                  | 169 ms                                                 | 159 ms: 1.06x faster                                                         |
| json_loads                 | 29.2 us                                                | 27.5 us: 1.06x faster                                                        |
| mdp                        | 2.77 sec                                               | 2.62 sec: 1.06x faster                                                       |
| sqlglot_transpile          | 1.75 ms                                                | 1.67 ms: 1.05x faster                                                        |
| unpickle_list              | 5.21 us                                                | 4.97 us: 1.05x faster                                                        |
| unpickle_pure_python       | 242 us                                                 | 232 us: 1.04x faster                                                         |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 718 ms: 1.04x faster                                                         |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                         |
| richards                   | 49.8 ms                                                | 47.8 ms: 1.04x faster                                                        |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 733 ms: 1.04x faster                                                         |
| sympy_integrate            | 21.5 ms                                                | 20.7 ms: 1.04x faster                                                        |
| raytrace                   | 309 ms                                                 | 298 ms: 1.03x faster                                                         |
| gc_traversal               | 4.01 ms                                                | 3.89 ms: 1.03x faster                                                        |
| logging_simple             | 6.22 us                                                | 6.05 us: 1.03x faster                                                        |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                         |
| json                       | 5.24 ms                                                | 5.11 ms: 1.03x faster                                                        |
| sympy_str                  | 297 ms                                                 | 290 ms: 1.02x faster                                                         |
| deepcopy_reduce            | 3.22 us                                                | 3.14 us: 1.02x faster                                                        |
| deepcopy                   | 365 us                                                 | 357 us: 1.02x faster                                                         |
| unpack_sequence            | 43.5 ns                                                | 42.9 ns: 1.01x faster                                                        |
| logging_format             | 6.81 us                                                | 6.76 us: 1.01x faster                                                        |
| pickle_dict                | 34.6 us                                                | 34.8 us: 1.01x slower                                                        |
| docutils                   | 2.66 sec                                               | 2.68 sec: 1.01x slower                                                       |
| deepcopy_memo              | 40.2 us                                                | 40.6 us: 1.01x slower                                                        |
| bench_thread_pool          | 834 us                                                 | 845 us: 1.01x slower                                                         |
| chaos                      | 71.9 ms                                                | 72.8 ms: 1.01x slower                                                        |
| xml_etree_iterparse        | 108 ms                                                 | 110 ms: 1.02x slower                                                         |
| sympy_expand               | 484 ms                                                 | 493 ms: 1.02x slower                                                         |
| scimark_lu                 | 116 ms                                                 | 119 ms: 1.02x slower                                                         |
| scimark_sor                | 121 ms                                                 | 124 ms: 1.02x slower                                                         |
| meteor_contest             | 109 ms                                                 | 113 ms: 1.04x slower                                                         |
| sqlglot_optimize           | 55.3 ms                                                | 57.6 ms: 1.04x slower                                                        |
| go                         | 149 ms                                                 | 155 ms: 1.04x slower                                                         |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                                        |
| chameleon                  | 6.70 ms                                                | 7.01 ms: 1.05x slower                                                        |
| regex_compile              | 141 ms                                                 | 150 ms: 1.06x slower                                                         |
| xml_etree_process          | 56.9 ms                                                | 60.6 ms: 1.06x slower                                                        |
| pprint_pformat             | 1.55 sec                                               | 1.66 sec: 1.07x slower                                                       |
| dulwich_log                | 64.6 ms                                                | 69.0 ms: 1.07x slower                                                        |
| pprint_safe_repr           | 747 ms                                                 | 799 ms: 1.07x slower                                                         |
| regex_effbot               | 3.51 ms                                                | 3.75 ms: 1.07x slower                                                        |
| 2to3                       | 264 ms                                                 | 284 ms: 1.07x slower                                                         |
| pycparser                  | 1.19 sec                                               | 1.28 sec: 1.08x slower                                                       |
| nqueens                    | 87.9 ms                                                | 94.8 ms: 1.08x slower                                                        |
| crypto_pyaes               | 76.7 ms                                                | 83.4 ms: 1.09x slower                                                        |
| pickle                     | 11.0 us                                                | 12.0 us: 1.09x slower                                                        |
| fannkuch                   | 405 ms                                                 | 444 ms: 1.09x slower                                                         |
| xml_etree_generate         | 81.1 ms                                                | 88.8 ms: 1.10x slower                                                        |
| sqlite_synth               | 2.57 us                                                | 2.86 us: 1.11x slower                                                        |
| unpickle                   | 13.8 us                                                | 15.4 us: 1.11x slower                                                        |
| regex_dna                  | 205 ms                                                 | 228 ms: 1.11x slower                                                         |
| tomli_loads                | 2.30 sec                                               | 2.61 sec: 1.13x slower                                                       |
| pickle_list                | 4.59 us                                                | 5.23 us: 1.14x slower                                                        |
| regex_v8                   | 22.9 ms                                                | 26.3 ms: 1.15x slower                                                        |
| scimark_monte_carlo        | 70.7 ms                                                | 81.3 ms: 1.15x slower                                                        |
| float                      | 78.9 ms                                                | 93.5 ms: 1.18x slower                                                        |
| pyflate                    | 434 ms                                                 | 518 ms: 1.19x slower                                                         |
| python_startup             | 8.56 ms                                                | 10.3 ms: 1.20x slower                                                        |
| hexiom                     | 6.89 ms                                                | 8.40 ms: 1.22x slower                                                        |
| coverage                   | 78.8 ms                                                | 96.9 ms: 1.23x slower                                                        |
| async_generators           | 374 ms                                                 | 461 ms: 1.23x slower                                                         |
| scimark_fft                | 345 ms                                                 | 433 ms: 1.25x slower                                                         |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.34 ms: 1.26x slower                                                        |
| nbody                      | 96.0 ms                                                | 121 ms: 1.26x slower                                                         |
| mypy2                      | 686 ms                                                 | 869 ms: 1.27x slower                                                         |
| telco                      | 6.86 ms                                                | 8.71 ms: 1.27x slower                                                        |
| spectral_norm              | 108 ms                                                 | 139 ms: 1.29x slower                                                         |
| mako                       | 10.7 ms                                                | 13.9 ms: 1.30x slower                                                        |
| python_startup_no_site     | 6.01 ms                                                | 8.88 ms: 1.48x slower                                                        |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                 |

Benchmark hidden because not significant (6): sqlglot_normalize, bench_mp_pool, tornado_http, pathlib, asyncio_websockets, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 89.45% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x