
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.02x faster
- HPT reliability: 50.23%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 277 ms: 1.05x slower                                           |
| chameleon      | 6.70 ms                                                | 7.09 ms: 1.06x slower                                          |
| docutils       | 2.66 sec                                               | 2.68 sec: 1.01x slower                                         |
| Geometric mean | (ref)                                                  | 1.03x slower                                                   |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 446 ms: 1.18x faster                                           |
| async_tree_memoization     | 639 ms                                                 | 569 ms: 1.12x faster                                           |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.09x faster                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 580 ms: 1.08x faster                                           |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 728 ms: 1.05x faster                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.05x faster                                           |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                           |
| nbody          | 96.0 ms                                                | 106 ms: 1.11x slower                                           |
| float          | 78.9 ms                                                | 88.1 ms: 1.12x slower                                          |
| Geometric mean | (ref)                                                  | 1.06x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 142 ms: 1.01x slower                                           |
| regex_dna      | 205 ms                                                 | 213 ms: 1.04x slower                                           |
| regex_effbot   | 3.51 ms                                                | 3.69 ms: 1.05x slower                                          |
| regex_v8       | 22.9 ms                                                | 26.1 ms: 1.14x slower                                          |
| Geometric mean | (ref)                                                  | 1.06x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.30x faster                                          |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                           |
| unpickle_pure_python | 242 us                                                 | 228 us: 1.06x faster                                           |
| json_loads           | 29.2 us                                                | 27.5 us: 1.06x faster                                          |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                           |
| tomli_loads          | 2.30 sec                                               | 2.25 sec: 1.02x faster                                         |
| unpickle_list        | 5.21 us                                                | 5.13 us: 1.02x faster                                          |
| xml_etree_iterparse  | 108 ms                                                 | 109 ms: 1.01x slower                                           |
| pickle_dict          | 34.6 us                                                | 35.4 us: 1.02x slower                                          |
| xml_etree_process    | 56.9 ms                                                | 59.0 ms: 1.04x slower                                          |
| unpickle             | 13.8 us                                                | 14.6 us: 1.05x slower                                          |
| pickle               | 11.0 us                                                | 11.6 us: 1.05x slower                                          |
| xml_etree_generate   | 81.1 ms                                                | 86.8 ms: 1.07x slower                                          |
| pickle_list          | 4.59 us                                                | 5.02 us: 1.10x slower                                          |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.20x slower                                          |
| python_startup_no_site | 6.01 ms                                                | 8.87 ms: 1.48x slower                                          |
| Geometric mean         | (ref)                                                  | 1.33x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.7 ms: 1.20x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 113 us: 4.60x faster                                           |
| generators                 | 74.9 ms                                                | 28.8 ms: 2.60x faster                                          |
| asyncio_tcp                | 875 ms                                                 | 496 ms: 1.77x faster                                           |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                         |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.30x faster                                          |
| coroutines                 | 27.0 ms                                                | 22.5 ms: 1.20x faster                                          |
| comprehensions             | 23.6 us                                                | 19.8 us: 1.19x faster                                          |
| async_tree_none            | 528 ms                                                 | 446 ms: 1.18x faster                                           |
| richards_super             | 61.9 ms                                                | 52.7 ms: 1.17x faster                                          |
| async_tree_memoization     | 639 ms                                                 | 569 ms: 1.12x faster                                           |
| sqlglot_parse              | 1.43 ms                                                | 1.29 ms: 1.11x faster                                          |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.09x faster                                           |
| raytrace                   | 309 ms                                                 | 282 ms: 1.09x faster                                           |
| sqlglot_transpile          | 1.75 ms                                                | 1.62 ms: 1.08x faster                                          |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                         |
| async_tree_memoization_tg  | 626 ms                                                 | 580 ms: 1.08x faster                                           |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                         |
| richards                   | 49.8 ms                                                | 46.3 ms: 1.08x faster                                          |
| logging_silent             | 111 ns                                                 | 103 ns: 1.07x faster                                           |
| logging_simple             | 6.22 us                                                | 5.83 us: 1.07x faster                                          |
| gc_traversal               | 4.01 ms                                                | 3.77 ms: 1.06x faster                                          |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                           |
| mdp                        | 2.77 sec                                               | 2.61 sec: 1.06x faster                                         |
| unpickle_pure_python       | 242 us                                                 | 228 us: 1.06x faster                                           |
| json_loads                 | 29.2 us                                                | 27.5 us: 1.06x faster                                          |
| deepcopy_reduce            | 3.22 us                                                | 3.04 us: 1.06x faster                                          |
| logging_format             | 6.81 us                                                | 6.45 us: 1.06x faster                                          |
| deepcopy_memo              | 40.2 us                                                | 38.1 us: 1.05x faster                                          |
| deepcopy                   | 365 us                                                 | 349 us: 1.05x faster                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 728 ms: 1.05x faster                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.05x faster                                           |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                           |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                           |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                           |
| sympy_str                  | 297 ms                                                 | 290 ms: 1.02x faster                                           |
| tomli_loads                | 2.30 sec                                               | 2.25 sec: 1.02x faster                                         |
| chaos                      | 71.9 ms                                                | 70.6 ms: 1.02x faster                                          |
| sqlglot_normalize          | 113 ms                                                 | 111 ms: 1.02x faster                                           |
| scimark_lu                 | 116 ms                                                 | 115 ms: 1.02x faster                                           |
| unpickle_list              | 5.21 us                                                | 5.13 us: 1.02x faster                                          |
| json                       | 5.24 ms                                                | 5.17 ms: 1.01x faster                                          |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                          |
| pycparser                  | 1.19 sec                                               | 1.17 sec: 1.01x faster                                         |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                          |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                           |
| docutils                   | 2.66 sec                                               | 2.68 sec: 1.01x slower                                         |
| xml_etree_iterparse        | 108 ms                                                 | 109 ms: 1.01x slower                                           |
| regex_compile              | 141 ms                                                 | 142 ms: 1.01x slower                                           |
| bench_thread_pool          | 834 us                                                 | 843 us: 1.01x slower                                           |
| meteor_contest             | 109 ms                                                 | 110 ms: 1.01x slower                                           |
| sqlglot_optimize           | 55.3 ms                                                | 56.2 ms: 1.02x slower                                          |
| go                         | 149 ms                                                 | 152 ms: 1.02x slower                                           |
| pickle_dict                | 34.6 us                                                | 35.4 us: 1.02x slower                                          |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                          |
| deltablue                  | 3.92 ms                                                | 4.07 ms: 1.04x slower                                          |
| nqueens                    | 87.9 ms                                                | 91.2 ms: 1.04x slower                                          |
| xml_etree_process          | 56.9 ms                                                | 59.0 ms: 1.04x slower                                          |
| regex_dna                  | 205 ms                                                 | 213 ms: 1.04x slower                                           |
| 2to3                       | 264 ms                                                 | 277 ms: 1.05x slower                                           |
| regex_effbot               | 3.51 ms                                                | 3.69 ms: 1.05x slower                                          |
| dulwich_log                | 64.6 ms                                                | 68.0 ms: 1.05x slower                                          |
| unpickle                   | 13.8 us                                                | 14.6 us: 1.05x slower                                          |
| pickle                     | 11.0 us                                                | 11.6 us: 1.05x slower                                          |
| chameleon                  | 6.70 ms                                                | 7.09 ms: 1.06x slower                                          |
| crypto_pyaes               | 76.7 ms                                                | 81.4 ms: 1.06x slower                                          |
| scimark_monte_carlo        | 70.7 ms                                                | 75.1 ms: 1.06x slower                                          |
| xml_etree_generate         | 81.1 ms                                                | 86.8 ms: 1.07x slower                                          |
| scimark_sor                | 121 ms                                                 | 131 ms: 1.08x slower                                           |
| pprint_safe_repr           | 747 ms                                                 | 807 ms: 1.08x slower                                           |
| pprint_pformat             | 1.55 sec                                               | 1.68 sec: 1.08x slower                                         |
| fannkuch                   | 405 ms                                                 | 438 ms: 1.08x slower                                           |
| pickle_list                | 4.59 us                                                | 5.02 us: 1.10x slower                                          |
| sqlite_synth               | 2.57 us                                                | 2.85 us: 1.11x slower                                          |
| nbody                      | 96.0 ms                                                | 106 ms: 1.11x slower                                           |
| float                      | 78.9 ms                                                | 88.1 ms: 1.12x slower                                          |
| unpack_sequence            | 43.5 ns                                                | 48.5 ns: 1.12x slower                                          |
| scimark_fft                | 345 ms                                                 | 391 ms: 1.13x slower                                           |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.72 ms: 1.14x slower                                          |
| regex_v8                   | 22.9 ms                                                | 26.1 ms: 1.14x slower                                          |
| pyflate                    | 434 ms                                                 | 504 ms: 1.16x slower                                           |
| hexiom                     | 6.89 ms                                                | 8.11 ms: 1.18x slower                                          |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.20x slower                                          |
| mako                       | 10.7 ms                                                | 12.7 ms: 1.20x slower                                          |
| coverage                   | 78.8 ms                                                | 95.4 ms: 1.21x slower                                          |
| async_generators           | 374 ms                                                 | 460 ms: 1.23x slower                                           |
| telco                      | 6.86 ms                                                | 8.50 ms: 1.24x slower                                          |
| mypy2                      | 686 ms                                                 | 866 ms: 1.26x slower                                           |
| spectral_norm              | 108 ms                                                 | 141 ms: 1.30x slower                                           |
| python_startup_no_site     | 6.01 ms                                                | 8.87 ms: 1.48x slower                                          |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                   |

Benchmark hidden because not significant (4): tornado_http, sympy_expand, bench_mp_pool, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 50.23% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.02x