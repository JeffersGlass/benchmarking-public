
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_continue
- machine: windows-amd64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| chameleon      | 5.26 ms                                                     | 4.71 ms: 1.12x faster                                                        |
| docutils       | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                       |
| tornado_http   | 92.8 ms                                                     | 83.9 ms: 1.11x faster                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                 |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 261 ms: 1.28x faster                                                         |
| async_tree_memoization     | 399 ms                                                      | 334 ms: 1.19x faster                                                         |
| async_tree_memoization_tg  | 405 ms                                                      | 339 ms: 1.19x faster                                                         |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 447 ms: 1.19x faster                                                         |
| async_tree_none_tg         | 309 ms                                                      | 268 ms: 1.15x faster                                                         |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 462 ms: 1.13x faster                                                         |
| async_tree_io              | 808 ms                                                      | 714 ms: 1.13x faster                                                         |
| async_tree_io_tg           | 829 ms                                                      | 748 ms: 1.11x faster                                                         |
| Geometric mean             | (ref)                                                       | 1.17x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 58.4 ms: 1.20x faster                                                        |
| float          | 54.4 ms                                                     | 49.5 ms: 1.10x faster                                                        |
| pidigits       | 150 ms                                                      | 151 ms: 1.00x slower                                                         |
| Geometric mean | (ref)                                                       | 1.10x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 76.9 ms: 1.18x faster                                                        |
| regex_dna      | 116 ms                                                      | 119 ms: 1.03x slower                                                         |
| regex_effbot   | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 15.1 ms: 1.06x slower                                                        |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.53 ms: 1.46x faster                                                        |
| unpickle_pure_python | 157 us                                                      | 123 us: 1.27x faster                                                         |
| tomli_loads          | 1.46 sec                                                    | 1.19 sec: 1.23x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 174 us: 1.20x faster                                                         |
| pickle_dict          | 18.5 us                                                     | 17.5 us: 1.06x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 92.7 ms: 1.05x faster                                                        |
| xml_etree_iterparse  | 65.6 ms                                                     | 62.7 ms: 1.05x faster                                                        |
| xml_etree_process    | 37.2 ms                                                     | 36.1 ms: 1.03x faster                                                        |
| xml_etree_generate   | 52.5 ms                                                     | 52.2 ms: 1.01x faster                                                        |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.05x slower                                                        |
| pickle               | 6.64 us                                                     | 7.10 us: 1.07x slower                                                        |
| unpickle_list        | 2.59 us                                                     | 2.78 us: 1.07x slower                                                        |
| unpickle             | 7.57 us                                                     | 8.50 us: 1.12x slower                                                        |
| pickle_list          | 2.70 us                                                     | 3.13 us: 1.16x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.1 ms: 1.02x slower                                                        |
| python_startup_no_site | 16.8 ms                                                     | 18.0 ms: 1.07x slower                                                        |
| Geometric mean         | (ref)                                                       | 1.04x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 5.98 ms: 1.27x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 70.5 us: 4.63x faster                                                        |
| generators                 | 34.0 ms                                                     | 19.9 ms: 1.71x faster                                                        |
| asyncio_tcp                | 726 ms                                                      | 472 ms: 1.54x faster                                                         |
| comprehensions             | 15.6 us                                                     | 10.6 us: 1.47x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.53 ms: 1.46x faster                                                        |
| deltablue                  | 2.70 ms                                                     | 1.94 ms: 1.39x faster                                                        |
| richards_super             | 38.7 ms                                                     | 27.9 ms: 1.39x faster                                                        |
| logging_silent             | 71.8 ns                                                     | 52.0 ns: 1.38x faster                                                        |
| raytrace                   | 213 ms                                                      | 167 ms: 1.28x faster                                                         |
| sqlglot_parse              | 953 us                                                      | 747 us: 1.28x faster                                                         |
| async_tree_none            | 332 ms                                                      | 261 ms: 1.28x faster                                                         |
| unpickle_pure_python       | 157 us                                                      | 123 us: 1.27x faster                                                         |
| mako                       | 7.58 ms                                                     | 5.98 ms: 1.27x faster                                                        |
| richards                   | 31.4 ms                                                     | 24.8 ms: 1.27x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 54.4 ms: 1.26x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 20.7 us: 1.25x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.19 sec: 1.23x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 963 us: 1.21x faster                                                         |
| unpack_sequence            | 46.9 ns                                                     | 38.8 ns: 1.21x faster                                                        |
| nbody                      | 70.3 ms                                                     | 58.4 ms: 1.20x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 174 us: 1.20x faster                                                         |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.69 sec: 1.20x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 334 ms: 1.19x faster                                                         |
| async_tree_memoization_tg  | 405 ms                                                      | 339 ms: 1.19x faster                                                         |
| chaos                      | 48.4 ms                                                     | 40.6 ms: 1.19x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 447 ms: 1.19x faster                                                         |
| regex_compile              | 91.0 ms                                                     | 76.9 ms: 1.18x faster                                                        |
| logging_simple             | 6.86 us                                                     | 5.84 us: 1.18x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 58.2 ms: 1.17x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.51 us: 1.17x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 39.6 ms: 1.17x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 12.8 ms: 1.17x faster                                                        |
| fannkuch                   | 253 ms                                                      | 218 ms: 1.16x faster                                                         |
| sympy_sum                  | 100 ms                                                      | 86.5 ms: 1.16x faster                                                        |
| scimark_lu                 | 62.8 ms                                                     | 54.4 ms: 1.16x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 268 ms: 1.15x faster                                                         |
| deepcopy                   | 246 us                                                      | 214 us: 1.15x faster                                                         |
| sympy_str                  | 185 ms                                                      | 161 ms: 1.15x faster                                                         |
| pprint_pformat             | 1.09 sec                                                    | 950 ms: 1.14x faster                                                         |
| pprint_safe_repr           | 529 ms                                                      | 465 ms: 1.14x faster                                                         |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 462 ms: 1.13x faster                                                         |
| async_tree_io              | 808 ms                                                      | 714 ms: 1.13x faster                                                         |
| logging_format             | 7.16 us                                                     | 6.35 us: 1.13x faster                                                        |
| go                         | 101 ms                                                      | 90.0 ms: 1.12x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 43.5 ms: 1.12x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.71 ms: 1.12x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 748 ms: 1.11x faster                                                         |
| tornado_http               | 92.8 ms                                                     | 83.9 ms: 1.11x faster                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.33 ms: 1.10x faster                                                        |
| pyflate                    | 312 ms                                                      | 284 ms: 1.10x faster                                                         |
| float                      | 54.4 ms                                                     | 49.5 ms: 1.10x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 12.8 ms: 1.09x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 174 ms: 1.09x faster                                                         |
| mypy2                      | 459 ms                                                      | 420 ms: 1.09x faster                                                         |
| sympy_expand               | 299 ms                                                      | 275 ms: 1.09x faster                                                         |
| bench_thread_pool          | 872 us                                                      | 803 us: 1.09x faster                                                         |
| deepcopy_reduce            | 2.06 us                                                     | 1.91 us: 1.08x faster                                                        |
| dask                       | 273 ms                                                      | 254 ms: 1.07x faster                                                         |
| pickle_dict                | 18.5 us                                                     | 17.5 us: 1.06x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 92.7 ms: 1.05x faster                                                        |
| docutils                   | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                       |
| pycparser                  | 720 ms                                                      | 686 ms: 1.05x faster                                                         |
| xml_etree_iterparse        | 65.6 ms                                                     | 62.7 ms: 1.05x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 33.3 ms: 1.04x faster                                                        |
| meteor_contest             | 75.2 ms                                                     | 72.4 ms: 1.04x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.54 sec: 1.03x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 36.1 ms: 1.03x faster                                                        |
| scimark_sor                | 78.1 ms                                                     | 76.1 ms: 1.03x faster                                                        |
| hexiom                     | 4.55 ms                                                     | 4.44 ms: 1.03x faster                                                        |
| scimark_fft                | 179 ms                                                      | 176 ms: 1.02x faster                                                         |
| xml_etree_generate         | 52.5 ms                                                     | 52.2 ms: 1.01x faster                                                        |
| pidigits                   | 150 ms                                                      | 151 ms: 1.00x slower                                                         |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                        |
| python_startup             | 19.8 ms                                                     | 20.1 ms: 1.02x slower                                                        |
| regex_dna                  | 116 ms                                                      | 119 ms: 1.03x slower                                                         |
| create_gc_cycles           | 713 us                                                      | 735 us: 1.03x slower                                                         |
| bench_mp_pool              | 63.2 ms                                                     | 65.6 ms: 1.04x slower                                                        |
| json_loads                 | 13.0 us                                                     | 13.6 us: 1.05x slower                                                        |
| scimark_monte_carlo        | 45.3 ms                                                     | 47.6 ms: 1.05x slower                                                        |
| regex_effbot               | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                        |
| pathlib                    | 70.9 ms                                                     | 75.2 ms: 1.06x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 15.1 ms: 1.06x slower                                                        |
| pickle                     | 6.64 us                                                     | 7.10 us: 1.07x slower                                                        |
| python_startup_no_site     | 16.8 ms                                                     | 18.0 ms: 1.07x slower                                                        |
| unpickle_list              | 2.59 us                                                     | 2.78 us: 1.07x slower                                                        |
| coverage                   | 43.4 ms                                                     | 47.0 ms: 1.08x slower                                                        |
| telco                      | 4.06 ms                                                     | 4.53 ms: 1.11x slower                                                        |
| unpickle                   | 7.57 us                                                     | 8.50 us: 1.12x slower                                                        |
| json                       | 2.98 ms                                                     | 3.38 ms: 1.14x slower                                                        |
| pickle_list                | 2.70 us                                                     | 3.13 us: 1.16x slower                                                        |
| async_generators           | 177 ms                                                      | 235 ms: 1.32x slower                                                         |
| Geometric mean             | (ref)                                                       | 1.13x faster                                                                 |

Benchmark hidden because not significant (1): 2to3
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown