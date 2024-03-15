
# Results vs. 3.11.0

- fork: python
- ref: 2e49bd06c5ffab7d1540
- machine: linux-x86_64
- commit hash: 2e49bd0
- commit date: 2022-04-05
- overall geometric mean: 1.02x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 293 ms: 1.02x slower                                                        |
| chameleon      | 7.92 ms                                                      | 7.97 ms: 1.01x slower                                                       |
| docutils       | 2.85 sec                                                     | 2.92 sec: 1.03x slower                                                      |
| html5lib       | 72.2 ms                                                      | 75.0 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none        | 518 ms                                                       | 523 ms: 1.01x slower                                                        |
| async_tree_memoization | 629 ms                                                       | 641 ms: 1.02x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                                |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 78.4 ms: 1.05x slower                                                       |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                |

Benchmark hidden because not significant (2): pidigits, nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.13 ms: 1.07x faster                                                       |
| regex_compile  | 156 ms                                                       | 159 ms: 1.02x slower                                                        |
| regex_v8       | 24.4 ms                                                      | 26.6 ms: 1.09x slower                                                       |
| regex_dna      | 227 ms                                                       | 253 ms: 1.11x slower                                                        |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads           | 28.9 us                                                      | 24.5 us: 1.18x faster                                                       |
| pickle_dict          | 32.3 us                                                      | 31.1 us: 1.04x faster                                                       |
| unpickle             | 13.3 us                                                      | 13.0 us: 1.02x faster                                                       |
| unpickle_list        | 4.60 us                                                      | 4.52 us: 1.02x faster                                                       |
| xml_etree_iterparse  | 107 ms                                                       | 106 ms: 1.01x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 157 ms: 1.01x slower                                                        |
| unpickle_pure_python | 238 us                                                       | 242 us: 1.02x slower                                                        |
| json_dumps           | 13.3 ms                                                      | 13.5 ms: 1.02x slower                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 82.8 ms: 1.04x slower                                                       |
| xml_etree_process    | 55.9 ms                                                      | 58.3 ms: 1.04x slower                                                       |
| pickle_list          | 3.94 us                                                      | 4.12 us: 1.05x slower                                                       |
| pickle_pure_python   | 316 us                                                       | 331 us: 1.05x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.00x faster                                                                |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 7.73 ms                                                      | 7.46 ms: 1.04x faster                                                       |
| python_startup         | 10.7 ms                                                      | 10.4 ms: 1.04x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.04x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 11.2 ms: 1.02x slower                                                       |
| django_template | 39.3 ms                                                      | 40.7 ms: 1.04x slower                                                       |
| genshi_xml      | 57.1 ms                                                      | 59.7 ms: 1.05x slower                                                       |
| genshi_text     | 25.5 ms                                                      | 26.8 ms: 1.05x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.04x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads              | 28.9 us                                                      | 24.5 us: 1.18x faster                                                       |
| gc_traversal            | 4.15 ms                                                      | 3.58 ms: 1.16x faster                                                       |
| dask                    | 410 ms                                                       | 367 ms: 1.12x faster                                                        |
| logging_simple          | 7.24 us                                                      | 6.69 us: 1.08x faster                                                       |
| json                    | 5.58 ms                                                      | 5.17 ms: 1.08x faster                                                       |
| regex_effbot            | 3.34 ms                                                      | 3.13 ms: 1.07x faster                                                       |
| sympy_sum               | 186 ms                                                       | 177 ms: 1.05x faster                                                        |
| pickle_dict             | 32.3 us                                                      | 31.1 us: 1.04x faster                                                       |
| python_startup_no_site  | 7.73 ms                                                      | 7.46 ms: 1.04x faster                                                       |
| python_startup          | 10.7 ms                                                      | 10.4 ms: 1.04x faster                                                       |
| chaos                   | 74.9 ms                                                      | 73.4 ms: 1.02x faster                                                       |
| sympy_str               | 337 ms                                                       | 330 ms: 1.02x faster                                                        |
| sympy_integrate         | 25.8 ms                                                      | 25.3 ms: 1.02x faster                                                       |
| unpickle                | 13.3 us                                                      | 13.0 us: 1.02x faster                                                       |
| unpickle_list           | 4.60 us                                                      | 4.52 us: 1.02x faster                                                       |
| logging_format          | 7.71 us                                                      | 7.59 us: 1.02x faster                                                       |
| deepcopy                | 391 us                                                       | 385 us: 1.01x faster                                                        |
| xml_etree_iterparse     | 107 ms                                                       | 106 ms: 1.01x faster                                                        |
| async_generators        | 322 ms                                                       | 319 ms: 1.01x faster                                                        |
| aiohttp                 | 986 us                                                       | 978 us: 1.01x faster                                                        |
| sympy_expand            | 553 ms                                                       | 549 ms: 1.01x faster                                                        |
| mdp                     | 2.77 sec                                                     | 2.76 sec: 1.01x faster                                                      |
| telco                   | 6.81 ms                                                      | 6.79 ms: 1.00x faster                                                       |
| chameleon               | 7.92 ms                                                      | 7.97 ms: 1.01x slower                                                       |
| async_tree_none         | 518 ms                                                       | 523 ms: 1.01x slower                                                        |
| flaskblogging           | 3.88 ms                                                      | 3.92 ms: 1.01x slower                                                       |
| xml_etree_parse         | 155 ms                                                       | 157 ms: 1.01x slower                                                        |
| pycparser               | 1.31 sec                                                     | 1.33 sec: 1.02x slower                                                      |
| pprint_pformat          | 1.67 sec                                                     | 1.69 sec: 1.02x slower                                                      |
| pprint_safe_repr        | 805 ms                                                       | 818 ms: 1.02x slower                                                        |
| unpickle_pure_python    | 238 us                                                       | 242 us: 1.02x slower                                                        |
| json_dumps              | 13.3 ms                                                      | 13.5 ms: 1.02x slower                                                       |
| regex_compile           | 156 ms                                                       | 159 ms: 1.02x slower                                                        |
| async_tree_memoization  | 629 ms                                                       | 641 ms: 1.02x slower                                                        |
| meteor_contest          | 131 ms                                                       | 133 ms: 1.02x slower                                                        |
| mako                    | 11.0 ms                                                      | 11.2 ms: 1.02x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                       |
| 2to3                    | 287 ms                                                       | 293 ms: 1.02x slower                                                        |
| deepcopy_reduce         | 3.40 us                                                      | 3.48 us: 1.02x slower                                                       |
| docutils                | 2.85 sec                                                     | 2.92 sec: 1.03x slower                                                      |
| scimark_sor             | 110 ms                                                       | 112 ms: 1.03x slower                                                        |
| pyflate                 | 449 ms                                                       | 464 ms: 1.03x slower                                                        |
| deepcopy_memo           | 37.5 us                                                      | 38.8 us: 1.03x slower                                                       |
| unpack_sequence         | 45.7 ns                                                      | 47.3 ns: 1.03x slower                                                       |
| dulwich_log             | 67.4 ms                                                      | 69.8 ms: 1.04x slower                                                       |
| django_template         | 39.3 ms                                                      | 40.7 ms: 1.04x slower                                                       |
| sqlalchemy_declarative  | 154 ms                                                       | 160 ms: 1.04x slower                                                        |
| html5lib                | 72.2 ms                                                      | 75.0 ms: 1.04x slower                                                       |
| xml_etree_generate      | 79.7 ms                                                      | 82.8 ms: 1.04x slower                                                       |
| sqlalchemy_imperative   | 19.8 ms                                                      | 20.5 ms: 1.04x slower                                                       |
| sqlglot_normalize       | 122 ms                                                       | 127 ms: 1.04x slower                                                        |
| raytrace                | 309 ms                                                       | 322 ms: 1.04x slower                                                        |
| logging_silent          | 100 ns                                                       | 105 ns: 1.04x slower                                                        |
| create_gc_cycles        | 1.58 ms                                                      | 1.65 ms: 1.04x slower                                                       |
| xml_etree_process       | 55.9 ms                                                      | 58.3 ms: 1.04x slower                                                       |
| coroutines              | 27.8 ms                                                      | 29.0 ms: 1.04x slower                                                       |
| float                   | 74.9 ms                                                      | 78.4 ms: 1.05x slower                                                       |
| pickle_list             | 3.94 us                                                      | 4.12 us: 1.05x slower                                                       |
| genshi_xml              | 57.1 ms                                                      | 59.7 ms: 1.05x slower                                                       |
| pickle_pure_python      | 316 us                                                       | 331 us: 1.05x slower                                                        |
| sqlglot_optimize        | 59.0 ms                                                      | 61.9 ms: 1.05x slower                                                       |
| genshi_text             | 25.5 ms                                                      | 26.8 ms: 1.05x slower                                                       |
| scimark_lu              | 114 ms                                                       | 120 ms: 1.05x slower                                                        |
| go                      | 158 ms                                                       | 166 ms: 1.06x slower                                                        |
| scimark_fft             | 281 ms                                                       | 297 ms: 1.06x slower                                                        |
| fannkuch                | 416 ms                                                       | 442 ms: 1.06x slower                                                        |
| richards                | 49.7 ms                                                      | 52.8 ms: 1.06x slower                                                       |
| deltablue               | 3.97 ms                                                      | 4.23 ms: 1.07x slower                                                       |
| crypto_pyaes            | 83.3 ms                                                      | 89.5 ms: 1.07x slower                                                       |
| regex_v8                | 24.4 ms                                                      | 26.6 ms: 1.09x slower                                                       |
| hexiom                  | 6.98 ms                                                      | 7.66 ms: 1.10x slower                                                       |
| scimark_monte_carlo     | 69.8 ms                                                      | 77.1 ms: 1.10x slower                                                       |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 4.51 ms: 1.11x slower                                                       |
| comprehensions          | 25.1 us                                                      | 27.8 us: 1.11x slower                                                       |
| regex_dna               | 227 ms                                                       | 253 ms: 1.11x slower                                                        |
| spectral_norm           | 95.1 ms                                                      | 107 ms: 1.13x slower                                                        |
| sqlglot_transpile       | 1.91 ms                                                      | 2.38 ms: 1.25x slower                                                       |
| sqlglot_parse           | 1.51 ms                                                      | 2.04 ms: 1.35x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.02x slower                                                                |

Benchmark hidden because not significant (15): bench_mp_pool, tornado_http, nqueens, thrift, sqlite_synth, pickle, asyncio_tcp, pidigits, async_tree_cpu_io_mixed, gunicorn, generators, async_tree_io, pylint, nbody, bench_thread_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.05x