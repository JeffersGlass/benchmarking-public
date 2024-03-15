
# Results vs. 3.11.0

- fork: python
- ref: 4297d7301b97aba2e0df
- machine: windows-amd64
- commit hash: 4297d73
- commit date: 2024-02-12
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 216 ms: 1.01x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.78 ms: 1.10x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.57 sec: 1.04x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 84.9 ms: 1.09x faster                                                       |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 263 ms: 1.26x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 333 ms: 1.20x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 340 ms: 1.19x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 451 ms: 1.18x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 269 ms: 1.15x faster                                                        |
| async_tree_io              | 808 ms                                                      | 716 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 466 ms: 1.12x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 746 ms: 1.11x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.17x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 61.7 ms: 1.14x faster                                                       |
| float          | 54.4 ms                                                     | 50.0 ms: 1.09x faster                                                       |
| pidigits       | 150 ms                                                      | 152 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 79.9 ms: 1.14x faster                                                       |
| regex_dna      | 116 ms                                                      | 119 ms: 1.03x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.55 ms: 1.46x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 125 us: 1.26x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 173 us: 1.21x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.27 sec: 1.15x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 17.6 us: 1.05x faster                                                       |
| xml_etree_parse      | 97.6 ms                                                     | 93.9 ms: 1.04x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.4 ms: 1.03x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 36.3 ms: 1.02x faster                                                       |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.06x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.76 us: 1.07x slower                                                       |
| pickle               | 6.64 us                                                     | 7.16 us: 1.08x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.54 us: 1.13x slower                                                       |
| pickle_list          | 2.70 us                                                     | 3.12 us: 1.16x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.2 ms: 1.02x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.1 ms: 1.07x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.44 ms: 1.18x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 69.1 us: 4.72x faster                                                       |
| generators                 | 34.0 ms                                                     | 20.0 ms: 1.70x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 465 ms: 1.56x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.55 ms: 1.46x faster                                                       |
| comprehensions             | 15.6 us                                                     | 11.3 us: 1.38x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 1.96 ms: 1.38x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 52.2 ns: 1.37x faster                                                       |
| richards_super             | 38.7 ms                                                     | 28.2 ms: 1.37x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 754 us: 1.26x faster                                                        |
| async_tree_none            | 332 ms                                                      | 263 ms: 1.26x faster                                                        |
| richards                   | 31.4 ms                                                     | 25.0 ms: 1.26x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 125 us: 1.26x faster                                                        |
| raytrace                   | 213 ms                                                      | 172 ms: 1.24x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 21.5 us: 1.21x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 173 us: 1.21x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 333 ms: 1.20x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 979 us: 1.19x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 340 ms: 1.19x faster                                                        |
| mako                       | 7.58 ms                                                     | 6.44 ms: 1.18x faster                                                       |
| logging_simple             | 6.86 us                                                     | 5.83 us: 1.18x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 451 ms: 1.18x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.51 us: 1.17x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 58.8 ms: 1.16x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 12.9 ms: 1.16x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 40.2 ms: 1.15x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 40.8 ns: 1.15x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 269 ms: 1.15x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.27 sec: 1.15x faster                                                      |
| logging_format             | 7.16 us                                                     | 6.28 us: 1.14x faster                                                       |
| chaos                      | 48.4 ms                                                     | 42.5 ms: 1.14x faster                                                       |
| nbody                      | 70.3 ms                                                     | 61.7 ms: 1.14x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 79.9 ms: 1.14x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 88.1 ms: 1.14x faster                                                       |
| deepcopy                   | 246 us                                                      | 217 us: 1.13x faster                                                        |
| async_tree_io              | 808 ms                                                      | 716 ms: 1.13x faster                                                        |
| scimark_lu                 | 62.8 ms                                                     | 55.9 ms: 1.12x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 466 ms: 1.12x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 746 ms: 1.11x faster                                                        |
| sympy_str                  | 185 ms                                                      | 167 ms: 1.11x faster                                                        |
| pprint_safe_repr           | 529 ms                                                      | 480 ms: 1.10x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.84 sec: 1.10x faster                                                      |
| chameleon                  | 5.26 ms                                                     | 4.78 ms: 1.10x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 991 ms: 1.10x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 84.9 ms: 1.09x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 1.89 us: 1.09x faster                                                       |
| float                      | 54.4 ms                                                     | 50.0 ms: 1.09x faster                                                       |
| mypy2                      | 459 ms                                                      | 425 ms: 1.08x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 45.5 ms: 1.07x faster                                                       |
| dask                       | 273 ms                                                      | 255 ms: 1.07x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 13.2 ms: 1.07x faster                                                       |
| sympy_expand               | 299 ms                                                      | 282 ms: 1.06x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 180 ms: 1.06x faster                                                        |
| bench_thread_pool          | 872 us                                                      | 826 us: 1.06x faster                                                        |
| pycparser                  | 720 ms                                                      | 685 ms: 1.05x faster                                                        |
| pickle_dict                | 18.5 us                                                     | 17.6 us: 1.05x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.57 sec: 1.04x faster                                                      |
| go                         | 101 ms                                                      | 97.1 ms: 1.04x faster                                                       |
| fannkuch                   | 253 ms                                                      | 243 ms: 1.04x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 65.7 ms: 1.04x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 93.9 ms: 1.04x faster                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.4 ms: 1.03x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.54 sec: 1.03x faster                                                      |
| xml_etree_process          | 37.2 ms                                                     | 36.3 ms: 1.02x faster                                                       |
| scimark_sor                | 78.1 ms                                                     | 77.2 ms: 1.01x faster                                                       |
| pyflate                    | 312 ms                                                      | 310 ms: 1.01x faster                                                        |
| meteor_contest             | 75.2 ms                                                     | 75.5 ms: 1.00x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.50 ms: 1.01x slower                                                       |
| 2to3                       | 214 ms                                                      | 216 ms: 1.01x slower                                                        |
| pidigits                   | 150 ms                                                      | 152 ms: 1.01x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 728 us: 1.02x slower                                                        |
| python_startup             | 19.8 ms                                                     | 20.2 ms: 1.02x slower                                                       |
| regex_dna                  | 116 ms                                                      | 119 ms: 1.03x slower                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.67 ms: 1.04x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 66.1 ms: 1.05x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 74.5 ms: 1.05x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.06x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.76 us: 1.07x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.1 ms: 1.07x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.16 us: 1.08x slower                                                       |
| scimark_fft                | 179 ms                                                      | 196 ms: 1.09x slower                                                        |
| coverage                   | 43.4 ms                                                     | 47.7 ms: 1.10x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.54 us: 1.13x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.22 ms: 1.15x slower                                                       |
| pickle_list                | 2.70 us                                                     | 3.12 us: 1.16x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.71 ms: 1.16x slower                                                       |
| json                       | 2.98 ms                                                     | 3.58 ms: 1.20x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 56.7 ms: 1.25x slower                                                       |
| async_generators           | 177 ms                                                      | 237 ms: 1.34x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (2): sqlglot_optimize, xml_etree_generate
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: unknown