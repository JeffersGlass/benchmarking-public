
# Results vs. 3.11.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: windows-amd64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.11x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| chameleon      | 5.26 ms                                                     | 4.90 ms: 1.07x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.53 sec: 1.07x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 86.2 ms: 1.08x faster                                                       |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 264 ms: 1.26x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 446 ms: 1.19x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 339 ms: 1.18x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 347 ms: 1.17x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.13x faster                                                        |
| async_tree_io              | 808 ms                                                      | 716 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 465 ms: 1.13x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 751 ms: 1.10x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.16x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 51.3 ms: 1.06x faster                                                       |
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| nbody          | 70.3 ms                                                     | 72.8 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 78.0 ms: 1.17x faster                                                       |
| regex_dna      | 116 ms                                                      | 117 ms: 1.01x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 128 us: 1.23x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 180 us: 1.16x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 92.9 ms: 1.05x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.5 ms: 1.03x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.42 sec: 1.02x faster                                                      |
| xml_etree_process    | 37.2 ms                                                     | 36.8 ms: 1.01x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.3 us: 1.01x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 54.3 ms: 1.03x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.69 us: 1.04x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.82 us: 1.05x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.05x slower                                                       |
| pickle               | 6.64 us                                                     | 7.18 us: 1.08x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.73 us: 1.15x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.3 ms: 1.09x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.48 ms: 1.17x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 71.9 us: 4.53x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.9 ms: 1.55x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 472 ms: 1.54x faster                                                        |
| comprehensions             | 15.6 us                                                     | 10.6 us: 1.47x faster                                                       |
| json_dumps                 | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.03 ms: 1.33x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 55.0 ns: 1.30x faster                                                       |
| raytrace                   | 213 ms                                                      | 169 ms: 1.26x faster                                                        |
| async_tree_none            | 332 ms                                                      | 264 ms: 1.26x faster                                                        |
| richards_super             | 38.7 ms                                                     | 31.2 ms: 1.24x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 128 us: 1.23x faster                                                        |
| sympy_sum                  | 100 ms                                                      | 82.4 ms: 1.21x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 785 us: 1.21x faster                                                        |
| chaos                      | 48.4 ms                                                     | 40.1 ms: 1.21x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.34 sec: 1.19x faster                                                      |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 446 ms: 1.19x faster                                                        |
| unpack_sequence            | 46.9 ns                                                     | 39.8 ns: 1.18x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 339 ms: 1.18x faster                                                        |
| hexiom                     | 4.55 ms                                                     | 3.87 ms: 1.18x faster                                                       |
| go                         | 101 ms                                                      | 86.0 ms: 1.18x faster                                                       |
| mako                       | 7.58 ms                                                     | 6.48 ms: 1.17x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 78.0 ms: 1.17x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 347 ms: 1.17x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 999 us: 1.17x faster                                                        |
| sympy_str                  | 185 ms                                                      | 159 ms: 1.16x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 180 us: 1.16x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 58.9 ms: 1.16x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 22.4 us: 1.16x faster                                                       |
| richards                   | 31.4 ms                                                     | 27.5 ms: 1.14x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 12.3 ms: 1.14x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.1 ms: 1.14x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 43.1 ms: 1.13x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.13x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 60.4 ms: 1.13x faster                                                       |
| logging_simple             | 6.86 us                                                     | 6.08 us: 1.13x faster                                                       |
| async_tree_io              | 808 ms                                                      | 716 ms: 1.13x faster                                                        |
| scimark_lu                 | 62.8 ms                                                     | 55.7 ms: 1.13x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 465 ms: 1.13x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.57 us: 1.12x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 41.4 ms: 1.12x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.82 sec: 1.11x faster                                                      |
| mypy2                      | 459 ms                                                      | 413 ms: 1.11x faster                                                        |
| scimark_monte_carlo        | 45.3 ms                                                     | 40.9 ms: 1.11x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 751 ms: 1.10x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.50 us: 1.10x faster                                                       |
| deepcopy                   | 246 us                                                      | 224 us: 1.10x faster                                                        |
| sympy_expand               | 299 ms                                                      | 273 ms: 1.10x faster                                                        |
| pyflate                    | 312 ms                                                      | 287 ms: 1.09x faster                                                        |
| pprint_pformat             | 1.09 sec                                                    | 1.01 sec: 1.08x faster                                                      |
| dask                       | 273 ms                                                      | 253 ms: 1.08x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 86.2 ms: 1.08x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 493 ms: 1.07x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.90 ms: 1.07x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 178 ms: 1.07x faster                                                        |
| docutils                   | 1.64 sec                                                    | 1.53 sec: 1.07x faster                                                      |
| deepcopy_reduce            | 2.06 us                                                     | 1.94 us: 1.06x faster                                                       |
| float                      | 54.4 ms                                                     | 51.3 ms: 1.06x faster                                                       |
| meteor_contest             | 75.2 ms                                                     | 71.5 ms: 1.05x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 92.9 ms: 1.05x faster                                                       |
| bench_thread_pool          | 872 us                                                      | 838 us: 1.04x faster                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.48 ms: 1.04x faster                                                       |
| fannkuch                   | 253 ms                                                      | 244 ms: 1.04x faster                                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.5 ms: 1.03x faster                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.42 sec: 1.02x faster                                                      |
| pidigits                   | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 33.9 ms: 1.02x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 36.8 ms: 1.01x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 18.3 us: 1.01x faster                                                       |
| regex_dna                  | 116 ms                                                      | 117 ms: 1.01x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 80.2 ms: 1.03x slower                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 54.3 ms: 1.03x slower                                                       |
| nbody                      | 70.3 ms                                                     | 72.8 ms: 1.03x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.69 us: 1.04x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.82 us: 1.05x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.6 us: 1.05x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 66.7 ms: 1.05x slower                                                       |
| coverage                   | 43.4 ms                                                     | 46.2 ms: 1.06x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.18 us: 1.08x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.3 ms: 1.09x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 79.2 ms: 1.12x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.73 us: 1.15x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.80 ms: 1.18x slower                                                       |
| async_generators           | 177 ms                                                      | 235 ms: 1.33x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.11x faster                                                                |

Benchmark hidden because not significant (6): json, pycparser, 2to3, gc_traversal, scimark_fft, create_gc_cycles
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.06x


# Memory

- memory change: unknown