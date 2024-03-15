
# Results vs. 3.11.0

- fork: python
- ref: 2e91dba437fe5c56c6f8
- machine: linux-x86_64
- commit hash: 2e91dba
- commit date: 2021-12-08
- overall geometric mean: 1.06x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 293 ms: 1.02x slower                                                        |
| chameleon      | 7.92 ms                                                      | 8.85 ms: 1.12x slower                                                       |
| docutils       | 2.85 sec                                                     | 3.02 sec: 1.06x slower                                                      |
| html5lib       | 72.2 ms                                                      | 75.1 ms: 1.04x slower                                                       |
| tornado_http   | 124 ms                                                       | 135 ms: 1.08x slower                                                        |
| Geometric mean | (ref)                                                        | 1.06x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 518 ms                                                       | 545 ms: 1.05x slower                                                        |
| async_tree_cpu_io_mixed | 753 ms                                                       | 811 ms: 1.08x slower                                                        |
| async_tree_memoization  | 629 ms                                                       | 686 ms: 1.09x slower                                                        |
| async_tree_io           | 1.17 sec                                                     | 1.32 sec: 1.13x slower                                                      |
| Geometric mean          | (ref)                                                        | 1.09x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 253 ms: 1.01x slower                                                        |
| float          | 74.9 ms                                                      | 80.9 ms: 1.08x slower                                                       |
| nbody          | 92.9 ms                                                      | 109 ms: 1.17x slower                                                        |
| Geometric mean | (ref)                                                        | 1.08x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.10 ms: 1.08x faster                                                       |
| regex_compile  | 156 ms                                                       | 153 ms: 1.02x faster                                                        |
| regex_v8       | 24.4 ms                                                      | 25.7 ms: 1.05x slower                                                       |
| regex_dna      | 227 ms                                                       | 261 ms: 1.15x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads           | 28.9 us                                                      | 25.3 us: 1.14x faster                                                       |
| unpickle_list        | 4.60 us                                                      | 4.53 us: 1.01x faster                                                       |
| pickle_dict          | 32.3 us                                                      | 33.0 us: 1.02x slower                                                       |
| xml_etree_iterparse  | 107 ms                                                       | 110 ms: 1.03x slower                                                        |
| pickle               | 9.89 us                                                      | 10.2 us: 1.03x slower                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 82.8 ms: 1.04x slower                                                       |
| json_dumps           | 13.3 ms                                                      | 14.1 ms: 1.06x slower                                                       |
| xml_etree_process    | 55.9 ms                                                      | 60.9 ms: 1.09x slower                                                       |
| pickle_list          | 3.94 us                                                      | 4.32 us: 1.10x slower                                                       |
| unpickle_pure_python | 238 us                                                       | 265 us: 1.11x slower                                                        |
| pickle_pure_python   | 316 us                                                       | 366 us: 1.16x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.04x slower                                                                |

Benchmark hidden because not significant (2): unpickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 7.73 ms                                                      | 7.14 ms: 1.08x faster                                                       |
| python_startup         | 10.7 ms                                                      | 10.1 ms: 1.06x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.07x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| genshi_xml      | 57.1 ms                                                      | 59.7 ms: 1.05x slower                                                       |
| genshi_text     | 25.5 ms                                                      | 28.2 ms: 1.11x slower                                                       |
| django_template | 39.3 ms                                                      | 44.9 ms: 1.14x slower                                                       |
| mako            | 11.0 ms                                                      | 12.9 ms: 1.17x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.12x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads              | 28.9 us                                                      | 25.3 us: 1.14x faster                                                       |
| generators              | 54.6 ms                                                      | 50.1 ms: 1.09x faster                                                       |
| python_startup_no_site  | 7.73 ms                                                      | 7.14 ms: 1.08x faster                                                       |
| regex_effbot            | 3.34 ms                                                      | 3.10 ms: 1.08x faster                                                       |
| gc_traversal            | 4.15 ms                                                      | 3.89 ms: 1.07x faster                                                       |
| json                    | 5.58 ms                                                      | 5.24 ms: 1.07x faster                                                       |
| python_startup          | 10.7 ms                                                      | 10.1 ms: 1.06x faster                                                       |
| scimark_lu              | 114 ms                                                       | 110 ms: 1.04x faster                                                        |
| coroutines              | 27.8 ms                                                      | 27.0 ms: 1.03x faster                                                       |
| logging_simple          | 7.24 us                                                      | 7.04 us: 1.03x faster                                                       |
| regex_compile           | 156 ms                                                       | 153 ms: 1.02x faster                                                        |
| unpickle_list           | 4.60 us                                                      | 4.53 us: 1.01x faster                                                       |
| meteor_contest          | 131 ms                                                       | 129 ms: 1.01x faster                                                        |
| async_generators        | 322 ms                                                       | 319 ms: 1.01x faster                                                        |
| mdp                     | 2.77 sec                                                     | 2.76 sec: 1.00x faster                                                      |
| pidigits                | 251 ms                                                       | 253 ms: 1.01x slower                                                        |
| unpack_sequence         | 45.7 ns                                                      | 46.3 ns: 1.01x slower                                                       |
| sympy_sum               | 186 ms                                                       | 189 ms: 1.02x slower                                                        |
| pickle_dict             | 32.3 us                                                      | 33.0 us: 1.02x slower                                                       |
| 2to3                    | 287 ms                                                       | 293 ms: 1.02x slower                                                        |
| sympy_integrate         | 25.8 ms                                                      | 26.5 ms: 1.03x slower                                                       |
| fannkuch                | 416 ms                                                       | 428 ms: 1.03x slower                                                        |
| pycparser               | 1.31 sec                                                     | 1.35 sec: 1.03x slower                                                      |
| xml_etree_iterparse     | 107 ms                                                       | 110 ms: 1.03x slower                                                        |
| pprint_safe_repr        | 805 ms                                                       | 832 ms: 1.03x slower                                                        |
| pickle                  | 9.89 us                                                      | 10.2 us: 1.03x slower                                                       |
| gunicorn                | 966 us                                                       | 1.00 ms: 1.04x slower                                                       |
| html5lib                | 72.2 ms                                                      | 75.1 ms: 1.04x slower                                                       |
| xml_etree_generate      | 79.7 ms                                                      | 82.8 ms: 1.04x slower                                                       |
| sympy_str               | 337 ms                                                       | 350 ms: 1.04x slower                                                        |
| pprint_pformat          | 1.67 sec                                                     | 1.74 sec: 1.04x slower                                                      |
| bench_mp_pool           | 4.70 ms                                                      | 4.90 ms: 1.04x slower                                                       |
| chaos                   | 74.9 ms                                                      | 78.3 ms: 1.04x slower                                                       |
| telco                   | 6.81 ms                                                      | 7.11 ms: 1.04x slower                                                       |
| deepcopy_reduce         | 3.40 us                                                      | 3.55 us: 1.05x slower                                                       |
| genshi_xml              | 57.1 ms                                                      | 59.7 ms: 1.05x slower                                                       |
| sympy_expand            | 553 ms                                                       | 579 ms: 1.05x slower                                                        |
| spectral_norm           | 95.1 ms                                                      | 99.9 ms: 1.05x slower                                                       |
| create_gc_cycles        | 1.58 ms                                                      | 1.66 ms: 1.05x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 19.9 ms: 1.05x slower                                                       |
| scimark_sor             | 110 ms                                                       | 115 ms: 1.05x slower                                                        |
| async_tree_none         | 518 ms                                                       | 545 ms: 1.05x slower                                                        |
| regex_v8                | 24.4 ms                                                      | 25.7 ms: 1.05x slower                                                       |
| bench_thread_pool       | 1.00 ms                                                      | 1.06 ms: 1.06x slower                                                       |
| json_dumps              | 13.3 ms                                                      | 14.1 ms: 1.06x slower                                                       |
| dask                    | 410 ms                                                       | 435 ms: 1.06x slower                                                        |
| docutils                | 2.85 sec                                                     | 3.02 sec: 1.06x slower                                                      |
| hexiom                  | 6.98 ms                                                      | 7.41 ms: 1.06x slower                                                       |
| deepcopy                | 391 us                                                       | 418 us: 1.07x slower                                                        |
| thrift                  | 931 us                                                       | 995 us: 1.07x slower                                                        |
| sqlite_synth            | 2.52 us                                                      | 2.70 us: 1.07x slower                                                       |
| async_tree_cpu_io_mixed | 753 ms                                                       | 811 ms: 1.08x slower                                                        |
| float                   | 74.9 ms                                                      | 80.9 ms: 1.08x slower                                                       |
| tornado_http            | 124 ms                                                       | 135 ms: 1.08x slower                                                        |
| dulwich_log             | 67.4 ms                                                      | 73.0 ms: 1.08x slower                                                       |
| xml_etree_process       | 55.9 ms                                                      | 60.9 ms: 1.09x slower                                                       |
| sqlglot_normalize       | 122 ms                                                       | 133 ms: 1.09x slower                                                        |
| coverage                | 66.1 ms                                                      | 72.1 ms: 1.09x slower                                                       |
| async_tree_memoization  | 629 ms                                                       | 686 ms: 1.09x slower                                                        |
| go                      | 158 ms                                                       | 173 ms: 1.09x slower                                                        |
| pickle_list             | 3.94 us                                                      | 4.32 us: 1.10x slower                                                       |
| sqlglot_optimize        | 59.0 ms                                                      | 64.7 ms: 1.10x slower                                                       |
| scimark_monte_carlo     | 69.8 ms                                                      | 76.7 ms: 1.10x slower                                                       |
| deepcopy_memo           | 37.5 us                                                      | 41.5 us: 1.10x slower                                                       |
| genshi_text             | 25.5 ms                                                      | 28.2 ms: 1.11x slower                                                       |
| unpickle_pure_python    | 238 us                                                       | 265 us: 1.11x slower                                                        |
| chameleon               | 7.92 ms                                                      | 8.85 ms: 1.12x slower                                                       |
| scimark_fft             | 281 ms                                                       | 314 ms: 1.12x slower                                                        |
| raytrace                | 309 ms                                                       | 347 ms: 1.12x slower                                                        |
| async_tree_io           | 1.17 sec                                                     | 1.32 sec: 1.13x slower                                                      |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 4.58 ms: 1.13x slower                                                       |
| crypto_pyaes            | 83.3 ms                                                      | 94.7 ms: 1.14x slower                                                       |
| richards                | 49.7 ms                                                      | 56.7 ms: 1.14x slower                                                       |
| django_template         | 39.3 ms                                                      | 44.9 ms: 1.14x slower                                                       |
| regex_dna               | 227 ms                                                       | 261 ms: 1.15x slower                                                        |
| logging_silent          | 100 ns                                                       | 116 ns: 1.16x slower                                                        |
| pickle_pure_python      | 316 us                                                       | 366 us: 1.16x slower                                                        |
| nbody                   | 92.9 ms                                                      | 109 ms: 1.17x slower                                                        |
| pyflate                 | 449 ms                                                       | 525 ms: 1.17x slower                                                        |
| mako                    | 11.0 ms                                                      | 12.9 ms: 1.17x slower                                                       |
| deltablue               | 3.97 ms                                                      | 4.78 ms: 1.20x slower                                                       |
| comprehensions          | 25.1 us                                                      | 30.6 us: 1.22x slower                                                       |
| flaskblogging           | 3.88 ms                                                      | 4.95 ms: 1.28x slower                                                       |
| sqlglot_transpile       | 1.91 ms                                                      | 2.60 ms: 1.36x slower                                                       |
| sqlglot_parse           | 1.51 ms                                                      | 2.21 ms: 1.46x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.06x slower                                                                |

Benchmark hidden because not significant (4): unpickle, logging_format, nqueens, xml_etree_parse
Ignored benchmarks (15) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.04x