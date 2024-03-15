
# Results vs. 3.11.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-amd64
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 216 ms: 1.01x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.74 ms: 1.11x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 84.6 ms: 1.10x faster                                                       |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 266 ms: 1.25x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 343 ms: 1.18x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 449 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 339 ms: 1.18x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 269 ms: 1.15x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 460 ms: 1.14x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 747 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 731 ms: 1.11x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.16x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 59.8 ms: 1.18x faster                                                       |
| float          | 54.4 ms                                                     | 50.2 ms: 1.08x faster                                                       |
| pidigits       | 150 ms                                                      | 152 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                       | 1.08x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 79.2 ms: 1.15x faster                                                       |
| regex_dna      | 116 ms                                                      | 121 ms: 1.04x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.64 ms: 1.09x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 126 us: 1.25x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 175 us: 1.19x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.29 sec: 1.13x faster                                                      |
| xml_etree_parse      | 97.6 ms                                                     | 91.6 ms: 1.07x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 17.4 us: 1.06x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 36.0 ms: 1.03x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.0 ms: 1.03x faster                                                       |
| pickle_list          | 2.70 us                                                     | 2.77 us: 1.03x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.06x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.81 us: 1.09x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.44 us: 1.11x slower                                                       |
| pickle               | 6.64 us                                                     | 7.47 us: 1.13x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.4 ms: 1.03x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.4 ms: 1.10x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.58 ms: 1.15x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 70.0 us: 4.66x faster                                                       |
| generators                 | 34.0 ms                                                     | 20.7 ms: 1.64x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 472 ms: 1.54x faster                                                        |
| comprehensions             | 15.6 us                                                     | 10.8 us: 1.45x faster                                                       |
| json_dumps                 | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                                       |
| richards_super             | 38.7 ms                                                     | 28.4 ms: 1.36x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 1.98 ms: 1.36x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 54.2 ns: 1.32x faster                                                       |
| raytrace                   | 213 ms                                                      | 167 ms: 1.28x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 759 us: 1.26x faster                                                        |
| async_tree_none            | 332 ms                                                      | 266 ms: 1.25x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 126 us: 1.25x faster                                                        |
| richards                   | 31.4 ms                                                     | 25.8 ms: 1.22x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 21.4 us: 1.22x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 38.6 ns: 1.21x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 971 us: 1.20x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 175 us: 1.19x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.49 us: 1.18x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 343 ms: 1.18x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 449 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 339 ms: 1.18x faster                                                        |
| nbody                      | 70.3 ms                                                     | 59.8 ms: 1.18x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.73 sec: 1.17x faster                                                      |
| chaos                      | 48.4 ms                                                     | 41.6 ms: 1.16x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 59.0 ms: 1.16x faster                                                       |
| logging_simple             | 6.86 us                                                     | 5.96 us: 1.15x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 40.3 ms: 1.15x faster                                                       |
| mako                       | 7.58 ms                                                     | 6.58 ms: 1.15x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 87.0 ms: 1.15x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 79.2 ms: 1.15x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 269 ms: 1.15x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 460 ms: 1.14x faster                                                        |
| sympy_str                  | 185 ms                                                      | 163 ms: 1.13x faster                                                        |
| deepcopy                   | 246 us                                                      | 218 us: 1.13x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.29 sec: 1.13x faster                                                      |
| scimark_lu                 | 62.8 ms                                                     | 55.9 ms: 1.12x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.39 us: 1.12x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 978 ms: 1.11x faster                                                        |
| pprint_safe_repr           | 529 ms                                                      | 476 ms: 1.11x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.74 ms: 1.11x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 747 ms: 1.11x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 13.5 ms: 1.11x faster                                                       |
| async_tree_io              | 808 ms                                                      | 731 ms: 1.11x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 12.7 ms: 1.10x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 84.6 ms: 1.10x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 174 ms: 1.09x faster                                                        |
| mypy2                      | 459 ms                                                      | 423 ms: 1.09x faster                                                        |
| float                      | 54.4 ms                                                     | 50.2 ms: 1.08x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 1.91 us: 1.08x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 45.4 ms: 1.08x faster                                                       |
| dask                       | 273 ms                                                      | 254 ms: 1.07x faster                                                        |
| sympy_expand               | 299 ms                                                      | 280 ms: 1.07x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 91.6 ms: 1.07x faster                                                       |
| spectral_norm              | 68.3 ms                                                     | 64.1 ms: 1.07x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 17.4 us: 1.06x faster                                                       |
| fannkuch                   | 253 ms                                                      | 240 ms: 1.06x faster                                                        |
| go                         | 101 ms                                                      | 95.8 ms: 1.06x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                      |
| scimark_sor                | 78.1 ms                                                     | 74.3 ms: 1.05x faster                                                       |
| bench_thread_pool          | 872 us                                                      | 837 us: 1.04x faster                                                        |
| xml_etree_process          | 37.2 ms                                                     | 36.0 ms: 1.03x faster                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 64.0 ms: 1.03x faster                                                       |
| pyflate                    | 312 ms                                                      | 306 ms: 1.02x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 33.9 ms: 1.02x faster                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.50 ms: 1.01x slower                                                       |
| meteor_contest             | 75.2 ms                                                     | 75.9 ms: 1.01x slower                                                       |
| 2to3                       | 214 ms                                                      | 216 ms: 1.01x slower                                                        |
| mdp                        | 1.59 sec                                                    | 1.61 sec: 1.01x slower                                                      |
| pidigits                   | 150 ms                                                      | 152 ms: 1.01x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 729 us: 1.02x slower                                                        |
| pickle_list                | 2.70 us                                                     | 2.77 us: 1.03x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.4 ms: 1.03x slower                                                       |
| scimark_fft                | 179 ms                                                      | 186 ms: 1.04x slower                                                        |
| regex_dna                  | 116 ms                                                      | 121 ms: 1.04x slower                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.70 ms: 1.05x slower                                                       |
| coverage                   | 43.4 ms                                                     | 45.6 ms: 1.05x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 66.7 ms: 1.05x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 74.9 ms: 1.06x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.06x slower                                                       |
| pycparser                  | 720 ms                                                      | 764 ms: 1.06x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.81 us: 1.09x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.64 ms: 1.09x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.4 ms: 1.10x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.44 us: 1.11x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.11 ms: 1.12x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.47 us: 1.13x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.67 ms: 1.15x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 56.4 ms: 1.25x slower                                                       |
| async_generators           | 177 ms                                                      | 240 ms: 1.35x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (2): xml_etree_generate, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown