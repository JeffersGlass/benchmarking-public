
# Results vs. 3.11.0

- fork: faster-cpython
- ref: nogil_latest
- machine: windows-amd64
- commit hash: 1d39009
- commit date: 2023-04-16
- overall geometric mean: 1.03x slower \*
- HPT reliability: 99.95%
- HPT 99th percentile: 1.01x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 224 ms: 1.05x slower                                                         |
| chameleon      | 5.26 ms                                                     | 5.66 ms: 1.08x slower                                                        |
| docutils       | 1.64 sec                                                    | 1.89 sec: 1.15x slower                                                       |
| html5lib       | 38.9 ms                                                     | 39.3 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                       | 1.07x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io           | 808 ms                                                      | 405 ms: 2.00x faster                                                         |
| async_tree_none         | 332 ms                                                      | 189 ms: 1.76x faster                                                         |
| async_tree_memoization  | 399 ms                                                      | 240 ms: 1.66x faster                                                         |
| async_tree_cpu_io_mixed | 530 ms                                                      | 371 ms: 1.43x faster                                                         |
| Geometric mean          | (ref)                                                       | 1.70x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 49.6 ms: 1.10x faster                                                        |
| pidigits       | 150 ms                                                      | 141 ms: 1.07x faster                                                         |
| nbody          | 70.3 ms                                                     | 89.9 ms: 1.28x slower                                                        |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 13.2 ms: 1.07x faster                                                        |
| regex_dna      | 116 ms                                                      | 110 ms: 1.05x faster                                                         |
| regex_effbot   | 1.50 ms                                                     | 1.53 ms: 1.02x slower                                                        |
| regex_compile  | 91.0 ms                                                     | 96.4 ms: 1.06x slower                                                        |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 6.50 ms: 1.24x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 82.9 ms: 1.18x faster                                                        |
| unpickle_pure_python | 157 us                                                      | 159 us: 1.02x slower                                                         |
| pickle_list          | 2.70 us                                                     | 2.81 us: 1.04x slower                                                        |
| pickle_pure_python   | 208 us                                                      | 218 us: 1.04x slower                                                         |
| pickle               | 6.64 us                                                     | 7.14 us: 1.08x slower                                                        |
| xml_etree_generate   | 52.5 ms                                                     | 57.5 ms: 1.09x slower                                                        |
| unpickle_list        | 2.59 us                                                     | 2.86 us: 1.10x slower                                                        |
| xml_etree_process    | 37.2 ms                                                     | 41.7 ms: 1.12x slower                                                        |
| json_loads           | 13.0 us                                                     | 14.6 us: 1.12x slower                                                        |
| xml_etree_iterparse  | 65.6 ms                                                     | 74.7 ms: 1.14x slower                                                        |
| pickle_dict          | 18.5 us                                                     | 21.8 us: 1.18x slower                                                        |
| unpickle             | 7.57 us                                                     | 9.19 us: 1.21x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.06x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.4 ms: 1.09x faster                                                        |
| python_startup         | 19.8 ms                                                     | 18.2 ms: 1.09x faster                                                        |
| Geometric mean         | (ref)                                                       | 1.09x faster                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| genshi_xml      | 39.9 ms                                                     | 35.3 ms: 1.13x faster                                                        |
| genshi_text     | 18.4 ms                                                     | 17.7 ms: 1.04x faster                                                        |
| django_template | 24.4 ms                                                     | 25.5 ms: 1.04x slower                                                        |
| mako            | 7.58 ms                                                     | 8.95 ms: 1.18x slower                                                        |
| Geometric mean  | (ref)                                                       | 1.01x slower                                                                 |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io           | 808 ms                                                      | 405 ms: 2.00x faster                                                         |
| async_tree_none         | 332 ms                                                      | 189 ms: 1.76x faster                                                         |
| async_tree_memoization  | 399 ms                                                      | 240 ms: 1.66x faster                                                         |
| asyncio_tcp             | 726 ms                                                      | 489 ms: 1.48x faster                                                         |
| async_tree_cpu_io_mixed | 530 ms                                                      | 371 ms: 1.43x faster                                                         |
| sqlite_synth            | 1.77 us                                                     | 1.35 us: 1.31x faster                                                        |
| json_dumps              | 8.09 ms                                                     | 6.50 ms: 1.24x faster                                                        |
| xml_etree_parse         | 97.6 ms                                                     | 82.9 ms: 1.18x faster                                                        |
| genshi_xml              | 39.9 ms                                                     | 35.3 ms: 1.13x faster                                                        |
| float                   | 54.4 ms                                                     | 49.6 ms: 1.10x faster                                                        |
| python_startup_no_site  | 16.8 ms                                                     | 15.4 ms: 1.09x faster                                                        |
| python_startup          | 19.8 ms                                                     | 18.2 ms: 1.09x faster                                                        |
| regex_v8                | 14.2 ms                                                     | 13.2 ms: 1.07x faster                                                        |
| pidigits                | 150 ms                                                      | 141 ms: 1.07x faster                                                         |
| dulwich_log             | 46.4 ms                                                     | 43.6 ms: 1.06x faster                                                        |
| regex_dna               | 116 ms                                                      | 110 ms: 1.05x faster                                                         |
| genshi_text             | 18.4 ms                                                     | 17.7 ms: 1.04x faster                                                        |
| nqueens                 | 68.3 ms                                                     | 65.6 ms: 1.04x faster                                                        |
| pyflate                 | 312 ms                                                      | 302 ms: 1.03x faster                                                         |
| pycparser               | 720 ms                                                      | 713 ms: 1.01x faster                                                         |
| deltablue               | 2.70 ms                                                     | 2.71 ms: 1.01x slower                                                        |
| logging_simple          | 6.86 us                                                     | 6.92 us: 1.01x slower                                                        |
| bench_mp_pool           | 63.2 ms                                                     | 63.9 ms: 1.01x slower                                                        |
| html5lib                | 38.9 ms                                                     | 39.3 ms: 1.01x slower                                                        |
| unpickle_pure_python    | 157 us                                                      | 159 us: 1.02x slower                                                         |
| go                      | 101 ms                                                      | 103 ms: 1.02x slower                                                         |
| regex_effbot            | 1.50 ms                                                     | 1.53 ms: 1.02x slower                                                        |
| mdp                     | 1.59 sec                                                    | 1.63 sec: 1.02x slower                                                       |
| richards                | 31.4 ms                                                     | 32.3 ms: 1.03x slower                                                        |
| logging_format          | 7.16 us                                                     | 7.40 us: 1.03x slower                                                        |
| pathlib                 | 70.9 ms                                                     | 73.6 ms: 1.04x slower                                                        |
| pickle_list             | 2.70 us                                                     | 2.81 us: 1.04x slower                                                        |
| sqlglot_normalize       | 190 ms                                                      | 199 ms: 1.04x slower                                                         |
| django_template         | 24.4 ms                                                     | 25.5 ms: 1.04x slower                                                        |
| pickle_pure_python      | 208 us                                                      | 218 us: 1.04x slower                                                         |
| gc_traversal            | 1.49 ms                                                     | 1.56 ms: 1.05x slower                                                        |
| logging_silent          | 71.8 ns                                                     | 75.0 ns: 1.05x slower                                                        |
| 2to3                    | 214 ms                                                      | 224 ms: 1.05x slower                                                         |
| create_gc_cycles        | 713 us                                                      | 748 us: 1.05x slower                                                         |
| sympy_integrate         | 14.0 ms                                                     | 14.8 ms: 1.06x slower                                                        |
| regex_compile           | 91.0 ms                                                     | 96.4 ms: 1.06x slower                                                        |
| sqlglot_optimize        | 34.5 ms                                                     | 36.8 ms: 1.06x slower                                                        |
| sympy_str               | 185 ms                                                      | 198 ms: 1.07x slower                                                         |
| sympy_expand            | 299 ms                                                      | 320 ms: 1.07x slower                                                         |
| pickle                  | 6.64 us                                                     | 7.14 us: 1.08x slower                                                        |
| chameleon               | 5.26 ms                                                     | 5.66 ms: 1.08x slower                                                        |
| crypto_pyaes            | 48.9 ms                                                     | 52.7 ms: 1.08x slower                                                        |
| telco                   | 4.06 ms                                                     | 4.41 ms: 1.08x slower                                                        |
| sympy_sum               | 100 ms                                                      | 109 ms: 1.09x slower                                                         |
| hexiom                  | 4.55 ms                                                     | 4.97 ms: 1.09x slower                                                        |
| xml_etree_generate      | 52.5 ms                                                     | 57.5 ms: 1.09x slower                                                        |
| thrift                  | 494 us                                                      | 542 us: 1.10x slower                                                         |
| deepcopy                | 246 us                                                      | 272 us: 1.10x slower                                                         |
| unpickle_list           | 2.59 us                                                     | 2.86 us: 1.10x slower                                                        |
| generators              | 34.0 ms                                                     | 37.5 ms: 1.11x slower                                                        |
| pprint_safe_repr        | 529 ms                                                      | 586 ms: 1.11x slower                                                         |
| chaos                   | 48.4 ms                                                     | 53.7 ms: 1.11x slower                                                        |
| pprint_pformat          | 1.09 sec                                                    | 1.21 sec: 1.11x slower                                                       |
| xml_etree_process       | 37.2 ms                                                     | 41.7 ms: 1.12x slower                                                        |
| coroutines              | 15.0 ms                                                     | 16.8 ms: 1.12x slower                                                        |
| json_loads              | 13.0 us                                                     | 14.6 us: 1.12x slower                                                        |
| fannkuch                | 253 ms                                                      | 285 ms: 1.12x slower                                                         |
| scimark_monte_carlo     | 45.3 ms                                                     | 51.2 ms: 1.13x slower                                                        |
| raytrace                | 213 ms                                                      | 241 ms: 1.13x slower                                                         |
| deepcopy_memo           | 26.0 us                                                     | 29.5 us: 1.14x slower                                                        |
| sqlglot_transpile       | 1.16 ms                                                     | 1.33 ms: 1.14x slower                                                        |
| xml_etree_iterparse     | 65.6 ms                                                     | 74.7 ms: 1.14x slower                                                        |
| scimark_sor             | 78.1 ms                                                     | 89.1 ms: 1.14x slower                                                        |
| docutils                | 1.64 sec                                                    | 1.89 sec: 1.15x slower                                                       |
| meteor_contest          | 75.2 ms                                                     | 86.5 ms: 1.15x slower                                                        |
| spectral_norm           | 68.3 ms                                                     | 78.8 ms: 1.15x slower                                                        |
| async_generators        | 177 ms                                                      | 205 ms: 1.16x slower                                                         |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.98 ms: 1.16x slower                                                        |
| scimark_lu              | 62.8 ms                                                     | 73.1 ms: 1.16x slower                                                        |
| deepcopy_reduce         | 2.06 us                                                     | 2.40 us: 1.16x slower                                                        |
| sqlglot_parse           | 953 us                                                      | 1.12 ms: 1.17x slower                                                        |
| unpack_sequence         | 46.9 ns                                                     | 55.2 ns: 1.18x slower                                                        |
| pickle_dict             | 18.5 us                                                     | 21.8 us: 1.18x slower                                                        |
| mako                    | 7.58 ms                                                     | 8.95 ms: 1.18x slower                                                        |
| bench_thread_pool       | 872 us                                                      | 1.03 ms: 1.18x slower                                                        |
| unpickle                | 7.57 us                                                     | 9.19 us: 1.21x slower                                                        |
| comprehensions          | 15.6 us                                                     | 19.1 us: 1.22x slower                                                        |
| scimark_fft             | 179 ms                                                      | 220 ms: 1.23x slower                                                         |
| nbody                   | 70.3 ms                                                     | 89.9 ms: 1.28x slower                                                        |
| coverage                | 43.4 ms                                                     | 59.9 ms: 1.38x slower                                                        |
| Geometric mean          | (ref)                                                       | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): json
Ignored benchmarks (16) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, dask, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 99.95% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: unknown