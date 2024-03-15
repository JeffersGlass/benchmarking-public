
# Results vs. 3.12.0

- fork: python
- ref: v3.11.0b3
- machine: linux-x86_64
- commit hash: eb0004c
- commit date: 2022-06-01
- overall geometric mean: 1.05x slower \*
- HPT reliability: 99.97%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 284 ms: 1.00x faster                                             |
| chameleon      | 7.23 ms                                                      | 7.60 ms: 1.05x slower                                            |
| docutils       | 2.87 sec                                                     | 2.83 sec: 1.01x faster                                           |
| tornado_http   | 121 ms                                                       | 119 ms: 1.02x faster                                             |
| Geometric mean | (ref)                                                        | 1.00x slower                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                           |
| async_tree_memoization  | 544 ms                                                       | 617 ms: 1.13x slower                                             |
| async_tree_none         | 452 ms                                                       | 513 ms: 1.14x slower                                             |
| async_tree_cpu_io_mixed | 696 ms                                                       | 810 ms: 1.16x slower                                             |
| Geometric mean          | (ref)                                                        | 1.14x slower                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 252 ms: 1.05x faster                                             |
| float          | 76.6 ms                                                      | 73.9 ms: 1.04x faster                                            |
| nbody          | 88.0 ms                                                      | 93.0 ms: 1.06x slower                                            |
| Geometric mean | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.05 ms: 1.17x faster                                            |
| regex_dna      | 239 ms                                                       | 219 ms: 1.09x faster                                             |
| regex_v8       | 23.6 ms                                                      | 24.3 ms: 1.03x slower                                            |
| regex_compile  | 144 ms                                                       | 156 ms: 1.08x slower                                             |
| Geometric mean | (ref)                                                        | 1.03x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.92 us: 1.13x faster                                            |
| unpickle             | 14.8 us                                                      | 13.2 us: 1.12x faster                                            |
| pickle               | 10.5 us                                                      | 9.80 us: 1.07x faster                                            |
| xml_etree_generate   | 86.1 ms                                                      | 80.2 ms: 1.07x faster                                            |
| xml_etree_process    | 58.4 ms                                                      | 55.9 ms: 1.04x faster                                            |
| pickle_dict          | 32.5 us                                                      | 31.3 us: 1.04x faster                                            |
| unpickle_list        | 4.66 us                                                      | 4.58 us: 1.02x faster                                            |
| json_loads           | 24.4 us                                                      | 25.2 us: 1.03x slower                                            |
| xml_etree_parse      | 144 ms                                                       | 153 ms: 1.07x slower                                             |
| unpickle_pure_python | 210 us                                                       | 238 us: 1.14x slower                                             |
| json_dumps           | 10.2 ms                                                      | 13.5 ms: 1.32x slower                                            |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                     |

Benchmark hidden because not significant (2): pickle_pure_python, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.70 ms: 1.12x faster                                            |
| python_startup         | 11.6 ms                                                      | 10.7 ms: 1.09x faster                                            |
| Geometric mean         | (ref)                                                        | 1.11x faster                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 41.4 ms: 1.08x slower                                            |
| mako            | 10.0 ms                                                      | 10.9 ms: 1.09x slower                                            |
| Geometric mean  | (ref)                                                        | 1.09x slower                                                     |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_generators        | 390 ms                                                       | 318 ms: 1.23x faster                                             |
| regex_effbot            | 3.57 ms                                                      | 3.05 ms: 1.17x faster                                            |
| unpack_sequence         | 53.2 ns                                                      | 45.4 ns: 1.17x faster                                            |
| pickle_list             | 4.43 us                                                      | 3.92 us: 1.13x faster                                            |
| python_startup_no_site  | 8.64 ms                                                      | 7.70 ms: 1.12x faster                                            |
| unpickle                | 14.8 us                                                      | 13.2 us: 1.12x faster                                            |
| sqlite_synth            | 2.77 us                                                      | 2.51 us: 1.10x faster                                            |
| python_startup          | 11.6 ms                                                      | 10.7 ms: 1.09x faster                                            |
| regex_dna               | 239 ms                                                       | 219 ms: 1.09x faster                                             |
| gunicorn                | 1.00 ms                                                      | 931 us: 1.07x faster                                             |
| pickle                  | 10.5 us                                                      | 9.80 us: 1.07x faster                                            |
| xml_etree_generate      | 86.1 ms                                                      | 80.2 ms: 1.07x faster                                            |
| aiohttp                 | 1.02 ms                                                      | 958 us: 1.06x faster                                             |
| bench_mp_pool           | 4.76 ms                                                      | 4.52 ms: 1.05x faster                                            |
| pidigits                | 265 ms                                                       | 252 ms: 1.05x faster                                             |
| scimark_fft             | 301 ms                                                       | 286 ms: 1.05x faster                                             |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 4.03 ms: 1.04x faster                                            |
| xml_etree_process       | 58.4 ms                                                      | 55.9 ms: 1.04x faster                                            |
| pprint_safe_repr        | 807 ms                                                       | 774 ms: 1.04x faster                                             |
| pickle_dict             | 32.5 us                                                      | 31.3 us: 1.04x faster                                            |
| float                   | 76.6 ms                                                      | 73.9 ms: 1.04x faster                                            |
| sqlalchemy_declarative  | 159 ms                                                       | 154 ms: 1.03x faster                                             |
| telco                   | 6.96 ms                                                      | 6.75 ms: 1.03x faster                                            |
| pprint_pformat          | 1.65 sec                                                     | 1.61 sec: 1.03x faster                                           |
| tornado_http            | 121 ms                                                       | 119 ms: 1.02x faster                                             |
| unpickle_list           | 4.66 us                                                      | 4.58 us: 1.02x faster                                            |
| docutils                | 2.87 sec                                                     | 2.83 sec: 1.01x faster                                           |
| 2to3                    | 285 ms                                                       | 284 ms: 1.00x faster                                             |
| pyflate                 | 439 ms                                                       | 441 ms: 1.01x slower                                             |
| scimark_monte_carlo     | 69.0 ms                                                      | 69.5 ms: 1.01x slower                                            |
| pathlib                 | 18.9 ms                                                      | 19.2 ms: 1.01x slower                                            |
| json                    | 5.12 ms                                                      | 5.20 ms: 1.02x slower                                            |
| raytrace                | 298 ms                                                       | 304 ms: 1.02x slower                                             |
| meteor_contest          | 128 ms                                                       | 131 ms: 1.02x slower                                             |
| deepcopy_memo           | 36.8 us                                                      | 37.7 us: 1.02x slower                                            |
| scimark_sor             | 109 ms                                                       | 112 ms: 1.03x slower                                             |
| regex_v8                | 23.6 ms                                                      | 24.3 ms: 1.03x slower                                            |
| deepcopy_reduce         | 3.37 us                                                      | 3.48 us: 1.03x slower                                            |
| sqlglot_optimize        | 57.5 ms                                                      | 59.4 ms: 1.03x slower                                            |
| json_loads              | 24.4 us                                                      | 25.2 us: 1.03x slower                                            |
| sqlalchemy_imperative   | 18.7 ms                                                      | 19.6 ms: 1.04x slower                                            |
| dulwich_log             | 65.4 ms                                                      | 68.4 ms: 1.05x slower                                            |
| chameleon               | 7.23 ms                                                      | 7.60 ms: 1.05x slower                                            |
| crypto_pyaes            | 80.3 ms                                                      | 84.5 ms: 1.05x slower                                            |
| logging_silent          | 94.4 ns                                                      | 99.3 ns: 1.05x slower                                            |
| sympy_integrate         | 23.9 ms                                                      | 25.2 ms: 1.05x slower                                            |
| dask                    | 392 ms                                                       | 414 ms: 1.06x slower                                             |
| create_gc_cycles        | 1.59 ms                                                      | 1.68 ms: 1.06x slower                                            |
| spectral_norm           | 91.6 ms                                                      | 96.8 ms: 1.06x slower                                            |
| nbody                   | 88.0 ms                                                      | 93.0 ms: 1.06x slower                                            |
| pycparser               | 1.23 sec                                                     | 1.31 sec: 1.06x slower                                           |
| deepcopy                | 368 us                                                       | 390 us: 1.06x slower                                             |
| logging_format          | 7.48 us                                                      | 7.95 us: 1.06x slower                                            |
| sqlglot_normalize       | 116 ms                                                       | 123 ms: 1.07x slower                                             |
| xml_etree_parse         | 144 ms                                                       | 153 ms: 1.07x slower                                             |
| logging_simple          | 6.71 us                                                      | 7.16 us: 1.07x slower                                            |
| bench_thread_pool       | 950 us                                                       | 1.01 ms: 1.07x slower                                            |
| richards                | 45.7 ms                                                      | 49.2 ms: 1.07x slower                                            |
| sympy_str               | 302 ms                                                       | 327 ms: 1.08x slower                                             |
| regex_compile           | 144 ms                                                       | 156 ms: 1.08x slower                                             |
| django_template         | 38.2 ms                                                      | 41.4 ms: 1.08x slower                                            |
| nqueens                 | 89.9 ms                                                      | 97.6 ms: 1.09x slower                                            |
| sympy_sum               | 162 ms                                                       | 177 ms: 1.09x slower                                             |
| mako                    | 10.0 ms                                                      | 10.9 ms: 1.09x slower                                            |
| mdp                     | 2.57 sec                                                     | 2.81 sec: 1.09x slower                                           |
| sympy_expand            | 484 ms                                                       | 531 ms: 1.10x slower                                             |
| go                      | 150 ms                                                       | 166 ms: 1.11x slower                                             |
| scimark_lu              | 98.8 ms                                                      | 110 ms: 1.11x slower                                             |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                           |
| async_tree_memoization  | 544 ms                                                       | 617 ms: 1.13x slower                                             |
| async_tree_none         | 452 ms                                                       | 513 ms: 1.14x slower                                             |
| unpickle_pure_python    | 210 us                                                       | 238 us: 1.14x slower                                             |
| chaos                   | 64.0 ms                                                      | 73.6 ms: 1.15x slower                                            |
| gc_traversal            | 3.48 ms                                                      | 4.03 ms: 1.16x slower                                            |
| async_tree_cpu_io_mixed | 696 ms                                                       | 810 ms: 1.16x slower                                             |
| hexiom                  | 5.96 ms                                                      | 7.00 ms: 1.17x slower                                            |
| coroutines              | 23.0 ms                                                      | 27.9 ms: 1.21x slower                                            |
| comprehensions          | 21.9 us                                                      | 28.3 us: 1.29x slower                                            |
| deltablue               | 3.24 ms                                                      | 4.20 ms: 1.30x slower                                            |
| sqlglot_transpile       | 1.78 ms                                                      | 2.32 ms: 1.31x slower                                            |
| json_dumps              | 10.2 ms                                                      | 13.5 ms: 1.32x slower                                            |
| fannkuch                | 350 ms                                                       | 496 ms: 1.42x slower                                             |
| sqlglot_parse           | 1.38 ms                                                      | 1.97 ms: 1.43x slower                                            |
| generators              | 37.4 ms                                                      | 56.0 ms: 1.50x slower                                            |
| asyncio_tcp             | 378 ms                                                       | 751 ms: 1.99x slower                                             |
| Geometric mean          | (ref)                                                        | 1.05x slower                                                     |

Benchmark hidden because not significant (2): pickle_pure_python, xml_etree_iterparse
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20220601-3.11.0b3-eb0004c/bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.97% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.90x