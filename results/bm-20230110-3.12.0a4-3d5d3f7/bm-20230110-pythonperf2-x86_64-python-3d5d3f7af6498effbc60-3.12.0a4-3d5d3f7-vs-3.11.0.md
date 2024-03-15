
# Results vs. 3.11.0

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: linux-x86_64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.03x faster \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 286 ms: 1.00x faster                                                        |
| chameleon      | 7.92 ms                                                      | 7.31 ms: 1.08x faster                                                       |
| docutils       | 2.85 sec                                                     | 2.78 sec: 1.03x faster                                                      |
| html5lib       | 72.2 ms                                                      | 66.8 ms: 1.08x faster                                                       |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 608 ms: 1.03x faster                                                        |
| async_tree_none         | 518 ms                                                       | 505 ms: 1.03x faster                                                        |
| async_tree_cpu_io_mixed | 753 ms                                                       | 742 ms: 1.02x faster                                                        |
| async_tree_io           | 1.17 sec                                                     | 1.15 sec: 1.01x faster                                                      |
| Geometric mean          | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 72.4 ms: 1.04x faster                                                       |
| pidigits       | 251 ms                                                       | 252 ms: 1.00x slower                                                        |
| nbody          | 92.9 ms                                                      | 98.1 ms: 1.06x slower                                                       |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 23.0 ms: 1.06x faster                                                       |
| regex_compile  | 156 ms                                                       | 149 ms: 1.05x faster                                                        |
| regex_dna      | 227 ms                                                       | 229 ms: 1.01x slower                                                        |
| regex_effbot   | 3.34 ms                                                      | 3.43 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.1 ms: 1.31x faster                                                       |
| json_loads           | 28.9 us                                                      | 24.0 us: 1.20x faster                                                       |
| unpickle_pure_python | 238 us                                                       | 214 us: 1.11x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 144 ms: 1.08x faster                                                        |
| pickle_list          | 3.94 us                                                      | 3.70 us: 1.07x faster                                                       |
| pickle_dict          | 32.3 us                                                      | 31.1 us: 1.04x faster                                                       |
| unpickle_list        | 4.60 us                                                      | 4.48 us: 1.03x faster                                                       |
| xml_etree_iterparse  | 107 ms                                                       | 104 ms: 1.02x faster                                                        |
| pickle               | 9.89 us                                                      | 9.71 us: 1.02x faster                                                       |
| pickle_pure_python   | 316 us                                                       | 313 us: 1.01x faster                                                        |
| xml_etree_process    | 55.9 ms                                                      | 55.4 ms: 1.01x faster                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 80.3 ms: 1.01x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.06x faster                                                                |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.8 ms: 1.00x slower                                                       |
| python_startup_no_site | 7.73 ms                                                      | 7.87 ms: 1.02x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako           | 11.0 ms                                                      | 10.2 ms: 1.08x faster                                                       |
| genshi_xml     | 57.1 ms                                                      | 53.7 ms: 1.06x faster                                                       |
| genshi_text    | 25.5 ms                                                      | 24.8 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                        | 1.04x faster                                                                |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| asyncio_tcp             | 747 ms                                                       | 386 ms: 1.94x faster                                                        |
| json_dumps              | 13.3 ms                                                      | 10.1 ms: 1.31x faster                                                       |
| json_loads              | 28.9 us                                                      | 24.0 us: 1.20x faster                                                       |
| gc_traversal            | 4.15 ms                                                      | 3.54 ms: 1.17x faster                                                       |
| scimark_lu              | 114 ms                                                       | 101 ms: 1.13x faster                                                        |
| unpickle_pure_python    | 238 us                                                       | 214 us: 1.11x faster                                                        |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 3.70 ms: 1.10x faster                                                       |
| fannkuch                | 416 ms                                                       | 380 ms: 1.09x faster                                                        |
| nqueens                 | 103 ms                                                       | 94.0 ms: 1.09x faster                                                       |
| chameleon               | 7.92 ms                                                      | 7.31 ms: 1.08x faster                                                       |
| html5lib                | 72.2 ms                                                      | 66.8 ms: 1.08x faster                                                       |
| xml_etree_parse         | 155 ms                                                       | 144 ms: 1.08x faster                                                        |
| deltablue               | 3.97 ms                                                      | 3.69 ms: 1.08x faster                                                       |
| mako                    | 11.0 ms                                                      | 10.2 ms: 1.08x faster                                                       |
| json                    | 5.58 ms                                                      | 5.24 ms: 1.07x faster                                                       |
| pickle_list             | 3.94 us                                                      | 3.70 us: 1.07x faster                                                       |
| genshi_xml              | 57.1 ms                                                      | 53.7 ms: 1.06x faster                                                       |
| regex_v8                | 24.4 ms                                                      | 23.0 ms: 1.06x faster                                                       |
| richards                | 49.7 ms                                                      | 46.9 ms: 1.06x faster                                                       |
| chaos                   | 74.9 ms                                                      | 70.9 ms: 1.06x faster                                                       |
| scimark_monte_carlo     | 69.8 ms                                                      | 66.6 ms: 1.05x faster                                                       |
| regex_compile           | 156 ms                                                       | 149 ms: 1.05x faster                                                        |
| logging_simple          | 7.24 us                                                      | 6.95 us: 1.04x faster                                                       |
| pickle_dict             | 32.3 us                                                      | 31.1 us: 1.04x faster                                                       |
| unpack_sequence         | 45.7 ns                                                      | 44.0 ns: 1.04x faster                                                       |
| pycparser               | 1.31 sec                                                     | 1.26 sec: 1.04x faster                                                      |
| pyflate                 | 449 ms                                                       | 433 ms: 1.04x faster                                                        |
| float                   | 74.9 ms                                                      | 72.4 ms: 1.04x faster                                                       |
| raytrace                | 309 ms                                                       | 299 ms: 1.04x faster                                                        |
| async_tree_memoization  | 629 ms                                                       | 608 ms: 1.03x faster                                                        |
| deepcopy                | 391 us                                                       | 379 us: 1.03x faster                                                        |
| hexiom                  | 6.98 ms                                                      | 6.77 ms: 1.03x faster                                                       |
| sympy_expand            | 553 ms                                                       | 537 ms: 1.03x faster                                                        |
| go                      | 158 ms                                                       | 153 ms: 1.03x faster                                                        |
| crypto_pyaes            | 83.3 ms                                                      | 81.1 ms: 1.03x faster                                                       |
| genshi_text             | 25.5 ms                                                      | 24.8 ms: 1.03x faster                                                       |
| thrift                  | 931 us                                                       | 908 us: 1.03x faster                                                        |
| unpickle_list           | 4.60 us                                                      | 4.48 us: 1.03x faster                                                       |
| docutils                | 2.85 sec                                                     | 2.78 sec: 1.03x faster                                                      |
| async_tree_none         | 518 ms                                                       | 505 ms: 1.03x faster                                                        |
| pprint_pformat          | 1.67 sec                                                     | 1.63 sec: 1.02x faster                                                      |
| deepcopy_memo           | 37.5 us                                                      | 36.7 us: 1.02x faster                                                       |
| xml_etree_iterparse     | 107 ms                                                       | 104 ms: 1.02x faster                                                        |
| pickle                  | 9.89 us                                                      | 9.71 us: 1.02x faster                                                       |
| deepcopy_reduce         | 3.40 us                                                      | 3.33 us: 1.02x faster                                                       |
| telco                   | 6.81 ms                                                      | 6.70 ms: 1.02x faster                                                       |
| async_tree_cpu_io_mixed | 753 ms                                                       | 742 ms: 1.02x faster                                                        |
| async_tree_io           | 1.17 sec                                                     | 1.15 sec: 1.01x faster                                                      |
| scimark_sor             | 110 ms                                                       | 108 ms: 1.01x faster                                                        |
| pprint_safe_repr        | 805 ms                                                       | 794 ms: 1.01x faster                                                        |
| sympy_integrate         | 25.8 ms                                                      | 25.6 ms: 1.01x faster                                                       |
| pickle_pure_python      | 316 us                                                       | 313 us: 1.01x faster                                                        |
| xml_etree_process       | 55.9 ms                                                      | 55.4 ms: 1.01x faster                                                       |
| mdp                     | 2.77 sec                                                     | 2.75 sec: 1.01x faster                                                      |
| sympy_str               | 337 ms                                                       | 335 ms: 1.01x faster                                                        |
| 2to3                    | 287 ms                                                       | 286 ms: 1.00x faster                                                        |
| sympy_sum               | 186 ms                                                       | 186 ms: 1.00x slower                                                        |
| pidigits                | 251 ms                                                       | 252 ms: 1.00x slower                                                        |
| python_startup          | 10.7 ms                                                      | 10.8 ms: 1.00x slower                                                       |
| coroutines              | 27.8 ms                                                      | 27.9 ms: 1.00x slower                                                       |
| meteor_contest          | 131 ms                                                       | 131 ms: 1.00x slower                                                        |
| sqlglot_optimize        | 59.0 ms                                                      | 59.3 ms: 1.01x slower                                                       |
| regex_dna               | 227 ms                                                       | 229 ms: 1.01x slower                                                        |
| scimark_fft             | 281 ms                                                       | 283 ms: 1.01x slower                                                        |
| xml_etree_generate      | 79.7 ms                                                      | 80.3 ms: 1.01x slower                                                       |
| sqlglot_normalize       | 122 ms                                                       | 123 ms: 1.01x slower                                                        |
| logging_silent          | 100 ns                                                       | 102 ns: 1.01x slower                                                        |
| sqlite_synth            | 2.52 us                                                      | 2.56 us: 1.02x slower                                                       |
| python_startup_no_site  | 7.73 ms                                                      | 7.87 ms: 1.02x slower                                                       |
| sqlglot_transpile       | 1.91 ms                                                      | 1.95 ms: 1.02x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 19.4 ms: 1.02x slower                                                       |
| regex_effbot            | 3.34 ms                                                      | 3.43 ms: 1.03x slower                                                       |
| sqlglot_parse           | 1.51 ms                                                      | 1.59 ms: 1.05x slower                                                       |
| bench_mp_pool           | 4.70 ms                                                      | 4.94 ms: 1.05x slower                                                       |
| nbody                   | 92.9 ms                                                      | 98.1 ms: 1.06x slower                                                       |
| spectral_norm           | 95.1 ms                                                      | 101 ms: 1.06x slower                                                        |
| comprehensions          | 25.1 us                                                      | 27.1 us: 1.08x slower                                                       |
| generators              | 54.6 ms                                                      | 60.5 ms: 1.11x slower                                                       |
| coverage                | 66.1 ms                                                      | 89.3 ms: 1.35x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.03x faster                                                                |

Benchmark hidden because not significant (8): bench_thread_pool, logging_format, dask, django_template, dulwich_log, async_generators, unpickle, create_gc_cycles
Ignored benchmarks (17) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x