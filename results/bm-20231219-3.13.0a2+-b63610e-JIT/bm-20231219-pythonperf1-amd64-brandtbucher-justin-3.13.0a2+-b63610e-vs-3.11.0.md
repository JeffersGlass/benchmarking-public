
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin
- machine: windows-amd64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.08x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 219 ms: 1.03x slower                                                |
| chameleon      | 5.26 ms                                                     | 4.86 ms: 1.08x faster                                               |
| docutils       | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                              |
| tornado_http   | 92.8 ms                                                     | 89.4 ms: 1.04x faster                                               |
| Geometric mean | (ref)                                                       | 1.03x faster                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 263 ms: 1.26x faster                                                |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 449 ms: 1.18x faster                                                |
| async_tree_memoization     | 399 ms                                                      | 338 ms: 1.18x faster                                                |
| async_tree_memoization_tg  | 405 ms                                                      | 354 ms: 1.14x faster                                                |
| async_tree_none_tg         | 309 ms                                                      | 271 ms: 1.14x faster                                                |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 464 ms: 1.13x faster                                                |
| async_tree_io_tg           | 829 ms                                                      | 745 ms: 1.11x faster                                                |
| async_tree_io              | 808 ms                                                      | 731 ms: 1.10x faster                                                |
| Geometric mean             | (ref)                                                       | 1.16x faster                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 61.9 ms: 1.14x faster                                               |
| float          | 54.4 ms                                                     | 51.4 ms: 1.06x faster                                               |
| pidigits       | 150 ms                                                      | 152 ms: 1.02x slower                                                |
| Geometric mean | (ref)                                                       | 1.06x faster                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 83.8 ms: 1.09x faster                                               |
| regex_dna      | 116 ms                                                      | 122 ms: 1.05x slower                                                |
| regex_effbot   | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                               |
| regex_v8       | 14.2 ms                                                     | 15.5 ms: 1.10x slower                                               |
| Geometric mean | (ref)                                                       | 1.03x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.61 ms: 1.44x faster                                               |
| unpickle_pure_python | 157 us                                                      | 133 us: 1.18x faster                                                |
| pickle_pure_python   | 208 us                                                      | 179 us: 1.17x faster                                                |
| tomli_loads          | 1.46 sec                                                    | 1.32 sec: 1.10x faster                                              |
| xml_etree_parse      | 97.6 ms                                                     | 92.8 ms: 1.05x faster                                               |
| pickle_dict          | 18.5 us                                                     | 17.6 us: 1.05x faster                                               |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.7 ms: 1.03x faster                                               |
| xml_etree_process    | 37.2 ms                                                     | 36.2 ms: 1.03x faster                                               |
| pickle_list          | 2.70 us                                                     | 2.77 us: 1.03x slower                                               |
| json_loads           | 13.0 us                                                     | 13.4 us: 1.03x slower                                               |
| unpickle_list        | 2.59 us                                                     | 2.72 us: 1.05x slower                                               |
| pickle               | 6.64 us                                                     | 7.20 us: 1.09x slower                                               |
| unpickle             | 7.57 us                                                     | 8.34 us: 1.10x slower                                               |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                        |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 21.0 ms: 1.06x slower                                               |
| python_startup_no_site | 16.8 ms                                                     | 19.1 ms: 1.14x slower                                               |
| Geometric mean         | (ref)                                                       | 1.10x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.59 ms: 1.15x faster                                               |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 72.2 us: 4.51x faster                                               |
| generators                 | 34.0 ms                                                     | 22.0 ms: 1.55x faster                                               |
| asyncio_tcp                | 726 ms                                                      | 472 ms: 1.54x faster                                                |
| json_dumps                 | 8.09 ms                                                     | 5.61 ms: 1.44x faster                                               |
| comprehensions             | 15.6 us                                                     | 11.6 us: 1.35x faster                                               |
| logging_silent             | 71.8 ns                                                     | 55.0 ns: 1.30x faster                                               |
| async_tree_none            | 332 ms                                                      | 263 ms: 1.26x faster                                                |
| deltablue                  | 2.70 ms                                                     | 2.14 ms: 1.26x faster                                               |
| unpack_sequence            | 46.9 ns                                                     | 37.5 ns: 1.25x faster                                               |
| richards_super             | 38.7 ms                                                     | 31.4 ms: 1.23x faster                                               |
| sqlglot_parse              | 953 us                                                      | 774 us: 1.23x faster                                                |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.68 sec: 1.21x faster                                              |
| raytrace                   | 213 ms                                                      | 180 ms: 1.18x faster                                                |
| unpickle_pure_python       | 157 us                                                      | 133 us: 1.18x faster                                                |
| richards                   | 31.4 ms                                                     | 26.6 ms: 1.18x faster                                               |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 449 ms: 1.18x faster                                                |
| async_tree_memoization     | 399 ms                                                      | 338 ms: 1.18x faster                                                |
| sqlglot_transpile          | 1.16 ms                                                     | 994 us: 1.17x faster                                                |
| pickle_pure_python         | 208 us                                                      | 179 us: 1.17x faster                                                |
| coroutines                 | 15.0 ms                                                     | 12.9 ms: 1.16x faster                                               |
| mako                       | 7.58 ms                                                     | 6.59 ms: 1.15x faster                                               |
| deepcopy_memo              | 26.0 us                                                     | 22.7 us: 1.15x faster                                               |
| sympy_sum                  | 100 ms                                                      | 87.4 ms: 1.14x faster                                               |
| async_tree_memoization_tg  | 405 ms                                                      | 354 ms: 1.14x faster                                                |
| sqlite_synth               | 1.77 us                                                     | 1.55 us: 1.14x faster                                               |
| async_tree_none_tg         | 309 ms                                                      | 271 ms: 1.14x faster                                                |
| nbody                      | 70.3 ms                                                     | 61.9 ms: 1.14x faster                                               |
| logging_simple             | 6.86 us                                                     | 6.09 us: 1.13x faster                                               |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 464 ms: 1.13x faster                                                |
| deepcopy                   | 246 us                                                      | 219 us: 1.12x faster                                                |
| nqueens                    | 68.3 ms                                                     | 60.9 ms: 1.12x faster                                               |
| chaos                      | 48.4 ms                                                     | 43.1 ms: 1.12x faster                                               |
| scimark_lu                 | 62.8 ms                                                     | 56.2 ms: 1.12x faster                                               |
| async_tree_io_tg           | 829 ms                                                      | 745 ms: 1.11x faster                                                |
| logging_format             | 7.16 us                                                     | 6.48 us: 1.11x faster                                               |
| async_tree_io              | 808 ms                                                      | 731 ms: 1.10x faster                                                |
| sympy_str                  | 185 ms                                                      | 168 ms: 1.10x faster                                                |
| tomli_loads                | 1.46 sec                                                    | 1.32 sec: 1.10x faster                                              |
| dulwich_log                | 46.4 ms                                                     | 42.2 ms: 1.10x faster                                               |
| regex_compile              | 91.0 ms                                                     | 83.8 ms: 1.09x faster                                               |
| chameleon                  | 5.26 ms                                                     | 4.86 ms: 1.08x faster                                               |
| deepcopy_reduce            | 2.06 us                                                     | 1.91 us: 1.08x faster                                               |
| mypy2                      | 459 ms                                                      | 432 ms: 1.06x faster                                                |
| float                      | 54.4 ms                                                     | 51.4 ms: 1.06x faster                                               |
| sympy_integrate            | 14.0 ms                                                     | 13.3 ms: 1.06x faster                                               |
| bench_thread_pool          | 872 us                                                      | 825 us: 1.06x faster                                                |
| dask                       | 273 ms                                                      | 259 ms: 1.05x faster                                                |
| sympy_expand               | 299 ms                                                      | 284 ms: 1.05x faster                                                |
| xml_etree_parse            | 97.6 ms                                                     | 92.8 ms: 1.05x faster                                               |
| pickle_dict                | 18.5 us                                                     | 17.6 us: 1.05x faster                                               |
| pyflate                    | 312 ms                                                      | 298 ms: 1.05x faster                                                |
| sqlglot_normalize          | 190 ms                                                      | 182 ms: 1.04x faster                                                |
| crypto_pyaes               | 48.9 ms                                                     | 46.9 ms: 1.04x faster                                               |
| pprint_safe_repr           | 529 ms                                                      | 508 ms: 1.04x faster                                                |
| pprint_pformat             | 1.09 sec                                                    | 1.04 sec: 1.04x faster                                              |
| tornado_http               | 92.8 ms                                                     | 89.4 ms: 1.04x faster                                               |
| pycparser                  | 720 ms                                                      | 694 ms: 1.04x faster                                                |
| docutils                   | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                              |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.7 ms: 1.03x faster                                               |
| spectral_norm              | 68.3 ms                                                     | 66.4 ms: 1.03x faster                                               |
| xml_etree_process          | 37.2 ms                                                     | 36.2 ms: 1.03x faster                                               |
| scimark_sor                | 78.1 ms                                                     | 76.2 ms: 1.02x faster                                               |
| fannkuch                   | 253 ms                                                      | 249 ms: 1.02x faster                                                |
| mdp                        | 1.59 sec                                                    | 1.58 sec: 1.01x faster                                              |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                               |
| pidigits                   | 150 ms                                                      | 152 ms: 1.02x slower                                                |
| scimark_monte_carlo        | 45.3 ms                                                     | 46.1 ms: 1.02x slower                                               |
| meteor_contest             | 75.2 ms                                                     | 76.6 ms: 1.02x slower                                               |
| sqlglot_optimize           | 34.5 ms                                                     | 35.4 ms: 1.02x slower                                               |
| pickle_list                | 2.70 us                                                     | 2.77 us: 1.03x slower                                               |
| 2to3                       | 214 ms                                                      | 219 ms: 1.03x slower                                                |
| json_loads                 | 13.0 us                                                     | 13.4 us: 1.03x slower                                               |
| go                         | 101 ms                                                      | 105 ms: 1.03x slower                                                |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.68 ms: 1.04x slower                                               |
| coverage                   | 43.4 ms                                                     | 45.4 ms: 1.05x slower                                               |
| unpickle_list              | 2.59 us                                                     | 2.72 us: 1.05x slower                                               |
| regex_dna                  | 116 ms                                                      | 122 ms: 1.05x slower                                                |
| python_startup             | 19.8 ms                                                     | 21.0 ms: 1.06x slower                                               |
| regex_effbot               | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                               |
| scimark_fft                | 179 ms                                                      | 193 ms: 1.08x slower                                                |
| pickle                     | 6.64 us                                                     | 7.20 us: 1.09x slower                                               |
| regex_v8                   | 14.2 ms                                                     | 15.5 ms: 1.10x slower                                               |
| unpickle                   | 7.57 us                                                     | 8.34 us: 1.10x slower                                               |
| telco                      | 4.06 ms                                                     | 4.59 ms: 1.13x slower                                               |
| bench_mp_pool              | 63.2 ms                                                     | 71.7 ms: 1.13x slower                                               |
| python_startup_no_site     | 16.8 ms                                                     | 19.1 ms: 1.14x slower                                               |
| pathlib                    | 70.9 ms                                                     | 80.7 ms: 1.14x slower                                               |
| hexiom                     | 4.55 ms                                                     | 5.42 ms: 1.19x slower                                               |
| async_generators           | 177 ms                                                      | 245 ms: 1.39x slower                                                |
| Geometric mean             | (ref)                                                       | 1.08x faster                                                        |

Benchmark hidden because not significant (3): json, xml_etree_generate, create_gc_cycles
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown