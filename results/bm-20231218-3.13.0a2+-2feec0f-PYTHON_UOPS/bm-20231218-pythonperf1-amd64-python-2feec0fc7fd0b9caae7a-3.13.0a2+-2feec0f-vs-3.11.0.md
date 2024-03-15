
# Results vs. 3.11.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: windows-amd64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.06x faster
- HPT reliability: 99.88%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 218 ms: 1.02x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.93 ms: 1.07x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 88.0 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 341 ms: 1.17x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 456 ms: 1.16x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 349 ms: 1.16x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 274 ms: 1.12x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 743 ms: 1.12x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 471 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 733 ms: 1.10x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 151 ms: 1.00x slower                                                        |
| float          | 54.4 ms                                                     | 57.1 ms: 1.05x slower                                                       |
| nbody          | 70.3 ms                                                     | 82.3 ms: 1.17x slower                                                       |
| Geometric mean | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 84.4 ms: 1.08x faster                                                       |
| regex_dna      | 116 ms                                                      | 121 ms: 1.04x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 15.1 ms: 1.07x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.62 ms: 1.44x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 135 us: 1.16x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 181 us: 1.15x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 94.2 ms: 1.04x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.47 sec: 1.01x slower                                                      |
| pickle_dict          | 18.5 us                                                     | 18.7 us: 1.01x slower                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 67.0 ms: 1.02x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.3 us: 1.02x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 54.8 ms: 1.04x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.72 us: 1.05x slower                                                       |
| pickle               | 6.64 us                                                     | 7.19 us: 1.08x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.37 us: 1.10x slower                                                       |
| pickle_list          | 2.70 us                                                     | 3.39 us: 1.26x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.3 ms: 1.02x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.1 ms: 1.08x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.96 ms: 1.09x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 74.3 us: 4.38x faster                                                       |
| generators                 | 34.0 ms                                                     | 22.2 ms: 1.53x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 478 ms: 1.52x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.62 ms: 1.44x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 54.8 ns: 1.31x faster                                                       |
| richards_super             | 38.7 ms                                                     | 30.7 ms: 1.26x faster                                                       |
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| raytrace                   | 213 ms                                                      | 173 ms: 1.24x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 775 us: 1.23x faster                                                        |
| comprehensions             | 15.6 us                                                     | 12.8 us: 1.22x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 39.2 ns: 1.20x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 12.8 ms: 1.17x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 341 ms: 1.17x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 997 us: 1.17x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.74 sec: 1.17x faster                                                      |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 456 ms: 1.16x faster                                                        |
| sympy_sum                  | 100 ms                                                      | 86.1 ms: 1.16x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 349 ms: 1.16x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 135 us: 1.16x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 181 us: 1.15x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 22.6 us: 1.15x faster                                                       |
| richards                   | 31.4 ms                                                     | 27.6 ms: 1.14x faster                                                       |
| sqlite_synth               | 1.77 us                                                     | 1.56 us: 1.13x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 274 ms: 1.12x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 743 ms: 1.12x faster                                                        |
| logging_simple             | 6.86 us                                                     | 6.16 us: 1.11x faster                                                       |
| sympy_str                  | 185 ms                                                      | 167 ms: 1.11x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 471 ms: 1.11x faster                                                        |
| scimark_lu                 | 62.8 ms                                                     | 56.5 ms: 1.11x faster                                                       |
| go                         | 101 ms                                                      | 91.2 ms: 1.11x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.44 sec: 1.10x faster                                                      |
| async_tree_io              | 808 ms                                                      | 733 ms: 1.10x faster                                                        |
| mypy2                      | 459 ms                                                      | 420 ms: 1.09x faster                                                        |
| deepcopy                   | 246 us                                                      | 226 us: 1.09x faster                                                        |
| mako                       | 7.58 ms                                                     | 6.96 ms: 1.09x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.58 us: 1.09x faster                                                       |
| chaos                      | 48.4 ms                                                     | 44.6 ms: 1.09x faster                                                       |
| sympy_expand               | 299 ms                                                      | 276 ms: 1.08x faster                                                        |
| regex_compile              | 91.0 ms                                                     | 84.4 ms: 1.08x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 43.3 ms: 1.07x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 63.9 ms: 1.07x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 13.1 ms: 1.07x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 4.93 ms: 1.07x faster                                                       |
| dask                       | 273 ms                                                      | 256 ms: 1.07x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 88.0 ms: 1.05x faster                                                       |
| pycparser                  | 720 ms                                                      | 684 ms: 1.05x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 1.97 us: 1.04x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 183 ms: 1.04x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 94.2 ms: 1.04x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| crypto_pyaes               | 48.9 ms                                                     | 47.8 ms: 1.02x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.07 sec: 1.02x faster                                                      |
| pprint_safe_repr           | 529 ms                                                      | 520 ms: 1.02x faster                                                        |
| scimark_sor                | 78.1 ms                                                     | 77.1 ms: 1.01x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.67 ms: 1.01x faster                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.48 ms: 1.01x faster                                                       |
| meteor_contest             | 75.2 ms                                                     | 75.6 ms: 1.00x slower                                                       |
| pidigits                   | 150 ms                                                      | 151 ms: 1.00x slower                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.47 sec: 1.01x slower                                                      |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                                       |
| pickle_dict                | 18.5 us                                                     | 18.7 us: 1.01x slower                                                       |
| 2to3                       | 214 ms                                                      | 218 ms: 1.02x slower                                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 67.0 ms: 1.02x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.3 us: 1.02x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.3 ms: 1.02x slower                                                       |
| pyflate                    | 312 ms                                                      | 321 ms: 1.03x slower                                                        |
| coverage                   | 43.4 ms                                                     | 44.9 ms: 1.03x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 739 us: 1.04x slower                                                        |
| regex_dna                  | 116 ms                                                      | 121 ms: 1.04x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 54.8 ms: 1.04x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| float                      | 54.4 ms                                                     | 57.1 ms: 1.05x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.72 us: 1.05x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 67.5 ms: 1.07x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.1 ms: 1.07x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.1 ms: 1.08x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.19 us: 1.08x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 49.5 ms: 1.09x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 4.99 ms: 1.10x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.37 us: 1.10x slower                                                       |
| fannkuch                   | 253 ms                                                      | 291 ms: 1.15x slower                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.98 ms: 1.16x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 81.9 ms: 1.16x slower                                                       |
| scimark_fft                | 179 ms                                                      | 209 ms: 1.17x slower                                                        |
| telco                      | 4.06 ms                                                     | 4.75 ms: 1.17x slower                                                       |
| nbody                      | 70.3 ms                                                     | 82.3 ms: 1.17x slower                                                       |
| spectral_norm              | 68.3 ms                                                     | 82.6 ms: 1.21x slower                                                       |
| pickle_list                | 2.70 us                                                     | 3.39 us: 1.26x slower                                                       |
| async_generators           | 177 ms                                                      | 230 ms: 1.30x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                |

Benchmark hidden because not significant (3): xml_etree_process, bench_thread_pool, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.88% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown