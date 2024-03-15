
# Results vs. 3.11.0

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-amd64
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.04x faster \*
- HPT reliability: 97.05%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 227 ms: 1.06x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.80 ms: 1.10x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.67 sec: 1.02x slower                                                      |
| tornado_http   | 92.8 ms                                                     | 85.6 ms: 1.08x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 265 ms: 1.26x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 344 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 339 ms: 1.18x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 454 ms: 1.17x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.14x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 467 ms: 1.12x faster                                                        |
| async_tree_io              | 808 ms                                                      | 728 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 750 ms: 1.11x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 61.9 ms: 1.14x faster                                                       |
| float          | 54.4 ms                                                     | 50.0 ms: 1.09x faster                                                       |
| pidigits       | 150 ms                                                      | 152 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 116 ms                                                      | 119 ms: 1.02x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| regex_compile  | 91.0 ms                                                     | 104 ms: 1.14x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 16.7 ms: 1.18x slower                                                       |
| Geometric mean | (ref)                                                       | 1.09x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 176 us: 1.18x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.32 sec: 1.10x faster                                                      |
| unpickle_pure_python | 157 us                                                      | 142 us: 1.10x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 92.3 ms: 1.06x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 17.6 us: 1.05x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.6 ms: 1.03x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 36.9 ms: 1.01x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 53.3 ms: 1.01x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.8 us: 1.06x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.78 us: 1.07x slower                                                       |
| pickle               | 6.64 us                                                     | 7.33 us: 1.11x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.50 us: 1.12x slower                                                       |
| pickle_list          | 2.70 us                                                     | 3.10 us: 1.15x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 23.2 ms: 1.17x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 20.9 ms: 1.24x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.21x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.45 ms: 1.18x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 70.8 us: 4.60x faster                                                       |
| generators                 | 34.0 ms                                                     | 20.9 ms: 1.62x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 475 ms: 1.53x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 55.4 ns: 1.29x faster                                                       |
| comprehensions             | 15.6 us                                                     | 12.2 us: 1.28x faster                                                       |
| async_tree_none            | 332 ms                                                      | 265 ms: 1.26x faster                                                        |
| deltablue                  | 2.70 ms                                                     | 2.18 ms: 1.24x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 21.8 us: 1.19x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 176 us: 1.18x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 344 ms: 1.18x faster                                                        |
| mako                       | 7.58 ms                                                     | 6.45 ms: 1.18x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 339 ms: 1.18x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 454 ms: 1.17x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 824 us: 1.16x faster                                                        |
| nbody                      | 70.3 ms                                                     | 61.9 ms: 1.14x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.14x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 13.2 ms: 1.13x faster                                                       |
| sqlite_synth               | 1.77 us                                                     | 1.57 us: 1.13x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.80 sec: 1.13x faster                                                      |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 467 ms: 1.12x faster                                                        |
| logging_simple             | 6.86 us                                                     | 6.13 us: 1.12x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.04 ms: 1.12x faster                                                       |
| raytrace                   | 213 ms                                                      | 191 ms: 1.12x faster                                                        |
| chaos                      | 48.4 ms                                                     | 43.5 ms: 1.11x faster                                                       |
| async_tree_io              | 808 ms                                                      | 728 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 750 ms: 1.11x faster                                                        |
| richards_super             | 38.7 ms                                                     | 35.0 ms: 1.11x faster                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.32 sec: 1.10x faster                                                      |
| unpickle_pure_python       | 157 us                                                      | 142 us: 1.10x faster                                                        |
| deepcopy                   | 246 us                                                      | 224 us: 1.10x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.53 us: 1.10x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 4.80 ms: 1.10x faster                                                       |
| float                      | 54.4 ms                                                     | 50.0 ms: 1.09x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 85.6 ms: 1.08x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 43.2 ms: 1.07x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 1.94 us: 1.06x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 94.2 ms: 1.06x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 46.1 ms: 1.06x faster                                                       |
| spectral_norm              | 68.3 ms                                                     | 64.5 ms: 1.06x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 92.3 ms: 1.06x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 64.7 ms: 1.06x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 17.6 us: 1.05x faster                                                       |
| bench_thread_pool          | 872 us                                                      | 841 us: 1.04x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 184 ms: 1.04x faster                                                        |
| sympy_str                  | 185 ms                                                      | 179 ms: 1.03x faster                                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.6 ms: 1.03x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 517 ms: 1.02x faster                                                        |
| pprint_pformat             | 1.09 sec                                                    | 1.07 sec: 1.02x faster                                                      |
| xml_etree_process          | 37.2 ms                                                     | 36.9 ms: 1.01x faster                                                       |
| pidigits                   | 150 ms                                                      | 152 ms: 1.01x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 53.3 ms: 1.01x slower                                                       |
| docutils                   | 1.64 sec                                                    | 1.67 sec: 1.02x slower                                                      |
| regex_dna                  | 116 ms                                                      | 119 ms: 1.02x slower                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.63 ms: 1.02x slower                                                       |
| meteor_contest             | 75.2 ms                                                     | 76.9 ms: 1.02x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 738 us: 1.04x slower                                                        |
| sympy_expand               | 299 ms                                                      | 310 ms: 1.04x slower                                                        |
| fannkuch                   | 253 ms                                                      | 263 ms: 1.04x slower                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 36.1 ms: 1.04x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| pyflate                    | 312 ms                                                      | 328 ms: 1.05x slower                                                        |
| scimark_monte_carlo        | 45.3 ms                                                     | 47.6 ms: 1.05x slower                                                       |
| mdp                        | 1.59 sec                                                    | 1.68 sec: 1.05x slower                                                      |
| json_loads                 | 13.0 us                                                     | 13.8 us: 1.06x slower                                                       |
| 2to3                       | 214 ms                                                      | 227 ms: 1.06x slower                                                        |
| unpickle_list              | 2.59 us                                                     | 2.78 us: 1.07x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 76.1 ms: 1.07x slower                                                       |
| go                         | 101 ms                                                      | 109 ms: 1.08x slower                                                        |
| scimark_fft                | 179 ms                                                      | 194 ms: 1.08x slower                                                        |
| bench_mp_pool              | 63.2 ms                                                     | 69.4 ms: 1.10x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.33 us: 1.11x slower                                                       |
| coverage                   | 43.4 ms                                                     | 48.0 ms: 1.11x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.50 us: 1.12x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.59 ms: 1.13x slower                                                       |
| regex_compile              | 91.0 ms                                                     | 104 ms: 1.14x slower                                                        |
| pickle_list                | 2.70 us                                                     | 3.10 us: 1.15x slower                                                       |
| python_startup             | 19.8 ms                                                     | 23.2 ms: 1.17x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 16.7 ms: 1.18x slower                                                       |
| scimark_lu                 | 62.8 ms                                                     | 76.6 ms: 1.22x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 20.9 ms: 1.24x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 102 ms: 1.31x slower                                                        |
| hexiom                     | 4.55 ms                                                     | 6.28 ms: 1.38x slower                                                       |
| async_generators           | 177 ms                                                      | 255 ms: 1.44x slower                                                        |
| unpack_sequence            | 46.9 ns                                                     | 88.5 ns: 1.89x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (6): sympy_integrate, mypy2, richards, gc_traversal, pycparser, json
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 97.05% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown