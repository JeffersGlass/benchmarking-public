
# Results vs. 3.11.0

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-amd64
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 212 ms: 1.01x faster                                                        |
| chameleon      | 5.26 ms                                                     | 4.98 ms: 1.06x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.57 sec: 1.05x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 84.0 ms: 1.10x faster                                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 453 ms: 1.17x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 341 ms: 1.17x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 354 ms: 1.14x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 275 ms: 1.12x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 468 ms: 1.12x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 753 ms: 1.10x faster                                                        |
| async_tree_io              | 808 ms                                                      | 738 ms: 1.09x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.02x faster                                                        |
| nbody          | 70.3 ms                                                     | 72.9 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 79.8 ms: 1.14x faster                                                       |
| regex_dna      | 116 ms                                                      | 120 ms: 1.04x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 15.6 ms: 1.10x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.65 ms: 1.43x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 133 us: 1.18x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 185 us: 1.13x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 94.1 ms: 1.04x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.41 sec: 1.03x faster                                                      |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.1 ms: 1.02x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.2 us: 1.01x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 36.7 ms: 1.01x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 53.9 ms: 1.03x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.71 us: 1.05x slower                                                       |
| json_loads           | 13.0 us                                                     | 14.0 us: 1.07x slower                                                       |
| pickle               | 6.64 us                                                     | 7.14 us: 1.08x slower                                                       |
| pickle_list          | 2.70 us                                                     | 3.00 us: 1.11x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.58 us: 1.13x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 17.6 ms: 1.05x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.03x slower                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.49 ms: 1.17x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 72.8 us: 4.47x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.5 ms: 1.58x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 463 ms: 1.57x faster                                                        |
| comprehensions             | 15.6 us                                                     | 10.6 us: 1.48x faster                                                       |
| json_dumps                 | 8.09 ms                                                     | 5.65 ms: 1.43x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.03 ms: 1.33x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 55.5 ns: 1.29x faster                                                       |
| raytrace                   | 213 ms                                                      | 166 ms: 1.29x faster                                                        |
| unpack_sequence            | 46.9 ns                                                     | 36.7 ns: 1.28x faster                                                       |
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| richards_super             | 38.7 ms                                                     | 31.3 ms: 1.24x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 781 us: 1.22x faster                                                        |
| chaos                      | 48.4 ms                                                     | 40.4 ms: 1.20x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 83.7 ms: 1.20x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 52.9 ms: 1.19x faster                                                       |
| go                         | 101 ms                                                      | 85.7 ms: 1.18x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 133 us: 1.18x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 453 ms: 1.17x faster                                                        |
| hexiom                     | 4.55 ms                                                     | 3.89 ms: 1.17x faster                                                       |
| mako                       | 7.58 ms                                                     | 6.49 ms: 1.17x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 341 ms: 1.17x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.37 sec: 1.16x faster                                                      |
| deepcopy_memo              | 26.0 us                                                     | 22.3 us: 1.16x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.00 ms: 1.16x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.75 sec: 1.16x faster                                                      |
| sympy_str                  | 185 ms                                                      | 160 ms: 1.16x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 40.4 ms: 1.15x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 354 ms: 1.14x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 59.8 ms: 1.14x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 79.8 ms: 1.14x faster                                                       |
| richards                   | 31.4 ms                                                     | 27.7 ms: 1.14x faster                                                       |
| logging_simple             | 6.86 us                                                     | 6.06 us: 1.13x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 185 us: 1.13x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 12.5 ms: 1.12x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 275 ms: 1.12x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 468 ms: 1.12x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.59 us: 1.11x faster                                                       |
| mypy2                      | 459 ms                                                      | 415 ms: 1.11x faster                                                        |
| scimark_monte_carlo        | 45.3 ms                                                     | 41.0 ms: 1.11x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.5 ms: 1.10x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 84.0 ms: 1.10x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 44.3 ms: 1.10x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 753 ms: 1.10x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.51 us: 1.10x faster                                                       |
| async_tree_io              | 808 ms                                                      | 738 ms: 1.09x faster                                                        |
| sympy_expand               | 299 ms                                                      | 275 ms: 1.09x faster                                                        |
| deepcopy                   | 246 us                                                      | 227 us: 1.08x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 177 ms: 1.08x faster                                                        |
| pyflate                    | 312 ms                                                      | 291 ms: 1.07x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 64.4 ms: 1.06x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.03 sec: 1.06x faster                                                      |
| pprint_safe_repr           | 529 ms                                                      | 501 ms: 1.06x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.98 ms: 1.06x faster                                                       |
| bench_thread_pool          | 872 us                                                      | 828 us: 1.05x faster                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.45 ms: 1.05x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.57 sec: 1.05x faster                                                      |
| meteor_contest             | 75.2 ms                                                     | 71.9 ms: 1.05x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 94.1 ms: 1.04x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 1.99 us: 1.04x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 33.4 ms: 1.03x faster                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.41 sec: 1.03x faster                                                      |
| xml_etree_iterparse        | 65.6 ms                                                     | 64.1 ms: 1.02x faster                                                       |
| fannkuch                   | 253 ms                                                      | 249 ms: 1.02x faster                                                        |
| pidigits                   | 150 ms                                                      | 148 ms: 1.02x faster                                                        |
| pickle_dict                | 18.5 us                                                     | 18.2 us: 1.01x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 36.7 ms: 1.01x faster                                                       |
| scimark_sor                | 78.1 ms                                                     | 77.2 ms: 1.01x faster                                                       |
| 2to3                       | 214 ms                                                      | 212 ms: 1.01x faster                                                        |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 64.0 ms: 1.01x slower                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 53.9 ms: 1.03x slower                                                       |
| regex_dna                  | 116 ms                                                      | 120 ms: 1.04x slower                                                        |
| nbody                      | 70.3 ms                                                     | 72.9 ms: 1.04x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.71 us: 1.05x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 17.6 ms: 1.05x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                       |
| pycparser                  | 720 ms                                                      | 770 ms: 1.07x slower                                                        |
| json_loads                 | 13.0 us                                                     | 14.0 us: 1.07x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 76.1 ms: 1.07x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.14 us: 1.08x slower                                                       |
| coverage                   | 43.4 ms                                                     | 47.2 ms: 1.09x slower                                                       |
| json                       | 2.98 ms                                                     | 3.28 ms: 1.10x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.6 ms: 1.10x slower                                                       |
| pickle_list                | 2.70 us                                                     | 3.00 us: 1.11x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.58 us: 1.13x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.86 ms: 1.19x slower                                                       |
| async_generators           | 177 ms                                                      | 226 ms: 1.28x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (4): float, create_gc_cycles, scimark_fft, python_startup
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.05x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: unknown