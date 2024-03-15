# Results vs. base

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: linux-x86_64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.07x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 262 ms                                                                                                            | 282 ms: 1.08x slower                                                                                                          |
| chameleon      | 6.96 ms                                                                                                           | 7.33 ms: 1.05x slower                                                                                                         |
| docutils       | 2.61 sec                                                                                                          | 2.71 sec: 1.04x slower                                                                                                        |
| tornado_http   | 93.8 ms                                                                                                           | 97.8 ms: 1.04x slower                                                                                                         |
| Geometric mean | (ref)                                                                                                             | 1.05x slower                                                                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| async_tree_io_tg           | 1.20 sec                                                                                                          | 1.22 sec: 1.01x slower                                                                                                        |
| async_tree_cpu_io_mixed_tg | 722 ms                                                                                                            | 734 ms: 1.02x slower                                                                                                          |
| async_tree_io              | 1.19 sec                                                                                                          | 1.21 sec: 1.02x slower                                                                                                        |
| async_tree_none_tg         | 444 ms                                                                                                            | 454 ms: 1.02x slower                                                                                                          |
| async_tree_cpu_io_mixed    | 710 ms                                                                                                            | 726 ms: 1.02x slower                                                                                                          |
| async_tree_memoization_tg  | 578 ms                                                                                                            | 591 ms: 1.02x slower                                                                                                          |
| async_tree_memoization     | 564 ms                                                                                                            | 581 ms: 1.03x slower                                                                                                          |
| async_tree_none            | 438 ms                                                                                                            | 454 ms: 1.04x slower                                                                                                          |
| Geometric mean             | (ref)                                                                                                             | 1.02x slower                                                                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                                                                            | 188 ms: 1.01x slower                                                                                                          |
| float          | 80.8 ms                                                                                                           | 92.2 ms: 1.14x slower                                                                                                         |
| nbody          | 88.8 ms                                                                                                           | 116 ms: 1.31x slower                                                                                                          |
| Geometric mean | (ref)                                                                                                             | 1.15x slower                                                                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| regex_effbot   | 3.72 ms                                                                                                           | 3.58 ms: 1.04x faster                                                                                                         |
| regex_dna      | 229 ms                                                                                                            | 225 ms: 1.02x faster                                                                                                          |
| regex_v8       | 23.8 ms                                                                                                           | 25.1 ms: 1.05x slower                                                                                                         |
| regex_compile  | 129 ms                                                                                                            | 151 ms: 1.17x slower                                                                                                          |
| Geometric mean | (ref)                                                                                                             | 1.04x slower                                                                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| pickle               | 11.2 us                                                                                                           | 10.9 us: 1.03x faster                                                                                                         |
| pickle_list          | 4.96 us                                                                                                           | 4.88 us: 1.02x faster                                                                                                         |
| pickle_dict          | 33.7 us                                                                                                           | 33.5 us: 1.01x faster                                                                                                         |
| json_dumps           | 10.3 ms                                                                                                           | 10.4 ms: 1.01x slower                                                                                                         |
| json_loads           | 28.1 us                                                                                                           | 28.3 us: 1.01x slower                                                                                                         |
| unpickle             | 14.6 us                                                                                                           | 14.9 us: 1.02x slower                                                                                                         |
| pickle_pure_python   | 295 us                                                                                                            | 302 us: 1.02x slower                                                                                                          |
| unpickle_list        | 5.06 us                                                                                                           | 5.20 us: 1.03x slower                                                                                                         |
| xml_etree_generate   | 85.2 ms                                                                                                           | 89.5 ms: 1.05x slower                                                                                                         |
| xml_etree_process    | 58.3 ms                                                                                                           | 61.4 ms: 1.05x slower                                                                                                         |
| xml_etree_iterparse  | 104 ms                                                                                                            | 111 ms: 1.07x slower                                                                                                          |
| unpickle_pure_python | 215 us                                                                                                            | 234 us: 1.08x slower                                                                                                          |
| tomli_loads          | 2.13 sec                                                                                                          | 2.41 sec: 1.13x slower                                                                                                        |
| Geometric mean       | (ref)                                                                                                             | 1.03x slower                                                                                                                  |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                                                           | 10.1 ms: 1.00x slower                                                                                                         |
| python_startup_no_site | 8.70 ms                                                                                                           | 8.72 ms: 1.00x slower                                                                                                         |
| Geometric mean         | (ref)                                                                                                             | 1.00x slower                                                                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|-----------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| mako      | 11.4 ms                                                                                                           | 14.1 ms: 1.24x slower                                                                                                         |

All benchmarks:
===============

| Benchmark                  | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------:|
| unpack_sequence            | 53.1 ns                                                                                                           | 46.2 ns: 1.15x faster                                                                                                         |
| regex_effbot               | 3.72 ms                                                                                                           | 3.58 ms: 1.04x faster                                                                                                         |
| pickle                     | 11.2 us                                                                                                           | 10.9 us: 1.03x faster                                                                                                         |
| regex_dna                  | 229 ms                                                                                                            | 225 ms: 1.02x faster                                                                                                          |
| pickle_list                | 4.96 us                                                                                                           | 4.88 us: 1.02x faster                                                                                                         |
| create_gc_cycles           | 1.48 ms                                                                                                           | 1.46 ms: 1.01x faster                                                                                                         |
| coverage                   | 95.2 ms                                                                                                           | 93.8 ms: 1.01x faster                                                                                                         |
| pickle_dict                | 33.7 us                                                                                                           | 33.5 us: 1.01x faster                                                                                                         |
| python_startup             | 10.1 ms                                                                                                           | 10.1 ms: 1.00x slower                                                                                                         |
| python_startup_no_site     | 8.70 ms                                                                                                           | 8.72 ms: 1.00x slower                                                                                                         |
| asyncio_tcp_ssl            | 1.78 sec                                                                                                          | 1.79 sec: 1.00x slower                                                                                                        |
| json_dumps                 | 10.3 ms                                                                                                           | 10.4 ms: 1.01x slower                                                                                                         |
| pidigits                   | 187 ms                                                                                                            | 188 ms: 1.01x slower                                                                                                          |
| deepcopy                   | 351 us                                                                                                            | 353 us: 1.01x slower                                                                                                          |
| json_loads                 | 28.1 us                                                                                                           | 28.3 us: 1.01x slower                                                                                                         |
| async_tree_io_tg           | 1.20 sec                                                                                                          | 1.22 sec: 1.01x slower                                                                                                        |
| dask                       | 361 ms                                                                                                            | 366 ms: 1.01x slower                                                                                                          |
| async_tree_cpu_io_mixed_tg | 722 ms                                                                                                            | 734 ms: 1.02x slower                                                                                                          |
| async_tree_io              | 1.19 sec                                                                                                          | 1.21 sec: 1.02x slower                                                                                                        |
| pycparser                  | 1.18 sec                                                                                                          | 1.20 sec: 1.02x slower                                                                                                        |
| unpickle                   | 14.6 us                                                                                                           | 14.9 us: 1.02x slower                                                                                                         |
| async_tree_none_tg         | 444 ms                                                                                                            | 454 ms: 1.02x slower                                                                                                          |
| async_tree_cpu_io_mixed    | 710 ms                                                                                                            | 726 ms: 1.02x slower                                                                                                          |
| async_tree_memoization_tg  | 578 ms                                                                                                            | 591 ms: 1.02x slower                                                                                                          |
| logging_silent             | 103 ns                                                                                                            | 105 ns: 1.02x slower                                                                                                          |
| pickle_pure_python         | 295 us                                                                                                            | 302 us: 1.02x slower                                                                                                          |
| scimark_sor                | 121 ms                                                                                                            | 124 ms: 1.03x slower                                                                                                          |
| richards                   | 47.0 ms                                                                                                           | 48.2 ms: 1.03x slower                                                                                                         |
| sqlite_synth               | 2.80 us                                                                                                           | 2.88 us: 1.03x slower                                                                                                         |
| async_generators           | 440 ms                                                                                                            | 452 ms: 1.03x slower                                                                                                          |
| bench_thread_pool          | 824 us                                                                                                            | 848 us: 1.03x slower                                                                                                          |
| unpickle_list              | 5.06 us                                                                                                           | 5.20 us: 1.03x slower                                                                                                         |
| richards_super             | 53.2 ms                                                                                                           | 54.8 ms: 1.03x slower                                                                                                         |
| asyncio_tcp                | 478 ms                                                                                                            | 493 ms: 1.03x slower                                                                                                          |
| async_tree_memoization     | 564 ms                                                                                                            | 581 ms: 1.03x slower                                                                                                          |
| async_tree_none            | 438 ms                                                                                                            | 454 ms: 1.04x slower                                                                                                          |
| docutils                   | 2.61 sec                                                                                                          | 2.71 sec: 1.04x slower                                                                                                        |
| coroutines                 | 21.8 ms                                                                                                           | 22.7 ms: 1.04x slower                                                                                                         |
| tornado_http               | 93.8 ms                                                                                                           | 97.8 ms: 1.04x slower                                                                                                         |
| telco                      | 8.20 ms                                                                                                           | 8.56 ms: 1.04x slower                                                                                                         |
| deepcopy_memo              | 38.4 us                                                                                                           | 40.1 us: 1.04x slower                                                                                                         |
| mdp                        | 2.53 sec                                                                                                          | 2.65 sec: 1.05x slower                                                                                                        |
| typing_runtime_protocols   | 111 us                                                                                                            | 117 us: 1.05x slower                                                                                                          |
| xml_etree_generate         | 85.2 ms                                                                                                           | 89.5 ms: 1.05x slower                                                                                                         |
| scimark_lu                 | 112 ms                                                                                                            | 118 ms: 1.05x slower                                                                                                          |
| generators                 | 28.3 ms                                                                                                           | 29.8 ms: 1.05x slower                                                                                                         |
| chameleon                  | 6.96 ms                                                                                                           | 7.33 ms: 1.05x slower                                                                                                         |
| xml_etree_process          | 58.3 ms                                                                                                           | 61.4 ms: 1.05x slower                                                                                                         |
| sqlglot_transpile          | 1.57 ms                                                                                                           | 1.65 ms: 1.05x slower                                                                                                         |
| regex_v8                   | 23.8 ms                                                                                                           | 25.1 ms: 1.05x slower                                                                                                         |
| meteor_contest             | 107 ms                                                                                                            | 114 ms: 1.06x slower                                                                                                          |
| dulwich_log                | 65.5 ms                                                                                                           | 69.9 ms: 1.07x slower                                                                                                         |
| sqlglot_parse              | 1.24 ms                                                                                                           | 1.33 ms: 1.07x slower                                                                                                         |
| xml_etree_iterparse        | 104 ms                                                                                                            | 111 ms: 1.07x slower                                                                                                          |
| sqlglot_normalize          | 106 ms                                                                                                            | 113 ms: 1.07x slower                                                                                                          |
| 2to3                       | 262 ms                                                                                                            | 282 ms: 1.08x slower                                                                                                          |
| logging_simple             | 5.63 us                                                                                                           | 6.07 us: 1.08x slower                                                                                                         |
| sympy_expand               | 455 ms                                                                                                            | 490 ms: 1.08x slower                                                                                                          |
| sqlglot_optimize           | 53.2 ms                                                                                                           | 57.7 ms: 1.08x slower                                                                                                         |
| unpickle_pure_python       | 215 us                                                                                                            | 234 us: 1.08x slower                                                                                                          |
| sympy_sum                  | 149 ms                                                                                                            | 161 ms: 1.08x slower                                                                                                          |
| sympy_str                  | 269 ms                                                                                                            | 293 ms: 1.09x slower                                                                                                          |
| pprint_safe_repr           | 744 ms                                                                                                            | 809 ms: 1.09x slower                                                                                                          |
| sympy_integrate            | 19.5 ms                                                                                                           | 21.2 ms: 1.09x slower                                                                                                         |
| pyflate                    | 458 ms                                                                                                            | 509 ms: 1.11x slower                                                                                                          |
| logging_format             | 6.20 us                                                                                                           | 6.91 us: 1.12x slower                                                                                                         |
| pprint_pformat             | 1.51 sec                                                                                                          | 1.69 sec: 1.12x slower                                                                                                        |
| gc_traversal               | 3.54 ms                                                                                                           | 3.97 ms: 1.12x slower                                                                                                         |
| go                         | 139 ms                                                                                                            | 156 ms: 1.12x slower                                                                                                          |
| tomli_loads                | 2.13 sec                                                                                                          | 2.41 sec: 1.13x slower                                                                                                        |
| float                      | 80.8 ms                                                                                                           | 92.2 ms: 1.14x slower                                                                                                         |
| fannkuch                   | 397 ms                                                                                                            | 457 ms: 1.15x slower                                                                                                          |
| raytrace                   | 260 ms                                                                                                            | 301 ms: 1.16x slower                                                                                                          |
| crypto_pyaes               | 71.9 ms                                                                                                           | 83.2 ms: 1.16x slower                                                                                                         |
| regex_compile              | 129 ms                                                                                                            | 151 ms: 1.17x slower                                                                                                          |
| scimark_fft                | 371 ms                                                                                                            | 442 ms: 1.19x slower                                                                                                          |
| nqueens                    | 79.8 ms                                                                                                           | 95.1 ms: 1.19x slower                                                                                                         |
| scimark_sparse_mat_mult    | 4.89 ms                                                                                                           | 5.85 ms: 1.20x slower                                                                                                         |
| scimark_monte_carlo        | 66.5 ms                                                                                                           | 81.0 ms: 1.22x slower                                                                                                         |
| chaos                      | 59.7 ms                                                                                                           | 73.2 ms: 1.23x slower                                                                                                         |
| mako                       | 11.4 ms                                                                                                           | 14.1 ms: 1.24x slower                                                                                                         |
| nbody                      | 88.8 ms                                                                                                           | 116 ms: 1.31x slower                                                                                                          |
| spectral_norm              | 111 ms                                                                                                            | 146 ms: 1.31x slower                                                                                                          |
| comprehensions             | 16.0 us                                                                                                           | 21.4 us: 1.34x slower                                                                                                         |
| hexiom                     | 6.00 ms                                                                                                           | 8.59 ms: 1.43x slower                                                                                                         |
| deltablue                  | 3.19 ms                                                                                                           | 4.67 ms: 1.47x slower                                                                                                         |
| Geometric mean             | (ref)                                                                                                             | 1.07x slower                                                                                                                  |

Benchmark hidden because not significant (7): deepcopy_reduce, pathlib, bench_mp_pool, xml_etree_parse, asyncio_websockets, json, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.00x