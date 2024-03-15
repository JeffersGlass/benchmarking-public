
# Results vs. 3.11.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: windows-amd64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.06x faster
- HPT reliability: 99.96%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 218 ms: 1.02x slower                                                        |
| chameleon      | 5.26 ms                                                     | 5.01 ms: 1.05x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 87.4 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.17x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 459 ms: 1.15x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 276 ms: 1.12x faster                                                        |
| async_tree_io              | 808 ms                                                      | 726 ms: 1.11x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 473 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 749 ms: 1.11x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.01x faster                                                        |
| float          | 54.4 ms                                                     | 55.8 ms: 1.03x slower                                                       |
| nbody          | 70.3 ms                                                     | 80.2 ms: 1.14x slower                                                       |
| Geometric mean | (ref)                                                       | 1.05x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 84.7 ms: 1.08x faster                                                       |
| regex_dna      | 116 ms                                                      | 122 ms: 1.05x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.58 ms: 1.45x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 135 us: 1.16x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 181 us: 1.15x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 94.2 ms: 1.04x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 18.4 us: 1.00x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 37.8 ms: 1.02x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.5 us: 1.04x slower                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 68.9 ms: 1.05x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 55.6 ms: 1.06x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.80 us: 1.08x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.30 us: 1.10x slower                                                       |
| pickle               | 6.64 us                                                     | 7.29 us: 1.10x slower                                                       |
| pickle_list          | 2.70 us                                                     | 3.18 us: 1.18x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.5 ms: 1.10x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 73.7 us: 4.42x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.6 ms: 1.57x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 469 ms: 1.55x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.58 ms: 1.45x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 55.7 ns: 1.29x faster                                                       |
| richards_super             | 38.7 ms                                                     | 30.6 ms: 1.26x faster                                                       |
| async_tree_none            | 332 ms                                                      | 268 ms: 1.24x faster                                                        |
| unpack_sequence            | 46.9 ns                                                     | 38.1 ns: 1.23x faster                                                       |
| raytrace                   | 213 ms                                                      | 174 ms: 1.23x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 783 us: 1.22x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.68 sec: 1.20x faster                                                      |
| comprehensions             | 15.6 us                                                     | 13.0 us: 1.20x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.17x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 135 us: 1.16x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.37 sec: 1.16x faster                                                      |
| deepcopy_memo              | 26.0 us                                                     | 22.4 us: 1.16x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.01 ms: 1.16x faster                                                       |
| richards                   | 31.4 ms                                                     | 27.2 ms: 1.16x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 459 ms: 1.15x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 181 us: 1.15x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 13.1 ms: 1.14x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 87.6 ms: 1.14x faster                                                       |
| sympy_str                  | 185 ms                                                      | 165 ms: 1.12x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 276 ms: 1.12x faster                                                        |
| deepcopy                   | 246 us                                                      | 221 us: 1.12x faster                                                        |
| logging_simple             | 6.86 us                                                     | 6.15 us: 1.12x faster                                                       |
| async_tree_io              | 808 ms                                                      | 726 ms: 1.11x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 473 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 749 ms: 1.11x faster                                                        |
| chaos                      | 48.4 ms                                                     | 43.9 ms: 1.10x faster                                                       |
| go                         | 101 ms                                                      | 92.0 ms: 1.10x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 42.3 ms: 1.10x faster                                                       |
| sympy_expand               | 299 ms                                                      | 274 ms: 1.09x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.57 us: 1.09x faster                                                       |
| mypy2                      | 459 ms                                                      | 422 ms: 1.09x faster                                                        |
| scimark_lu                 | 62.8 ms                                                     | 58.0 ms: 1.08x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 84.7 ms: 1.08x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 13.1 ms: 1.07x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 64.0 ms: 1.07x faster                                                       |
| dask                       | 273 ms                                                      | 256 ms: 1.07x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 87.4 ms: 1.06x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 5.01 ms: 1.05x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 181 ms: 1.05x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 1.97 us: 1.05x faster                                                       |
| pycparser                  | 720 ms                                                      | 690 ms: 1.04x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 47.1 ms: 1.04x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 94.2 ms: 1.04x faster                                                       |
| bench_thread_pool          | 872 us                                                      | 841 us: 1.04x faster                                                        |
| docutils                   | 1.64 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| scimark_sor                | 78.1 ms                                                     | 76.7 ms: 1.02x faster                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                                      |
| pidigits                   | 150 ms                                                      | 148 ms: 1.01x faster                                                        |
| pickle_dict                | 18.5 us                                                     | 18.4 us: 1.00x faster                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.50 ms: 1.01x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                                       |
| xml_etree_process          | 37.2 ms                                                     | 37.8 ms: 1.02x slower                                                       |
| 2to3                       | 214 ms                                                      | 218 ms: 1.02x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 728 us: 1.02x slower                                                        |
| float                      | 54.4 ms                                                     | 55.8 ms: 1.03x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 47.1 ms: 1.04x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.5 us: 1.04x slower                                                       |
| pyflate                    | 312 ms                                                      | 325 ms: 1.04x slower                                                        |
| coverage                   | 43.4 ms                                                     | 45.3 ms: 1.04x slower                                                       |
| regex_dna                  | 116 ms                                                      | 122 ms: 1.05x slower                                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 68.9 ms: 1.05x slower                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 55.6 ms: 1.06x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 67.3 ms: 1.06x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                       |
| fannkuch                   | 253 ms                                                      | 271 ms: 1.07x slower                                                        |
| hexiom                     | 4.55 ms                                                     | 4.87 ms: 1.07x slower                                                       |
| json                       | 2.98 ms                                                     | 3.19 ms: 1.07x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.80 us: 1.08x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.30 us: 1.10x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.29 us: 1.10x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.5 ms: 1.10x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 79.5 ms: 1.12x slower                                                       |
| nbody                      | 70.3 ms                                                     | 80.2 ms: 1.14x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.74 ms: 1.17x slower                                                       |
| scimark_fft                | 179 ms                                                      | 211 ms: 1.17x slower                                                        |
| pickle_list                | 2.70 us                                                     | 3.18 us: 1.18x slower                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.06 ms: 1.19x slower                                                       |
| spectral_norm              | 68.3 ms                                                     | 84.3 ms: 1.23x slower                                                       |
| async_generators           | 177 ms                                                      | 230 ms: 1.30x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                |

Benchmark hidden because not significant (5): pprint_safe_repr, meteor_contest, deltablue, pprint_pformat, mako
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.96% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown