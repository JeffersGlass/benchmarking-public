
# Results vs. 3.11.0

- fork: mdboom
- ref: force_mimalloc
- machine: linux-x86_64
- commit hash: f8250a4
- commit date: 2024-02-14
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 258 ms: 1.02x faster                                             |
| docutils       | 2.66 sec                                               | 2.66 sec: 1.00x faster                                           |
| tornado_http   | 98.1 ms                                                | 91.7 ms: 1.07x faster                                            |
| Geometric mean | (ref)                                                  | 1.02x faster                                                     |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 473 ms: 1.12x faster                                             |
| async_tree_none_tg         | 491 ms                                                 | 481 ms: 1.02x faster                                             |
| async_tree_memoization     | 639 ms                                                 | 628 ms: 1.02x faster                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 771 ms: 1.01x slower                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 763 ms: 1.02x slower                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.34 sec: 1.04x slower                                           |
| async_tree_io              | 1.29 sec                                               | 1.34 sec: 1.04x slower                                           |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                     |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 181 ms: 1.07x faster                                             |
| nbody          | 96.0 ms                                                | 90.1 ms: 1.07x faster                                            |
| float          | 78.9 ms                                                | 80.0 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                  | 1.04x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 126 ms: 1.13x faster                                             |
| regex_effbot   | 3.51 ms                                                | 3.50 ms: 1.00x faster                                            |
| regex_dna      | 205 ms                                                 | 218 ms: 1.07x slower                                             |
| regex_v8       | 22.9 ms                                                | 24.5 ms: 1.07x slower                                            |
| Geometric mean | (ref)                                                  | 1.00x slower                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.2 ms: 1.31x faster                                            |
| unpickle_pure_python | 242 us                                                 | 213 us: 1.14x faster                                             |
| tomli_loads          | 2.30 sec                                               | 2.08 sec: 1.11x faster                                           |
| pickle_pure_python   | 320 us                                                 | 292 us: 1.10x faster                                             |
| json_loads           | 29.2 us                                                | 27.1 us: 1.08x faster                                            |
| unpickle_list        | 5.21 us                                                | 4.92 us: 1.06x faster                                            |
| xml_etree_parse      | 164 ms                                                 | 155 ms: 1.06x faster                                             |
| xml_etree_iterparse  | 108 ms                                                 | 103 ms: 1.05x faster                                             |
| pickle_dict          | 34.6 us                                                | 35.0 us: 1.01x slower                                            |
| xml_etree_process    | 56.9 ms                                                | 58.5 ms: 1.03x slower                                            |
| xml_etree_generate   | 81.1 ms                                                | 84.1 ms: 1.04x slower                                            |
| pickle               | 11.0 us                                                | 11.5 us: 1.04x slower                                            |
| pickle_list          | 4.59 us                                                | 5.11 us: 1.11x slower                                            |
| unpickle             | 13.8 us                                                | 16.1 us: 1.16x slower                                            |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                            |
| python_startup_no_site | 6.01 ms                                                | 8.70 ms: 1.45x slower                                            |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.2 ms: 1.05x faster                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 107 us: 4.86x faster                                             |
| generators                 | 74.9 ms                                                | 29.0 ms: 2.58x faster                                            |
| asyncio_tcp                | 875 ms                                                 | 498 ms: 1.76x faster                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.82 sec: 1.71x faster                                           |
| comprehensions             | 23.6 us                                                | 16.1 us: 1.47x faster                                            |
| json_dumps                 | 13.3 ms                                                | 10.2 ms: 1.31x faster                                            |
| coroutines                 | 27.0 ms                                                | 21.5 ms: 1.25x faster                                            |
| deltablue                  | 3.92 ms                                                | 3.17 ms: 1.24x faster                                            |
| chaos                      | 71.9 ms                                                | 58.3 ms: 1.23x faster                                            |
| raytrace                   | 309 ms                                                 | 259 ms: 1.19x faster                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.22 ms: 1.18x faster                                            |
| sympy_sum                  | 169 ms                                                 | 145 ms: 1.16x faster                                             |
| richards_super             | 61.9 ms                                                | 53.5 ms: 1.16x faster                                            |
| sqlglot_transpile          | 1.75 ms                                                | 1.52 ms: 1.15x faster                                            |
| logging_silent             | 111 ns                                                 | 96.9 ns: 1.15x faster                                            |
| sympy_str                  | 297 ms                                                 | 260 ms: 1.14x faster                                             |
| unpickle_pure_python       | 242 us                                                 | 213 us: 1.14x faster                                             |
| hexiom                     | 6.89 ms                                                | 6.09 ms: 1.13x faster                                            |
| regex_compile              | 141 ms                                                 | 126 ms: 1.13x faster                                             |
| nqueens                    | 87.9 ms                                                | 78.5 ms: 1.12x faster                                            |
| sympy_integrate            | 21.5 ms                                                | 19.2 ms: 1.12x faster                                            |
| async_tree_none            | 528 ms                                                 | 473 ms: 1.12x faster                                             |
| logging_simple             | 6.22 us                                                | 5.62 us: 1.11x faster                                            |
| tomli_loads                | 2.30 sec                                               | 2.08 sec: 1.11x faster                                           |
| sqlglot_normalize          | 113 ms                                                 | 102 ms: 1.11x faster                                             |
| logging_format             | 6.81 us                                                | 6.17 us: 1.10x faster                                            |
| deepcopy_memo              | 40.2 us                                                | 36.5 us: 1.10x faster                                            |
| deepcopy                   | 365 us                                                 | 332 us: 1.10x faster                                             |
| pickle_pure_python         | 320 us                                                 | 292 us: 1.10x faster                                             |
| go                         | 149 ms                                                 | 137 ms: 1.08x faster                                             |
| deepcopy_reduce            | 3.22 us                                                | 2.97 us: 1.08x faster                                            |
| sympy_expand               | 484 ms                                                 | 448 ms: 1.08x faster                                             |
| crypto_pyaes               | 76.7 ms                                                | 71.1 ms: 1.08x faster                                            |
| json_loads                 | 29.2 us                                                | 27.1 us: 1.08x faster                                            |
| pprint_pformat             | 1.55 sec                                               | 1.44 sec: 1.08x faster                                           |
| sqlglot_optimize           | 55.3 ms                                                | 51.5 ms: 1.07x faster                                            |
| pycparser                  | 1.19 sec                                               | 1.10 sec: 1.07x faster                                           |
| pathlib                    | 18.5 ms                                                | 17.3 ms: 1.07x faster                                            |
| mdp                        | 2.77 sec                                               | 2.59 sec: 1.07x faster                                           |
| pidigits                   | 194 ms                                                 | 181 ms: 1.07x faster                                             |
| gc_traversal               | 4.01 ms                                                | 3.75 ms: 1.07x faster                                            |
| spectral_norm              | 108 ms                                                 | 101 ms: 1.07x faster                                             |
| scimark_monte_carlo        | 70.7 ms                                                | 66.1 ms: 1.07x faster                                            |
| tornado_http               | 98.1 ms                                                | 91.7 ms: 1.07x faster                                            |
| unpack_sequence            | 43.5 ns                                                | 40.8 ns: 1.07x faster                                            |
| nbody                      | 96.0 ms                                                | 90.1 ms: 1.07x faster                                            |
| richards                   | 49.8 ms                                                | 46.9 ms: 1.06x faster                                            |
| unpickle_list              | 5.21 us                                                | 4.92 us: 1.06x faster                                            |
| xml_etree_parse            | 164 ms                                                 | 155 ms: 1.06x faster                                             |
| json                       | 5.24 ms                                                | 4.98 ms: 1.05x faster                                            |
| pprint_safe_repr           | 747 ms                                                 | 710 ms: 1.05x faster                                             |
| mako                       | 10.7 ms                                                | 10.2 ms: 1.05x faster                                            |
| xml_etree_iterparse        | 108 ms                                                 | 103 ms: 1.05x faster                                             |
| fannkuch                   | 405 ms                                                 | 388 ms: 1.04x faster                                             |
| scimark_sor                | 121 ms                                                 | 117 ms: 1.04x faster                                             |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.86 ms: 1.03x faster                                            |
| scimark_lu                 | 116 ms                                                 | 113 ms: 1.03x faster                                             |
| 2to3                       | 264 ms                                                 | 258 ms: 1.02x faster                                             |
| async_tree_none_tg         | 491 ms                                                 | 481 ms: 1.02x faster                                             |
| dulwich_log                | 64.6 ms                                                | 63.4 ms: 1.02x faster                                            |
| async_tree_memoization     | 639 ms                                                 | 628 ms: 1.02x faster                                             |
| asyncio_websockets         | 550 ms                                                 | 543 ms: 1.01x faster                                             |
| docutils                   | 2.66 sec                                               | 2.66 sec: 1.00x faster                                           |
| regex_effbot               | 3.51 ms                                                | 3.50 ms: 1.00x faster                                            |
| meteor_contest             | 109 ms                                                 | 109 ms: 1.00x slower                                             |
| pyflate                    | 434 ms                                                 | 438 ms: 1.01x slower                                             |
| pickle_dict                | 34.6 us                                                | 35.0 us: 1.01x slower                                            |
| float                      | 78.9 ms                                                | 80.0 ms: 1.01x slower                                            |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 771 ms: 1.01x slower                                             |
| scimark_fft                | 345 ms                                                 | 350 ms: 1.01x slower                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 763 ms: 1.02x slower                                             |
| xml_etree_process          | 56.9 ms                                                | 58.5 ms: 1.03x slower                                            |
| xml_etree_generate         | 81.1 ms                                                | 84.1 ms: 1.04x slower                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.34 sec: 1.04x slower                                           |
| async_tree_io              | 1.29 sec                                               | 1.34 sec: 1.04x slower                                           |
| pickle                     | 11.0 us                                                | 11.5 us: 1.04x slower                                            |
| sqlite_synth               | 2.57 us                                                | 2.72 us: 1.06x slower                                            |
| regex_dna                  | 205 ms                                                 | 218 ms: 1.07x slower                                             |
| regex_v8                   | 22.9 ms                                                | 24.5 ms: 1.07x slower                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.54 ms: 1.08x slower                                            |
| pickle_list                | 4.59 us                                                | 5.11 us: 1.11x slower                                            |
| unpickle                   | 13.8 us                                                | 16.1 us: 1.16x slower                                            |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                            |
| async_generators           | 374 ms                                                 | 442 ms: 1.18x slower                                             |
| telco                      | 6.86 ms                                                | 8.18 ms: 1.19x slower                                            |
| coverage                   | 78.8 ms                                                | 95.5 ms: 1.21x slower                                            |
| mypy2                      | 686 ms                                                 | 855 ms: 1.25x slower                                             |
| bench_thread_pool          | 834 us                                                 | 1.20 ms: 1.44x slower                                            |
| python_startup_no_site     | 6.01 ms                                                | 8.70 ms: 1.45x slower                                            |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                     |

Benchmark hidden because not significant (4): bench_mp_pool, async_tree_memoization_tg, chameleon, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 1.07x