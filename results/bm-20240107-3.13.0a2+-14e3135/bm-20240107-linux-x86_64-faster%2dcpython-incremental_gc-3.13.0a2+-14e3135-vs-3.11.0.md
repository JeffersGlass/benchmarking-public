
# Results vs. 3.11.0

- fork: faster-cpython
- ref: incremental_gc
- machine: linux-x86_64
- commit hash: 14e3135
- commit date: 2024-01-07
- overall geometric mean: 1.08x faster
- HPT reliability: 99.97%
- HPT 99th percentile: 1.01x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 270 ms: 1.02x slower                                                       |
| chameleon      | 6.70 ms                                                | 6.97 ms: 1.04x slower                                                      |
| docutils       | 2.66 sec                                               | 2.53 sec: 1.05x faster                                                     |
| tornado_http   | 98.1 ms                                                | 93.6 ms: 1.05x faster                                                      |
| Geometric mean | (ref)                                                  | 1.01x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.29 sec                                               | 751 ms: 1.72x faster                                                       |
| async_tree_io              | 1.29 sec                                               | 804 ms: 1.60x faster                                                       |
| async_tree_none            | 528 ms                                                 | 356 ms: 1.48x faster                                                       |
| async_tree_none_tg         | 491 ms                                                 | 347 ms: 1.42x faster                                                       |
| async_tree_memoization     | 639 ms                                                 | 459 ms: 1.39x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 456 ms: 1.37x faster                                                       |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 604 ms: 1.26x faster                                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 625 ms: 1.20x faster                                                       |
| Geometric mean             | (ref)                                                  | 1.42x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 91.6 ms: 1.05x faster                                                      |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                       |
| float          | 78.9 ms                                                | 85.8 ms: 1.09x slower                                                      |
| Geometric mean | (ref)                                                  | 1.00x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 131 ms: 1.08x faster                                                       |
| regex_effbot   | 3.51 ms                                                | 3.67 ms: 1.05x slower                                                      |
| regex_dna      | 205 ms                                                 | 227 ms: 1.11x slower                                                       |
| regex_v8       | 22.9 ms                                                | 25.5 ms: 1.11x slower                                                      |
| Geometric mean | (ref)                                                  | 1.05x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                      |
| unpickle_pure_python | 242 us                                                 | 216 us: 1.12x faster                                                       |
| pickle_pure_python   | 320 us                                                 | 298 us: 1.07x faster                                                       |
| tomli_loads          | 2.30 sec                                               | 2.17 sec: 1.06x faster                                                     |
| json_loads           | 29.2 us                                                | 28.4 us: 1.03x faster                                                      |
| pickle_dict          | 34.6 us                                                | 34.6 us: 1.00x slower                                                      |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                                      |
| unpickle_list        | 5.21 us                                                | 5.47 us: 1.05x slower                                                      |
| xml_etree_process    | 56.9 ms                                                | 60.7 ms: 1.07x slower                                                      |
| unpickle             | 13.8 us                                                | 14.9 us: 1.07x slower                                                      |
| pickle_list          | 4.59 us                                                | 5.00 us: 1.09x slower                                                      |
| xml_etree_generate   | 81.1 ms                                                | 90.2 ms: 1.11x slower                                                      |
| xml_etree_iterparse  | 108 ms                                                 | 130 ms: 1.20x slower                                                       |
| xml_etree_parse      | 164 ms                                                 | 205 ms: 1.25x slower                                                       |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                      |
| python_startup_no_site | 6.01 ms                                                | 8.55 ms: 1.42x slower                                                      |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.4 ms: 1.07x slower                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-14e3135 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 112 us: 4.64x faster                                                       |
| generators                 | 74.9 ms                                                | 29.7 ms: 2.52x faster                                                      |
| asyncio_tcp                | 875 ms                                                 | 475 ms: 1.84x faster                                                       |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.75x faster                                                     |
| async_tree_io_tg           | 1.29 sec                                               | 751 ms: 1.72x faster                                                       |
| async_tree_io              | 1.29 sec                                               | 804 ms: 1.60x faster                                                       |
| async_tree_none            | 528 ms                                                 | 356 ms: 1.48x faster                                                       |
| comprehensions             | 23.6 us                                                | 16.3 us: 1.45x faster                                                      |
| async_tree_none_tg         | 491 ms                                                 | 347 ms: 1.42x faster                                                       |
| async_tree_memoization     | 639 ms                                                 | 459 ms: 1.39x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 456 ms: 1.37x faster                                                       |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                      |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 604 ms: 1.26x faster                                                       |
| deltablue                  | 3.92 ms                                                | 3.22 ms: 1.22x faster                                                      |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 625 ms: 1.20x faster                                                       |
| chaos                      | 71.9 ms                                                | 60.1 ms: 1.20x faster                                                      |
| coroutines                 | 27.0 ms                                                | 22.9 ms: 1.18x faster                                                      |
| raytrace                   | 309 ms                                                 | 263 ms: 1.18x faster                                                       |
| richards_super             | 61.9 ms                                                | 54.0 ms: 1.15x faster                                                      |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                       |
| sqlglot_parse              | 1.43 ms                                                | 1.27 ms: 1.12x faster                                                      |
| unpickle_pure_python       | 242 us                                                 | 216 us: 1.12x faster                                                       |
| sympy_str                  | 297 ms                                                 | 267 ms: 1.12x faster                                                       |
| hexiom                     | 6.89 ms                                                | 6.20 ms: 1.11x faster                                                      |
| sqlglot_transpile          | 1.75 ms                                                | 1.59 ms: 1.10x faster                                                      |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                      |
| logging_simple             | 6.22 us                                                | 5.69 us: 1.09x faster                                                      |
| nqueens                    | 87.9 ms                                                | 80.7 ms: 1.09x faster                                                      |
| logging_format             | 6.81 us                                                | 6.30 us: 1.08x faster                                                      |
| regex_compile              | 141 ms                                                 | 131 ms: 1.08x faster                                                       |
| pickle_pure_python         | 320 us                                                 | 298 us: 1.07x faster                                                       |
| sympy_expand               | 484 ms                                                 | 453 ms: 1.07x faster                                                       |
| logging_silent             | 111 ns                                                 | 104 ns: 1.07x faster                                                       |
| crypto_pyaes               | 76.7 ms                                                | 72.0 ms: 1.06x faster                                                      |
| tomli_loads                | 2.30 sec                                               | 2.17 sec: 1.06x faster                                                     |
| go                         | 149 ms                                                 | 140 ms: 1.06x faster                                                       |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.06x faster                                                       |
| docutils                   | 2.66 sec                                               | 2.53 sec: 1.05x faster                                                     |
| deepcopy                   | 365 us                                                 | 347 us: 1.05x faster                                                       |
| nbody                      | 96.0 ms                                                | 91.6 ms: 1.05x faster                                                      |
| tornado_http               | 98.1 ms                                                | 93.6 ms: 1.05x faster                                                      |
| deepcopy_memo              | 40.2 us                                                | 38.3 us: 1.05x faster                                                      |
| richards                   | 49.8 ms                                                | 47.6 ms: 1.05x faster                                                      |
| pprint_pformat             | 1.55 sec                                               | 1.49 sec: 1.04x faster                                                     |
| unpack_sequence            | 43.5 ns                                                | 41.8 ns: 1.04x faster                                                      |
| scimark_lu                 | 116 ms                                                 | 112 ms: 1.04x faster                                                       |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                       |
| scimark_monte_carlo        | 70.7 ms                                                | 68.3 ms: 1.03x faster                                                      |
| sqlglot_optimize           | 55.3 ms                                                | 53.6 ms: 1.03x faster                                                      |
| pycparser                  | 1.19 sec                                               | 1.15 sec: 1.03x faster                                                     |
| dask                       | 365 ms                                                 | 355 ms: 1.03x faster                                                       |
| pprint_safe_repr           | 747 ms                                                 | 727 ms: 1.03x faster                                                       |
| json_loads                 | 29.2 us                                                | 28.4 us: 1.03x faster                                                      |
| deepcopy_reduce            | 3.22 us                                                | 3.13 us: 1.03x faster                                                      |
| gc_traversal               | 4.01 ms                                                | 3.93 ms: 1.02x faster                                                      |
| mdp                        | 2.77 sec                                               | 2.72 sec: 1.02x faster                                                     |
| scimark_sor                | 121 ms                                                 | 119 ms: 1.02x faster                                                       |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                                      |
| meteor_contest             | 109 ms                                                 | 108 ms: 1.01x faster                                                       |
| bench_thread_pool          | 834 us                                                 | 831 us: 1.00x faster                                                       |
| pickle_dict                | 34.6 us                                                | 34.6 us: 1.00x slower                                                      |
| create_gc_cycles           | 1.43 ms                                                | 1.44 ms: 1.00x slower                                                      |
| asyncio_websockets         | 550 ms                                                 | 553 ms: 1.00x slower                                                       |
| spectral_norm              | 108 ms                                                 | 109 ms: 1.01x slower                                                       |
| 2to3                       | 264 ms                                                 | 270 ms: 1.02x slower                                                       |
| fannkuch                   | 405 ms                                                 | 415 ms: 1.02x slower                                                       |
| dulwich_log                | 64.6 ms                                                | 66.3 ms: 1.03x slower                                                      |
| chameleon                  | 6.70 ms                                                | 6.97 ms: 1.04x slower                                                      |
| regex_effbot               | 3.51 ms                                                | 3.67 ms: 1.05x slower                                                      |
| pickle                     | 11.0 us                                                | 11.5 us: 1.05x slower                                                      |
| unpickle_list              | 5.21 us                                                | 5.47 us: 1.05x slower                                                      |
| scimark_fft                | 345 ms                                                 | 364 ms: 1.05x slower                                                       |
| xml_etree_process          | 56.9 ms                                                | 60.7 ms: 1.07x slower                                                      |
| mako                       | 10.7 ms                                                | 11.4 ms: 1.07x slower                                                      |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.07x slower                                                      |
| pyflate                    | 434 ms                                                 | 468 ms: 1.08x slower                                                       |
| float                      | 78.9 ms                                                | 85.8 ms: 1.09x slower                                                      |
| mypy2                      | 686 ms                                                 | 745 ms: 1.09x slower                                                       |
| pickle_list                | 4.59 us                                                | 5.00 us: 1.09x slower                                                      |
| sqlite_synth               | 2.57 us                                                | 2.84 us: 1.10x slower                                                      |
| regex_dna                  | 205 ms                                                 | 227 ms: 1.11x slower                                                       |
| xml_etree_generate         | 81.1 ms                                                | 90.2 ms: 1.11x slower                                                      |
| regex_v8                   | 22.9 ms                                                | 25.5 ms: 1.11x slower                                                      |
| async_generators           | 374 ms                                                 | 442 ms: 1.18x slower                                                       |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                      |
| coverage                   | 78.8 ms                                                | 94.6 ms: 1.20x slower                                                      |
| xml_etree_iterparse        | 108 ms                                                 | 130 ms: 1.20x slower                                                       |
| xml_etree_parse            | 164 ms                                                 | 205 ms: 1.25x slower                                                       |
| telco                      | 6.86 ms                                                | 8.66 ms: 1.26x slower                                                      |
| python_startup_no_site     | 6.01 ms                                                | 8.55 ms: 1.42x slower                                                      |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                               |

Benchmark hidden because not significant (3): scimark_sparse_mat_mult, json, bench_mp_pool
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.97% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 1.00x