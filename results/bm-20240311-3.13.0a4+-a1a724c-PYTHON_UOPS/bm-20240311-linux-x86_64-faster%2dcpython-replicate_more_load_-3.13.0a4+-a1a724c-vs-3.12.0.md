# Results vs. 3.12.0

- fork: faster-cpython
- ref: replicate_more_load_
- machine: linux-x86_64
- commit hash: a1a724c
- commit date: 2024-03-11
- overall geometric mean: 1.11x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x slower
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 310 ms: 1.13x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.09 ms: 1.05x faster                                                            |
| docutils       | 2.77 sec                                               | 2.91 sec: 1.05x slower                                                           |
| tornado_http   | 103 ms                                                 | 105 ms: 1.02x slower                                                             |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 726 ms                                                 | 745 ms: 1.03x slower                                                             |
| async_tree_memoization     | 578 ms                                                 | 599 ms: 1.04x slower                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 754 ms: 1.04x slower                                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 601 ms: 1.05x slower                                                             |
| async_tree_none_tg         | 450 ms                                                 | 474 ms: 1.05x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.27 sec: 1.07x slower                                                           |
| async_tree_io              | 1.16 sec                                               | 1.25 sec: 1.08x slower                                                           |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                                     |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 193 ms: 1.03x slower                                                             |
| float          | 84.7 ms                                                | 109 ms: 1.28x slower                                                             |
| nbody          | 97.0 ms                                                | 143 ms: 1.47x slower                                                             |
| Geometric mean | (ref)                                                  | 1.25x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.47 ms: 1.04x faster                                                            |
| regex_dna      | 212 ms                                                 | 215 ms: 1.01x slower                                                             |
| regex_v8       | 23.1 ms                                                | 24.8 ms: 1.07x slower                                                            |
| regex_compile  | 148 ms                                                 | 192 ms: 1.29x slower                                                             |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list        | 5.29 us                                                | 4.87 us: 1.09x faster                                                            |
| unpickle             | 15.9 us                                                | 15.3 us: 1.04x faster                                                            |
| pickle_pure_python   | 324 us                                                 | 312 us: 1.04x faster                                                             |
| json_loads           | 28.5 us                                                | 28.2 us: 1.01x faster                                                            |
| pickle_dict          | 35.5 us                                                | 35.2 us: 1.01x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 161 ms: 1.01x slower                                                             |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| xml_etree_process    | 61.7 ms                                                | 63.6 ms: 1.03x slower                                                            |
| pickle               | 11.6 us                                                | 12.0 us: 1.03x slower                                                            |
| xml_etree_generate   | 89.2 ms                                                | 93.9 ms: 1.05x slower                                                            |
| pickle_list          | 5.08 us                                                | 5.36 us: 1.05x slower                                                            |
| xml_etree_iterparse  | 107 ms                                                 | 117 ms: 1.09x slower                                                             |
| tomli_loads          | 2.33 sec                                               | 2.76 sec: 1.19x slower                                                           |
| unpickle_pure_python | 230 us                                                 | 313 us: 1.36x slower                                                             |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 9.01 ms: 1.30x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.19x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| django_template | 34.6 ms                                                | 35.2 ms: 1.02x slower                                                            |
| mako            | 11.9 ms                                                | 15.0 ms: 1.26x slower                                                            |
| Geometric mean  | (ref)                                                  | 1.13x slower                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 120 us: 1.32x faster                                                             |
| unpickle_list              | 5.29 us                                                | 4.87 us: 1.09x faster                                                            |
| deepcopy_reduce            | 3.35 us                                                | 3.12 us: 1.07x faster                                                            |
| chameleon                  | 7.41 ms                                                | 7.09 ms: 1.05x faster                                                            |
| regex_effbot               | 3.61 ms                                                | 3.47 ms: 1.04x faster                                                            |
| unpickle                   | 15.9 us                                                | 15.3 us: 1.04x faster                                                            |
| pickle_pure_python         | 324 us                                                 | 312 us: 1.04x faster                                                             |
| generators                 | 31.2 ms                                                | 30.3 ms: 1.03x faster                                                            |
| logging_format             | 7.23 us                                                | 7.04 us: 1.03x faster                                                            |
| logging_simple             | 6.46 us                                                | 6.32 us: 1.02x faster                                                            |
| json_loads                 | 28.5 us                                                | 28.2 us: 1.01x faster                                                            |
| json                       | 5.26 ms                                                | 5.21 ms: 1.01x faster                                                            |
| pickle_dict                | 35.5 us                                                | 35.2 us: 1.01x faster                                                            |
| deepcopy                   | 371 us                                                 | 368 us: 1.01x faster                                                             |
| coroutines                 | 23.2 ms                                                | 23.0 ms: 1.01x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 170 ms: 1.01x slower                                                             |
| xml_etree_parse            | 159 ms                                                 | 161 ms: 1.01x slower                                                             |
| logging_silent             | 104 ns                                                 | 105 ns: 1.01x slower                                                             |
| json_dumps                 | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                            |
| regex_dna                  | 212 ms                                                 | 215 ms: 1.01x slower                                                             |
| django_template            | 34.6 ms                                                | 35.2 ms: 1.02x slower                                                            |
| asyncio_websockets         | 551 ms                                                 | 563 ms: 1.02x slower                                                             |
| dask                       | 372 ms                                                 | 380 ms: 1.02x slower                                                             |
| tornado_http               | 103 ms                                                 | 105 ms: 1.02x slower                                                             |
| async_tree_cpu_io_mixed    | 726 ms                                                 | 745 ms: 1.03x slower                                                             |
| pidigits                   | 187 ms                                                 | 193 ms: 1.03x slower                                                             |
| sympy_integrate            | 21.4 ms                                                | 22.1 ms: 1.03x slower                                                            |
| xml_etree_process          | 61.7 ms                                                | 63.6 ms: 1.03x slower                                                            |
| pickle                     | 11.6 us                                                | 12.0 us: 1.03x slower                                                            |
| asyncio_tcp                | 491 ms                                                 | 508 ms: 1.04x slower                                                             |
| async_tree_memoization     | 578 ms                                                 | 599 ms: 1.04x slower                                                             |
| sympy_str                  | 300 ms                                                 | 311 ms: 1.04x slower                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 754 ms: 1.04x slower                                                             |
| async_generators           | 463 ms                                                 | 482 ms: 1.04x slower                                                             |
| create_gc_cycles           | 1.48 ms                                                | 1.54 ms: 1.04x slower                                                            |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.86 sec: 1.04x slower                                                           |
| sqlglot_normalize          | 110 ms                                                 | 115 ms: 1.04x slower                                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 601 ms: 1.05x slower                                                             |
| docutils                   | 2.77 sec                                               | 2.91 sec: 1.05x slower                                                           |
| xml_etree_generate         | 89.2 ms                                                | 93.9 ms: 1.05x slower                                                            |
| async_tree_none_tg         | 450 ms                                                 | 474 ms: 1.05x slower                                                             |
| pickle_list                | 5.08 us                                                | 5.36 us: 1.05x slower                                                            |
| bench_thread_pool          | 842 us                                                 | 888 us: 1.06x slower                                                             |
| mdp                        | 2.63 sec                                               | 2.78 sec: 1.06x slower                                                           |
| sqlite_synth               | 2.83 us                                                | 3.01 us: 1.06x slower                                                            |
| gunicorn                   | 1.24 ms                                                | 1.32 ms: 1.07x slower                                                            |
| aiohttp                    | 1.15 ms                                                | 1.23 ms: 1.07x slower                                                            |
| async_tree_io_tg           | 1.18 sec                                               | 1.27 sec: 1.07x slower                                                           |
| regex_v8                   | 23.1 ms                                                | 24.8 ms: 1.07x slower                                                            |
| gc_traversal               | 3.79 ms                                                | 4.10 ms: 1.08x slower                                                            |
| async_tree_io              | 1.16 sec                                               | 1.25 sec: 1.08x slower                                                           |
| deepcopy_memo              | 40.7 us                                                | 44.0 us: 1.08x slower                                                            |
| dulwich_log                | 68.5 ms                                                | 74.0 ms: 1.08x slower                                                            |
| sympy_expand               | 478 ms                                                 | 522 ms: 1.09x slower                                                             |
| python_startup             | 9.55 ms                                                | 10.4 ms: 1.09x slower                                                            |
| xml_etree_iterparse        | 107 ms                                                 | 117 ms: 1.09x slower                                                             |
| sqlglot_transpile          | 1.68 ms                                                | 1.85 ms: 1.10x slower                                                            |
| comprehensions             | 21.8 us                                                | 24.0 us: 1.10x slower                                                            |
| sqlglot_parse              | 1.36 ms                                                | 1.51 ms: 1.11x slower                                                            |
| deltablue                  | 3.72 ms                                                | 4.12 ms: 1.11x slower                                                            |
| mypy2                      | 830 ms                                                 | 929 ms: 1.12x slower                                                             |
| pycparser                  | 1.18 sec                                               | 1.33 sec: 1.13x slower                                                           |
| 2to3                       | 274 ms                                                 | 310 ms: 1.13x slower                                                             |
| meteor_contest             | 112 ms                                                 | 128 ms: 1.13x slower                                                             |
| crypto_pyaes               | 81.9 ms                                                | 93.1 ms: 1.14x slower                                                            |
| sqlglot_optimize           | 54.8 ms                                                | 63.4 ms: 1.16x slower                                                            |
| tomli_loads                | 2.33 sec                                               | 2.76 sec: 1.19x slower                                                           |
| scimark_sor                | 129 ms                                                 | 155 ms: 1.20x slower                                                             |
| raytrace                   | 312 ms                                                 | 374 ms: 1.20x slower                                                             |
| pprint_safe_repr           | 776 ms                                                 | 958 ms: 1.23x slower                                                             |
| unpack_sequence            | 54.0 ns                                                | 67.0 ns: 1.24x slower                                                            |
| chaos                      | 67.0 ms                                                | 83.3 ms: 1.24x slower                                                            |
| mako                       | 11.9 ms                                                | 15.0 ms: 1.26x slower                                                            |
| pprint_pformat             | 1.57 sec                                               | 1.98 sec: 1.26x slower                                                           |
| telco                      | 7.10 ms                                                | 9.09 ms: 1.28x slower                                                            |
| float                      | 84.7 ms                                                | 109 ms: 1.28x slower                                                             |
| regex_compile              | 148 ms                                                 | 192 ms: 1.29x slower                                                             |
| python_startup_no_site     | 6.94 ms                                                | 9.01 ms: 1.30x slower                                                            |
| richards_super             | 51.5 ms                                                | 67.9 ms: 1.32x slower                                                            |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 6.73 ms: 1.33x slower                                                            |
| scimark_fft                | 382 ms                                                 | 510 ms: 1.33x slower                                                             |
| coverage                   | 72.7 ms                                                | 97.3 ms: 1.34x slower                                                            |
| richards                   | 45.8 ms                                                | 61.4 ms: 1.34x slower                                                            |
| fannkuch                   | 417 ms                                                 | 564 ms: 1.35x slower                                                             |
| unpickle_pure_python       | 230 us                                                 | 313 us: 1.36x slower                                                             |
| spectral_norm              | 115 ms                                                 | 156 ms: 1.36x slower                                                             |
| go                         | 139 ms                                                 | 190 ms: 1.36x slower                                                             |
| nqueens                    | 83.3 ms                                                | 114 ms: 1.37x slower                                                             |
| pyflate                    | 482 ms                                                 | 663 ms: 1.37x slower                                                             |
| scimark_monte_carlo        | 75.1 ms                                                | 104 ms: 1.39x slower                                                             |
| scimark_lu                 | 118 ms                                                 | 172 ms: 1.45x slower                                                             |
| nbody                      | 97.0 ms                                                | 143 ms: 1.47x slower                                                             |
| hexiom                     | 6.41 ms                                                | 10.8 ms: 1.68x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.11x slower                                                                     |

Benchmark hidden because not significant (3): async_tree_none, bench_mp_pool, pathlib
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240311-3.13.0a4+-a1a724c-PYTHON_UOPS/bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.06x
- 99% likely to have a slowdown of 1.05x


# Memory

- memory change: 0.95x