
# Results vs. 3.12.0

- fork: python
- ref: v3.11.0b3
- machine: windows-amd64
- commit hash: eb0004c
- commit date: 2022-06-01
- overall geometric mean: 1.08x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 212 ms: 1.03x faster                                            |
| chameleon      | 4.98 ms                                                     | 5.63 ms: 1.13x slower                                           |
| tornado_http   | 89.5 ms                                                     | 94.8 ms: 1.06x slower                                           |
| Geometric mean | (ref)                                                       | 1.04x slower                                                    |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 519 ms: 1.06x slower                                            |
| async_tree_io           | 731 ms                                                      | 781 ms: 1.07x slower                                            |
| async_tree_none         | 291 ms                                                      | 339 ms: 1.16x slower                                            |
| async_tree_memoization  | 339 ms                                                      | 402 ms: 1.19x slower                                            |
| Geometric mean          | (ref)                                                       | 1.12x slower                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 154 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                       | 1.01x slower                                                    |

Benchmark hidden because not significant (2): nbody, float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                           |
| regex_compile  | 87.5 ms                                                     | 94.2 ms: 1.08x slower                                           |
| Geometric mean | (ref)                                                       | 1.04x slower                                                    |

Benchmark hidden because not significant (2): regex_effbot, regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.83 us: 1.09x faster                                           |
| pickle_dict          | 18.4 us                                                     | 17.7 us: 1.04x faster                                           |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.3 ms: 1.03x faster                                           |
| unpickle_list        | 2.75 us                                                     | 2.71 us: 1.01x faster                                           |
| pickle_list          | 2.83 us                                                     | 2.81 us: 1.00x faster                                           |
| unpickle             | 8.18 us                                                     | 8.33 us: 1.02x slower                                           |
| json_loads           | 13.9 us                                                     | 14.2 us: 1.02x slower                                           |
| xml_etree_process    | 37.7 ms                                                     | 38.9 ms: 1.03x slower                                           |
| xml_etree_parse      | 93.0 ms                                                     | 97.4 ms: 1.05x slower                                           |
| pickle_pure_python   | 195 us                                                      | 212 us: 1.09x slower                                            |
| unpickle_pure_python | 133 us                                                      | 158 us: 1.19x slower                                            |
| json_dumps           | 5.70 ms                                                     | 7.98 ms: 1.40x slower                                           |
| Geometric mean       | (ref)                                                       | 1.04x slower                                                    |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 16.4 ms: 1.01x slower                                           |
| Geometric mean         | (ref)                                                       | 1.00x slower                                                    |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 7.38 ms: 1.04x slower                                           |
| django_template | 22.9 ms                                                     | 25.4 ms: 1.11x slower                                           |
| Geometric mean  | (ref)                                                       | 1.07x slower                                                    |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_generators        | 239 ms                                                      | 192 ms: 1.25x faster                                            |
| create_gc_cycles        | 752 us                                                      | 686 us: 1.10x faster                                            |
| pathlib                 | 80.5 ms                                                     | 73.6 ms: 1.09x faster                                           |
| pickle                  | 7.43 us                                                     | 6.83 us: 1.09x faster                                           |
| logging_simple          | 6.28 us                                                     | 5.96 us: 1.05x faster                                           |
| logging_format          | 6.72 us                                                     | 6.43 us: 1.05x faster                                           |
| pickle_dict             | 18.4 us                                                     | 17.7 us: 1.04x faster                                           |
| bench_mp_pool           | 69.2 ms                                                     | 67.0 ms: 1.03x faster                                           |
| xml_etree_iterparse     | 65.2 ms                                                     | 63.3 ms: 1.03x faster                                           |
| 2to3                    | 218 ms                                                      | 212 ms: 1.03x faster                                            |
| gc_traversal            | 1.52 ms                                                     | 1.49 ms: 1.02x faster                                           |
| unpack_sequence         | 37.5 ns                                                     | 36.8 ns: 1.02x faster                                           |
| unpickle_list           | 2.75 us                                                     | 2.71 us: 1.01x faster                                           |
| scimark_sor             | 78.8 ms                                                     | 77.7 ms: 1.01x faster                                           |
| sqlite_synth            | 1.76 us                                                     | 1.74 us: 1.01x faster                                           |
| pickle_list             | 2.83 us                                                     | 2.81 us: 1.00x faster                                           |
| pidigits                | 152 ms                                                      | 154 ms: 1.01x slower                                            |
| python_startup_no_site  | 16.2 ms                                                     | 16.4 ms: 1.01x slower                                           |
| aiohttp                 | 884 us                                                      | 897 us: 1.01x slower                                            |
| unpickle                | 8.18 us                                                     | 8.33 us: 1.02x slower                                           |
| json_loads              | 13.9 us                                                     | 14.2 us: 1.02x slower                                           |
| scimark_fft             | 184 ms                                                      | 188 ms: 1.02x slower                                            |
| dulwich_log             | 44.3 ms                                                     | 45.5 ms: 1.03x slower                                           |
| xml_etree_process       | 37.7 ms                                                     | 38.9 ms: 1.03x slower                                           |
| meteor_contest          | 74.6 ms                                                     | 77.1 ms: 1.03x slower                                           |
| sqlglot_optimize        | 34.5 ms                                                     | 35.9 ms: 1.04x slower                                           |
| scimark_monte_carlo     | 43.7 ms                                                     | 45.4 ms: 1.04x slower                                           |
| bench_thread_pool       | 857 us                                                      | 890 us: 1.04x slower                                            |
| mako                    | 7.09 ms                                                     | 7.38 ms: 1.04x slower                                           |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.68 ms: 1.05x slower                                           |
| xml_etree_parse         | 93.0 ms                                                     | 97.4 ms: 1.05x slower                                           |
| crypto_pyaes            | 48.5 ms                                                     | 50.9 ms: 1.05x slower                                           |
| pycparser               | 699 ms                                                      | 735 ms: 1.05x slower                                            |
| pprint_safe_repr        | 513 ms                                                      | 541 ms: 1.06x slower                                            |
| tornado_http            | 89.5 ms                                                     | 94.8 ms: 1.06x slower                                           |
| sqlglot_normalize       | 187 ms                                                      | 198 ms: 1.06x slower                                            |
| deepcopy_reduce         | 2.09 us                                                     | 2.22 us: 1.06x slower                                           |
| async_tree_cpu_io_mixed | 489 ms                                                      | 519 ms: 1.06x slower                                            |
| regex_v8                | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                           |
| spectral_norm           | 66.9 ms                                                     | 71.4 ms: 1.07x slower                                           |
| async_tree_io           | 731 ms                                                      | 781 ms: 1.07x slower                                            |
| dask                    | 263 ms                                                      | 281 ms: 1.07x slower                                            |
| json                    | 3.05 ms                                                     | 3.26 ms: 1.07x slower                                           |
| pprint_pformat          | 1.05 sec                                                    | 1.12 sec: 1.08x slower                                          |
| regex_compile           | 87.5 ms                                                     | 94.2 ms: 1.08x slower                                           |
| sympy_expand            | 284 ms                                                      | 306 ms: 1.08x slower                                            |
| pyflate                 | 295 ms                                                      | 318 ms: 1.08x slower                                            |
| scimark_lu              | 58.9 ms                                                     | 63.6 ms: 1.08x slower                                           |
| richards                | 28.4 ms                                                     | 30.7 ms: 1.08x slower                                           |
| sympy_str               | 175 ms                                                      | 190 ms: 1.08x slower                                            |
| pickle_pure_python      | 195 us                                                      | 212 us: 1.09x slower                                            |
| sympy_sum               | 91.5 ms                                                     | 100 ms: 1.10x slower                                            |
| deepcopy_memo           | 23.7 us                                                     | 26.0 us: 1.10x slower                                           |
| coroutines              | 14.3 ms                                                     | 15.7 ms: 1.10x slower                                           |
| sympy_integrate         | 13.0 ms                                                     | 14.2 ms: 1.10x slower                                           |
| django_template         | 22.9 ms                                                     | 25.4 ms: 1.11x slower                                           |
| sqlalchemy_imperative   | 9.29 ms                                                     | 10.3 ms: 1.11x slower                                           |
| deepcopy                | 238 us                                                      | 265 us: 1.11x slower                                            |
| raytrace                | 192 ms                                                      | 215 ms: 1.12x slower                                            |
| fannkuch                | 247 ms                                                      | 278 ms: 1.13x slower                                            |
| nqueens                 | 62.8 ms                                                     | 71.0 ms: 1.13x slower                                           |
| chameleon               | 4.98 ms                                                     | 5.63 ms: 1.13x slower                                           |
| go                      | 91.6 ms                                                     | 104 ms: 1.14x slower                                            |
| async_tree_none         | 291 ms                                                      | 339 ms: 1.16x slower                                            |
| hexiom                  | 4.10 ms                                                     | 4.82 ms: 1.18x slower                                           |
| unpickle_pure_python    | 133 us                                                      | 158 us: 1.19x slower                                            |
| async_tree_memoization  | 339 ms                                                      | 402 ms: 1.19x slower                                            |
| chaos                   | 43.3 ms                                                     | 51.8 ms: 1.19x slower                                           |
| logging_silent          | 60.5 ns                                                     | 72.7 ns: 1.20x slower                                           |
| mdp                     | 1.37 sec                                                    | 1.66 sec: 1.21x slower                                          |
| deltablue               | 2.16 ms                                                     | 2.78 ms: 1.29x slower                                           |
| comprehensions          | 14.1 us                                                     | 18.7 us: 1.33x slower                                           |
| sqlglot_transpile       | 1.02 ms                                                     | 1.41 ms: 1.38x slower                                           |
| json_dumps              | 5.70 ms                                                     | 7.98 ms: 1.40x slower                                           |
| sqlglot_parse           | 804 us                                                      | 1.21 ms: 1.50x slower                                           |
| asyncio_tcp             | 487 ms                                                      | 762 ms: 1.56x slower                                            |
| generators              | 22.5 ms                                                     | 35.4 ms: 1.57x slower                                           |
| coverage                | 40.8 ms                                                     | 108 ms: 2.64x slower                                            |
| Geometric mean          | (ref)                                                       | 1.08x slower                                                    |

Benchmark hidden because not significant (9): python_startup, sqlalchemy_declarative, regex_effbot, xml_etree_generate, nbody, telco, docutils, regex_dna, float
Ignored benchmarks (9) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20220601-3.11.0b3-eb0004c/bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: unknown