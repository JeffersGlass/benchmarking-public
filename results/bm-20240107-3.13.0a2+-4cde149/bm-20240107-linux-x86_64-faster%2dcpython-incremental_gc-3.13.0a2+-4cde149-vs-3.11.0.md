
# Results vs. 3.11.0

- fork: faster-cpython
- ref: incremental_gc
- machine: linux-x86_64
- commit hash: 4cde149
- commit date: 2024-01-07
- overall geometric mean: 1.08x faster
- HPT reliability: 99.84%
- HPT 99th percentile: 1.01x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 270 ms: 1.02x slower                                                       |
| chameleon      | 6.70 ms                                                | 7.02 ms: 1.05x slower                                                      |
| docutils       | 2.66 sec                                               | 2.53 sec: 1.05x faster                                                     |
| tornado_http   | 98.1 ms                                                | 93.6 ms: 1.05x faster                                                      |
| Geometric mean | (ref)                                                  | 1.01x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.29 sec                                               | 760 ms: 1.70x faster                                                       |
| async_tree_io              | 1.29 sec                                               | 806 ms: 1.60x faster                                                       |
| async_tree_none            | 528 ms                                                 | 358 ms: 1.48x faster                                                       |
| async_tree_none_tg         | 491 ms                                                 | 349 ms: 1.41x faster                                                       |
| async_tree_memoization     | 639 ms                                                 | 463 ms: 1.38x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 459 ms: 1.36x faster                                                       |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 607 ms: 1.25x faster                                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 631 ms: 1.19x faster                                                       |
| Geometric mean             | (ref)                                                  | 1.41x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 91.9 ms: 1.04x faster                                                      |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                       |
| float          | 78.9 ms                                                | 86.6 ms: 1.10x slower                                                      |
| Geometric mean | (ref)                                                  | 1.00x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 133 ms: 1.06x faster                                                       |
| regex_effbot   | 3.51 ms                                                | 3.78 ms: 1.08x slower                                                      |
| regex_dna      | 205 ms                                                 | 223 ms: 1.09x slower                                                       |
| regex_v8       | 22.9 ms                                                | 26.0 ms: 1.14x slower                                                      |
| Geometric mean | (ref)                                                  | 1.06x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                      |
| unpickle_pure_python | 242 us                                                 | 216 us: 1.12x faster                                                       |
| tomli_loads          | 2.30 sec                                               | 2.15 sec: 1.07x faster                                                     |
| pickle_pure_python   | 320 us                                                 | 299 us: 1.07x faster                                                       |
| json_loads           | 29.2 us                                                | 28.2 us: 1.03x faster                                                      |
| pickle_dict          | 34.6 us                                                | 34.5 us: 1.00x faster                                                      |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                                      |
| unpickle_list        | 5.21 us                                                | 5.49 us: 1.05x slower                                                      |
| xml_etree_process    | 56.9 ms                                                | 61.1 ms: 1.07x slower                                                      |
| pickle_list          | 4.59 us                                                | 4.97 us: 1.08x slower                                                      |
| unpickle             | 13.8 us                                                | 15.1 us: 1.09x slower                                                      |
| xml_etree_generate   | 81.1 ms                                                | 90.5 ms: 1.12x slower                                                      |
| xml_etree_iterparse  | 108 ms                                                 | 132 ms: 1.22x slower                                                       |
| xml_etree_parse      | 164 ms                                                 | 207 ms: 1.26x slower                                                       |
| Geometric mean       | (ref)                                                  | 1.03x slower                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                      |
| python_startup_no_site | 6.01 ms                                                | 8.56 ms: 1.42x slower                                                      |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.4 ms: 1.07x slower                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240107-linux-x86_64-faster%2dcpython-incremental_gc-3.13.0a2+-4cde149 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 115 us: 4.52x faster                                                       |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                                      |
| asyncio_tcp                | 875 ms                                                 | 483 ms: 1.81x faster                                                       |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.74x faster                                                     |
| async_tree_io_tg           | 1.29 sec                                               | 760 ms: 1.70x faster                                                       |
| async_tree_io              | 1.29 sec                                               | 806 ms: 1.60x faster                                                       |
| async_tree_none            | 528 ms                                                 | 358 ms: 1.48x faster                                                       |
| comprehensions             | 23.6 us                                                | 16.3 us: 1.45x faster                                                      |
| async_tree_none_tg         | 491 ms                                                 | 349 ms: 1.41x faster                                                       |
| async_tree_memoization     | 639 ms                                                 | 463 ms: 1.38x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 459 ms: 1.36x faster                                                       |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                      |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 607 ms: 1.25x faster                                                       |
| chaos                      | 71.9 ms                                                | 58.8 ms: 1.22x faster                                                      |
| deltablue                  | 3.92 ms                                                | 3.23 ms: 1.21x faster                                                      |
| coroutines                 | 27.0 ms                                                | 22.7 ms: 1.19x faster                                                      |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 631 ms: 1.19x faster                                                       |
| raytrace                   | 309 ms                                                 | 261 ms: 1.18x faster                                                       |
| sqlglot_parse              | 1.43 ms                                                | 1.25 ms: 1.15x faster                                                      |
| richards_super             | 61.9 ms                                                | 54.0 ms: 1.14x faster                                                      |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                       |
| sqlglot_transpile          | 1.75 ms                                                | 1.56 ms: 1.12x faster                                                      |
| hexiom                     | 6.89 ms                                                | 6.15 ms: 1.12x faster                                                      |
| unpickle_pure_python       | 242 us                                                 | 216 us: 1.12x faster                                                       |
| sympy_str                  | 297 ms                                                 | 270 ms: 1.10x faster                                                       |
| sympy_integrate            | 21.5 ms                                                | 19.6 ms: 1.09x faster                                                      |
| logging_simple             | 6.22 us                                                | 5.71 us: 1.09x faster                                                      |
| mdp                        | 2.77 sec                                               | 2.55 sec: 1.09x faster                                                     |
| logging_silent             | 111 ns                                                 | 103 ns: 1.08x faster                                                       |
| logging_format             | 6.81 us                                                | 6.29 us: 1.08x faster                                                      |
| nqueens                    | 87.9 ms                                                | 81.1 ms: 1.08x faster                                                      |
| go                         | 149 ms                                                 | 138 ms: 1.07x faster                                                       |
| tomli_loads                | 2.30 sec                                               | 2.15 sec: 1.07x faster                                                     |
| pickle_pure_python         | 320 us                                                 | 299 us: 1.07x faster                                                       |
| regex_compile              | 141 ms                                                 | 133 ms: 1.06x faster                                                       |
| sympy_expand               | 484 ms                                                 | 456 ms: 1.06x faster                                                       |
| crypto_pyaes               | 76.7 ms                                                | 72.3 ms: 1.06x faster                                                      |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.06x faster                                                       |
| docutils                   | 2.66 sec                                               | 2.53 sec: 1.05x faster                                                     |
| deepcopy_memo              | 40.2 us                                                | 38.3 us: 1.05x faster                                                      |
| gc_traversal               | 4.01 ms                                                | 3.82 ms: 1.05x faster                                                      |
| tornado_http               | 98.1 ms                                                | 93.6 ms: 1.05x faster                                                      |
| deepcopy                   | 365 us                                                 | 349 us: 1.05x faster                                                       |
| pprint_pformat             | 1.55 sec                                               | 1.49 sec: 1.04x faster                                                     |
| nbody                      | 96.0 ms                                                | 91.9 ms: 1.04x faster                                                      |
| richards                   | 49.8 ms                                                | 47.7 ms: 1.04x faster                                                      |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                       |
| scimark_monte_carlo        | 70.7 ms                                                | 68.4 ms: 1.03x faster                                                      |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.03x faster                                                      |
| deepcopy_reduce            | 3.22 us                                                | 3.11 us: 1.03x faster                                                      |
| scimark_lu                 | 116 ms                                                 | 113 ms: 1.03x faster                                                       |
| sqlglot_optimize           | 55.3 ms                                                | 53.6 ms: 1.03x faster                                                      |
| pprint_safe_repr           | 747 ms                                                 | 727 ms: 1.03x faster                                                       |
| dask                       | 365 ms                                                 | 356 ms: 1.03x faster                                                       |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.93 ms: 1.02x faster                                                      |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                                      |
| json                       | 5.24 ms                                                | 5.18 ms: 1.01x faster                                                      |
| scimark_sor                | 121 ms                                                 | 120 ms: 1.01x faster                                                       |
| pickle_dict                | 34.6 us                                                | 34.5 us: 1.00x faster                                                      |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                       |
| bench_thread_pool          | 834 us                                                 | 837 us: 1.00x slower                                                       |
| create_gc_cycles           | 1.43 ms                                                | 1.44 ms: 1.01x slower                                                      |
| meteor_contest             | 109 ms                                                 | 110 ms: 1.01x slower                                                       |
| 2to3                       | 264 ms                                                 | 270 ms: 1.02x slower                                                       |
| dulwich_log                | 64.6 ms                                                | 66.5 ms: 1.03x slower                                                      |
| fannkuch                   | 405 ms                                                 | 420 ms: 1.04x slower                                                       |
| spectral_norm              | 108 ms                                                 | 113 ms: 1.05x slower                                                       |
| chameleon                  | 6.70 ms                                                | 7.02 ms: 1.05x slower                                                      |
| pickle                     | 11.0 us                                                | 11.5 us: 1.05x slower                                                      |
| unpickle_list              | 5.21 us                                                | 5.49 us: 1.05x slower                                                      |
| mako                       | 10.7 ms                                                | 11.4 ms: 1.07x slower                                                      |
| scimark_fft                | 345 ms                                                 | 370 ms: 1.07x slower                                                       |
| pyflate                    | 434 ms                                                 | 466 ms: 1.07x slower                                                       |
| xml_etree_process          | 56.9 ms                                                | 61.1 ms: 1.07x slower                                                      |
| regex_effbot               | 3.51 ms                                                | 3.78 ms: 1.08x slower                                                      |
| pickle_list                | 4.59 us                                                | 4.97 us: 1.08x slower                                                      |
| mypy2                      | 686 ms                                                 | 748 ms: 1.09x slower                                                       |
| regex_dna                  | 205 ms                                                 | 223 ms: 1.09x slower                                                       |
| unpickle                   | 13.8 us                                                | 15.1 us: 1.09x slower                                                      |
| float                      | 78.9 ms                                                | 86.6 ms: 1.10x slower                                                      |
| sqlite_synth               | 2.57 us                                                | 2.86 us: 1.11x slower                                                      |
| xml_etree_generate         | 81.1 ms                                                | 90.5 ms: 1.12x slower                                                      |
| regex_v8                   | 22.9 ms                                                | 26.0 ms: 1.14x slower                                                      |
| unpack_sequence            | 43.5 ns                                                | 50.4 ns: 1.16x slower                                                      |
| async_generators           | 374 ms                                                 | 436 ms: 1.17x slower                                                       |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                      |
| coverage                   | 78.8 ms                                                | 95.9 ms: 1.22x slower                                                      |
| xml_etree_iterparse        | 108 ms                                                 | 132 ms: 1.22x slower                                                       |
| telco                      | 6.86 ms                                                | 8.44 ms: 1.23x slower                                                      |
| xml_etree_parse            | 164 ms                                                 | 207 ms: 1.26x slower                                                       |
| python_startup_no_site     | 6.01 ms                                                | 8.56 ms: 1.42x slower                                                      |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                               |

Benchmark hidden because not significant (2): bench_mp_pool, pycparser
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.84% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 1.00x