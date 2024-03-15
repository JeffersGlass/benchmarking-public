
# Results vs. 3.11.0

- fork: python
- ref: v3.12.1
- machine: windows-amd64
- commit hash: 2305ca5
- commit date: 2023-12-07
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 215 ms: 1.01x slower                                        |
| chameleon      | 5.26 ms                                                     | 5.06 ms: 1.04x faster                                       |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                      |
| tornado_http   | 92.8 ms                                                     | 87.0 ms: 1.07x faster                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_memoization     | 399 ms                                                      | 340 ms: 1.17x faster                                        |
| async_tree_none            | 332 ms                                                      | 288 ms: 1.15x faster                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 351 ms: 1.15x faster                                        |
| async_tree_none_tg         | 309 ms                                                      | 279 ms: 1.11x faster                                        |
| async_tree_io              | 808 ms                                                      | 731 ms: 1.10x faster                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 483 ms: 1.10x faster                                        |
| async_tree_io_tg           | 829 ms                                                      | 762 ms: 1.09x faster                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 490 ms: 1.07x faster                                        |
| Geometric mean             | (ref)                                                       | 1.12x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 69.5 ms: 1.01x faster                                       |
| pidigits       | 150 ms                                                      | 151 ms: 1.01x slower                                        |
| Geometric mean | (ref)                                                       | 1.00x faster                                                |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 85.0 ms: 1.07x faster                                       |
| regex_v8       | 14.2 ms                                                     | 14.1 ms: 1.00x faster                                       |
| regex_dna      | 116 ms                                                      | 121 ms: 1.04x slower                                        |
| regex_effbot   | 1.50 ms                                                     | 1.63 ms: 1.09x slower                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.69 ms: 1.42x faster                                       |
| unpickle_pure_python | 157 us                                                      | 133 us: 1.18x faster                                        |
| pickle_pure_python   | 208 us                                                      | 193 us: 1.08x faster                                        |
| tomli_loads          | 1.46 sec                                                    | 1.36 sec: 1.07x faster                                      |
| xml_etree_parse      | 97.6 ms                                                     | 92.8 ms: 1.05x faster                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.0 ms: 1.02x faster                                       |
| pickle_dict          | 18.5 us                                                     | 18.2 us: 1.01x faster                                       |
| xml_etree_process    | 37.2 ms                                                     | 38.4 ms: 1.03x slower                                       |
| unpickle_list        | 2.59 us                                                     | 2.68 us: 1.03x slower                                       |
| pickle               | 6.64 us                                                     | 6.95 us: 1.05x slower                                       |
| pickle_list          | 2.70 us                                                     | 2.85 us: 1.06x slower                                       |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.06x slower                                       |
| unpickle             | 7.57 us                                                     | 8.13 us: 1.07x slower                                       |
| xml_etree_generate   | 52.5 ms                                                     | 57.1 ms: 1.09x slower                                       |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 16.3 ms: 1.03x faster                                       |
| python_startup         | 19.8 ms                                                     | 19.5 ms: 1.02x faster                                       |
| Geometric mean         | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 7.58 ms                                                     | 6.89 ms: 1.10x faster                                       |
| django_template | 24.4 ms                                                     | 23.7 ms: 1.03x faster                                       |
| Geometric mean  | (ref)                                                       | 1.06x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 76.4 us: 4.26x faster                                       |
| asyncio_tcp                | 726 ms                                                      | 470 ms: 1.54x faster                                        |
| generators                 | 34.0 ms                                                     | 22.6 ms: 1.50x faster                                       |
| json_dumps                 | 8.09 ms                                                     | 5.69 ms: 1.42x faster                                       |
| richards_super             | 38.7 ms                                                     | 30.5 ms: 1.27x faster                                       |
| deltablue                  | 2.70 ms                                                     | 2.14 ms: 1.26x faster                                       |
| unpickle_pure_python       | 157 us                                                      | 133 us: 1.18x faster                                        |
| unpack_sequence            | 46.9 ns                                                     | 39.9 ns: 1.18x faster                                       |
| async_tree_memoization     | 399 ms                                                      | 340 ms: 1.17x faster                                        |
| richards                   | 31.4 ms                                                     | 26.9 ms: 1.17x faster                                       |
| sqlglot_parse              | 953 us                                                      | 821 us: 1.16x faster                                        |
| mdp                        | 1.59 sec                                                    | 1.38 sec: 1.16x faster                                      |
| logging_silent             | 71.8 ns                                                     | 62.1 ns: 1.16x faster                                       |
| async_tree_none            | 332 ms                                                      | 288 ms: 1.15x faster                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 351 ms: 1.15x faster                                        |
| go                         | 101 ms                                                      | 87.8 ms: 1.15x faster                                       |
| coverage                   | 43.4 ms                                                     | 38.2 ms: 1.14x faster                                       |
| sqlalchemy_imperative      | 10.4 ms                                                     | 9.23 ms: 1.13x faster                                       |
| hexiom                     | 4.55 ms                                                     | 4.03 ms: 1.13x faster                                       |
| sympy_sum                  | 100 ms                                                      | 89.1 ms: 1.12x faster                                       |
| comprehensions             | 15.6 us                                                     | 13.9 us: 1.12x faster                                       |
| chaos                      | 48.4 ms                                                     | 43.2 ms: 1.12x faster                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.04 ms: 1.12x faster                                       |
| async_tree_none_tg         | 309 ms                                                      | 279 ms: 1.11x faster                                        |
| async_tree_io              | 808 ms                                                      | 731 ms: 1.10x faster                                        |
| raytrace                   | 213 ms                                                      | 193 ms: 1.10x faster                                        |
| mako                       | 7.58 ms                                                     | 6.89 ms: 1.10x faster                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 483 ms: 1.10x faster                                        |
| deepcopy_memo              | 26.0 us                                                     | 23.7 us: 1.09x faster                                       |
| sympy_integrate            | 14.0 ms                                                     | 12.9 ms: 1.09x faster                                       |
| nqueens                    | 68.3 ms                                                     | 62.6 ms: 1.09x faster                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.86 sec: 1.09x faster                                      |
| async_tree_io_tg           | 829 ms                                                      | 762 ms: 1.09x faster                                        |
| spectral_norm              | 68.3 ms                                                     | 63.2 ms: 1.08x faster                                       |
| pickle_pure_python         | 208 us                                                      | 193 us: 1.08x faster                                        |
| logging_simple             | 6.86 us                                                     | 6.39 us: 1.07x faster                                       |
| sympy_str                  | 185 ms                                                      | 173 ms: 1.07x faster                                        |
| dulwich_log                | 46.4 ms                                                     | 43.2 ms: 1.07x faster                                       |
| regex_compile              | 91.0 ms                                                     | 85.0 ms: 1.07x faster                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 490 ms: 1.07x faster                                        |
| tomli_loads                | 1.46 sec                                                    | 1.36 sec: 1.07x faster                                      |
| tornado_http               | 92.8 ms                                                     | 87.0 ms: 1.07x faster                                       |
| pyflate                    | 312 ms                                                      | 294 ms: 1.06x faster                                        |
| coroutines                 | 15.0 ms                                                     | 14.1 ms: 1.06x faster                                       |
| deepcopy                   | 246 us                                                      | 233 us: 1.06x faster                                        |
| fannkuch                   | 253 ms                                                      | 239 ms: 1.06x faster                                        |
| scimark_lu                 | 62.8 ms                                                     | 59.4 ms: 1.06x faster                                       |
| dask                       | 273 ms                                                      | 259 ms: 1.05x faster                                        |
| sympy_expand               | 299 ms                                                      | 284 ms: 1.05x faster                                        |
| xml_etree_parse            | 97.6 ms                                                     | 92.8 ms: 1.05x faster                                       |
| crypto_pyaes               | 48.9 ms                                                     | 46.5 ms: 1.05x faster                                       |
| pycparser                  | 720 ms                                                      | 687 ms: 1.05x faster                                        |
| logging_format             | 7.16 us                                                     | 6.87 us: 1.04x faster                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.04 sec: 1.04x faster                                      |
| chameleon                  | 5.26 ms                                                     | 5.06 ms: 1.04x faster                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.49 ms: 1.04x faster                                       |
| pprint_safe_repr           | 529 ms                                                      | 511 ms: 1.04x faster                                        |
| django_template            | 24.4 ms                                                     | 23.7 ms: 1.03x faster                                       |
| python_startup_no_site     | 16.8 ms                                                     | 16.3 ms: 1.03x faster                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 44.1 ms: 1.03x faster                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 64.0 ms: 1.02x faster                                       |
| docutils                   | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                      |
| aiohttp                    | 883 us                                                      | 864 us: 1.02x faster                                        |
| meteor_contest             | 75.2 ms                                                     | 73.7 ms: 1.02x faster                                       |
| sqlglot_normalize          | 190 ms                                                      | 187 ms: 1.02x faster                                        |
| python_startup             | 19.8 ms                                                     | 19.5 ms: 1.02x faster                                       |
| pickle_dict                | 18.5 us                                                     | 18.2 us: 1.01x faster                                       |
| nbody                      | 70.3 ms                                                     | 69.5 ms: 1.01x faster                                       |
| sqlalchemy_declarative     | 85.6 ms                                                     | 84.7 ms: 1.01x faster                                       |
| scimark_sor                | 78.1 ms                                                     | 77.8 ms: 1.00x faster                                       |
| regex_v8                   | 14.2 ms                                                     | 14.1 ms: 1.00x faster                                       |
| 2to3                       | 214 ms                                                      | 215 ms: 1.01x slower                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                       |
| pidigits                   | 150 ms                                                      | 151 ms: 1.01x slower                                        |
| telco                      | 4.06 ms                                                     | 4.12 ms: 1.01x slower                                       |
| create_gc_cycles           | 713 us                                                      | 730 us: 1.02x slower                                        |
| deepcopy_reduce            | 2.06 us                                                     | 2.13 us: 1.03x slower                                       |
| bench_mp_pool              | 63.2 ms                                                     | 65.3 ms: 1.03x slower                                       |
| xml_etree_process          | 37.2 ms                                                     | 38.4 ms: 1.03x slower                                       |
| unpickle_list              | 2.59 us                                                     | 2.68 us: 1.03x slower                                       |
| regex_dna                  | 116 ms                                                      | 121 ms: 1.04x slower                                        |
| pickle                     | 6.64 us                                                     | 6.95 us: 1.05x slower                                       |
| pickle_list                | 2.70 us                                                     | 2.85 us: 1.06x slower                                       |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.06x slower                                       |
| unpickle                   | 7.57 us                                                     | 8.13 us: 1.07x slower                                       |
| xml_etree_generate         | 52.5 ms                                                     | 57.1 ms: 1.09x slower                                       |
| regex_effbot               | 1.50 ms                                                     | 1.63 ms: 1.09x slower                                       |
| mypy2                      | 459 ms                                                      | 501 ms: 1.09x slower                                        |
| pathlib                    | 70.9 ms                                                     | 80.7 ms: 1.14x slower                                       |
| async_generators           | 177 ms                                                      | 237 ms: 1.34x slower                                        |
| Geometric mean             | (ref)                                                       | 1.07x faster                                                |

Benchmark hidden because not significant (6): bench_thread_pool, json, gc_traversal, scimark_fft, sqlite_synth, float
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: unknown