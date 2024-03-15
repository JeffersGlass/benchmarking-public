
# Results vs. 3.11.0

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 92a3b61
- commit date: 2024-01-16
- overall geometric mean: 1.01x slower
- HPT reliability: 97.95%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 288 ms: 1.09x slower                                                   |
| chameleon      | 6.70 ms                                                | 7.11 ms: 1.06x slower                                                  |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 445 ms: 1.19x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 574 ms: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 452 ms: 1.09x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 588 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 731 ms: 1.04x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                   |
| float          | 78.9 ms                                                | 94.2 ms: 1.19x slower                                                  |
| nbody          | 96.0 ms                                                | 120 ms: 1.25x slower                                                   |
| Geometric mean | (ref)                                                  | 1.13x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                  |
| regex_v8       | 22.9 ms                                                | 24.7 ms: 1.08x slower                                                  |
| regex_dna      | 205 ms                                                 | 223 ms: 1.09x slower                                                   |
| regex_compile  | 141 ms                                                 | 164 ms: 1.16x slower                                                   |
| Geometric mean | (ref)                                                  | 1.09x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.8 ms: 1.24x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| unpickle_pure_python | 242 us                                                 | 233 us: 1.04x faster                                                   |
| json_loads           | 29.2 us                                                | 28.5 us: 1.02x faster                                                  |
| pickle_dict          | 34.6 us                                                | 33.9 us: 1.02x faster                                                  |
| unpickle_list        | 5.21 us                                                | 5.32 us: 1.02x slower                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 111 ms: 1.02x slower                                                   |
| pickle               | 11.0 us                                                | 11.7 us: 1.06x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 60.9 ms: 1.07x slower                                                  |
| unpickle             | 13.8 us                                                | 14.8 us: 1.07x slower                                                  |
| tomli_loads          | 2.30 sec                                               | 2.49 sec: 1.08x slower                                                 |
| xml_etree_generate   | 81.1 ms                                                | 89.4 ms: 1.10x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.13 us: 1.12x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.17x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.70 ms: 1.45x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 14.2 ms: 1.34x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 117 us: 4.46x faster                                                   |
| generators                 | 74.9 ms                                                | 29.1 ms: 2.57x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 493 ms: 1.77x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.8 ms: 1.24x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.6 ms: 1.20x faster                                                  |
| async_tree_none            | 528 ms                                                 | 445 ms: 1.19x faster                                                   |
| richards_super             | 61.9 ms                                                | 55.0 ms: 1.13x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 574 ms: 1.11x faster                                                   |
| comprehensions             | 23.6 us                                                | 21.5 us: 1.10x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 452 ms: 1.09x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                 |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.07x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 588 ms: 1.07x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                                   |
| mdp                        | 2.77 sec                                               | 2.63 sec: 1.05x faster                                                 |
| sqlglot_transpile          | 1.75 ms                                                | 1.67 ms: 1.05x faster                                                  |
| logging_silent             | 111 ns                                                 | 106 ns: 1.05x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.05x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 731 ms: 1.04x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 233 us: 1.04x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.04x faster                                                   |
| richards                   | 49.8 ms                                                | 48.3 ms: 1.03x faster                                                  |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                   |
| json_loads                 | 29.2 us                                                | 28.5 us: 1.02x faster                                                  |
| pickle_dict                | 34.6 us                                                | 33.9 us: 1.02x faster                                                  |
| deepcopy                   | 365 us                                                 | 358 us: 1.02x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.15 us: 1.02x faster                                                  |
| raytrace                   | 309 ms                                                 | 304 ms: 1.01x faster                                                   |
| sympy_str                  | 297 ms                                                 | 295 ms: 1.01x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 21.4 ms: 1.00x faster                                                  |
| gc_traversal               | 4.01 ms                                                | 4.00 ms: 1.00x faster                                                  |
| deepcopy_memo              | 40.2 us                                                | 40.4 us: 1.01x slower                                                  |
| logging_simple             | 6.22 us                                                | 6.29 us: 1.01x slower                                                  |
| sympy_expand               | 484 ms                                                 | 492 ms: 1.02x slower                                                   |
| bench_thread_pool          | 834 us                                                 | 848 us: 1.02x slower                                                   |
| docutils                   | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                 |
| unpickle_list              | 5.21 us                                                | 5.32 us: 1.02x slower                                                  |
| sqlglot_normalize          | 113 ms                                                 | 115 ms: 1.02x slower                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 111 ms: 1.02x slower                                                   |
| scimark_lu                 | 116 ms                                                 | 119 ms: 1.02x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                                  |
| chaos                      | 71.9 ms                                                | 74.0 ms: 1.03x slower                                                  |
| logging_format             | 6.81 us                                                | 7.02 us: 1.03x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.26 sec: 1.06x slower                                                 |
| chameleon                  | 6.70 ms                                                | 7.11 ms: 1.06x slower                                                  |
| pickle                     | 11.0 us                                                | 11.7 us: 1.06x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 60.9 ms: 1.07x slower                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 59.3 ms: 1.07x slower                                                  |
| unpickle                   | 13.8 us                                                | 14.8 us: 1.07x slower                                                  |
| meteor_contest             | 109 ms                                                 | 117 ms: 1.07x slower                                                   |
| dulwich_log                | 64.6 ms                                                | 69.3 ms: 1.07x slower                                                  |
| scimark_sor                | 121 ms                                                 | 131 ms: 1.08x slower                                                   |
| regex_v8                   | 22.9 ms                                                | 24.7 ms: 1.08x slower                                                  |
| tomli_loads                | 2.30 sec                                               | 2.49 sec: 1.08x slower                                                 |
| regex_dna                  | 205 ms                                                 | 223 ms: 1.09x slower                                                   |
| 2to3                       | 264 ms                                                 | 288 ms: 1.09x slower                                                   |
| crypto_pyaes               | 76.7 ms                                                | 84.5 ms: 1.10x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 89.4 ms: 1.10x slower                                                  |
| nqueens                    | 87.9 ms                                                | 97.0 ms: 1.10x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.13 us: 1.12x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.91 us: 1.13x slower                                                  |
| go                         | 149 ms                                                 | 168 ms: 1.13x slower                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.80 sec: 1.16x slower                                                 |
| regex_compile              | 141 ms                                                 | 164 ms: 1.16x slower                                                   |
| pprint_safe_repr           | 747 ms                                                 | 870 ms: 1.16x slower                                                   |
| unpack_sequence            | 43.5 ns                                                | 50.9 ns: 1.17x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.17x slower                                                  |
| float                      | 78.9 ms                                                | 94.2 ms: 1.19x slower                                                  |
| fannkuch                   | 405 ms                                                 | 485 ms: 1.20x slower                                                   |
| async_generators           | 374 ms                                                 | 452 ms: 1.21x slower                                                   |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.12 ms: 1.22x slower                                                  |
| coverage                   | 78.8 ms                                                | 96.1 ms: 1.22x slower                                                  |
| deltablue                  | 3.92 ms                                                | 4.84 ms: 1.23x slower                                                  |
| nbody                      | 96.0 ms                                                | 120 ms: 1.25x slower                                                   |
| telco                      | 6.86 ms                                                | 8.67 ms: 1.26x slower                                                  |
| hexiom                     | 6.89 ms                                                | 8.74 ms: 1.27x slower                                                  |
| mypy2                      | 686 ms                                                 | 871 ms: 1.27x slower                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 90.2 ms: 1.28x slower                                                  |
| scimark_fft                | 345 ms                                                 | 458 ms: 1.33x slower                                                   |
| mako                       | 10.7 ms                                                | 14.2 ms: 1.34x slower                                                  |
| spectral_norm              | 108 ms                                                 | 146 ms: 1.35x slower                                                   |
| pyflate                    | 434 ms                                                 | 589 ms: 1.36x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.70 ms: 1.45x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (6): json, bench_mp_pool, tornado_http, asyncio_websockets, pathlib, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 97.95% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x