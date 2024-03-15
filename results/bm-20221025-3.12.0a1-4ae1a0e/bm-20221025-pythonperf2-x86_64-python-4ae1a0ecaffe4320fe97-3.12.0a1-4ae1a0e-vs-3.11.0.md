
# Results vs. 3.11.0

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: linux-x86_64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 278 ms: 1.03x faster                                                        |
| chameleon      | 7.92 ms                                                      | 7.62 ms: 1.04x faster                                                       |
| docutils       | 2.85 sec                                                     | 2.79 sec: 1.02x faster                                                      |
| html5lib       | 72.2 ms                                                      | 66.2 ms: 1.09x faster                                                       |
| tornado_http   | 124 ms                                                       | 114 ms: 1.09x faster                                                        |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_memoization | 629 ms                                                       | 618 ms: 1.02x faster                                                        |
| async_tree_io          | 1.17 sec                                                     | 1.16 sec: 1.01x faster                                                      |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                                |

Benchmark hidden because not significant (2): async_tree_none, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 73.2 ms: 1.02x faster                                                       |
| nbody          | 92.9 ms                                                      | 98.1 ms: 1.06x slower                                                       |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 146 ms: 1.07x faster                                                        |
| regex_v8       | 24.4 ms                                                      | 22.9 ms: 1.07x faster                                                       |
| regex_dna      | 227 ms                                                       | 232 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.4 ms: 1.28x faster                                                       |
| json_loads           | 28.9 us                                                      | 24.3 us: 1.19x faster                                                       |
| unpickle_pure_python | 238 us                                                       | 208 us: 1.15x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 138 ms: 1.12x faster                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 103 ms: 1.04x faster                                                        |
| xml_etree_process    | 55.9 ms                                                      | 54.1 ms: 1.03x faster                                                       |
| unpickle_list        | 4.60 us                                                      | 4.47 us: 1.03x faster                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 77.6 ms: 1.03x faster                                                       |
| pickle_list          | 3.94 us                                                      | 3.84 us: 1.03x faster                                                       |
| pickle_dict          | 32.3 us                                                      | 31.9 us: 1.01x faster                                                       |
| pickle_pure_python   | 316 us                                                       | 313 us: 1.01x faster                                                        |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.06x faster                                                                |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 7.73 ms                                                      | 7.62 ms: 1.01x faster                                                       |
| python_startup         | 10.7 ms                                                      | 10.6 ms: 1.01x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 10.4 ms: 1.05x faster                                                       |
| genshi_text     | 25.5 ms                                                      | 24.7 ms: 1.03x faster                                                       |
| genshi_xml      | 57.1 ms                                                      | 55.5 ms: 1.03x faster                                                       |
| django_template | 39.3 ms                                                      | 40.6 ms: 1.03x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.02x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps              | 13.3 ms                                                      | 10.4 ms: 1.28x faster                                                       |
| json_loads              | 28.9 us                                                      | 24.3 us: 1.19x faster                                                       |
| gc_traversal            | 4.15 ms                                                      | 3.54 ms: 1.17x faster                                                       |
| unpickle_pure_python    | 238 us                                                       | 208 us: 1.15x faster                                                        |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 3.58 ms: 1.13x faster                                                       |
| xml_etree_parse         | 155 ms                                                       | 138 ms: 1.12x faster                                                        |
| json                    | 5.58 ms                                                      | 5.05 ms: 1.11x faster                                                       |
| aiohttp                 | 986 us                                                       | 894 us: 1.10x faster                                                        |
| html5lib                | 72.2 ms                                                      | 66.2 ms: 1.09x faster                                                       |
| tornado_http            | 124 ms                                                       | 114 ms: 1.09x faster                                                        |
| gunicorn                | 966 us                                                       | 888 us: 1.09x faster                                                        |
| deltablue               | 3.97 ms                                                      | 3.65 ms: 1.09x faster                                                       |
| regex_compile           | 156 ms                                                       | 146 ms: 1.07x faster                                                        |
| regex_v8                | 24.4 ms                                                      | 22.9 ms: 1.07x faster                                                       |
| pprint_pformat          | 1.67 sec                                                     | 1.57 sec: 1.06x faster                                                      |
| pprint_safe_repr        | 805 ms                                                       | 761 ms: 1.06x faster                                                        |
| nqueens                 | 103 ms                                                       | 97.1 ms: 1.06x faster                                                       |
| hexiom                  | 6.98 ms                                                      | 6.61 ms: 1.06x faster                                                       |
| mako                    | 11.0 ms                                                      | 10.4 ms: 1.05x faster                                                       |
| logging_silent          | 100 ns                                                       | 95.5 ns: 1.05x faster                                                       |
| sympy_expand            | 553 ms                                                       | 527 ms: 1.05x faster                                                        |
| pycparser               | 1.31 sec                                                     | 1.25 sec: 1.05x faster                                                      |
| richards                | 49.7 ms                                                      | 47.6 ms: 1.04x faster                                                       |
| pyflate                 | 449 ms                                                       | 431 ms: 1.04x faster                                                        |
| xml_etree_iterparse     | 107 ms                                                       | 103 ms: 1.04x faster                                                        |
| chameleon               | 7.92 ms                                                      | 7.62 ms: 1.04x faster                                                       |
| meteor_contest          | 131 ms                                                       | 126 ms: 1.04x faster                                                        |
| pylint                  | 514 ms                                                       | 496 ms: 1.04x faster                                                        |
| raytrace                | 309 ms                                                       | 298 ms: 1.04x faster                                                        |
| bench_thread_pool       | 1.00 ms                                                      | 966 us: 1.04x faster                                                        |
| comprehensions          | 25.1 us                                                      | 24.2 us: 1.03x faster                                                       |
| sympy_str               | 337 ms                                                       | 326 ms: 1.03x faster                                                        |
| 2to3                    | 287 ms                                                       | 278 ms: 1.03x faster                                                        |
| deepcopy_memo           | 37.5 us                                                      | 36.4 us: 1.03x faster                                                       |
| xml_etree_process       | 55.9 ms                                                      | 54.1 ms: 1.03x faster                                                       |
| bench_mp_pool           | 4.70 ms                                                      | 4.56 ms: 1.03x faster                                                       |
| genshi_text             | 25.5 ms                                                      | 24.7 ms: 1.03x faster                                                       |
| scimark_monte_carlo     | 69.8 ms                                                      | 67.8 ms: 1.03x faster                                                       |
| genshi_xml              | 57.1 ms                                                      | 55.5 ms: 1.03x faster                                                       |
| unpickle_list           | 4.60 us                                                      | 4.47 us: 1.03x faster                                                       |
| scimark_lu              | 114 ms                                                       | 111 ms: 1.03x faster                                                        |
| fannkuch                | 416 ms                                                       | 405 ms: 1.03x faster                                                        |
| xml_etree_generate      | 79.7 ms                                                      | 77.6 ms: 1.03x faster                                                       |
| telco                   | 6.81 ms                                                      | 6.64 ms: 1.03x faster                                                       |
| logging_simple          | 7.24 us                                                      | 7.06 us: 1.03x faster                                                       |
| pickle_list             | 3.94 us                                                      | 3.84 us: 1.03x faster                                                       |
| sympy_sum               | 186 ms                                                       | 181 ms: 1.03x faster                                                        |
| float                   | 74.9 ms                                                      | 73.2 ms: 1.02x faster                                                       |
| mdp                     | 2.77 sec                                                     | 2.71 sec: 1.02x faster                                                      |
| dulwich_log             | 67.4 ms                                                      | 65.9 ms: 1.02x faster                                                       |
| chaos                   | 74.9 ms                                                      | 73.4 ms: 1.02x faster                                                       |
| go                      | 158 ms                                                       | 155 ms: 1.02x faster                                                        |
| docutils                | 2.85 sec                                                     | 2.79 sec: 1.02x faster                                                      |
| async_tree_memoization  | 629 ms                                                       | 618 ms: 1.02x faster                                                        |
| sympy_integrate         | 25.8 ms                                                      | 25.4 ms: 1.02x faster                                                       |
| python_startup_no_site  | 7.73 ms                                                      | 7.62 ms: 1.01x faster                                                       |
| unpack_sequence         | 45.7 ns                                                      | 45.0 ns: 1.01x faster                                                       |
| python_startup          | 10.7 ms                                                      | 10.6 ms: 1.01x faster                                                       |
| deepcopy_reduce         | 3.40 us                                                      | 3.35 us: 1.01x faster                                                       |
| sqlglot_optimize        | 59.0 ms                                                      | 58.2 ms: 1.01x faster                                                       |
| sqlglot_normalize       | 122 ms                                                       | 120 ms: 1.01x faster                                                        |
| pickle_dict             | 32.3 us                                                      | 31.9 us: 1.01x faster                                                       |
| coroutines              | 27.8 ms                                                      | 27.4 ms: 1.01x faster                                                       |
| scimark_sor             | 110 ms                                                       | 108 ms: 1.01x faster                                                        |
| async_tree_io           | 1.17 sec                                                     | 1.16 sec: 1.01x faster                                                      |
| pickle_pure_python      | 316 us                                                       | 313 us: 1.01x faster                                                        |
| sqlglot_transpile       | 1.91 ms                                                      | 1.90 ms: 1.01x faster                                                       |
| logging_format          | 7.71 us                                                      | 7.77 us: 1.01x slower                                                       |
| deepcopy                | 391 us                                                       | 394 us: 1.01x slower                                                        |
| spectral_norm           | 95.1 ms                                                      | 96.1 ms: 1.01x slower                                                       |
| create_gc_cycles        | 1.58 ms                                                      | 1.61 ms: 1.02x slower                                                       |
| regex_dna               | 227 ms                                                       | 232 ms: 1.02x slower                                                        |
| thrift                  | 931 us                                                       | 953 us: 1.02x slower                                                        |
| pickle                  | 9.89 us                                                      | 10.1 us: 1.02x slower                                                       |
| scimark_fft             | 281 ms                                                       | 288 ms: 1.03x slower                                                        |
| django_template         | 39.3 ms                                                      | 40.6 ms: 1.03x slower                                                       |
| nbody                   | 92.9 ms                                                      | 98.1 ms: 1.06x slower                                                       |
| coverage                | 66.1 ms                                                      | 81.5 ms: 1.23x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.03x faster                                                                |

Benchmark hidden because not significant (13): async_tree_none, async_generators, sqlglot_parse, generators, dask, crypto_pyaes, asyncio_tcp, regex_effbot, pidigits, pathlib, unpickle, async_tree_cpu_io_mixed, sqlite_synth
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 1.01x