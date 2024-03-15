
# Results vs. 3.11.0

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 262 ms: 1.01x faster                                      |
| docutils       | 2.66 sec                                               | 2.56 sec: 1.04x faster                                    |
| tornado_http   | 98.1 ms                                                | 94.3 ms: 1.04x faster                                     |
| Geometric mean | (ref)                                                  | 1.02x faster                                              |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 431 ms: 1.22x faster                                      |
| async_tree_memoization     | 639 ms                                                 | 555 ms: 1.15x faster                                      |
| async_tree_none_tg         | 491 ms                                                 | 442 ms: 1.11x faster                                      |
| async_tree_memoization_tg  | 626 ms                                                 | 565 ms: 1.11x faster                                      |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                    |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.09x faster                                    |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 701 ms: 1.07x faster                                      |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 714 ms: 1.07x faster                                      |
| Geometric mean             | (ref)                                                  | 1.11x faster                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.7 ms: 1.08x faster                                     |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                      |
| Geometric mean | (ref)                                                  | 1.04x faster                                              |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 127 ms: 1.11x faster                                      |
| regex_effbot   | 3.51 ms                                                | 3.61 ms: 1.03x slower                                     |
| regex_v8       | 22.9 ms                                                | 23.8 ms: 1.04x slower                                     |
| regex_dna      | 205 ms                                                 | 223 ms: 1.09x slower                                      |
| Geometric mean | (ref)                                                  | 1.01x slower                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.29x faster                                     |
| unpickle_pure_python | 242 us                                                 | 210 us: 1.15x faster                                      |
| tomli_loads          | 2.30 sec                                               | 2.09 sec: 1.10x faster                                    |
| pickle_pure_python   | 320 us                                                 | 293 us: 1.09x faster                                      |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                      |
| unpickle_list        | 5.21 us                                                | 4.98 us: 1.05x faster                                     |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                     |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                      |
| pickle_dict          | 34.6 us                                                | 34.0 us: 1.02x faster                                     |
| xml_etree_process    | 56.9 ms                                                | 57.8 ms: 1.02x slower                                     |
| xml_etree_generate   | 81.1 ms                                                | 84.5 ms: 1.04x slower                                     |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                     |
| pickle_list          | 4.59 us                                                | 4.92 us: 1.07x slower                                     |
| unpickle             | 13.8 us                                                | 15.8 us: 1.14x slower                                     |
| Geometric mean       | (ref)                                                  | 1.03x faster                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                     |
| python_startup_no_site | 6.01 ms                                                | 8.78 ms: 1.46x slower                                     |
| Geometric mean         | (ref)                                                  | 1.32x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.1 ms: 1.04x slower                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 108 us: 4.80x faster                                      |
| generators                 | 74.9 ms                                                | 28.9 ms: 2.59x faster                                     |
| asyncio_tcp                | 875 ms                                                 | 484 ms: 1.81x faster                                      |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                    |
| comprehensions             | 23.6 us                                                | 16.0 us: 1.48x faster                                     |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.29x faster                                     |
| deltablue                  | 3.92 ms                                                | 3.19 ms: 1.23x faster                                     |
| async_tree_none            | 528 ms                                                 | 431 ms: 1.22x faster                                      |
| chaos                      | 71.9 ms                                                | 58.8 ms: 1.22x faster                                     |
| coroutines                 | 27.0 ms                                                | 22.5 ms: 1.20x faster                                     |
| raytrace                   | 309 ms                                                 | 260 ms: 1.19x faster                                      |
| logging_silent             | 111 ns                                                 | 94.7 ns: 1.17x faster                                     |
| richards_super             | 61.9 ms                                                | 52.8 ms: 1.17x faster                                     |
| hexiom                     | 6.89 ms                                                | 5.91 ms: 1.16x faster                                     |
| sqlglot_parse              | 1.43 ms                                                | 1.24 ms: 1.15x faster                                     |
| unpickle_pure_python       | 242 us                                                 | 210 us: 1.15x faster                                      |
| async_tree_memoization     | 639 ms                                                 | 555 ms: 1.15x faster                                      |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                      |
| nqueens                    | 87.9 ms                                                | 77.9 ms: 1.13x faster                                     |
| sqlglot_transpile          | 1.75 ms                                                | 1.55 ms: 1.13x faster                                     |
| sympy_str                  | 297 ms                                                 | 264 ms: 1.13x faster                                      |
| regex_compile              | 141 ms                                                 | 127 ms: 1.11x faster                                      |
| async_tree_none_tg         | 491 ms                                                 | 442 ms: 1.11x faster                                      |
| logging_simple             | 6.22 us                                                | 5.61 us: 1.11x faster                                     |
| sympy_integrate            | 21.5 ms                                                | 19.4 ms: 1.11x faster                                     |
| logging_format             | 6.81 us                                                | 6.14 us: 1.11x faster                                     |
| async_tree_memoization_tg  | 626 ms                                                 | 565 ms: 1.11x faster                                      |
| tomli_loads                | 2.30 sec                                               | 2.09 sec: 1.10x faster                                    |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.56 ms: 1.10x faster                                     |
| deepcopy_memo              | 40.2 us                                                | 36.4 us: 1.10x faster                                     |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                    |
| pickle_pure_python         | 320 us                                                 | 293 us: 1.09x faster                                      |
| async_tree_io_tg           | 1.29 sec                                               | 1.18 sec: 1.09x faster                                    |
| crypto_pyaes               | 76.7 ms                                                | 70.6 ms: 1.09x faster                                     |
| sympy_expand               | 484 ms                                                 | 447 ms: 1.08x faster                                      |
| nbody                      | 96.0 ms                                                | 88.7 ms: 1.08x faster                                     |
| deepcopy                   | 365 us                                                 | 338 us: 1.08x faster                                      |
| sqlglot_normalize          | 113 ms                                                 | 104 ms: 1.08x faster                                      |
| deepcopy_reduce            | 3.22 us                                                | 2.99 us: 1.08x faster                                     |
| scimark_monte_carlo        | 70.7 ms                                                | 65.9 ms: 1.07x faster                                     |
| go                         | 149 ms                                                 | 139 ms: 1.07x faster                                      |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 701 ms: 1.07x faster                                      |
| richards                   | 49.8 ms                                                | 46.7 ms: 1.07x faster                                     |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 714 ms: 1.07x faster                                      |
| gc_traversal               | 4.01 ms                                                | 3.78 ms: 1.06x faster                                     |
| pprint_pformat             | 1.55 sec                                               | 1.47 sec: 1.06x faster                                    |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                      |
| unpickle_list              | 5.21 us                                                | 4.98 us: 1.05x faster                                     |
| scimark_lu                 | 116 ms                                                 | 111 ms: 1.05x faster                                      |
| sqlglot_optimize           | 55.3 ms                                                | 52.9 ms: 1.05x faster                                     |
| docutils                   | 2.66 sec                                               | 2.56 sec: 1.04x faster                                    |
| fannkuch                   | 405 ms                                                 | 390 ms: 1.04x faster                                      |
| tornado_http               | 98.1 ms                                                | 94.3 ms: 1.04x faster                                     |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                      |
| pprint_safe_repr           | 747 ms                                                 | 721 ms: 1.04x faster                                      |
| pycparser                  | 1.19 sec                                               | 1.15 sec: 1.04x faster                                    |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                     |
| xml_etree_iterparse        | 108 ms                                                 | 105 ms: 1.03x faster                                      |
| json                       | 5.24 ms                                                | 5.10 ms: 1.03x faster                                     |
| pathlib                    | 18.5 ms                                                | 18.1 ms: 1.02x faster                                     |
| bench_thread_pool          | 834 us                                                 | 816 us: 1.02x faster                                      |
| mdp                        | 2.77 sec                                               | 2.72 sec: 1.02x faster                                    |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.02x faster                                      |
| dask                       | 365 ms                                                 | 359 ms: 1.02x faster                                      |
| pickle_dict                | 34.6 us                                                | 34.0 us: 1.02x faster                                     |
| 2to3                       | 264 ms                                                 | 262 ms: 1.01x faster                                      |
| dulwich_log                | 64.6 ms                                                | 65.1 ms: 1.01x slower                                     |
| xml_etree_process          | 56.9 ms                                                | 57.8 ms: 1.02x slower                                     |
| spectral_norm              | 108 ms                                                 | 110 ms: 1.02x slower                                      |
| scimark_fft                | 345 ms                                                 | 352 ms: 1.02x slower                                      |
| regex_effbot               | 3.51 ms                                                | 3.61 ms: 1.03x slower                                     |
| regex_v8                   | 22.9 ms                                                | 23.8 ms: 1.04x slower                                     |
| mako                       | 10.7 ms                                                | 11.1 ms: 1.04x slower                                     |
| xml_etree_generate         | 81.1 ms                                                | 84.5 ms: 1.04x slower                                     |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                     |
| scimark_sor                | 121 ms                                                 | 129 ms: 1.06x slower                                      |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                     |
| pickle_list                | 4.59 us                                                | 4.92 us: 1.07x slower                                     |
| pyflate                    | 434 ms                                                 | 466 ms: 1.07x slower                                      |
| sqlite_synth               | 2.57 us                                                | 2.77 us: 1.08x slower                                     |
| regex_dna                  | 205 ms                                                 | 223 ms: 1.09x slower                                      |
| unpickle                   | 13.8 us                                                | 15.8 us: 1.14x slower                                     |
| unpack_sequence            | 43.5 ns                                                | 50.1 ns: 1.15x slower                                     |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                     |
| async_generators           | 374 ms                                                 | 448 ms: 1.20x slower                                      |
| telco                      | 6.86 ms                                                | 8.23 ms: 1.20x slower                                     |
| coverage                   | 78.8 ms                                                | 95.2 ms: 1.21x slower                                     |
| mypy2                      | 686 ms                                                 | 842 ms: 1.23x slower                                      |
| python_startup_no_site     | 6.01 ms                                                | 8.78 ms: 1.46x slower                                     |
| Geometric mean             | (ref)                                                  | 1.08x faster                                              |

Benchmark hidden because not significant (4): chameleon, bench_mp_pool, asyncio_websockets, float
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 0.98x