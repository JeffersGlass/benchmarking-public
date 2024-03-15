
# Results vs. 3.10.4

- fork: faster-cpython
- ref: nogil_latest
- machine: windows-amd64
- commit hash: 1d39009
- commit date: 2023-04-16
- overall geometric mean: 1.09x faster \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 224 ms: 1.10x faster                                                         |
| chameleon      | 5.79 ms                                                     | 5.66 ms: 1.02x faster                                                        |
| docutils       | 1.92 sec                                                    | 1.89 sec: 1.02x faster                                                       |
| html5lib       | 51.0 ms                                                     | 39.3 ms: 1.30x faster                                                        |
| Geometric mean | (ref)                                                       | 1.10x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 405 ms: 2.74x faster                                                         |
| async_tree_none         | 435 ms                                                      | 189 ms: 2.30x faster                                                         |
| async_tree_memoization  | 526 ms                                                      | 240 ms: 2.19x faster                                                         |
| async_tree_cpu_io_mixed | 638 ms                                                      | 371 ms: 1.72x faster                                                         |
| Geometric mean          | (ref)                                                       | 2.21x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 49.6 ms: 1.25x faster                                                        |
| pidigits       | 149 ms                                                      | 141 ms: 1.06x faster                                                         |
| nbody          | 71.3 ms                                                     | 89.9 ms: 1.26x slower                                                        |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 110 ms: 1.24x faster                                                         |
| regex_v8       | 15.4 ms                                                     | 13.2 ms: 1.17x faster                                                        |
| regex_compile  | 106 ms                                                      | 96.4 ms: 1.10x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.53 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                       | 1.15x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 6.50 ms: 1.41x faster                                                        |
| pickle_pure_python   | 270 us                                                      | 218 us: 1.24x faster                                                         |
| xml_etree_parse      | 96.8 ms                                                     | 82.9 ms: 1.17x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 159 us: 1.15x faster                                                         |
| xml_etree_process    | 44.5 ms                                                     | 41.7 ms: 1.07x faster                                                        |
| unpickle             | 9.09 us                                                     | 9.19 us: 1.01x slower                                                        |
| pickle_list          | 2.75 us                                                     | 2.81 us: 1.02x slower                                                        |
| xml_etree_generate   | 55.5 ms                                                     | 57.5 ms: 1.03x slower                                                        |
| json_loads           | 14.0 us                                                     | 14.6 us: 1.04x slower                                                        |
| pickle               | 6.85 us                                                     | 7.14 us: 1.04x slower                                                        |
| unpickle_list        | 2.71 us                                                     | 2.86 us: 1.05x slower                                                        |
| xml_etree_iterparse  | 65.0 ms                                                     | 74.7 ms: 1.15x slower                                                        |
| pickle_dict          | 17.2 us                                                     | 21.8 us: 1.27x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup | 20.6 ms                                                     | 18.2 ms: 1.13x faster                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                 |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| genshi_xml      | 41.0 ms                                                     | 35.3 ms: 1.16x faster                                                        |
| django_template | 28.9 ms                                                     | 25.5 ms: 1.13x faster                                                        |
| genshi_text     | 19.8 ms                                                     | 17.7 ms: 1.12x faster                                                        |
| Geometric mean  | (ref)                                                       | 1.10x faster                                                                 |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 405 ms: 2.74x faster                                                         |
| async_tree_none         | 435 ms                                                      | 189 ms: 2.30x faster                                                         |
| async_tree_memoization  | 526 ms                                                      | 240 ms: 2.19x faster                                                         |
| async_tree_cpu_io_mixed | 638 ms                                                      | 371 ms: 1.72x faster                                                         |
| deltablue               | 4.19 ms                                                     | 2.71 ms: 1.54x faster                                                        |
| asyncio_tcp             | 732 ms                                                      | 489 ms: 1.50x faster                                                         |
| sqlite_synth            | 1.91 us                                                     | 1.35 us: 1.41x faster                                                        |
| json_dumps              | 9.16 ms                                                     | 6.50 ms: 1.41x faster                                                        |
| pyflate                 | 409 ms                                                      | 302 ms: 1.35x faster                                                         |
| go                      | 139 ms                                                      | 103 ms: 1.35x faster                                                         |
| richards                | 42.4 ms                                                     | 32.3 ms: 1.31x faster                                                        |
| pycparser               | 930 ms                                                      | 713 ms: 1.31x faster                                                         |
| html5lib                | 51.0 ms                                                     | 39.3 ms: 1.30x faster                                                        |
| logging_silent          | 94.6 ns                                                     | 75.0 ns: 1.26x faster                                                        |
| float                   | 61.7 ms                                                     | 49.6 ms: 1.25x faster                                                        |
| pickle_pure_python      | 270 us                                                      | 218 us: 1.24x faster                                                         |
| regex_dna               | 136 ms                                                      | 110 ms: 1.24x faster                                                         |
| scimark_sor             | 106 ms                                                      | 89.1 ms: 1.19x faster                                                        |
| crypto_pyaes            | 62.5 ms                                                     | 52.7 ms: 1.19x faster                                                        |
| scimark_lu              | 85.8 ms                                                     | 73.1 ms: 1.17x faster                                                        |
| regex_v8                | 15.4 ms                                                     | 13.2 ms: 1.17x faster                                                        |
| xml_etree_parse         | 96.8 ms                                                     | 82.9 ms: 1.17x faster                                                        |
| genshi_xml              | 41.0 ms                                                     | 35.3 ms: 1.16x faster                                                        |
| dulwich_log             | 50.5 ms                                                     | 43.6 ms: 1.16x faster                                                        |
| hexiom                  | 5.74 ms                                                     | 4.97 ms: 1.16x faster                                                        |
| unpickle_pure_python    | 183 us                                                      | 159 us: 1.15x faster                                                         |
| chaos                   | 61.7 ms                                                     | 53.7 ms: 1.15x faster                                                        |
| thrift                  | 617 us                                                      | 542 us: 1.14x faster                                                         |
| raytrace                | 273 ms                                                      | 241 ms: 1.13x faster                                                         |
| django_template         | 28.9 ms                                                     | 25.5 ms: 1.13x faster                                                        |
| python_startup          | 20.6 ms                                                     | 18.2 ms: 1.13x faster                                                        |
| genshi_text             | 19.8 ms                                                     | 17.7 ms: 1.12x faster                                                        |
| scimark_monte_carlo     | 57.3 ms                                                     | 51.2 ms: 1.12x faster                                                        |
| sqlglot_transpile       | 1.48 ms                                                     | 1.33 ms: 1.11x faster                                                        |
| regex_compile           | 106 ms                                                      | 96.4 ms: 1.10x faster                                                        |
| 2to3                    | 246 ms                                                      | 224 ms: 1.10x faster                                                         |
| mdp                     | 1.78 sec                                                    | 1.63 sec: 1.09x faster                                                       |
| sqlglot_parse           | 1.22 ms                                                     | 1.12 ms: 1.09x faster                                                        |
| sqlglot_optimize        | 39.8 ms                                                     | 36.8 ms: 1.08x faster                                                        |
| regex_effbot            | 1.66 ms                                                     | 1.53 ms: 1.08x faster                                                        |
| async_generators        | 222 ms                                                      | 205 ms: 1.08x faster                                                         |
| create_gc_cycles        | 800 us                                                      | 748 us: 1.07x faster                                                         |
| xml_etree_process       | 44.5 ms                                                     | 41.7 ms: 1.07x faster                                                        |
| json                    | 3.14 ms                                                     | 2.94 ms: 1.07x faster                                                        |
| pidigits                | 149 ms                                                      | 141 ms: 1.06x faster                                                         |
| sqlglot_normalize       | 205 ms                                                      | 199 ms: 1.03x faster                                                         |
| sympy_integrate         | 15.3 ms                                                     | 14.8 ms: 1.03x faster                                                        |
| pathlib                 | 75.7 ms                                                     | 73.6 ms: 1.03x faster                                                        |
| chameleon               | 5.79 ms                                                     | 5.66 ms: 1.02x faster                                                        |
| docutils                | 1.92 sec                                                    | 1.89 sec: 1.02x faster                                                       |
| nqueens                 | 66.6 ms                                                     | 65.6 ms: 1.02x faster                                                        |
| pprint_safe_repr        | 592 ms                                                      | 586 ms: 1.01x faster                                                         |
| pprint_pformat          | 1.22 sec                                                    | 1.21 sec: 1.01x faster                                                       |
| unpickle                | 9.09 us                                                     | 9.19 us: 1.01x slower                                                        |
| sympy_expand            | 314 ms                                                      | 320 ms: 1.02x slower                                                         |
| sympy_str               | 194 ms                                                      | 198 ms: 1.02x slower                                                         |
| spectral_norm           | 77.3 ms                                                     | 78.8 ms: 1.02x slower                                                        |
| pickle_list             | 2.75 us                                                     | 2.81 us: 1.02x slower                                                        |
| sympy_sum               | 107 ms                                                      | 109 ms: 1.02x slower                                                         |
| deepcopy_memo           | 28.8 us                                                     | 29.5 us: 1.02x slower                                                        |
| bench_mp_pool           | 62.0 ms                                                     | 63.9 ms: 1.03x slower                                                        |
| xml_etree_generate      | 55.5 ms                                                     | 57.5 ms: 1.03x slower                                                        |
| json_loads              | 14.0 us                                                     | 14.6 us: 1.04x slower                                                        |
| pickle                  | 6.85 us                                                     | 7.14 us: 1.04x slower                                                        |
| coroutines              | 16.0 ms                                                     | 16.8 ms: 1.05x slower                                                        |
| unpickle_list           | 2.71 us                                                     | 2.86 us: 1.05x slower                                                        |
| deepcopy                | 255 us                                                      | 272 us: 1.06x slower                                                         |
| bench_thread_pool       | 958 us                                                      | 1.03 ms: 1.07x slower                                                        |
| deepcopy_reduce         | 2.20 us                                                     | 2.40 us: 1.09x slower                                                        |
| logging_format          | 6.76 us                                                     | 7.40 us: 1.10x slower                                                        |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.98 ms: 1.10x slower                                                        |
| gc_traversal            | 1.41 ms                                                     | 1.56 ms: 1.11x slower                                                        |
| logging_simple          | 6.22 us                                                     | 6.92 us: 1.11x slower                                                        |
| fannkuch                | 256 ms                                                      | 285 ms: 1.11x slower                                                         |
| telco                   | 3.94 ms                                                     | 4.41 ms: 1.12x slower                                                        |
| meteor_contest          | 75.9 ms                                                     | 86.5 ms: 1.14x slower                                                        |
| xml_etree_iterparse     | 65.0 ms                                                     | 74.7 ms: 1.15x slower                                                        |
| comprehensions          | 16.5 us                                                     | 19.1 us: 1.16x slower                                                        |
| generators              | 32.4 ms                                                     | 37.5 ms: 1.16x slower                                                        |
| scimark_fft             | 187 ms                                                      | 220 ms: 1.17x slower                                                         |
| nbody                   | 71.3 ms                                                     | 89.9 ms: 1.26x slower                                                        |
| pickle_dict             | 17.2 us                                                     | 21.8 us: 1.27x slower                                                        |
| unpack_sequence         | 39.6 ns                                                     | 55.2 ns: 1.39x slower                                                        |
| coverage                | 39.0 ms                                                     | 59.9 ms: 1.54x slower                                                        |
| Geometric mean          | (ref)                                                       | 1.09x faster                                                                 |

Benchmark hidden because not significant (2): mako, python_startup_no_site
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, dask, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown