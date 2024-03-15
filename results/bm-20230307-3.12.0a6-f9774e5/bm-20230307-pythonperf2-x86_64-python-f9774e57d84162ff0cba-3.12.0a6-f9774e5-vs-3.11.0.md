
# Results vs. 3.11.0

- fork: python
- ref: f9774e57d84162ff0cba
- machine: linux-x86_64
- commit hash: f9774e5
- commit date: 2023-03-07
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 1.15x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 284 ms: 1.01x faster                                                        |
| chameleon      | 7.92 ms                                                      | 6.94 ms: 1.14x faster                                                       |
| docutils       | 2.85 sec                                                     | 2.79 sec: 1.02x faster                                                      |
| html5lib       | 72.2 ms                                                      | 65.9 ms: 1.10x faster                                                       |
| tornado_http   | 124 ms                                                       | 115 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                        | 1.07x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 611 ms: 1.03x faster                                                        |
| async_tree_none         | 518 ms                                                       | 510 ms: 1.02x faster                                                        |
| async_tree_cpu_io_mixed | 753 ms                                                       | 745 ms: 1.01x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.01x faster                                                                |

Benchmark hidden because not significant (1): async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 73.9 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                |

Benchmark hidden because not significant (2): nbody, pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 22.8 ms: 1.07x faster                                                       |
| regex_compile  | 156 ms                                                       | 146 ms: 1.07x faster                                                        |
| regex_dna      | 227 ms                                                       | 225 ms: 1.01x faster                                                        |
| regex_effbot   | 3.34 ms                                                      | 3.36 ms: 1.01x slower                                                       |
| Geometric mean | (ref)                                                        | 1.04x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.2 ms: 1.29x faster                                                       |
| json_loads           | 28.9 us                                                      | 24.4 us: 1.19x faster                                                       |
| unpickle_pure_python | 238 us                                                       | 202 us: 1.18x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 144 ms: 1.07x faster                                                        |
| pickle_list          | 3.94 us                                                      | 3.80 us: 1.04x faster                                                       |
| unpickle_list        | 4.60 us                                                      | 4.44 us: 1.04x faster                                                       |
| pickle_pure_python   | 316 us                                                       | 306 us: 1.03x faster                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 103 ms: 1.03x faster                                                        |
| pickle_dict          | 32.3 us                                                      | 31.8 us: 1.02x faster                                                       |
| unpickle             | 13.3 us                                                      | 13.4 us: 1.01x slower                                                       |
| pickle               | 9.89 us                                                      | 10.0 us: 1.01x slower                                                       |
| xml_etree_process    | 55.9 ms                                                      | 57.3 ms: 1.03x slower                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 83.5 ms: 1.05x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.06x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.3 ms: 1.05x slower                                                       |
| python_startup_no_site | 7.73 ms                                                      | 8.34 ms: 1.08x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako           | 11.0 ms                                                      | 10.0 ms: 1.10x faster                                                       |
| genshi_xml     | 57.1 ms                                                      | 53.0 ms: 1.08x faster                                                       |
| genshi_text    | 25.5 ms                                                      | 24.6 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| asyncio_tcp             | 747 ms                                                       | 382 ms: 1.96x faster                                                        |
| generators              | 54.6 ms                                                      | 38.4 ms: 1.42x faster                                                       |
| json_dumps              | 13.3 ms                                                      | 10.2 ms: 1.29x faster                                                       |
| deltablue               | 3.97 ms                                                      | 3.33 ms: 1.19x faster                                                       |
| json_loads              | 28.9 us                                                      | 24.4 us: 1.19x faster                                                       |
| unpickle_pure_python    | 238 us                                                       | 202 us: 1.18x faster                                                        |
| chameleon               | 7.92 ms                                                      | 6.94 ms: 1.14x faster                                                       |
| coroutines              | 27.8 ms                                                      | 24.7 ms: 1.12x faster                                                       |
| json                    | 5.58 ms                                                      | 5.00 ms: 1.12x faster                                                       |
| html5lib                | 72.2 ms                                                      | 65.9 ms: 1.10x faster                                                       |
| mako                    | 11.0 ms                                                      | 10.0 ms: 1.10x faster                                                       |
| mdp                     | 2.77 sec                                                     | 2.54 sec: 1.09x faster                                                      |
| scimark_lu              | 114 ms                                                       | 105 ms: 1.09x faster                                                        |
| tornado_http            | 124 ms                                                       | 115 ms: 1.08x faster                                                        |
| hexiom                  | 6.98 ms                                                      | 6.46 ms: 1.08x faster                                                       |
| genshi_xml              | 57.1 ms                                                      | 53.0 ms: 1.08x faster                                                       |
| xml_etree_parse         | 155 ms                                                       | 144 ms: 1.07x faster                                                        |
| regex_v8                | 24.4 ms                                                      | 22.8 ms: 1.07x faster                                                       |
| pprint_pformat          | 1.67 sec                                                     | 1.55 sec: 1.07x faster                                                      |
| richards                | 49.7 ms                                                      | 46.4 ms: 1.07x faster                                                       |
| regex_compile           | 156 ms                                                       | 146 ms: 1.07x faster                                                        |
| raytrace                | 309 ms                                                       | 290 ms: 1.07x faster                                                        |
| logging_simple          | 7.24 us                                                      | 6.79 us: 1.07x faster                                                       |
| deepcopy_memo           | 37.5 us                                                      | 35.4 us: 1.06x faster                                                       |
| logging_silent          | 100 ns                                                       | 94.5 ns: 1.06x faster                                                       |
| pycparser               | 1.31 sec                                                     | 1.23 sec: 1.06x faster                                                      |
| nqueens                 | 103 ms                                                       | 96.9 ms: 1.06x faster                                                       |
| dulwich_log             | 67.4 ms                                                      | 63.7 ms: 1.06x faster                                                       |
| chaos                   | 74.9 ms                                                      | 70.9 ms: 1.06x faster                                                       |
| pprint_safe_repr        | 805 ms                                                       | 762 ms: 1.06x faster                                                        |
| go                      | 158 ms                                                       | 151 ms: 1.05x faster                                                        |
| scimark_sor             | 110 ms                                                       | 105 ms: 1.04x faster                                                        |
| pyflate                 | 449 ms                                                       | 432 ms: 1.04x faster                                                        |
| gc_traversal            | 4.15 ms                                                      | 3.99 ms: 1.04x faster                                                       |
| pickle_list             | 3.94 us                                                      | 3.80 us: 1.04x faster                                                       |
| deepcopy                | 391 us                                                       | 377 us: 1.04x faster                                                        |
| unpickle_list           | 4.60 us                                                      | 4.44 us: 1.04x faster                                                       |
| genshi_text             | 25.5 ms                                                      | 24.6 ms: 1.04x faster                                                       |
| pickle_pure_python      | 316 us                                                       | 306 us: 1.03x faster                                                        |
| xml_etree_iterparse     | 107 ms                                                       | 103 ms: 1.03x faster                                                        |
| sympy_integrate         | 25.8 ms                                                      | 25.0 ms: 1.03x faster                                                       |
| async_tree_memoization  | 629 ms                                                       | 611 ms: 1.03x faster                                                        |
| sympy_expand            | 553 ms                                                       | 538 ms: 1.03x faster                                                        |
| unpack_sequence         | 45.7 ns                                                      | 44.4 ns: 1.03x faster                                                       |
| bench_thread_pool       | 1.00 ms                                                      | 974 us: 1.03x faster                                                        |
| sympy_str               | 337 ms                                                       | 328 ms: 1.03x faster                                                        |
| thrift                  | 931 us                                                       | 909 us: 1.02x faster                                                        |
| crypto_pyaes            | 83.3 ms                                                      | 81.5 ms: 1.02x faster                                                       |
| pathlib                 | 18.9 ms                                                      | 18.5 ms: 1.02x faster                                                       |
| fannkuch                | 416 ms                                                       | 408 ms: 1.02x faster                                                        |
| docutils                | 2.85 sec                                                     | 2.79 sec: 1.02x faster                                                      |
| deepcopy_reduce         | 3.40 us                                                      | 3.33 us: 1.02x faster                                                       |
| meteor_contest          | 131 ms                                                       | 128 ms: 1.02x faster                                                        |
| pickle_dict             | 32.3 us                                                      | 31.8 us: 1.02x faster                                                       |
| logging_format          | 7.71 us                                                      | 7.59 us: 1.02x faster                                                       |
| async_tree_none         | 518 ms                                                       | 510 ms: 1.02x faster                                                        |
| sqlglot_optimize        | 59.0 ms                                                      | 58.2 ms: 1.01x faster                                                       |
| float                   | 74.9 ms                                                      | 73.9 ms: 1.01x faster                                                       |
| sqlglot_normalize       | 122 ms                                                       | 120 ms: 1.01x faster                                                        |
| regex_dna               | 227 ms                                                       | 225 ms: 1.01x faster                                                        |
| async_tree_cpu_io_mixed | 753 ms                                                       | 745 ms: 1.01x faster                                                        |
| 2to3                    | 287 ms                                                       | 284 ms: 1.01x faster                                                        |
| scimark_fft             | 281 ms                                                       | 278 ms: 1.01x faster                                                        |
| sympy_sum               | 186 ms                                                       | 184 ms: 1.01x faster                                                        |
| regex_effbot            | 3.34 ms                                                      | 3.36 ms: 1.01x slower                                                       |
| spectral_norm           | 95.1 ms                                                      | 95.6 ms: 1.01x slower                                                       |
| unpickle                | 13.3 us                                                      | 13.4 us: 1.01x slower                                                       |
| telco                   | 6.81 ms                                                      | 6.90 ms: 1.01x slower                                                       |
| pickle                  | 9.89 us                                                      | 10.0 us: 1.01x slower                                                       |
| sqlglot_transpile       | 1.91 ms                                                      | 1.94 ms: 1.01x slower                                                       |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 4.14 ms: 1.02x slower                                                       |
| xml_etree_process       | 55.9 ms                                                      | 57.3 ms: 1.03x slower                                                       |
| create_gc_cycles        | 1.58 ms                                                      | 1.63 ms: 1.03x slower                                                       |
| sqlite_synth            | 2.52 us                                                      | 2.63 us: 1.04x slower                                                       |
| sqlglot_parse           | 1.51 ms                                                      | 1.58 ms: 1.04x slower                                                       |
| xml_etree_generate      | 79.7 ms                                                      | 83.5 ms: 1.05x slower                                                       |
| python_startup          | 10.7 ms                                                      | 11.3 ms: 1.05x slower                                                       |
| comprehensions          | 25.1 us                                                      | 26.7 us: 1.07x slower                                                       |
| python_startup_no_site  | 7.73 ms                                                      | 8.34 ms: 1.08x slower                                                       |
| async_generators        | 322 ms                                                       | 385 ms: 1.20x slower                                                        |
| coverage                | 66.1 ms                                                      | 82.2 ms: 1.24x slower                                                       |
| dask                    | 410 ms                                                       | 560 ms: 1.37x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.04x faster                                                                |

Benchmark hidden because not significant (6): nbody, django_template, scimark_monte_carlo, async_tree_io, pidigits, bench_mp_pool
Ignored benchmarks (16) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 1.15x