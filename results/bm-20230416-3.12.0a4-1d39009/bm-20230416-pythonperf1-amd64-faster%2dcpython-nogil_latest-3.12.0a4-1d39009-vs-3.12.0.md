
# Results vs. 3.12.0

- fork: faster-cpython
- ref: nogil_latest
- machine: windows-amd64
- commit hash: 1d39009
- commit date: 2023-04-16
- overall geometric mean: 1.08x slower \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.03x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 224 ms: 1.03x slower                                                         |
| chameleon      | 4.98 ms                                                     | 5.66 ms: 1.14x slower                                                        |
| docutils       | 1.66 sec                                                    | 1.89 sec: 1.14x slower                                                       |
| Geometric mean | (ref)                                                       | 1.10x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io           | 731 ms                                                      | 405 ms: 1.81x faster                                                         |
| async_tree_none         | 291 ms                                                      | 189 ms: 1.54x faster                                                         |
| async_tree_memoization  | 339 ms                                                      | 240 ms: 1.41x faster                                                         |
| async_tree_cpu_io_mixed | 489 ms                                                      | 371 ms: 1.32x faster                                                         |
| Geometric mean          | (ref)                                                       | 1.51x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 49.6 ms: 1.15x faster                                                        |
| pidigits       | 152 ms                                                      | 141 ms: 1.08x faster                                                         |
| nbody          | 71.9 ms                                                     | 89.9 ms: 1.25x slower                                                        |
| Geometric mean | (ref)                                                       | 1.00x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 110 ms: 1.15x faster                                                         |
| regex_v8       | 14.2 ms                                                     | 13.2 ms: 1.08x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.53 ms: 1.06x faster                                                        |
| regex_compile  | 87.5 ms                                                     | 96.4 ms: 1.10x slower                                                        |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| xml_etree_parse      | 93.0 ms                                                     | 82.9 ms: 1.12x faster                                                        |
| pickle               | 7.43 us                                                     | 7.14 us: 1.04x faster                                                        |
| pickle_list          | 2.83 us                                                     | 2.81 us: 1.01x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 57.5 ms: 1.03x slower                                                        |
| unpickle_list        | 2.75 us                                                     | 2.86 us: 1.04x slower                                                        |
| json_loads           | 13.9 us                                                     | 14.6 us: 1.05x slower                                                        |
| xml_etree_process    | 37.7 ms                                                     | 41.7 ms: 1.10x slower                                                        |
| pickle_pure_python   | 195 us                                                      | 218 us: 1.11x slower                                                         |
| unpickle             | 8.18 us                                                     | 9.19 us: 1.12x slower                                                        |
| json_dumps           | 5.70 ms                                                     | 6.50 ms: 1.14x slower                                                        |
| xml_etree_iterparse  | 65.2 ms                                                     | 74.7 ms: 1.15x slower                                                        |
| pickle_dict          | 18.4 us                                                     | 21.8 us: 1.18x slower                                                        |
| unpickle_pure_python | 133 us                                                      | 159 us: 1.20x slower                                                         |
| Geometric mean       | (ref)                                                       | 1.07x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 18.2 ms: 1.07x faster                                                        |
| python_startup_no_site | 16.2 ms                                                     | 15.4 ms: 1.06x faster                                                        |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| django_template | 22.9 ms                                                     | 25.5 ms: 1.11x slower                                                        |
| mako            | 7.09 ms                                                     | 8.95 ms: 1.26x slower                                                        |
| Geometric mean  | (ref)                                                       | 1.19x slower                                                                 |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io           | 731 ms                                                      | 405 ms: 1.81x faster                                                         |
| async_tree_none         | 291 ms                                                      | 189 ms: 1.54x faster                                                         |
| async_tree_memoization  | 339 ms                                                      | 240 ms: 1.41x faster                                                         |
| async_tree_cpu_io_mixed | 489 ms                                                      | 371 ms: 1.32x faster                                                         |
| sqlite_synth            | 1.76 us                                                     | 1.35 us: 1.30x faster                                                        |
| async_generators        | 239 ms                                                      | 205 ms: 1.17x faster                                                         |
| regex_dna               | 126 ms                                                      | 110 ms: 1.15x faster                                                         |
| float                   | 56.8 ms                                                     | 49.6 ms: 1.15x faster                                                        |
| xml_etree_parse         | 93.0 ms                                                     | 82.9 ms: 1.12x faster                                                        |
| pathlib                 | 80.5 ms                                                     | 73.6 ms: 1.09x faster                                                        |
| bench_mp_pool           | 69.2 ms                                                     | 63.9 ms: 1.08x faster                                                        |
| pidigits                | 152 ms                                                      | 141 ms: 1.08x faster                                                         |
| regex_v8                | 14.2 ms                                                     | 13.2 ms: 1.08x faster                                                        |
| python_startup          | 19.5 ms                                                     | 18.2 ms: 1.07x faster                                                        |
| python_startup_no_site  | 16.2 ms                                                     | 15.4 ms: 1.06x faster                                                        |
| regex_effbot            | 1.62 ms                                                     | 1.53 ms: 1.06x faster                                                        |
| pickle                  | 7.43 us                                                     | 7.14 us: 1.04x faster                                                        |
| json                    | 3.05 ms                                                     | 2.94 ms: 1.04x faster                                                        |
| dulwich_log             | 44.3 ms                                                     | 43.6 ms: 1.02x faster                                                        |
| pickle_list             | 2.83 us                                                     | 2.81 us: 1.01x faster                                                        |
| pycparser               | 699 ms                                                      | 713 ms: 1.02x slower                                                         |
| pyflate                 | 295 ms                                                      | 302 ms: 1.02x slower                                                         |
| gc_traversal            | 1.52 ms                                                     | 1.56 ms: 1.03x slower                                                        |
| 2to3                    | 218 ms                                                      | 224 ms: 1.03x slower                                                         |
| xml_etree_generate      | 55.8 ms                                                     | 57.5 ms: 1.03x slower                                                        |
| unpickle_list           | 2.75 us                                                     | 2.86 us: 1.04x slower                                                        |
| nqueens                 | 62.8 ms                                                     | 65.6 ms: 1.04x slower                                                        |
| json_loads              | 13.9 us                                                     | 14.6 us: 1.05x slower                                                        |
| sqlglot_normalize       | 187 ms                                                      | 199 ms: 1.06x slower                                                         |
| sqlglot_optimize        | 34.5 ms                                                     | 36.8 ms: 1.06x slower                                                        |
| telco                   | 4.13 ms                                                     | 4.41 ms: 1.07x slower                                                        |
| crypto_pyaes            | 48.5 ms                                                     | 52.7 ms: 1.09x slower                                                        |
| regex_compile           | 87.5 ms                                                     | 96.4 ms: 1.10x slower                                                        |
| logging_format          | 6.72 us                                                     | 7.40 us: 1.10x slower                                                        |
| logging_simple          | 6.28 us                                                     | 6.92 us: 1.10x slower                                                        |
| xml_etree_process       | 37.7 ms                                                     | 41.7 ms: 1.10x slower                                                        |
| django_template         | 22.9 ms                                                     | 25.5 ms: 1.11x slower                                                        |
| pickle_pure_python      | 195 us                                                      | 218 us: 1.11x slower                                                         |
| go                      | 91.6 ms                                                     | 103 ms: 1.12x slower                                                         |
| unpickle                | 8.18 us                                                     | 9.19 us: 1.12x slower                                                        |
| sympy_expand            | 284 ms                                                      | 320 ms: 1.13x slower                                                         |
| scimark_sor             | 78.8 ms                                                     | 89.1 ms: 1.13x slower                                                        |
| sympy_str               | 175 ms                                                      | 198 ms: 1.13x slower                                                         |
| docutils                | 1.66 sec                                                    | 1.89 sec: 1.14x slower                                                       |
| chameleon               | 4.98 ms                                                     | 5.66 ms: 1.14x slower                                                        |
| richards                | 28.4 ms                                                     | 32.3 ms: 1.14x slower                                                        |
| deepcopy                | 238 us                                                      | 272 us: 1.14x slower                                                         |
| pprint_safe_repr        | 513 ms                                                      | 586 ms: 1.14x slower                                                         |
| json_dumps              | 5.70 ms                                                     | 6.50 ms: 1.14x slower                                                        |
| sympy_integrate         | 13.0 ms                                                     | 14.8 ms: 1.15x slower                                                        |
| xml_etree_iterparse     | 65.2 ms                                                     | 74.7 ms: 1.15x slower                                                        |
| deepcopy_reduce         | 2.09 us                                                     | 2.40 us: 1.15x slower                                                        |
| fannkuch                | 247 ms                                                      | 285 ms: 1.15x slower                                                         |
| pprint_pformat          | 1.05 sec                                                    | 1.21 sec: 1.16x slower                                                       |
| meteor_contest          | 74.6 ms                                                     | 86.5 ms: 1.16x slower                                                        |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.98 ms: 1.17x slower                                                        |
| scimark_monte_carlo     | 43.7 ms                                                     | 51.2 ms: 1.17x slower                                                        |
| spectral_norm           | 66.9 ms                                                     | 78.8 ms: 1.18x slower                                                        |
| coroutines              | 14.3 ms                                                     | 16.8 ms: 1.18x slower                                                        |
| pickle_dict             | 18.4 us                                                     | 21.8 us: 1.18x slower                                                        |
| mdp                     | 1.37 sec                                                    | 1.63 sec: 1.19x slower                                                       |
| scimark_fft             | 184 ms                                                      | 220 ms: 1.19x slower                                                         |
| sympy_sum               | 91.5 ms                                                     | 109 ms: 1.19x slower                                                         |
| unpickle_pure_python    | 133 us                                                      | 159 us: 1.20x slower                                                         |
| bench_thread_pool       | 857 us                                                      | 1.03 ms: 1.20x slower                                                        |
| hexiom                  | 4.10 ms                                                     | 4.97 ms: 1.21x slower                                                        |
| chaos                   | 43.3 ms                                                     | 53.7 ms: 1.24x slower                                                        |
| logging_silent          | 60.5 ns                                                     | 75.0 ns: 1.24x slower                                                        |
| scimark_lu              | 58.9 ms                                                     | 73.1 ms: 1.24x slower                                                        |
| deepcopy_memo           | 23.7 us                                                     | 29.5 us: 1.24x slower                                                        |
| nbody                   | 71.9 ms                                                     | 89.9 ms: 1.25x slower                                                        |
| raytrace                | 192 ms                                                      | 241 ms: 1.25x slower                                                         |
| deltablue               | 2.16 ms                                                     | 2.71 ms: 1.26x slower                                                        |
| mako                    | 7.09 ms                                                     | 8.95 ms: 1.26x slower                                                        |
| sqlglot_transpile       | 1.02 ms                                                     | 1.33 ms: 1.30x slower                                                        |
| comprehensions          | 14.1 us                                                     | 19.1 us: 1.35x slower                                                        |
| sqlglot_parse           | 804 us                                                      | 1.12 ms: 1.39x slower                                                        |
| coverage                | 40.8 ms                                                     | 59.9 ms: 1.47x slower                                                        |
| unpack_sequence         | 37.5 ns                                                     | 55.2 ns: 1.47x slower                                                        |
| generators              | 22.5 ms                                                     | 37.5 ms: 1.67x slower                                                        |
| Geometric mean          | (ref)                                                       | 1.08x slower                                                                 |

Benchmark hidden because not significant (2): create_gc_cycles, asyncio_tcp
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, dask, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20230416-3.12.0a4-1d39009/bm-20230416-pythonperf1-amd64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: unknown