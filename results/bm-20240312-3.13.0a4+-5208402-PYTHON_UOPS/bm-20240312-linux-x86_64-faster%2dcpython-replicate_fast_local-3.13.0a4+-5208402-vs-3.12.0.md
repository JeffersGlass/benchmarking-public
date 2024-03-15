# Results vs. 3.12.0

- fork: faster-cpython
- ref: replicate_fast_local
- machine: linux-x86_64
- commit hash: 5208402
- commit date: 2024-03-12
- overall geometric mean: 1.07x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 301 ms: 1.10x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.08 ms: 1.05x faster                                                            |
| docutils       | 2.77 sec                                               | 2.89 sec: 1.04x slower                                                           |
| Geometric mean | (ref)                                                  | 1.03x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 461 ms: 1.02x faster                                                             |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 742 ms: 1.02x slower                                                             |
| async_tree_memoization     | 578 ms                                                 | 592 ms: 1.02x slower                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 750 ms: 1.03x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 470 ms: 1.05x slower                                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 602 ms: 1.05x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.24 sec: 1.07x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 192 ms: 1.02x slower                                                             |
| float          | 84.7 ms                                                | 94.6 ms: 1.12x slower                                                            |
| nbody          | 97.0 ms                                                | 124 ms: 1.28x slower                                                             |
| Geometric mean | (ref)                                                  | 1.13x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.71 ms: 1.03x slower                                                            |
| regex_dna      | 212 ms                                                 | 221 ms: 1.04x slower                                                             |
| regex_v8       | 23.1 ms                                                | 24.6 ms: 1.07x slower                                                            |
| regex_compile  | 148 ms                                                 | 179 ms: 1.21x slower                                                             |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                | 5.06 us: 1.05x faster                                                            |
| pickle_pure_python   | 324 us                                                 | 311 us: 1.04x faster                                                             |
| pickle_dict          | 35.5 us                                                | 34.4 us: 1.03x faster                                                            |
| json_loads           | 28.5 us                                                | 28.3 us: 1.01x faster                                                            |
| pickle_list          | 5.08 us                                                | 5.06 us: 1.01x faster                                                            |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 161 ms: 1.01x slower                                                             |
| xml_etree_process    | 61.7 ms                                                | 63.5 ms: 1.03x slower                                                            |
| json_dumps           | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                            |
| xml_etree_generate   | 89.2 ms                                                | 92.7 ms: 1.04x slower                                                            |
| xml_etree_iterparse  | 107 ms                                                 | 112 ms: 1.05x slower                                                             |
| tomli_loads          | 2.33 sec                                               | 2.55 sec: 1.09x slower                                                           |
| unpickle_pure_python | 230 us                                                 | 277 us: 1.21x slower                                                             |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.99 ms: 1.30x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.19x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| django_template | 34.6 ms                                                | 35.0 ms: 1.01x slower                                                            |
| mako            | 11.9 ms                                                | 12.8 ms: 1.08x slower                                                            |
| Geometric mean  | (ref)                                                  | 1.04x slower                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 115 us: 1.37x faster                                                             |
| deepcopy_reduce            | 3.35 us                                                | 3.11 us: 1.08x faster                                                            |
| chameleon                  | 7.41 ms                                                | 7.08 ms: 1.05x faster                                                            |
| unpickle_list              | 5.29 us                                                | 5.06 us: 1.05x faster                                                            |
| pickle_pure_python         | 324 us                                                 | 311 us: 1.04x faster                                                             |
| pickle_dict                | 35.5 us                                                | 34.4 us: 1.03x faster                                                            |
| generators                 | 31.2 ms                                                | 30.3 ms: 1.03x faster                                                            |
| deepcopy                   | 371 us                                                 | 362 us: 1.03x faster                                                             |
| logging_silent             | 104 ns                                                 | 102 ns: 1.02x faster                                                             |
| comprehensions             | 21.8 us                                                | 21.3 us: 1.02x faster                                                            |
| async_tree_none            | 472 ms                                                 | 461 ms: 1.02x faster                                                             |
| logging_format             | 7.23 us                                                | 7.07 us: 1.02x faster                                                            |
| logging_simple             | 6.46 us                                                | 6.34 us: 1.02x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 167 ms: 1.01x faster                                                             |
| json_loads                 | 28.5 us                                                | 28.3 us: 1.01x faster                                                            |
| pickle_list                | 5.08 us                                                | 5.06 us: 1.01x faster                                                            |
| pickle                     | 11.6 us                                                | 11.5 us: 1.01x faster                                                            |
| sympy_integrate            | 21.4 ms                                                | 21.6 ms: 1.01x slower                                                            |
| xml_etree_parse            | 159 ms                                                 | 161 ms: 1.01x slower                                                             |
| django_template            | 34.6 ms                                                | 35.0 ms: 1.01x slower                                                            |
| dask                       | 372 ms                                                 | 377 ms: 1.02x slower                                                             |
| sympy_str                  | 300 ms                                                 | 304 ms: 1.02x slower                                                             |
| deepcopy_memo              | 40.7 us                                                | 41.5 us: 1.02x slower                                                            |
| asyncio_websockets         | 551 ms                                                 | 563 ms: 1.02x slower                                                             |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 742 ms: 1.02x slower                                                             |
| pidigits                   | 187 ms                                                 | 192 ms: 1.02x slower                                                             |
| sqlglot_normalize          | 110 ms                                                 | 113 ms: 1.02x slower                                                             |
| async_tree_memoization     | 578 ms                                                 | 592 ms: 1.02x slower                                                             |
| mdp                        | 2.63 sec                                               | 2.70 sec: 1.03x slower                                                           |
| regex_effbot               | 3.61 ms                                                | 3.71 ms: 1.03x slower                                                            |
| xml_etree_process          | 61.7 ms                                                | 63.5 ms: 1.03x slower                                                            |
| json_dumps                 | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                            |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 750 ms: 1.03x slower                                                             |
| asyncio_tcp                | 491 ms                                                 | 507 ms: 1.03x slower                                                             |
| bench_thread_pool          | 842 us                                                 | 874 us: 1.04x slower                                                             |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.86 sec: 1.04x slower                                                           |
| xml_etree_generate         | 89.2 ms                                                | 92.7 ms: 1.04x slower                                                            |
| create_gc_cycles           | 1.48 ms                                                | 1.54 ms: 1.04x slower                                                            |
| docutils                   | 2.77 sec                                               | 2.89 sec: 1.04x slower                                                           |
| regex_dna                  | 212 ms                                                 | 221 ms: 1.04x slower                                                             |
| sqlite_synth               | 2.83 us                                                | 2.96 us: 1.05x slower                                                            |
| async_generators           | 463 ms                                                 | 484 ms: 1.05x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 470 ms: 1.05x slower                                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 602 ms: 1.05x slower                                                             |
| crypto_pyaes               | 81.9 ms                                                | 85.8 ms: 1.05x slower                                                            |
| deltablue                  | 3.72 ms                                                | 3.90 ms: 1.05x slower                                                            |
| xml_etree_iterparse        | 107 ms                                                 | 112 ms: 1.05x slower                                                             |
| meteor_contest             | 112 ms                                                 | 119 ms: 1.06x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.25 sec: 1.06x slower                                                           |
| gunicorn                   | 1.24 ms                                                | 1.32 ms: 1.06x slower                                                            |
| sqlglot_transpile          | 1.68 ms                                                | 1.79 ms: 1.06x slower                                                            |
| sqlglot_parse              | 1.36 ms                                                | 1.45 ms: 1.06x slower                                                            |
| aiohttp                    | 1.15 ms                                                | 1.22 ms: 1.06x slower                                                            |
| coroutines                 | 23.2 ms                                                | 24.7 ms: 1.06x slower                                                            |
| regex_v8                   | 23.1 ms                                                | 24.6 ms: 1.07x slower                                                            |
| async_tree_io              | 1.16 sec                                               | 1.24 sec: 1.07x slower                                                           |
| dulwich_log                | 68.5 ms                                                | 73.7 ms: 1.08x slower                                                            |
| mako                       | 11.9 ms                                                | 12.8 ms: 1.08x slower                                                            |
| sympy_expand               | 478 ms                                                 | 517 ms: 1.08x slower                                                             |
| python_startup             | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                            |
| tomli_loads                | 2.33 sec                                               | 2.55 sec: 1.09x slower                                                           |
| raytrace                   | 312 ms                                                 | 343 ms: 1.10x slower                                                             |
| 2to3                       | 274 ms                                                 | 301 ms: 1.10x slower                                                             |
| pycparser                  | 1.18 sec                                               | 1.30 sec: 1.10x slower                                                           |
| mypy2                      | 830 ms                                                 | 922 ms: 1.11x slower                                                             |
| sqlglot_optimize           | 54.8 ms                                                | 61.2 ms: 1.12x slower                                                            |
| float                      | 84.7 ms                                                | 94.6 ms: 1.12x slower                                                            |
| pprint_safe_repr           | 776 ms                                                 | 885 ms: 1.14x slower                                                             |
| chaos                      | 67.0 ms                                                | 76.6 ms: 1.14x slower                                                            |
| unpack_sequence            | 54.0 ns                                                | 62.0 ns: 1.15x slower                                                            |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 5.91 ms: 1.17x slower                                                            |
| fannkuch                   | 417 ms                                                 | 490 ms: 1.17x slower                                                             |
| scimark_monte_carlo        | 75.1 ms                                                | 88.3 ms: 1.18x slower                                                            |
| pprint_pformat             | 1.57 sec                                               | 1.85 sec: 1.18x slower                                                           |
| scimark_sor                | 129 ms                                                 | 154 ms: 1.19x slower                                                             |
| scimark_fft                | 382 ms                                                 | 459 ms: 1.20x slower                                                             |
| unpickle_pure_python       | 230 us                                                 | 277 us: 1.21x slower                                                             |
| regex_compile              | 148 ms                                                 | 179 ms: 1.21x slower                                                             |
| richards_super             | 51.5 ms                                                | 62.7 ms: 1.22x slower                                                            |
| nqueens                    | 83.3 ms                                                | 101 ms: 1.22x slower                                                             |
| richards                   | 45.8 ms                                                | 56.1 ms: 1.22x slower                                                            |
| pyflate                    | 482 ms                                                 | 594 ms: 1.23x slower                                                             |
| spectral_norm              | 115 ms                                                 | 142 ms: 1.24x slower                                                             |
| telco                      | 7.10 ms                                                | 8.79 ms: 1.24x slower                                                            |
| go                         | 139 ms                                                 | 178 ms: 1.28x slower                                                             |
| nbody                      | 97.0 ms                                                | 124 ms: 1.28x slower                                                             |
| python_startup_no_site     | 6.94 ms                                                | 8.99 ms: 1.30x slower                                                            |
| scimark_lu                 | 118 ms                                                 | 160 ms: 1.36x slower                                                             |
| coverage                   | 72.7 ms                                                | 99.2 ms: 1.36x slower                                                            |
| hexiom                     | 6.41 ms                                                | 9.23 ms: 1.44x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.07x slower                                                                     |

Benchmark hidden because not significant (6): json, bench_mp_pool, gc_traversal, pathlib, unpickle, tornado_http
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240312-3.13.0a4+-5208402-PYTHON_UOPS/bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.95x