
# Results vs. 3.12.0

- fork: python
- ref: f9774e57d84162ff0cba
- machine: linux-x86_64
- commit hash: f9774e5
- commit date: 2023-03-07
- overall geometric mean: 1.01x slower \*
- HPT reliability: 85.47%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 284 ms: 1.00x faster                                                        |
| chameleon      | 7.23 ms                                                      | 6.94 ms: 1.04x faster                                                       |
| docutils       | 2.87 sec                                                     | 2.79 sec: 1.03x faster                                                      |
| tornado_http   | 121 ms                                                       | 115 ms: 1.05x faster                                                        |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 745 ms: 1.07x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                                      |
| async_tree_memoization  | 544 ms                                                       | 611 ms: 1.12x slower                                                        |
| async_tree_none         | 452 ms                                                       | 510 ms: 1.13x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.11x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 251 ms: 1.06x faster                                                        |
| float          | 76.6 ms                                                      | 73.9 ms: 1.04x faster                                                       |
| nbody          | 88.0 ms                                                      | 91.0 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.36 ms: 1.06x faster                                                       |
| regex_dna      | 239 ms                                                       | 225 ms: 1.06x faster                                                        |
| regex_v8       | 23.6 ms                                                      | 22.8 ms: 1.04x faster                                                       |
| regex_compile  | 144 ms                                                       | 146 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                        | 1.04x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.80 us: 1.17x faster                                                       |
| unpickle             | 14.8 us                                                      | 13.4 us: 1.10x faster                                                       |
| pickle               | 10.5 us                                                      | 10.0 us: 1.05x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.44 us: 1.05x faster                                                       |
| pickle_pure_python   | 318 us                                                       | 306 us: 1.04x faster                                                        |
| unpickle_pure_python | 210 us                                                       | 202 us: 1.04x faster                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 83.5 ms: 1.03x faster                                                       |
| pickle_dict          | 32.5 us                                                      | 31.8 us: 1.02x faster                                                       |
| xml_etree_process    | 58.4 ms                                                      | 57.3 ms: 1.02x faster                                                       |
| json_dumps           | 10.2 ms                                                      | 10.2 ms: 1.00x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.04x faster                                                                |

Benchmark hidden because not significant (3): xml_etree_parse, json_loads, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 8.34 ms: 1.04x faster                                                       |
| python_startup         | 11.6 ms                                                      | 11.3 ms: 1.03x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.03x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 39.1 ms: 1.03x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.01x slower                                                                |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpack_sequence         | 53.2 ns                                                      | 44.4 ns: 1.20x faster                                                       |
| pickle_list             | 4.43 us                                                      | 3.80 us: 1.17x faster                                                       |
| unpickle                | 14.8 us                                                      | 13.4 us: 1.10x faster                                                       |
| scimark_fft             | 301 ms                                                       | 278 ms: 1.08x faster                                                        |
| pprint_pformat          | 1.65 sec                                                     | 1.55 sec: 1.06x faster                                                      |
| regex_effbot            | 3.57 ms                                                      | 3.36 ms: 1.06x faster                                                       |
| regex_dna               | 239 ms                                                       | 225 ms: 1.06x faster                                                        |
| pprint_safe_repr        | 807 ms                                                       | 762 ms: 1.06x faster                                                        |
| sqlite_synth            | 2.77 us                                                      | 2.63 us: 1.06x faster                                                       |
| pidigits                | 265 ms                                                       | 251 ms: 1.06x faster                                                        |
| tornado_http            | 121 ms                                                       | 115 ms: 1.05x faster                                                        |
| pickle                  | 10.5 us                                                      | 10.0 us: 1.05x faster                                                       |
| unpickle_list           | 4.66 us                                                      | 4.44 us: 1.05x faster                                                       |
| chameleon               | 7.23 ms                                                      | 6.94 ms: 1.04x faster                                                       |
| pickle_pure_python      | 318 us                                                       | 306 us: 1.04x faster                                                        |
| deepcopy_memo           | 36.8 us                                                      | 35.4 us: 1.04x faster                                                       |
| regex_v8                | 23.6 ms                                                      | 22.8 ms: 1.04x faster                                                       |
| scimark_sor             | 109 ms                                                       | 105 ms: 1.04x faster                                                        |
| float                   | 76.6 ms                                                      | 73.9 ms: 1.04x faster                                                       |
| unpickle_pure_python    | 210 us                                                       | 202 us: 1.04x faster                                                        |
| python_startup_no_site  | 8.64 ms                                                      | 8.34 ms: 1.04x faster                                                       |
| python_startup          | 11.6 ms                                                      | 11.3 ms: 1.03x faster                                                       |
| xml_etree_generate      | 86.1 ms                                                      | 83.5 ms: 1.03x faster                                                       |
| raytrace                | 298 ms                                                       | 290 ms: 1.03x faster                                                        |
| docutils                | 2.87 sec                                                     | 2.79 sec: 1.03x faster                                                      |
| dulwich_log             | 65.4 ms                                                      | 63.7 ms: 1.03x faster                                                       |
| json                    | 5.12 ms                                                      | 5.00 ms: 1.02x faster                                                       |
| pickle_dict             | 32.5 us                                                      | 31.8 us: 1.02x faster                                                       |
| xml_etree_process       | 58.4 ms                                                      | 57.3 ms: 1.02x faster                                                       |
| pathlib                 | 18.9 ms                                                      | 18.5 ms: 1.02x faster                                                       |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 4.14 ms: 1.02x faster                                                       |
| pyflate                 | 439 ms                                                       | 432 ms: 1.02x faster                                                        |
| async_generators        | 390 ms                                                       | 385 ms: 1.01x faster                                                        |
| deepcopy_reduce         | 3.37 us                                                      | 3.33 us: 1.01x faster                                                       |
| mdp                     | 2.57 sec                                                     | 2.54 sec: 1.01x faster                                                      |
| telco                   | 6.96 ms                                                      | 6.90 ms: 1.01x faster                                                       |
| 2to3                    | 285 ms                                                       | 284 ms: 1.00x faster                                                        |
| json_dumps              | 10.2 ms                                                      | 10.2 ms: 1.00x slower                                                       |
| meteor_contest          | 128 ms                                                       | 128 ms: 1.00x slower                                                        |
| go                      | 150 ms                                                       | 151 ms: 1.01x slower                                                        |
| scimark_monte_carlo     | 69.0 ms                                                      | 69.5 ms: 1.01x slower                                                       |
| asyncio_tcp             | 378 ms                                                       | 382 ms: 1.01x slower                                                        |
| logging_simple          | 6.71 us                                                      | 6.79 us: 1.01x slower                                                       |
| sqlglot_optimize        | 57.5 ms                                                      | 58.2 ms: 1.01x slower                                                       |
| regex_compile           | 144 ms                                                       | 146 ms: 1.01x slower                                                        |
| logging_format          | 7.48 us                                                      | 7.59 us: 1.01x slower                                                       |
| crypto_pyaes            | 80.3 ms                                                      | 81.5 ms: 1.01x slower                                                       |
| richards                | 45.7 ms                                                      | 46.4 ms: 1.01x slower                                                       |
| deepcopy                | 368 us                                                       | 377 us: 1.02x slower                                                        |
| create_gc_cycles        | 1.59 ms                                                      | 1.63 ms: 1.02x slower                                                       |
| django_template         | 38.2 ms                                                      | 39.1 ms: 1.03x slower                                                       |
| bench_thread_pool       | 950 us                                                       | 974 us: 1.03x slower                                                        |
| generators              | 37.4 ms                                                      | 38.4 ms: 1.03x slower                                                       |
| deltablue               | 3.24 ms                                                      | 3.33 ms: 1.03x slower                                                       |
| nbody                   | 88.0 ms                                                      | 91.0 ms: 1.03x slower                                                       |
| sqlglot_normalize       | 116 ms                                                       | 120 ms: 1.04x slower                                                        |
| spectral_norm           | 91.6 ms                                                      | 95.6 ms: 1.04x slower                                                       |
| sympy_integrate         | 23.9 ms                                                      | 25.0 ms: 1.04x slower                                                       |
| scimark_lu              | 98.8 ms                                                      | 105 ms: 1.06x slower                                                        |
| async_tree_cpu_io_mixed | 696 ms                                                       | 745 ms: 1.07x slower                                                        |
| coroutines              | 23.0 ms                                                      | 24.7 ms: 1.07x slower                                                       |
| nqueens                 | 89.9 ms                                                      | 96.9 ms: 1.08x slower                                                       |
| hexiom                  | 5.96 ms                                                      | 6.46 ms: 1.08x slower                                                       |
| sympy_str               | 302 ms                                                       | 328 ms: 1.09x slower                                                        |
| sqlglot_transpile       | 1.78 ms                                                      | 1.94 ms: 1.09x slower                                                       |
| chaos                   | 64.0 ms                                                      | 70.9 ms: 1.11x slower                                                       |
| sympy_expand            | 484 ms                                                       | 538 ms: 1.11x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                                      |
| async_tree_memoization  | 544 ms                                                       | 611 ms: 1.12x slower                                                        |
| async_tree_none         | 452 ms                                                       | 510 ms: 1.13x slower                                                        |
| sympy_sum               | 162 ms                                                       | 184 ms: 1.14x slower                                                        |
| sqlglot_parse           | 1.38 ms                                                      | 1.58 ms: 1.15x slower                                                       |
| gc_traversal            | 3.48 ms                                                      | 3.99 ms: 1.15x slower                                                       |
| fannkuch                | 350 ms                                                       | 408 ms: 1.16x slower                                                        |
| comprehensions          | 21.9 us                                                      | 26.7 us: 1.22x slower                                                       |
| coverage                | 66.7 ms                                                      | 82.2 ms: 1.23x slower                                                       |
| dask                    | 392 ms                                                       | 560 ms: 1.43x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.01x slower                                                                |

Benchmark hidden because not significant (7): pycparser, logging_silent, xml_etree_parse, json_loads, mako, xml_etree_iterparse, bench_mp_pool
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20230307-3.12.0a6-f9774e5/bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 85.47% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x