
# Results vs. 3.11.0

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.04x faster \*
- HPT reliability: 94.08%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 275 ms: 1.04x slower                                      |
| chameleon      | 6.70 ms                                                | 6.82 ms: 1.02x slower                                     |
| docutils       | 2.66 sec                                               | 2.63 sec: 1.01x faster                                    |
| tornado_http   | 98.1 ms                                                | 96.4 ms: 1.02x faster                                     |
| Geometric mean | (ref)                                                  | 1.01x slower                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 440 ms: 1.20x faster                                      |
| async_tree_memoization     | 639 ms                                                 | 567 ms: 1.13x faster                                      |
| async_tree_none_tg         | 491 ms                                                 | 451 ms: 1.09x faster                                      |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                    |
| async_tree_memoization_tg  | 626 ms                                                 | 581 ms: 1.08x faster                                      |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                    |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 726 ms: 1.05x faster                                      |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.05x faster                                      |
| Geometric mean             | (ref)                                                  | 1.09x faster                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                      |
| nbody          | 96.0 ms                                                | 103 ms: 1.07x slower                                      |
| float          | 78.9 ms                                                | 85.3 ms: 1.08x slower                                     |
| Geometric mean | (ref)                                                  | 1.04x slower                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 140 ms: 1.01x faster                                      |
| regex_effbot   | 3.51 ms                                                | 3.60 ms: 1.03x slower                                     |
| regex_dna      | 205 ms                                                 | 218 ms: 1.07x slower                                      |
| regex_v8       | 22.9 ms                                                | 25.4 ms: 1.11x slower                                     |
| Geometric mean | (ref)                                                  | 1.05x slower                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.29x faster                                     |
| pickle_pure_python   | 320 us                                                 | 294 us: 1.09x faster                                      |
| unpickle_pure_python | 242 us                                                 | 228 us: 1.06x faster                                      |
| xml_etree_parse      | 164 ms                                                 | 154 ms: 1.06x faster                                      |
| tomli_loads          | 2.30 sec                                               | 2.21 sec: 1.04x faster                                    |
| json_loads           | 29.2 us                                                | 28.2 us: 1.04x faster                                     |
| pickle_dict          | 34.6 us                                                | 34.0 us: 1.02x faster                                     |
| unpickle_list        | 5.21 us                                                | 5.14 us: 1.01x faster                                     |
| xml_etree_iterparse  | 108 ms                                                 | 107 ms: 1.01x faster                                      |
| xml_etree_process    | 56.9 ms                                                | 58.2 ms: 1.02x slower                                     |
| pickle               | 11.0 us                                                | 11.3 us: 1.03x slower                                     |
| xml_etree_generate   | 81.1 ms                                                | 85.7 ms: 1.06x slower                                     |
| unpickle             | 13.8 us                                                | 15.0 us: 1.09x slower                                     |
| pickle_list          | 4.59 us                                                | 5.04 us: 1.10x slower                                     |
| Geometric mean       | (ref)                                                  | 1.02x faster                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                     |
| python_startup_no_site | 6.01 ms                                                | 8.81 ms: 1.46x slower                                     |
| Geometric mean         | (ref)                                                  | 1.32x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.1 ms: 1.14x slower                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 113 us: 4.60x faster                                      |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.56x faster                                     |
| asyncio_tcp                | 875 ms                                                 | 502 ms: 1.74x faster                                      |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                    |
| comprehensions             | 23.6 us                                                | 18.1 us: 1.30x faster                                     |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.29x faster                                     |
| richards_super             | 61.9 ms                                                | 51.4 ms: 1.20x faster                                     |
| async_tree_none            | 528 ms                                                 | 440 ms: 1.20x faster                                      |
| coroutines                 | 27.0 ms                                                | 23.0 ms: 1.17x faster                                     |
| deltablue                  | 3.92 ms                                                | 3.34 ms: 1.17x faster                                     |
| gc_traversal               | 4.01 ms                                                | 3.53 ms: 1.14x faster                                     |
| async_tree_memoization     | 639 ms                                                 | 567 ms: 1.13x faster                                      |
| logging_silent             | 111 ns                                                 | 99.6 ns: 1.12x faster                                     |
| sqlglot_parse              | 1.43 ms                                                | 1.29 ms: 1.11x faster                                     |
| richards                   | 49.8 ms                                                | 45.1 ms: 1.10x faster                                     |
| raytrace                   | 309 ms                                                 | 282 ms: 1.09x faster                                      |
| logging_format             | 6.81 us                                                | 6.22 us: 1.09x faster                                     |
| pickle_pure_python         | 320 us                                                 | 294 us: 1.09x faster                                      |
| logging_simple             | 6.22 us                                                | 5.71 us: 1.09x faster                                     |
| async_tree_none_tg         | 491 ms                                                 | 451 ms: 1.09x faster                                      |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                    |
| sqlglot_transpile          | 1.75 ms                                                | 1.61 ms: 1.09x faster                                     |
| async_tree_memoization_tg  | 626 ms                                                 | 581 ms: 1.08x faster                                      |
| sympy_sum                  | 169 ms                                                 | 157 ms: 1.08x faster                                      |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                    |
| mdp                        | 2.77 sec                                               | 2.59 sec: 1.07x faster                                    |
| unpickle_pure_python       | 242 us                                                 | 228 us: 1.06x faster                                      |
| xml_etree_parse            | 164 ms                                                 | 154 ms: 1.06x faster                                      |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.06x faster                                      |
| sympy_str                  | 297 ms                                                 | 281 ms: 1.06x faster                                      |
| sympy_integrate            | 21.5 ms                                                | 20.3 ms: 1.06x faster                                     |
| deepcopy                   | 365 us                                                 | 346 us: 1.05x faster                                      |
| deepcopy_reduce            | 3.22 us                                                | 3.05 us: 1.05x faster                                     |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 726 ms: 1.05x faster                                      |
| deepcopy_memo              | 40.2 us                                                | 38.4 us: 1.05x faster                                     |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.05x faster                                      |
| tomli_loads                | 2.30 sec                                               | 2.21 sec: 1.04x faster                                    |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.04x faster                                     |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                      |
| sympy_expand               | 484 ms                                                 | 474 ms: 1.02x faster                                      |
| scimark_lu                 | 116 ms                                                 | 114 ms: 1.02x faster                                      |
| json                       | 5.24 ms                                                | 5.13 ms: 1.02x faster                                     |
| pathlib                    | 18.5 ms                                                | 18.2 ms: 1.02x faster                                     |
| pickle_dict                | 34.6 us                                                | 34.0 us: 1.02x faster                                     |
| tornado_http               | 98.1 ms                                                | 96.4 ms: 1.02x faster                                     |
| unpickle_list              | 5.21 us                                                | 5.14 us: 1.01x faster                                     |
| docutils                   | 2.66 sec                                               | 2.63 sec: 1.01x faster                                    |
| regex_compile              | 141 ms                                                 | 140 ms: 1.01x faster                                      |
| scimark_sor                | 121 ms                                                 | 120 ms: 1.01x faster                                      |
| xml_etree_iterparse        | 108 ms                                                 | 107 ms: 1.01x faster                                      |
| sqlglot_optimize           | 55.3 ms                                                | 54.7 ms: 1.01x faster                                     |
| asyncio_websockets         | 550 ms                                                 | 553 ms: 1.00x slower                                      |
| nqueens                    | 87.9 ms                                                | 89.4 ms: 1.02x slower                                     |
| chameleon                  | 6.70 ms                                                | 6.82 ms: 1.02x slower                                     |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                     |
| crypto_pyaes               | 76.7 ms                                                | 78.4 ms: 1.02x slower                                     |
| xml_etree_process          | 56.9 ms                                                | 58.2 ms: 1.02x slower                                     |
| regex_effbot               | 3.51 ms                                                | 3.60 ms: 1.03x slower                                     |
| pprint_pformat             | 1.55 sec                                               | 1.60 sec: 1.03x slower                                    |
| pprint_safe_repr           | 747 ms                                                 | 769 ms: 1.03x slower                                      |
| pickle                     | 11.0 us                                                | 11.3 us: 1.03x slower                                     |
| fannkuch                   | 405 ms                                                 | 422 ms: 1.04x slower                                      |
| 2to3                       | 264 ms                                                 | 275 ms: 1.04x slower                                      |
| dulwich_log                | 64.6 ms                                                | 67.9 ms: 1.05x slower                                     |
| scimark_monte_carlo        | 70.7 ms                                                | 74.5 ms: 1.05x slower                                     |
| xml_etree_generate         | 81.1 ms                                                | 85.7 ms: 1.06x slower                                     |
| regex_dna                  | 205 ms                                                 | 218 ms: 1.07x slower                                      |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.36 ms: 1.07x slower                                     |
| nbody                      | 96.0 ms                                                | 103 ms: 1.07x slower                                      |
| scimark_fft                | 345 ms                                                 | 371 ms: 1.07x slower                                      |
| float                      | 78.9 ms                                                | 85.3 ms: 1.08x slower                                     |
| unpickle                   | 13.8 us                                                | 15.0 us: 1.09x slower                                     |
| sqlite_synth               | 2.57 us                                                | 2.81 us: 1.09x slower                                     |
| pickle_list                | 4.59 us                                                | 5.04 us: 1.10x slower                                     |
| regex_v8                   | 22.9 ms                                                | 25.4 ms: 1.11x slower                                     |
| hexiom                     | 6.89 ms                                                | 7.68 ms: 1.11x slower                                     |
| mako                       | 10.7 ms                                                | 12.1 ms: 1.14x slower                                     |
| pyflate                    | 434 ms                                                 | 506 ms: 1.17x slower                                      |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                     |
| unpack_sequence            | 43.5 ns                                                | 52.7 ns: 1.21x slower                                     |
| async_generators           | 374 ms                                                 | 456 ms: 1.22x slower                                      |
| spectral_norm              | 108 ms                                                 | 132 ms: 1.22x slower                                      |
| coverage                   | 78.8 ms                                                | 96.8 ms: 1.23x slower                                     |
| telco                      | 6.86 ms                                                | 8.50 ms: 1.24x slower                                     |
| mypy2                      | 686 ms                                                 | 869 ms: 1.27x slower                                      |
| python_startup_no_site     | 6.01 ms                                                | 8.81 ms: 1.46x slower                                     |
| Geometric mean             | (ref)                                                  | 1.04x faster                                              |

Benchmark hidden because not significant (7): chaos, dask, pycparser, bench_mp_pool, meteor_contest, bench_thread_pool, go
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 94.08% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x