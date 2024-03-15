
# Results vs. 3.11.0

- fork: faster-cpython
- ref: load_attr_module_con
- machine: linux-x86_64
- commit hash: 76389dd
- commit date: 2024-02-15
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.83%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 292 ms: 1.10x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.10 ms: 1.06x slower                                                            |
| docutils       | 2.66 sec                                               | 2.80 sec: 1.05x slower                                                           |
| tornado_http   | 98.1 ms                                                | 99.0 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 574 ms: 1.11x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 455 ms: 1.08x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 603 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.04x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 89.8 ms: 1.14x slower                                                            |
| nbody          | 96.0 ms                                                | 115 ms: 1.20x slower                                                             |
| Geometric mean | (ref)                                                  | 1.10x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.58 ms: 1.02x slower                                                            |
| regex_dna      | 205 ms                                                 | 221 ms: 1.08x slower                                                             |
| regex_v8       | 22.9 ms                                                | 25.1 ms: 1.10x slower                                                            |
| regex_compile  | 141 ms                                                 | 176 ms: 1.25x slower                                                             |
| Geometric mean | (ref)                                                  | 1.11x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                                             |
| json_loads           | 29.2 us                                                | 27.7 us: 1.05x faster                                                            |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| pickle_dict          | 34.6 us                                                | 33.6 us: 1.03x faster                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 61.0 ms: 1.07x slower                                                            |
| unpickle             | 13.8 us                                                | 15.1 us: 1.09x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 89.5 ms: 1.10x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.08 us: 1.11x slower                                                            |
| unpickle_pure_python | 242 us                                                 | 271 us: 1.12x slower                                                             |
| tomli_loads          | 2.30 sec                                               | 2.64 sec: 1.15x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.82 ms: 1.47x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 14.0 ms: 1.32x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 114 us: 4.55x faster                                                             |
| generators                 | 74.9 ms                                                | 29.4 ms: 2.54x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 491 ms: 1.78x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                            |
| coroutines                 | 27.0 ms                                                | 23.0 ms: 1.18x faster                                                            |
| async_tree_none            | 528 ms                                                 | 450 ms: 1.17x faster                                                             |
| comprehensions             | 23.6 us                                                | 21.0 us: 1.12x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 574 ms: 1.11x faster                                                             |
| logging_silent             | 111 ns                                                 | 100 ns: 1.11x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 455 ms: 1.08x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                           |
| gc_traversal               | 4.01 ms                                                | 3.75 ms: 1.07x faster                                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                                             |
| deltablue                  | 3.92 ms                                                | 3.72 ms: 1.05x faster                                                            |
| json_loads                 | 29.2 us                                                | 27.7 us: 1.05x faster                                                            |
| mdp                        | 2.77 sec                                               | 2.66 sec: 1.04x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                             |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 603 ms: 1.04x faster                                                             |
| json                       | 5.24 ms                                                | 5.04 ms: 1.04x faster                                                            |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.04x faster                                                             |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.04x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.11 us: 1.03x faster                                                            |
| pickle_dict                | 34.6 us                                                | 33.6 us: 1.03x faster                                                            |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                                            |
| deepcopy                   | 365 us                                                 | 360 us: 1.01x faster                                                             |
| logging_simple             | 6.22 us                                                | 6.17 us: 1.01x faster                                                            |
| sqlglot_normalize          | 113 ms                                                 | 113 ms: 1.01x slower                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.76 ms: 1.01x slower                                                            |
| tornado_http               | 98.1 ms                                                | 99.0 ms: 1.01x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.58 ms: 1.02x slower                                                            |
| xml_etree_iterparse        | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| chaos                      | 71.9 ms                                                | 73.9 ms: 1.03x slower                                                            |
| pathlib                    | 18.5 ms                                                | 19.1 ms: 1.03x slower                                                            |
| bench_thread_pool          | 834 us                                                 | 862 us: 1.03x slower                                                             |
| logging_format             | 6.81 us                                                | 7.05 us: 1.04x slower                                                            |
| deepcopy_memo              | 40.2 us                                                | 41.7 us: 1.04x slower                                                            |
| sympy_expand               | 484 ms                                                 | 505 ms: 1.04x slower                                                             |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                            |
| docutils                   | 2.66 sec                                               | 2.80 sec: 1.05x slower                                                           |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.10 ms: 1.06x slower                                                            |
| meteor_contest             | 109 ms                                                 | 116 ms: 1.06x slower                                                             |
| richards_super             | 61.9 ms                                                | 66.0 ms: 1.07x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 61.0 ms: 1.07x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.27 sec: 1.07x slower                                                           |
| regex_dna                  | 205 ms                                                 | 221 ms: 1.08x slower                                                             |
| sqlglot_optimize           | 55.3 ms                                                | 60.2 ms: 1.09x slower                                                            |
| unpickle                   | 13.8 us                                                | 15.1 us: 1.09x slower                                                            |
| crypto_pyaes               | 76.7 ms                                                | 83.9 ms: 1.09x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 25.1 ms: 1.10x slower                                                            |
| 2to3                       | 264 ms                                                 | 292 ms: 1.10x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 89.5 ms: 1.10x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.08 us: 1.11x slower                                                            |
| unpickle_pure_python       | 242 us                                                 | 271 us: 1.12x slower                                                             |
| sqlite_synth               | 2.57 us                                                | 2.89 us: 1.12x slower                                                            |
| dulwich_log                | 64.6 ms                                                | 72.7 ms: 1.13x slower                                                            |
| float                      | 78.9 ms                                                | 89.8 ms: 1.14x slower                                                            |
| nqueens                    | 87.9 ms                                                | 100 ms: 1.14x slower                                                             |
| pprint_safe_repr           | 747 ms                                                 | 851 ms: 1.14x slower                                                             |
| tomli_loads                | 2.30 sec                                               | 2.64 sec: 1.15x slower                                                           |
| raytrace                   | 309 ms                                                 | 355 ms: 1.15x slower                                                             |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.82 ms: 1.16x slower                                                            |
| scimark_sor                | 121 ms                                                 | 141 ms: 1.16x slower                                                             |
| fannkuch                   | 405 ms                                                 | 473 ms: 1.17x slower                                                             |
| pprint_pformat             | 1.55 sec                                               | 1.82 sec: 1.17x slower                                                           |
| go                         | 149 ms                                                 | 176 ms: 1.19x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| nbody                      | 96.0 ms                                                | 115 ms: 1.20x slower                                                             |
| richards                   | 49.8 ms                                                | 59.9 ms: 1.20x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 85.6 ms: 1.21x slower                                                            |
| scimark_fft                | 345 ms                                                 | 419 ms: 1.21x slower                                                             |
| coverage                   | 78.8 ms                                                | 97.9 ms: 1.24x slower                                                            |
| async_generators           | 374 ms                                                 | 466 ms: 1.25x slower                                                             |
| regex_compile              | 141 ms                                                 | 176 ms: 1.25x slower                                                             |
| spectral_norm              | 108 ms                                                 | 136 ms: 1.26x slower                                                             |
| telco                      | 6.86 ms                                                | 8.81 ms: 1.28x slower                                                            |
| mypy2                      | 686 ms                                                 | 896 ms: 1.31x slower                                                             |
| unpack_sequence            | 43.5 ns                                                | 57.0 ns: 1.31x slower                                                            |
| mako                       | 10.7 ms                                                | 14.0 ms: 1.32x slower                                                            |
| hexiom                     | 6.89 ms                                                | 9.15 ms: 1.33x slower                                                            |
| pyflate                    | 434 ms                                                 | 588 ms: 1.35x slower                                                             |
| scimark_lu                 | 116 ms                                                 | 167 ms: 1.43x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.82 ms: 1.47x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (6): sqlglot_parse, bench_mp_pool, sympy_str, asyncio_websockets, unpickle_list, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.83% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x