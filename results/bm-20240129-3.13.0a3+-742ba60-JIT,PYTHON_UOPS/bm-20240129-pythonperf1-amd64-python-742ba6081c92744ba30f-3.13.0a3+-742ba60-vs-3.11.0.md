
# Results vs. 3.11.0

- fork: python
- ref: 742ba6081c92744ba30f
- machine: windows-amd64
- commit hash: 742ba60
- commit date: 2024-01-29
- overall geometric mean: 1.08x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 221 ms: 1.04x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.79 ms: 1.10x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 87.6 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 273 ms: 1.22x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 340 ms: 1.17x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 460 ms: 1.15x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 364 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 741 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 481 ms: 1.09x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 284 ms: 1.09x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 774 ms: 1.07x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 60.9 ms: 1.15x faster                                                       |
| float          | 54.4 ms                                                     | 51.0 ms: 1.07x faster                                                       |
| pidigits       | 150 ms                                                      | 152 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 81.0 ms: 1.12x faster                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                       |
| regex_dna      | 116 ms                                                      | 124 ms: 1.07x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 21.9 ms: 1.55x slower                                                       |
| Geometric mean | (ref)                                                       | 1.12x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.55 ms: 1.46x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 125 us: 1.26x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 173 us: 1.20x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.29 sec: 1.13x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 17.7 us: 1.05x faster                                                       |
| xml_etree_parse      | 97.6 ms                                                     | 94.6 ms: 1.03x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 37.0 ms: 1.01x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 53.5 ms: 1.02x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.77 us: 1.03x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.06x slower                                                       |
| pickle               | 6.64 us                                                     | 7.28 us: 1.10x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.87 us: 1.11x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.54 us: 1.13x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 21.3 ms: 1.08x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 19.1 ms: 1.14x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.11x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.82 ms: 1.11x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 69.9 us: 4.66x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.1 ms: 1.61x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 492 ms: 1.47x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.55 ms: 1.46x faster                                                       |
| richards_super             | 38.7 ms                                                     | 28.1 ms: 1.38x faster                                                       |
| comprehensions             | 15.6 us                                                     | 11.4 us: 1.37x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 53.5 ns: 1.34x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.09 ms: 1.29x faster                                                       |
| raytrace                   | 213 ms                                                      | 168 ms: 1.27x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 750 us: 1.27x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 125 us: 1.26x faster                                                        |
| richards                   | 31.4 ms                                                     | 25.1 ms: 1.25x faster                                                       |
| async_tree_none            | 332 ms                                                      | 273 ms: 1.22x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 21.4 us: 1.21x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 173 us: 1.20x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 976 us: 1.19x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 340 ms: 1.17x faster                                                        |
| logging_simple             | 6.86 us                                                     | 5.89 us: 1.16x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 54.1 ms: 1.16x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 12.9 ms: 1.16x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 59.0 ms: 1.16x faster                                                       |
| nbody                      | 70.3 ms                                                     | 60.9 ms: 1.15x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 40.7 ns: 1.15x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 460 ms: 1.15x faster                                                        |
| chaos                      | 48.4 ms                                                     | 42.4 ms: 1.14x faster                                                       |
| deepcopy                   | 246 us                                                      | 217 us: 1.13x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.56 us: 1.13x faster                                                       |
| sympy_str                  | 185 ms                                                      | 164 ms: 1.13x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.29 sec: 1.13x faster                                                      |
| sympy_sum                  | 100 ms                                                      | 88.8 ms: 1.13x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 81.0 ms: 1.12x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.40 us: 1.12x faster                                                       |
| mako                       | 7.58 ms                                                     | 6.82 ms: 1.11x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 364 ms: 1.11x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.79 ms: 1.10x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 173 ms: 1.10x faster                                                        |
| async_tree_io              | 808 ms                                                      | 741 ms: 1.09x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 1.89 us: 1.09x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 481 ms: 1.09x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 284 ms: 1.09x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.87 sec: 1.09x faster                                                      |
| dulwich_log                | 46.4 ms                                                     | 43.3 ms: 1.07x faster                                                       |
| sympy_expand               | 299 ms                                                      | 279 ms: 1.07x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 774 ms: 1.07x faster                                                        |
| float                      | 54.4 ms                                                     | 51.0 ms: 1.07x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 13.2 ms: 1.06x faster                                                       |
| bench_thread_pool          | 872 us                                                      | 821 us: 1.06x faster                                                        |
| mypy2                      | 459 ms                                                      | 432 ms: 1.06x faster                                                        |
| pprint_pformat             | 1.09 sec                                                    | 1.02 sec: 1.06x faster                                                      |
| tornado_http               | 92.8 ms                                                     | 87.6 ms: 1.06x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 500 ms: 1.06x faster                                                        |
| go                         | 101 ms                                                      | 96.0 ms: 1.05x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 17.7 us: 1.05x faster                                                       |
| scimark_sor                | 78.1 ms                                                     | 74.7 ms: 1.05x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 46.9 ms: 1.04x faster                                                       |
| spectral_norm              | 68.3 ms                                                     | 65.8 ms: 1.04x faster                                                       |
| pycparser                  | 720 ms                                                      | 695 ms: 1.04x faster                                                        |
| dask                       | 273 ms                                                      | 263 ms: 1.04x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 94.6 ms: 1.03x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                      |
| fannkuch                   | 253 ms                                                      | 246 ms: 1.03x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.55 sec: 1.03x faster                                                      |
| sqlglot_optimize           | 34.5 ms                                                     | 34.1 ms: 1.01x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 37.0 ms: 1.01x faster                                                       |
| pidigits                   | 150 ms                                                      | 152 ms: 1.02x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 53.5 ms: 1.02x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.77 us: 1.03x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.54 ms: 1.03x slower                                                       |
| 2to3                       | 214 ms                                                      | 221 ms: 1.04x slower                                                        |
| meteor_contest             | 75.2 ms                                                     | 78.0 ms: 1.04x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 742 us: 1.04x slower                                                        |
| coverage                   | 43.4 ms                                                     | 45.5 ms: 1.05x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.06x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                       |
| regex_dna                  | 116 ms                                                      | 124 ms: 1.07x slower                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.76 ms: 1.07x slower                                                       |
| scimark_fft                | 179 ms                                                      | 193 ms: 1.08x slower                                                        |
| python_startup             | 19.8 ms                                                     | 21.3 ms: 1.08x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 69.1 ms: 1.09x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.28 us: 1.10x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.87 us: 1.11x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.54 us: 1.13x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.18 ms: 1.14x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 19.1 ms: 1.14x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.67 ms: 1.15x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 81.7 ms: 1.15x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 57.0 ms: 1.26x slower                                                       |
| async_generators           | 177 ms                                                      | 244 ms: 1.38x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 21.9 ms: 1.55x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.08x faster                                                                |

Benchmark hidden because not significant (3): pyflate, xml_etree_iterparse, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown