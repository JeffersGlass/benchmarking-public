
# Results vs. 3.11.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-amd64
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.76%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 220 ms: 1.03x slower                                                        |
| chameleon      | 5.26 ms                                                     | 5.12 ms: 1.03x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 85.4 ms: 1.09x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 270 ms: 1.23x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 458 ms: 1.16x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 346 ms: 1.15x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 353 ms: 1.15x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 274 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 471 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 733 ms: 1.10x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 763 ms: 1.09x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| float          | 54.4 ms                                                     | 58.3 ms: 1.07x slower                                                       |
| nbody          | 70.3 ms                                                     | 75.6 ms: 1.07x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 84.8 ms: 1.07x faster                                                       |
| regex_dna      | 116 ms                                                      | 119 ms: 1.02x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 14.7 ms: 1.04x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.65 ms: 1.43x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 184 us: 1.13x faster                                                        |
| unpickle_pure_python | 157 us                                                      | 140 us: 1.12x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 92.9 ms: 1.05x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.3 us: 1.01x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 37.4 ms: 1.01x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 54.0 ms: 1.03x slower                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 67.4 ms: 1.03x slower                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.51 sec: 1.04x slower                                                      |
| json_loads           | 13.0 us                                                     | 13.5 us: 1.04x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.85 us: 1.06x slower                                                       |
| pickle               | 6.64 us                                                     | 7.10 us: 1.07x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.86 us: 1.10x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.43 us: 1.11x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.0 ms: 1.01x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.0 ms: 1.07x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.04x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.67 ms: 1.01x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 74.0 us: 4.40x faster                                                       |
| generators                 | 34.0 ms                                                     | 20.3 ms: 1.67x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 465 ms: 1.56x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.65 ms: 1.43x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 56.0 ns: 1.28x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.15 ms: 1.26x faster                                                       |
| richards_super             | 38.7 ms                                                     | 31.0 ms: 1.25x faster                                                       |
| comprehensions             | 15.6 us                                                     | 12.5 us: 1.25x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.64 sec: 1.24x faster                                                      |
| unpack_sequence            | 46.9 ns                                                     | 37.9 ns: 1.24x faster                                                       |
| async_tree_none            | 332 ms                                                      | 270 ms: 1.23x faster                                                        |
| raytrace                   | 213 ms                                                      | 174 ms: 1.23x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 790 us: 1.21x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 458 ms: 1.16x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 346 ms: 1.15x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 1.01 ms: 1.15x faster                                                       |
| richards                   | 31.4 ms                                                     | 27.3 ms: 1.15x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 353 ms: 1.15x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 13.2 ms: 1.14x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 88.4 ms: 1.13x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 184 us: 1.13x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 274 ms: 1.13x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 23.2 us: 1.12x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 140 us: 1.12x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 41.5 ms: 1.12x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 471 ms: 1.11x faster                                                        |
| scimark_lu                 | 62.8 ms                                                     | 56.9 ms: 1.10x faster                                                       |
| sympy_str                  | 185 ms                                                      | 168 ms: 1.10x faster                                                        |
| async_tree_io              | 808 ms                                                      | 733 ms: 1.10x faster                                                        |
| logging_simple             | 6.86 us                                                     | 6.29 us: 1.09x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 763 ms: 1.09x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 85.4 ms: 1.09x faster                                                       |
| chaos                      | 48.4 ms                                                     | 44.5 ms: 1.09x faster                                                       |
| mypy2                      | 459 ms                                                      | 424 ms: 1.08x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 13.0 ms: 1.08x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.47 sec: 1.08x faster                                                      |
| go                         | 101 ms                                                      | 93.7 ms: 1.08x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 84.8 ms: 1.07x faster                                                       |
| deepcopy                   | 246 us                                                      | 231 us: 1.07x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.75 us: 1.06x faster                                                       |
| dask                       | 273 ms                                                      | 257 ms: 1.06x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 64.4 ms: 1.06x faster                                                       |
| sympy_expand               | 299 ms                                                      | 284 ms: 1.05x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 92.9 ms: 1.05x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 182 ms: 1.04x faster                                                        |
| bench_thread_pool          | 872 us                                                      | 843 us: 1.03x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 1.99 us: 1.03x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                      |
| crypto_pyaes               | 48.9 ms                                                     | 47.5 ms: 1.03x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 5.12 ms: 1.03x faster                                                       |
| pidigits                   | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| pickle_dict                | 18.5 us                                                     | 18.3 us: 1.01x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 523 ms: 1.01x faster                                                        |
| pprint_pformat             | 1.09 sec                                                    | 1.08 sec: 1.01x faster                                                      |
| xml_etree_process          | 37.2 ms                                                     | 37.4 ms: 1.01x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                                       |
| meteor_contest             | 75.2 ms                                                     | 76.0 ms: 1.01x slower                                                       |
| mako                       | 7.58 ms                                                     | 7.67 ms: 1.01x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.0 ms: 1.01x slower                                                       |
| regex_dna                  | 116 ms                                                      | 119 ms: 1.02x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 54.0 ms: 1.03x slower                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 67.4 ms: 1.03x slower                                                       |
| 2to3                       | 214 ms                                                      | 220 ms: 1.03x slower                                                        |
| bench_mp_pool              | 63.2 ms                                                     | 65.1 ms: 1.03x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 738 us: 1.04x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 14.7 ms: 1.04x slower                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.51 sec: 1.04x slower                                                      |
| json_loads                 | 13.0 us                                                     | 13.5 us: 1.04x slower                                                       |
| fannkuch                   | 253 ms                                                      | 266 ms: 1.05x slower                                                        |
| pyflate                    | 312 ms                                                      | 328 ms: 1.05x slower                                                        |
| regex_effbot               | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.85 us: 1.06x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 75.5 ms: 1.07x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.10 us: 1.07x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.0 ms: 1.07x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 83.8 ms: 1.07x slower                                                       |
| float                      | 54.4 ms                                                     | 58.3 ms: 1.07x slower                                                       |
| nbody                      | 70.3 ms                                                     | 75.6 ms: 1.07x slower                                                       |
| coverage                   | 43.4 ms                                                     | 47.0 ms: 1.08x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 49.4 ms: 1.09x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.00 ms: 1.10x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.86 us: 1.10x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.43 us: 1.11x slower                                                       |
| pycparser                  | 720 ms                                                      | 823 ms: 1.14x slower                                                        |
| scimark_fft                | 179 ms                                                      | 205 ms: 1.15x slower                                                        |
| spectral_norm              | 68.3 ms                                                     | 81.0 ms: 1.19x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.87 ms: 1.20x slower                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.22 ms: 1.25x slower                                                       |
| async_generators           | 177 ms                                                      | 231 ms: 1.31x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                |

Benchmark hidden because not significant (2): gc_traversal, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.76% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown