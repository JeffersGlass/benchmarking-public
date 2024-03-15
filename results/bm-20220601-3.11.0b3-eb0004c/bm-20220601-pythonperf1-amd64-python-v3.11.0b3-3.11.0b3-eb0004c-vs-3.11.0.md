
# Results vs. 3.11.0

- fork: python
- ref: v3.11.0b3
- machine: windows-amd64
- commit hash: eb0004c
- commit date: 2022-06-01
- overall geometric mean: 1.04x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 212 ms: 1.01x faster                                            |
| chameleon      | 5.26 ms                                                     | 5.63 ms: 1.07x slower                                           |
| docutils       | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                          |
| html5lib       | 38.9 ms                                                     | 41.2 ms: 1.06x slower                                           |
| tornado_http   | 92.8 ms                                                     | 94.8 ms: 1.02x slower                                           |
| Geometric mean | (ref)                                                       | 1.03x slower                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io           | 808 ms                                                      | 781 ms: 1.03x faster                                            |
| async_tree_cpu_io_mixed | 530 ms                                                      | 519 ms: 1.02x faster                                            |
| async_tree_none         | 332 ms                                                      | 339 ms: 1.02x slower                                            |
| Geometric mean          | (ref)                                                       | 1.01x faster                                                    |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 71.9 ms: 1.02x slower                                           |
| pidigits       | 150 ms                                                      | 154 ms: 1.02x slower                                            |
| float          | 54.4 ms                                                     | 57.2 ms: 1.05x slower                                           |
| Geometric mean | (ref)                                                       | 1.03x slower                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 94.2 ms: 1.04x slower                                           |
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                           |
| regex_effbot   | 1.50 ms                                                     | 1.62 ms: 1.08x slower                                           |
| regex_dna      | 116 ms                                                      | 127 ms: 1.09x slower                                            |
| Geometric mean | (ref)                                                       | 1.07x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle_dict          | 18.5 us                                                     | 17.7 us: 1.04x faster                                           |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.3 ms: 1.04x faster                                           |
| json_dumps           | 8.09 ms                                                     | 7.98 ms: 1.01x faster                                           |
| unpickle_pure_python | 157 us                                                      | 158 us: 1.01x slower                                            |
| pickle_pure_python   | 208 us                                                      | 212 us: 1.02x slower                                            |
| pickle               | 6.64 us                                                     | 6.83 us: 1.03x slower                                           |
| pickle_list          | 2.70 us                                                     | 2.81 us: 1.04x slower                                           |
| xml_etree_process    | 37.2 ms                                                     | 38.9 ms: 1.05x slower                                           |
| unpickle_list        | 2.59 us                                                     | 2.71 us: 1.05x slower                                           |
| xml_etree_generate   | 52.5 ms                                                     | 55.8 ms: 1.06x slower                                           |
| json_loads           | 13.0 us                                                     | 14.2 us: 1.09x slower                                           |
| unpickle             | 7.57 us                                                     | 8.33 us: 1.10x slower                                           |
| Geometric mean       | (ref)                                                       | 1.03x slower                                                    |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 16.4 ms: 1.03x faster                                           |
| python_startup         | 19.8 ms                                                     | 19.4 ms: 1.02x faster                                           |
| Geometric mean         | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako            | 7.58 ms                                                     | 7.38 ms: 1.03x faster                                           |
| genshi_xml      | 39.9 ms                                                     | 41.0 ms: 1.03x slower                                           |
| django_template | 24.4 ms                                                     | 25.4 ms: 1.04x slower                                           |
| Geometric mean  | (ref)                                                       | 1.01x slower                                                    |

Benchmark hidden because not significant (1): genshi_text

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| unpack_sequence         | 46.9 ns                                                     | 36.8 ns: 1.27x faster                                           |
| logging_simple          | 6.86 us                                                     | 5.96 us: 1.15x faster                                           |
| logging_format          | 7.16 us                                                     | 6.43 us: 1.11x faster                                           |
| pickle_dict             | 18.5 us                                                     | 17.7 us: 1.04x faster                                           |
| create_gc_cycles        | 713 us                                                      | 686 us: 1.04x faster                                            |
| xml_etree_iterparse     | 65.6 ms                                                     | 63.3 ms: 1.04x faster                                           |
| async_tree_io           | 808 ms                                                      | 781 ms: 1.03x faster                                            |
| mako                    | 7.58 ms                                                     | 7.38 ms: 1.03x faster                                           |
| python_startup_no_site  | 16.8 ms                                                     | 16.4 ms: 1.03x faster                                           |
| richards                | 31.4 ms                                                     | 30.7 ms: 1.02x faster                                           |
| python_startup          | 19.8 ms                                                     | 19.4 ms: 1.02x faster                                           |
| async_tree_cpu_io_mixed | 530 ms                                                      | 519 ms: 1.02x faster                                            |
| dulwich_log             | 46.4 ms                                                     | 45.5 ms: 1.02x faster                                           |
| sqlite_synth            | 1.77 us                                                     | 1.74 us: 1.02x faster                                           |
| json_dumps              | 8.09 ms                                                     | 7.98 ms: 1.01x faster                                           |
| sqlalchemy_imperative   | 10.4 ms                                                     | 10.3 ms: 1.01x faster                                           |
| 2to3                    | 214 ms                                                      | 212 ms: 1.01x faster                                            |
| scimark_sor             | 78.1 ms                                                     | 77.7 ms: 1.00x faster                                           |
| unpickle_pure_python    | 157 us                                                      | 158 us: 1.01x slower                                            |
| raytrace                | 213 ms                                                      | 215 ms: 1.01x slower                                            |
| scimark_lu              | 62.8 ms                                                     | 63.6 ms: 1.01x slower                                           |
| docutils                | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                          |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                          |
| sympy_integrate         | 14.0 ms                                                     | 14.2 ms: 1.01x slower                                           |
| logging_silent          | 71.8 ns                                                     | 72.7 ns: 1.01x slower                                           |
| telco                   | 4.06 ms                                                     | 4.13 ms: 1.02x slower                                           |
| aiohttp                 | 883 us                                                      | 897 us: 1.02x slower                                            |
| pyflate                 | 312 ms                                                      | 318 ms: 1.02x slower                                            |
| pickle_pure_python      | 208 us                                                      | 212 us: 1.02x slower                                            |
| async_tree_none         | 332 ms                                                      | 339 ms: 1.02x slower                                            |
| bench_thread_pool       | 872 us                                                      | 890 us: 1.02x slower                                            |
| pycparser               | 720 ms                                                      | 735 ms: 1.02x slower                                            |
| tornado_http            | 92.8 ms                                                     | 94.8 ms: 1.02x slower                                           |
| nbody                   | 70.3 ms                                                     | 71.9 ms: 1.02x slower                                           |
| sympy_expand            | 299 ms                                                      | 306 ms: 1.02x slower                                            |
| pprint_safe_repr        | 529 ms                                                      | 541 ms: 1.02x slower                                            |
| pylint                  | 323 ms                                                      | 331 ms: 1.02x slower                                            |
| pidigits                | 150 ms                                                      | 154 ms: 1.02x slower                                            |
| sympy_str               | 185 ms                                                      | 190 ms: 1.02x slower                                            |
| genshi_xml              | 39.9 ms                                                     | 41.0 ms: 1.03x slower                                           |
| meteor_contest          | 75.2 ms                                                     | 77.1 ms: 1.03x slower                                           |
| pickle                  | 6.64 us                                                     | 6.83 us: 1.03x slower                                           |
| deltablue               | 2.70 ms                                                     | 2.78 ms: 1.03x slower                                           |
| dask                    | 273 ms                                                      | 281 ms: 1.03x slower                                            |
| go                      | 101 ms                                                      | 104 ms: 1.03x slower                                            |
| pprint_pformat          | 1.09 sec                                                    | 1.12 sec: 1.03x slower                                          |
| regex_compile           | 91.0 ms                                                     | 94.2 ms: 1.04x slower                                           |
| sqlglot_optimize        | 34.5 ms                                                     | 35.9 ms: 1.04x slower                                           |
| nqueens                 | 68.3 ms                                                     | 71.0 ms: 1.04x slower                                           |
| pathlib                 | 70.9 ms                                                     | 73.6 ms: 1.04x slower                                           |
| django_template         | 24.4 ms                                                     | 25.4 ms: 1.04x slower                                           |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.68 ms: 1.04x slower                                           |
| mdp                     | 1.59 sec                                                    | 1.66 sec: 1.04x slower                                          |
| thrift                  | 494 us                                                      | 514 us: 1.04x slower                                            |
| crypto_pyaes            | 48.9 ms                                                     | 50.9 ms: 1.04x slower                                           |
| sqlglot_normalize       | 190 ms                                                      | 198 ms: 1.04x slower                                            |
| generators              | 34.0 ms                                                     | 35.4 ms: 1.04x slower                                           |
| pickle_list             | 2.70 us                                                     | 2.81 us: 1.04x slower                                           |
| spectral_norm           | 68.3 ms                                                     | 71.4 ms: 1.05x slower                                           |
| xml_etree_process       | 37.2 ms                                                     | 38.9 ms: 1.05x slower                                           |
| coroutines              | 15.0 ms                                                     | 15.7 ms: 1.05x slower                                           |
| unpickle_list           | 2.59 us                                                     | 2.71 us: 1.05x slower                                           |
| asyncio_tcp             | 726 ms                                                      | 762 ms: 1.05x slower                                            |
| float                   | 54.4 ms                                                     | 57.2 ms: 1.05x slower                                           |
| scimark_fft             | 179 ms                                                      | 188 ms: 1.05x slower                                            |
| hexiom                  | 4.55 ms                                                     | 4.82 ms: 1.06x slower                                           |
| html5lib                | 38.9 ms                                                     | 41.2 ms: 1.06x slower                                           |
| bench_mp_pool           | 63.2 ms                                                     | 67.0 ms: 1.06x slower                                           |
| xml_etree_generate      | 52.5 ms                                                     | 55.8 ms: 1.06x slower                                           |
| chameleon               | 5.26 ms                                                     | 5.63 ms: 1.07x slower                                           |
| chaos                   | 48.4 ms                                                     | 51.8 ms: 1.07x slower                                           |
| regex_v8                | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                           |
| deepcopy                | 246 us                                                      | 265 us: 1.07x slower                                            |
| deepcopy_reduce         | 2.06 us                                                     | 2.22 us: 1.08x slower                                           |
| regex_effbot            | 1.50 ms                                                     | 1.62 ms: 1.08x slower                                           |
| async_generators        | 177 ms                                                      | 192 ms: 1.08x slower                                            |
| json_loads              | 13.0 us                                                     | 14.2 us: 1.09x slower                                           |
| regex_dna               | 116 ms                                                      | 127 ms: 1.09x slower                                            |
| fannkuch                | 253 ms                                                      | 278 ms: 1.10x slower                                            |
| json                    | 2.98 ms                                                     | 3.26 ms: 1.10x slower                                           |
| unpickle                | 7.57 us                                                     | 8.33 us: 1.10x slower                                           |
| comprehensions          | 15.6 us                                                     | 18.7 us: 1.20x slower                                           |
| sqlglot_transpile       | 1.16 ms                                                     | 1.41 ms: 1.21x slower                                           |
| sqlglot_parse           | 953 us                                                      | 1.21 ms: 1.27x slower                                           |
| coverage                | 43.4 ms                                                     | 108 ms: 2.48x slower                                            |
| Geometric mean          | (ref)                                                       | 1.04x slower                                                    |

Benchmark hidden because not significant (8): gc_traversal, xml_etree_parse, deepcopy_memo, scimark_monte_carlo, sympy_sum, sqlalchemy_declarative, genshi_text, async_tree_memoization
Ignored benchmarks (9) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: unknown