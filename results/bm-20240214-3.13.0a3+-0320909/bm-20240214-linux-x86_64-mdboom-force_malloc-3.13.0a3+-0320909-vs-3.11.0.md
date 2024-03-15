
# Results vs. 3.11.0

- fork: mdboom
- ref: force_malloc
- machine: linux-x86_64
- commit hash: 0320909
- commit date: 2024-02-14
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 262 ms: 1.01x faster                                           |
| chameleon      | 6.70 ms                                                | 6.82 ms: 1.02x slower                                          |
| docutils       | 2.66 sec                                               | 2.59 sec: 1.03x faster                                         |
| tornado_http   | 98.1 ms                                                | 94.8 ms: 1.03x faster                                          |
| Geometric mean | (ref)                                                  | 1.01x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 424 ms: 1.25x faster                                           |
| async_tree_memoization     | 639 ms                                                 | 553 ms: 1.15x faster                                           |
| async_tree_none_tg         | 491 ms                                                 | 427 ms: 1.15x faster                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 557 ms: 1.12x faster                                           |
| async_tree_io              | 1.29 sec                                               | 1.15 sec: 1.12x faster                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.17 sec: 1.11x faster                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 703 ms: 1.08x faster                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 697 ms: 1.07x faster                                           |
| Geometric mean             | (ref)                                                  | 1.13x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 91.9 ms: 1.04x faster                                          |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                           |
| float          | 78.9 ms                                                | 76.2 ms: 1.04x faster                                          |
| Geometric mean | (ref)                                                  | 1.04x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 127 ms: 1.11x faster                                           |
| regex_effbot   | 3.51 ms                                                | 3.67 ms: 1.05x slower                                          |
| regex_dna      | 205 ms                                                 | 220 ms: 1.08x slower                                           |
| regex_v8       | 22.9 ms                                                | 25.2 ms: 1.10x slower                                          |
| Geometric mean | (ref)                                                  | 1.03x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                          |
| unpickle_pure_python | 242 us                                                 | 212 us: 1.14x faster                                           |
| pickle_pure_python   | 320 us                                                 | 291 us: 1.10x faster                                           |
| tomli_loads          | 2.30 sec                                               | 2.13 sec: 1.08x faster                                         |
| unpickle_list        | 5.21 us                                                | 4.89 us: 1.07x faster                                          |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                           |
| json_loads           | 29.2 us                                                | 27.7 us: 1.05x faster                                          |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                           |
| pickle_dict          | 34.6 us                                                | 34.7 us: 1.00x slower                                          |
| xml_etree_process    | 56.9 ms                                                | 57.9 ms: 1.02x slower                                          |
| xml_etree_generate   | 81.1 ms                                                | 84.5 ms: 1.04x slower                                          |
| pickle               | 11.0 us                                                | 11.8 us: 1.07x slower                                          |
| unpickle             | 13.8 us                                                | 15.4 us: 1.12x slower                                          |
| pickle_list          | 4.59 us                                                | 5.13 us: 1.12x slower                                          |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                   |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                          |
| python_startup_no_site | 6.01 ms                                                | 8.70 ms: 1.45x slower                                          |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.1 ms: 1.04x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_malloc-3.13.0a3+-0320909 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 108 us: 4.83x faster                                           |
| generators                 | 74.9 ms                                                | 29.5 ms: 2.54x faster                                          |
| asyncio_tcp                | 875 ms                                                 | 484 ms: 1.81x faster                                           |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                         |
| comprehensions             | 23.6 us                                                | 15.9 us: 1.48x faster                                          |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                          |
| coroutines                 | 27.0 ms                                                | 21.5 ms: 1.26x faster                                          |
| async_tree_none            | 528 ms                                                 | 424 ms: 1.25x faster                                           |
| deltablue                  | 3.92 ms                                                | 3.16 ms: 1.24x faster                                          |
| chaos                      | 71.9 ms                                                | 59.5 ms: 1.21x faster                                          |
| raytrace                   | 309 ms                                                 | 258 ms: 1.20x faster                                           |
| richards_super             | 61.9 ms                                                | 52.7 ms: 1.17x faster                                          |
| logging_silent             | 111 ns                                                 | 95.2 ns: 1.17x faster                                          |
| async_tree_memoization     | 639 ms                                                 | 553 ms: 1.15x faster                                           |
| sqlglot_parse              | 1.43 ms                                                | 1.25 ms: 1.15x faster                                          |
| async_tree_none_tg         | 491 ms                                                 | 427 ms: 1.15x faster                                           |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                           |
| hexiom                     | 6.89 ms                                                | 6.04 ms: 1.14x faster                                          |
| unpickle_pure_python       | 242 us                                                 | 212 us: 1.14x faster                                           |
| sqlglot_transpile          | 1.75 ms                                                | 1.56 ms: 1.13x faster                                          |
| async_tree_memoization_tg  | 626 ms                                                 | 557 ms: 1.12x faster                                           |
| async_tree_io              | 1.29 sec                                               | 1.15 sec: 1.12x faster                                         |
| sympy_str                  | 297 ms                                                 | 266 ms: 1.12x faster                                           |
| logging_simple             | 6.22 us                                                | 5.56 us: 1.12x faster                                          |
| logging_format             | 6.81 us                                                | 6.09 us: 1.12x faster                                          |
| regex_compile              | 141 ms                                                 | 127 ms: 1.11x faster                                           |
| sympy_integrate            | 21.5 ms                                                | 19.4 ms: 1.11x faster                                          |
| async_tree_io_tg           | 1.29 sec                                               | 1.17 sec: 1.11x faster                                         |
| mdp                        | 2.77 sec                                               | 2.51 sec: 1.11x faster                                         |
| pickle_pure_python         | 320 us                                                 | 291 us: 1.10x faster                                           |
| go                         | 149 ms                                                 | 135 ms: 1.10x faster                                           |
| deepcopy_reduce            | 3.22 us                                                | 2.95 us: 1.09x faster                                          |
| nqueens                    | 87.9 ms                                                | 80.6 ms: 1.09x faster                                          |
| crypto_pyaes               | 76.7 ms                                                | 70.6 ms: 1.09x faster                                          |
| gc_traversal               | 4.01 ms                                                | 3.69 ms: 1.09x faster                                          |
| tomli_loads                | 2.30 sec                                               | 2.13 sec: 1.08x faster                                         |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 703 ms: 1.08x faster                                           |
| deepcopy_memo              | 40.2 us                                                | 37.1 us: 1.08x faster                                          |
| deepcopy                   | 365 us                                                 | 338 us: 1.08x faster                                           |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.66 ms: 1.08x faster                                          |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 697 ms: 1.07x faster                                           |
| sympy_expand               | 484 ms                                                 | 451 ms: 1.07x faster                                           |
| sqlglot_normalize          | 113 ms                                                 | 105 ms: 1.07x faster                                           |
| unpickle_list              | 5.21 us                                                | 4.89 us: 1.07x faster                                          |
| scimark_monte_carlo        | 70.7 ms                                                | 66.3 ms: 1.07x faster                                          |
| fannkuch                   | 405 ms                                                 | 381 ms: 1.06x faster                                           |
| richards                   | 49.8 ms                                                | 47.0 ms: 1.06x faster                                          |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                           |
| json_loads                 | 29.2 us                                                | 27.7 us: 1.05x faster                                          |
| scimark_lu                 | 116 ms                                                 | 111 ms: 1.05x faster                                           |
| bench_thread_pool          | 834 us                                                 | 798 us: 1.05x faster                                           |
| nbody                      | 96.0 ms                                                | 91.9 ms: 1.04x faster                                          |
| pprint_pformat             | 1.55 sec                                               | 1.49 sec: 1.04x faster                                         |
| sqlglot_optimize           | 55.3 ms                                                | 53.2 ms: 1.04x faster                                          |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                           |
| float                      | 78.9 ms                                                | 76.2 ms: 1.04x faster                                          |
| xml_etree_iterparse        | 108 ms                                                 | 104 ms: 1.04x faster                                           |
| tornado_http               | 98.1 ms                                                | 94.8 ms: 1.03x faster                                          |
| scimark_sor                | 121 ms                                                 | 117 ms: 1.03x faster                                           |
| json                       | 5.24 ms                                                | 5.08 ms: 1.03x faster                                          |
| docutils                   | 2.66 sec                                               | 2.59 sec: 1.03x faster                                         |
| pathlib                    | 18.5 ms                                                | 18.0 ms: 1.03x faster                                          |
| pycparser                  | 1.19 sec                                               | 1.16 sec: 1.02x faster                                         |
| pprint_safe_repr           | 747 ms                                                 | 732 ms: 1.02x faster                                           |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.02x faster                                           |
| dask                       | 365 ms                                                 | 360 ms: 1.01x faster                                           |
| 2to3                       | 264 ms                                                 | 262 ms: 1.01x faster                                           |
| pickle_dict                | 34.6 us                                                | 34.7 us: 1.00x slower                                          |
| dulwich_log                | 64.6 ms                                                | 65.2 ms: 1.01x slower                                          |
| chameleon                  | 6.70 ms                                                | 6.82 ms: 1.02x slower                                          |
| xml_etree_process          | 56.9 ms                                                | 57.9 ms: 1.02x slower                                          |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                          |
| scimark_fft                | 345 ms                                                 | 354 ms: 1.02x slower                                           |
| pyflate                    | 434 ms                                                 | 447 ms: 1.03x slower                                           |
| mako                       | 10.7 ms                                                | 11.1 ms: 1.04x slower                                          |
| xml_etree_generate         | 81.1 ms                                                | 84.5 ms: 1.04x slower                                          |
| regex_effbot               | 3.51 ms                                                | 3.67 ms: 1.05x slower                                          |
| pickle                     | 11.0 us                                                | 11.8 us: 1.07x slower                                          |
| regex_dna                  | 205 ms                                                 | 220 ms: 1.08x slower                                           |
| sqlite_synth               | 2.57 us                                                | 2.80 us: 1.09x slower                                          |
| regex_v8                   | 22.9 ms                                                | 25.2 ms: 1.10x slower                                          |
| unpickle                   | 13.8 us                                                | 15.4 us: 1.12x slower                                          |
| pickle_list                | 4.59 us                                                | 5.13 us: 1.12x slower                                          |
| unpack_sequence            | 43.5 ns                                                | 49.8 ns: 1.15x slower                                          |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                          |
| async_generators           | 374 ms                                                 | 442 ms: 1.18x slower                                           |
| telco                      | 6.86 ms                                                | 8.35 ms: 1.22x slower                                          |
| coverage                   | 78.8 ms                                                | 95.9 ms: 1.22x slower                                          |
| mypy2                      | 686 ms                                                 | 841 ms: 1.23x slower                                           |
| python_startup_no_site     | 6.01 ms                                                | 8.70 ms: 1.45x slower                                          |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                   |

Benchmark hidden because not significant (3): bench_mp_pool, asyncio_websockets, spectral_norm
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 1.00x