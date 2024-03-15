
# Results vs. 3.11.0

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: d73fe0a
- commit date: 2024-01-16
- overall geometric mean: 1.04x slower
- HPT reliability: 99.93%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 290 ms: 1.10x slower                                                   |
| chameleon      | 6.70 ms                                                | 7.32 ms: 1.09x slower                                                  |
| docutils       | 2.66 sec                                               | 2.85 sec: 1.07x slower                                                 |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 452 ms: 1.09x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 587 ms: 1.07x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 729 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 722 ms: 1.04x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                   |
| float          | 78.9 ms                                                | 93.4 ms: 1.18x slower                                                  |
| nbody          | 96.0 ms                                                | 120 ms: 1.25x slower                                                   |
| Geometric mean | (ref)                                                  | 1.13x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.61 ms: 1.03x slower                                                  |
| regex_v8       | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                  |
| regex_dna      | 205 ms                                                 | 227 ms: 1.11x slower                                                   |
| regex_compile  | 141 ms                                                 | 172 ms: 1.21x slower                                                   |
| Geometric mean | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 299 us: 1.07x faster                                                   |
| unpickle_list        | 5.21 us                                                | 4.93 us: 1.06x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| json_loads           | 29.2 us                                                | 28.4 us: 1.03x faster                                                  |
| pickle               | 11.0 us                                                | 11.4 us: 1.04x slower                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 112 ms: 1.04x slower                                                   |
| unpickle             | 13.8 us                                                | 14.8 us: 1.07x slower                                                  |
| pickle_dict          | 34.6 us                                                | 37.0 us: 1.07x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 62.2 ms: 1.09x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 90.8 ms: 1.12x slower                                                  |
| unpickle_pure_python | 242 us                                                 | 278 us: 1.15x slower                                                   |
| pickle_list          | 4.59 us                                                | 5.34 us: 1.16x slower                                                  |
| tomli_loads          | 2.30 sec                                               | 2.73 sec: 1.18x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.74 ms: 1.45x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 14.0 ms: 1.31x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-d73fe0a |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 116 us: 4.46x faster                                                   |
| generators                 | 74.9 ms                                                | 29.4 ms: 2.55x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 495 ms: 1.77x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.4 ms: 1.21x faster                                                  |
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.52 ms: 1.14x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 452 ms: 1.09x faster                                                   |
| comprehensions             | 23.6 us                                                | 22.0 us: 1.07x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| pickle_pure_python         | 320 us                                                 | 299 us: 1.07x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 587 ms: 1.07x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                 |
| unpickle_list              | 5.21 us                                                | 4.93 us: 1.06x faster                                                  |
| logging_silent             | 111 ns                                                 | 106 ns: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 729 ms: 1.04x faster                                                   |
| mdp                        | 2.77 sec                                               | 2.66 sec: 1.04x faster                                                 |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 722 ms: 1.04x faster                                                   |
| json_loads                 | 29.2 us                                                | 28.4 us: 1.03x faster                                                  |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 164 ms: 1.03x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.15 us: 1.02x faster                                                  |
| deepcopy                   | 365 us                                                 | 358 us: 1.02x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.42 ms: 1.01x faster                                                  |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                   |
| json                       | 5.24 ms                                                | 5.28 ms: 1.01x slower                                                  |
| dask                       | 365 ms                                                 | 370 ms: 1.01x slower                                                   |
| sympy_str                  | 297 ms                                                 | 302 ms: 1.02x slower                                                   |
| sympy_integrate            | 21.5 ms                                                | 21.8 ms: 1.02x slower                                                  |
| raytrace                   | 309 ms                                                 | 316 ms: 1.02x slower                                                   |
| bench_thread_pool          | 834 us                                                 | 855 us: 1.02x slower                                                   |
| deepcopy_memo              | 40.2 us                                                | 41.3 us: 1.03x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.61 ms: 1.03x slower                                                  |
| pathlib                    | 18.5 ms                                                | 19.1 ms: 1.03x slower                                                  |
| logging_simple             | 6.22 us                                                | 6.44 us: 1.04x slower                                                  |
| pickle                     | 11.0 us                                                | 11.4 us: 1.04x slower                                                  |
| sympy_expand               | 484 ms                                                 | 503 ms: 1.04x slower                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 112 ms: 1.04x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                  |
| chaos                      | 71.9 ms                                                | 75.7 ms: 1.05x slower                                                  |
| sqlglot_normalize          | 113 ms                                                 | 119 ms: 1.06x slower                                                   |
| logging_format             | 6.81 us                                                | 7.24 us: 1.06x slower                                                  |
| meteor_contest             | 109 ms                                                 | 116 ms: 1.07x slower                                                   |
| unpickle                   | 13.8 us                                                | 14.8 us: 1.07x slower                                                  |
| pickle_dict                | 34.6 us                                                | 37.0 us: 1.07x slower                                                  |
| docutils                   | 2.66 sec                                               | 2.85 sec: 1.07x slower                                                 |
| pycparser                  | 1.19 sec                                               | 1.28 sec: 1.08x slower                                                 |
| chameleon                  | 6.70 ms                                                | 7.32 ms: 1.09x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 62.2 ms: 1.09x slower                                                  |
| 2to3                       | 264 ms                                                 | 290 ms: 1.10x slower                                                   |
| crypto_pyaes               | 76.7 ms                                                | 84.6 ms: 1.10x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 71.3 ms: 1.10x slower                                                  |
| regex_dna                  | 205 ms                                                 | 227 ms: 1.11x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.86 us: 1.11x slower                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 61.5 ms: 1.11x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 90.8 ms: 1.12x slower                                                  |
| nqueens                    | 87.9 ms                                                | 99.0 ms: 1.13x slower                                                  |
| unpickle_pure_python       | 242 us                                                 | 278 us: 1.15x slower                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.80 sec: 1.16x slower                                                 |
| pickle_list                | 4.59 us                                                | 5.34 us: 1.16x slower                                                  |
| pprint_safe_repr           | 747 ms                                                 | 873 ms: 1.17x slower                                                   |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| float                      | 78.9 ms                                                | 93.4 ms: 1.18x slower                                                  |
| tomli_loads                | 2.30 sec                                               | 2.73 sec: 1.18x slower                                                 |
| go                         | 149 ms                                                 | 176 ms: 1.19x slower                                                   |
| fannkuch                   | 405 ms                                                 | 485 ms: 1.20x slower                                                   |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.05 ms: 1.20x slower                                                  |
| coverage                   | 78.8 ms                                                | 95.4 ms: 1.21x slower                                                  |
| regex_compile              | 141 ms                                                 | 172 ms: 1.21x slower                                                   |
| async_generators           | 374 ms                                                 | 458 ms: 1.22x slower                                                   |
| scimark_sor                | 121 ms                                                 | 150 ms: 1.23x slower                                                   |
| nbody                      | 96.0 ms                                                | 120 ms: 1.25x slower                                                   |
| unpack_sequence            | 43.5 ns                                                | 54.3 ns: 1.25x slower                                                  |
| richards_super             | 61.9 ms                                                | 77.6 ms: 1.25x slower                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 89.4 ms: 1.26x slower                                                  |
| telco                      | 6.86 ms                                                | 8.72 ms: 1.27x slower                                                  |
| mypy2                      | 686 ms                                                 | 896 ms: 1.31x slower                                                   |
| scimark_fft                | 345 ms                                                 | 452 ms: 1.31x slower                                                   |
| scimark_lu                 | 116 ms                                                 | 152 ms: 1.31x slower                                                   |
| deltablue                  | 3.92 ms                                                | 5.14 ms: 1.31x slower                                                  |
| mako                       | 10.7 ms                                                | 14.0 ms: 1.31x slower                                                  |
| pyflate                    | 434 ms                                                 | 579 ms: 1.33x slower                                                   |
| hexiom                     | 6.89 ms                                                | 9.28 ms: 1.35x slower                                                  |
| spectral_norm              | 108 ms                                                 | 149 ms: 1.37x slower                                                   |
| richards                   | 49.8 ms                                                | 68.4 ms: 1.37x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 8.74 ms: 1.45x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (3): bench_mp_pool, tornado_http, sqlglot_transpile
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.93% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.99x