
# Results vs. 3.11.0

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-amd64
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.02x faster \*
- HPT reliability: 63.62%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 225 ms: 1.06x slower                                                        |
| chameleon      | 5.26 ms                                                     | 5.07 ms: 1.04x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                                      |
| tornado_http   | 92.8 ms                                                     | 86.2 ms: 1.08x faster                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 271 ms: 1.22x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 458 ms: 1.16x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 345 ms: 1.15x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 467 ms: 1.12x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 276 ms: 1.12x faster                                                        |
| async_tree_io              | 808 ms                                                      | 729 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 764 ms: 1.08x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| float          | 54.4 ms                                                     | 59.0 ms: 1.09x slower                                                       |
| nbody          | 70.3 ms                                                     | 81.4 ms: 1.16x slower                                                       |
| Geometric mean | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 116 ms                                                      | 118 ms: 1.02x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.04x slower                                                       |
| regex_compile  | 91.0 ms                                                     | 102 ms: 1.13x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 16.6 ms: 1.17x slower                                                       |
| Geometric mean | (ref)                                                       | 1.09x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.68 ms: 1.43x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 186 us: 1.12x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 92.7 ms: 1.05x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.4 us: 1.00x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 38.8 ms: 1.04x slower                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 68.6 ms: 1.05x slower                                                       |
| pickle               | 6.64 us                                                     | 7.03 us: 1.06x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.75 us: 1.06x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.8 us: 1.07x slower                                                       |
| unpickle_pure_python | 157 us                                                      | 168 us: 1.07x slower                                                        |
| xml_etree_generate   | 52.5 ms                                                     | 56.8 ms: 1.08x slower                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.58 sec: 1.08x slower                                                      |
| unpickle             | 7.57 us                                                     | 8.32 us: 1.10x slower                                                       |
| pickle_list          | 2.70 us                                                     | 3.20 us: 1.19x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.02x slower                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 19.9 ms: 1.01x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 17.9 ms: 1.06x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.04x slower                                                                |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 75.3 us: 4.33x faster                                                       |
| generators                 | 34.0 ms                                                     | 20.6 ms: 1.65x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 466 ms: 1.56x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.68 ms: 1.43x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 56.9 ns: 1.26x faster                                                       |
| async_tree_none            | 332 ms                                                      | 271 ms: 1.22x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 458 ms: 1.16x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 345 ms: 1.15x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.76 sec: 1.15x faster                                                      |
| deltablue                  | 2.70 ms                                                     | 2.35 ms: 1.15x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 835 us: 1.14x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 13.2 ms: 1.13x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 467 ms: 1.12x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 186 us: 1.12x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 276 ms: 1.12x faster                                                        |
| async_tree_io              | 808 ms                                                      | 729 ms: 1.11x faster                                                        |
| unpack_sequence            | 46.9 ns                                                     | 42.4 ns: 1.11x faster                                                       |
| sqlite_synth               | 1.77 us                                                     | 1.60 us: 1.11x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.06 ms: 1.09x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.46 sec: 1.09x faster                                                      |
| richards_super             | 38.7 ms                                                     | 35.7 ms: 1.09x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 764 ms: 1.08x faster                                                        |
| comprehensions             | 15.6 us                                                     | 14.5 us: 1.08x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 86.2 ms: 1.08x faster                                                       |
| logging_simple             | 6.86 us                                                     | 6.42 us: 1.07x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 94.0 ms: 1.07x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 43.6 ms: 1.06x faster                                                       |
| chaos                      | 48.4 ms                                                     | 45.7 ms: 1.06x faster                                                       |
| raytrace                   | 213 ms                                                      | 202 ms: 1.06x faster                                                        |
| deepcopy                   | 246 us                                                      | 234 us: 1.05x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 92.7 ms: 1.05x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 24.8 us: 1.05x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.86 us: 1.04x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 5.07 ms: 1.04x faster                                                       |
| sympy_str                  | 185 ms                                                      | 179 ms: 1.03x faster                                                        |
| mypy2                      | 459 ms                                                      | 445 ms: 1.03x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 2.01 us: 1.03x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 47.9 ms: 1.02x faster                                                       |
| pidigits                   | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 189 ms: 1.00x faster                                                        |
| pickle_dict                | 18.5 us                                                     | 18.4 us: 1.00x faster                                                       |
| sympy_expand               | 299 ms                                                      | 300 ms: 1.00x slower                                                        |
| python_startup             | 19.8 ms                                                     | 19.9 ms: 1.01x slower                                                       |
| docutils                   | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                                      |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                       |
| richards                   | 31.4 ms                                                     | 31.9 ms: 1.02x slower                                                       |
| regex_dna                  | 116 ms                                                      | 118 ms: 1.02x slower                                                        |
| meteor_contest             | 75.2 ms                                                     | 76.9 ms: 1.02x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 65.0 ms: 1.03x slower                                                       |
| go                         | 101 ms                                                      | 104 ms: 1.03x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 738 us: 1.03x slower                                                        |
| pycparser                  | 720 ms                                                      | 746 ms: 1.04x slower                                                        |
| nqueens                    | 68.3 ms                                                     | 71.4 ms: 1.04x slower                                                       |
| xml_etree_process          | 37.2 ms                                                     | 38.8 ms: 1.04x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.57 ms: 1.04x slower                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 68.6 ms: 1.05x slower                                                       |
| 2to3                       | 214 ms                                                      | 225 ms: 1.06x slower                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 36.6 ms: 1.06x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.03 us: 1.06x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.75 us: 1.06x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 17.9 ms: 1.06x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.8 us: 1.07x slower                                                       |
| unpickle_pure_python       | 157 us                                                      | 168 us: 1.07x slower                                                        |
| pprint_safe_repr           | 529 ms                                                      | 569 ms: 1.07x slower                                                        |
| pprint_pformat             | 1.09 sec                                                    | 1.17 sec: 1.08x slower                                                      |
| fannkuch                   | 253 ms                                                      | 273 ms: 1.08x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 56.8 ms: 1.08x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 76.8 ms: 1.08x slower                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.58 sec: 1.08x slower                                                      |
| float                      | 54.4 ms                                                     | 59.0 ms: 1.09x slower                                                       |
| coverage                   | 43.4 ms                                                     | 47.5 ms: 1.09x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.32 us: 1.10x slower                                                       |
| regex_compile              | 91.0 ms                                                     | 102 ms: 1.13x slower                                                        |
| pyflate                    | 312 ms                                                      | 352 ms: 1.13x slower                                                        |
| nbody                      | 70.3 ms                                                     | 81.4 ms: 1.16x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 16.6 ms: 1.17x slower                                                       |
| pickle_list                | 2.70 us                                                     | 3.20 us: 1.19x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.85 ms: 1.19x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 94.1 ms: 1.20x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 54.7 ms: 1.21x slower                                                       |
| scimark_fft                | 179 ms                                                      | 219 ms: 1.22x slower                                                        |
| spectral_norm              | 68.3 ms                                                     | 83.5 ms: 1.22x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.61 ms: 1.23x slower                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.22 ms: 1.25x slower                                                       |
| scimark_lu                 | 62.8 ms                                                     | 81.1 ms: 1.29x slower                                                       |
| async_generators           | 177 ms                                                      | 237 ms: 1.34x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (4): json, bench_thread_pool, mako, sympy_integrate
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 63.62% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown