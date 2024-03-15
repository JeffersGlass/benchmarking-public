
# Results vs. 3.11.0

- fork: faster-cpython
- ref: remove_pep_523_check
- machine: linux-x86_64
- commit hash: 42374f4
- commit date: 2024-01-17
- overall geometric mean: 1.01x faster
- HPT reliability: 91.10%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 282 ms: 1.07x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.31 ms: 1.09x slower                                                            |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 457 ms: 1.07x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 586 ms: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 90.3 ms: 1.14x slower                                                            |
| nbody          | 96.0 ms                                                | 114 ms: 1.19x slower                                                             |
| Geometric mean | (ref)                                                  | 1.10x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.52 ms: 1.00x slower                                                            |
| regex_compile  | 141 ms                                                 | 149 ms: 1.06x slower                                                             |
| regex_v8       | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                            |
| regex_dna      | 205 ms                                                 | 223 ms: 1.09x slower                                                             |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.07x faster                                                             |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| unpickle_pure_python | 242 us                                                 | 234 us: 1.03x faster                                                             |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                                            |
| unpickle_list        | 5.21 us                                                | 5.06 us: 1.03x faster                                                            |
| pickle_dict          | 34.6 us                                                | 35.0 us: 1.01x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.34 sec: 1.01x slower                                                           |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| pickle               | 11.0 us                                                | 11.6 us: 1.05x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 60.3 ms: 1.06x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 88.2 ms: 1.09x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.27 us: 1.15x slower                                                            |
| unpickle             | 13.8 us                                                | 16.4 us: 1.19x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.78 ms: 1.46x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.2 ms: 1.23x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-remove_pep_523_check-3.13.0a3+-42374f4 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 114 us: 4.55x faster                                                             |
| generators                 | 74.9 ms                                                | 29.5 ms: 2.53x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 487 ms: 1.80x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                            |
| coroutines                 | 27.0 ms                                                | 21.8 ms: 1.24x faster                                                            |
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                             |
| comprehensions             | 23.6 us                                                | 20.4 us: 1.15x faster                                                            |
| richards_super             | 61.9 ms                                                | 53.9 ms: 1.15x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.32 ms: 1.09x faster                                                            |
| logging_silent             | 111 ns                                                 | 103 ns: 1.08x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 457 ms: 1.07x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 586 ms: 1.07x faster                                                             |
| gc_traversal               | 4.01 ms                                                | 3.76 ms: 1.07x faster                                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.07x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.65 ms: 1.06x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 159 ms: 1.06x faster                                                             |
| richards                   | 49.8 ms                                                | 47.5 ms: 1.05x faster                                                            |
| raytrace                   | 309 ms                                                 | 295 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                             |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| unpickle_pure_python       | 242 us                                                 | 234 us: 1.03x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                                            |
| unpickle_list              | 5.21 us                                                | 5.06 us: 1.03x faster                                                            |
| sympy_str                  | 297 ms                                                 | 289 ms: 1.03x faster                                                             |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| logging_simple             | 6.22 us                                                | 6.05 us: 1.03x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 21.0 ms: 1.02x faster                                                            |
| deepcopy                   | 365 us                                                 | 358 us: 1.02x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.16 us: 1.02x faster                                                            |
| json                       | 5.24 ms                                                | 5.17 ms: 1.01x faster                                                            |
| logging_format             | 6.81 us                                                | 6.74 us: 1.01x faster                                                            |
| unpack_sequence            | 43.5 ns                                                | 43.1 ns: 1.01x faster                                                            |
| mdp                        | 2.77 sec                                               | 2.75 sec: 1.01x faster                                                           |
| chaos                      | 71.9 ms                                                | 71.5 ms: 1.01x faster                                                            |
| regex_effbot               | 3.51 ms                                                | 3.52 ms: 1.00x slower                                                            |
| sympy_expand               | 484 ms                                                 | 487 ms: 1.00x slower                                                             |
| sqlglot_normalize          | 113 ms                                                 | 113 ms: 1.01x slower                                                             |
| dask                       | 365 ms                                                 | 369 ms: 1.01x slower                                                             |
| pickle_dict                | 34.6 us                                                | 35.0 us: 1.01x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.01x slower                                                           |
| bench_thread_pool          | 834 us                                                 | 846 us: 1.01x slower                                                             |
| tomli_loads                | 2.30 sec                                               | 2.34 sec: 1.01x slower                                                           |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| xml_etree_iterparse        | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| scimark_lu                 | 116 ms                                                 | 118 ms: 1.02x slower                                                             |
| deepcopy_memo              | 40.2 us                                                | 41.0 us: 1.02x slower                                                            |
| meteor_contest             | 109 ms                                                 | 112 ms: 1.03x slower                                                             |
| go                         | 149 ms                                                 | 153 ms: 1.03x slower                                                             |
| nqueens                    | 87.9 ms                                                | 91.1 ms: 1.04x slower                                                            |
| sqlglot_optimize           | 55.3 ms                                                | 57.4 ms: 1.04x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                            |
| pickle                     | 11.0 us                                                | 11.6 us: 1.05x slower                                                            |
| regex_compile              | 141 ms                                                 | 149 ms: 1.06x slower                                                             |
| xml_etree_process          | 56.9 ms                                                | 60.3 ms: 1.06x slower                                                            |
| fannkuch                   | 405 ms                                                 | 431 ms: 1.06x slower                                                             |
| crypto_pyaes               | 76.7 ms                                                | 81.6 ms: 1.06x slower                                                            |
| 2to3                       | 264 ms                                                 | 282 ms: 1.07x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 69.2 ms: 1.07x slower                                                            |
| pprint_safe_repr           | 747 ms                                                 | 805 ms: 1.08x slower                                                             |
| pprint_pformat             | 1.55 sec                                               | 1.68 sec: 1.08x slower                                                           |
| scimark_sor                | 121 ms                                                 | 132 ms: 1.08x slower                                                             |
| regex_v8                   | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                            |
| xml_etree_generate         | 81.1 ms                                                | 88.2 ms: 1.09x slower                                                            |
| regex_dna                  | 205 ms                                                 | 223 ms: 1.09x slower                                                             |
| chameleon                  | 6.70 ms                                                | 7.31 ms: 1.09x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 78.9 ms: 1.12x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.88 us: 1.12x slower                                                            |
| deltablue                  | 3.92 ms                                                | 4.47 ms: 1.14x slower                                                            |
| float                      | 78.9 ms                                                | 90.3 ms: 1.14x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.27 us: 1.15x slower                                                            |
| pyflate                    | 434 ms                                                 | 504 ms: 1.16x slower                                                             |
| hexiom                     | 6.89 ms                                                | 8.05 ms: 1.17x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.93 ms: 1.18x slower                                                            |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| unpickle                   | 13.8 us                                                | 16.4 us: 1.19x slower                                                            |
| nbody                      | 96.0 ms                                                | 114 ms: 1.19x slower                                                             |
| coverage                   | 78.8 ms                                                | 96.4 ms: 1.22x slower                                                            |
| async_generators           | 374 ms                                                 | 458 ms: 1.23x slower                                                             |
| mako                       | 10.7 ms                                                | 13.2 ms: 1.23x slower                                                            |
| mypy2                      | 686 ms                                                 | 865 ms: 1.26x slower                                                             |
| telco                      | 6.86 ms                                                | 8.69 ms: 1.27x slower                                                            |
| spectral_norm              | 108 ms                                                 | 140 ms: 1.29x slower                                                             |
| scimark_fft                | 345 ms                                                 | 450 ms: 1.30x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.78 ms: 1.46x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (4): tornado_http, bench_mp_pool, asyncio_websockets, pathlib
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 91.10% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x