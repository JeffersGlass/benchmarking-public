
# Results vs. 3.11.0

- fork: python
- ref: 35ef8cb25917bfd6cbbd
- machine: linux-x86_64
- commit hash: 35ef8cb
- commit date: 2024-01-04
- overall geometric mean: 1.01x slower \*
- HPT reliability: 99.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 285 ms: 1.08x slower                                                   |
| chameleon      | 6.70 ms                                                | 7.27 ms: 1.09x slower                                                  |
| docutils       | 2.66 sec                                               | 2.72 sec: 1.02x slower                                                 |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 456 ms: 1.16x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 583 ms: 1.10x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.23 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 594 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 737 ms: 1.03x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                                   |
| float          | 78.9 ms                                                | 94.0 ms: 1.19x slower                                                  |
| nbody          | 96.0 ms                                                | 126 ms: 1.32x slower                                                   |
| Geometric mean | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.63 ms: 1.03x slower                                                  |
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.08x slower                                                  |
| regex_compile  | 141 ms                                                 | 156 ms: 1.10x slower                                                   |
| regex_dna      | 205 ms                                                 | 227 ms: 1.11x slower                                                   |
| Geometric mean | (ref)                                                  | 1.08x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 304 us: 1.05x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.05x faster                                                   |
| json_loads           | 29.2 us                                                | 28.2 us: 1.04x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 239 us: 1.01x faster                                                   |
| pickle_dict          | 34.6 us                                                | 35.1 us: 1.02x slower                                                  |
| unpickle_list        | 5.21 us                                                | 5.39 us: 1.03x slower                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 113 ms: 1.05x slower                                                   |
| pickle               | 11.0 us                                                | 11.6 us: 1.05x slower                                                  |
| unpickle             | 13.8 us                                                | 14.7 us: 1.06x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 62.0 ms: 1.09x slower                                                  |
| tomli_loads          | 2.30 sec                                               | 2.53 sec: 1.10x slower                                                 |
| pickle_list          | 4.59 us                                                | 5.13 us: 1.12x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 90.9 ms: 1.12x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.77 ms: 1.46x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 14.7 ms: 1.37x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 117 us: 4.45x faster                                                   |
| generators                 | 74.9 ms                                                | 29.1 ms: 2.57x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 494 ms: 1.77x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.5 ms: 1.20x faster                                                  |
| async_tree_none            | 528 ms                                                 | 456 ms: 1.16x faster                                                   |
| richards_super             | 61.9 ms                                                | 56.0 ms: 1.10x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 583 ms: 1.10x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.34 ms: 1.07x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.23 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 594 ms: 1.05x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 304 us: 1.05x faster                                                   |
| comprehensions             | 23.6 us                                                | 22.5 us: 1.05x faster                                                  |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.05x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.83 ms: 1.05x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.68 ms: 1.04x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.66 sec: 1.04x faster                                                 |
| unpack_sequence            | 43.5 ns                                                | 41.7 ns: 1.04x faster                                                  |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.04x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.04x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 737 ms: 1.03x faster                                                   |
| logging_silent             | 111 ns                                                 | 108 ns: 1.03x faster                                                   |
| pidigits                   | 194 ms                                                 | 190 ms: 1.02x faster                                                   |
| logging_simple             | 6.22 us                                                | 6.08 us: 1.02x faster                                                  |
| deepcopy_reduce            | 3.22 us                                                | 3.16 us: 1.02x faster                                                  |
| raytrace                   | 309 ms                                                 | 304 ms: 1.02x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 239 us: 1.01x faster                                                   |
| deepcopy                   | 365 us                                                 | 360 us: 1.01x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 21.6 ms: 1.01x slower                                                  |
| pickle_dict                | 34.6 us                                                | 35.1 us: 1.02x slower                                                  |
| docutils                   | 2.66 sec                                               | 2.72 sec: 1.02x slower                                                 |
| pathlib                    | 18.5 ms                                                | 18.9 ms: 1.02x slower                                                  |
| scimark_lu                 | 116 ms                                                 | 119 ms: 1.02x slower                                                   |
| bench_thread_pool          | 834 us                                                 | 854 us: 1.02x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.02x slower                                                  |
| sqlglot_normalize          | 113 ms                                                 | 116 ms: 1.03x slower                                                   |
| regex_effbot               | 3.51 ms                                                | 3.63 ms: 1.03x slower                                                  |
| unpickle_list              | 5.21 us                                                | 5.39 us: 1.03x slower                                                  |
| sympy_expand               | 484 ms                                                 | 505 ms: 1.04x slower                                                   |
| deepcopy_memo              | 40.2 us                                                | 41.9 us: 1.04x slower                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 113 ms: 1.05x slower                                                   |
| pickle                     | 11.0 us                                                | 11.6 us: 1.05x slower                                                  |
| chaos                      | 71.9 ms                                                | 76.0 ms: 1.06x slower                                                  |
| unpickle                   | 13.8 us                                                | 14.7 us: 1.06x slower                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 58.9 ms: 1.07x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 68.9 ms: 1.07x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 24.6 ms: 1.08x slower                                                  |
| 2to3                       | 264 ms                                                 | 285 ms: 1.08x slower                                                   |
| go                         | 149 ms                                                 | 161 ms: 1.08x slower                                                   |
| chameleon                  | 6.70 ms                                                | 7.27 ms: 1.09x slower                                                  |
| scimark_sor                | 121 ms                                                 | 132 ms: 1.09x slower                                                   |
| xml_etree_process          | 56.9 ms                                                | 62.0 ms: 1.09x slower                                                  |
| meteor_contest             | 109 ms                                                 | 119 ms: 1.09x slower                                                   |
| tomli_loads                | 2.30 sec                                               | 2.53 sec: 1.10x slower                                                 |
| regex_compile              | 141 ms                                                 | 156 ms: 1.10x slower                                                   |
| regex_dna                  | 205 ms                                                 | 227 ms: 1.11x slower                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.74 sec: 1.12x slower                                                 |
| pprint_safe_repr           | 747 ms                                                 | 836 ms: 1.12x slower                                                   |
| pickle_list                | 4.59 us                                                | 5.13 us: 1.12x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 90.9 ms: 1.12x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.92 us: 1.13x slower                                                  |
| crypto_pyaes               | 76.7 ms                                                | 87.4 ms: 1.14x slower                                                  |
| nqueens                    | 87.9 ms                                                | 101 ms: 1.15x slower                                                   |
| fannkuch                   | 405 ms                                                 | 477 ms: 1.18x slower                                                   |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| float                      | 78.9 ms                                                | 94.0 ms: 1.19x slower                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 84.8 ms: 1.20x slower                                                  |
| coverage                   | 78.8 ms                                                | 94.7 ms: 1.20x slower                                                  |
| async_generators           | 374 ms                                                 | 453 ms: 1.21x slower                                                   |
| deltablue                  | 3.92 ms                                                | 4.87 ms: 1.24x slower                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.30 ms: 1.25x slower                                                  |
| mypy2                      | 686 ms                                                 | 865 ms: 1.26x slower                                                   |
| pyflate                    | 434 ms                                                 | 554 ms: 1.28x slower                                                   |
| telco                      | 6.86 ms                                                | 8.88 ms: 1.30x slower                                                  |
| hexiom                     | 6.89 ms                                                | 9.02 ms: 1.31x slower                                                  |
| nbody                      | 96.0 ms                                                | 126 ms: 1.32x slower                                                   |
| scimark_fft                | 345 ms                                                 | 472 ms: 1.37x slower                                                   |
| mako                       | 10.7 ms                                                | 14.7 ms: 1.37x slower                                                  |
| spectral_norm              | 108 ms                                                 | 157 ms: 1.45x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.77 ms: 1.46x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (9): logging_format, richards, bench_mp_pool, tornado_http, json, asyncio_websockets, sympy_str, pycparser, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x