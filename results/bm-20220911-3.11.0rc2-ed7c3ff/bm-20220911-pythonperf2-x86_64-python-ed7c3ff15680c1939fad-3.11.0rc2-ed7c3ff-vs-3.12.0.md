
# Results vs. 3.12.0

- fork: python
- ref: ed7c3ff15680c1939fad
- machine: linux-x86_64
- commit hash: ed7c3ff
- commit date: 2022-09-11
- overall geometric mean: 1.05x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 287 ms: 1.01x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.50 ms: 1.04x slower                                                        |
| tornado_http   | 121 ms                                                       | 125 ms: 1.03x slower                                                         |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 746 ms: 1.07x slower                                                         |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.13x slower                                                       |
| async_tree_none         | 452 ms                                                       | 517 ms: 1.14x slower                                                         |
| async_tree_memoization  | 544 ms                                                       | 636 ms: 1.17x slower                                                         |
| Geometric mean          | (ref)                                                        | 1.13x slower                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 251 ms: 1.05x faster                                                         |
| float          | 76.6 ms                                                      | 75.1 ms: 1.02x faster                                                        |
| nbody          | 88.0 ms                                                      | 89.6 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.29 ms: 1.08x faster                                                        |
| regex_dna      | 239 ms                                                       | 225 ms: 1.06x faster                                                         |
| regex_v8       | 23.6 ms                                                      | 24.3 ms: 1.03x slower                                                        |
| regex_compile  | 144 ms                                                       | 157 ms: 1.09x slower                                                         |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.77 us: 1.18x faster                                                        |
| unpickle             | 14.8 us                                                      | 13.0 us: 1.14x faster                                                        |
| pickle               | 10.5 us                                                      | 9.61 us: 1.10x faster                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 80.8 ms: 1.07x faster                                                        |
| pickle_dict          | 32.5 us                                                      | 30.7 us: 1.06x faster                                                        |
| xml_etree_process    | 58.4 ms                                                      | 57.0 ms: 1.02x faster                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 104 ms: 1.01x slower                                                         |
| pickle_pure_python   | 318 us                                                       | 324 us: 1.02x slower                                                         |
| xml_etree_parse      | 144 ms                                                       | 160 ms: 1.11x slower                                                         |
| json_loads           | 24.4 us                                                      | 28.4 us: 1.17x slower                                                        |
| unpickle_pure_python | 210 us                                                       | 250 us: 1.19x slower                                                         |
| json_dumps           | 10.2 ms                                                      | 13.5 ms: 1.32x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.72 ms: 1.12x faster                                                        |
| python_startup         | 11.6 ms                                                      | 10.7 ms: 1.09x faster                                                        |
| Geometric mean         | (ref)                                                        | 1.10x faster                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 39.7 ms: 1.04x slower                                                        |
| mako            | 10.0 ms                                                      | 10.9 ms: 1.09x slower                                                        |
| Geometric mean  | (ref)                                                        | 1.06x slower                                                                 |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_generators        | 390 ms                                                       | 328 ms: 1.19x faster                                                         |
| pickle_list             | 4.43 us                                                      | 3.77 us: 1.18x faster                                                        |
| unpack_sequence         | 53.2 ns                                                      | 45.7 ns: 1.16x faster                                                        |
| unpickle                | 14.8 us                                                      | 13.0 us: 1.14x faster                                                        |
| python_startup_no_site  | 8.64 ms                                                      | 7.72 ms: 1.12x faster                                                        |
| sqlite_synth            | 2.77 us                                                      | 2.48 us: 1.12x faster                                                        |
| pickle                  | 10.5 us                                                      | 9.61 us: 1.10x faster                                                        |
| python_startup          | 11.6 ms                                                      | 10.7 ms: 1.09x faster                                                        |
| scimark_fft             | 301 ms                                                       | 277 ms: 1.09x faster                                                         |
| regex_effbot            | 3.57 ms                                                      | 3.29 ms: 1.08x faster                                                        |
| xml_etree_generate      | 86.1 ms                                                      | 80.8 ms: 1.07x faster                                                        |
| gunicorn                | 1.00 ms                                                      | 941 us: 1.06x faster                                                         |
| pickle_dict             | 32.5 us                                                      | 30.7 us: 1.06x faster                                                        |
| regex_dna               | 239 ms                                                       | 225 ms: 1.06x faster                                                         |
| pidigits                | 265 ms                                                       | 251 ms: 1.05x faster                                                         |
| aiohttp                 | 1.02 ms                                                      | 966 us: 1.05x faster                                                         |
| bench_mp_pool           | 4.76 ms                                                      | 4.54 ms: 1.05x faster                                                        |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 4.01 ms: 1.05x faster                                                        |
| sqlalchemy_declarative  | 159 ms                                                       | 155 ms: 1.03x faster                                                         |
| xml_etree_process       | 58.4 ms                                                      | 57.0 ms: 1.02x faster                                                        |
| pprint_safe_repr        | 807 ms                                                       | 791 ms: 1.02x faster                                                         |
| float                   | 76.6 ms                                                      | 75.1 ms: 1.02x faster                                                        |
| telco                   | 6.96 ms                                                      | 6.88 ms: 1.01x faster                                                        |
| pprint_pformat          | 1.65 sec                                                     | 1.65 sec: 1.01x faster                                                       |
| 2to3                    | 285 ms                                                       | 287 ms: 1.01x slower                                                         |
| scimark_sor             | 109 ms                                                       | 110 ms: 1.01x slower                                                         |
| xml_etree_iterparse     | 103 ms                                                       | 104 ms: 1.01x slower                                                         |
| pathlib                 | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                        |
| pickle_pure_python      | 318 us                                                       | 324 us: 1.02x slower                                                         |
| nbody                   | 88.0 ms                                                      | 89.6 ms: 1.02x slower                                                        |
| sqlglot_optimize        | 57.5 ms                                                      | 58.8 ms: 1.02x slower                                                        |
| pyflate                 | 439 ms                                                       | 450 ms: 1.03x slower                                                         |
| regex_v8                | 23.6 ms                                                      | 24.3 ms: 1.03x slower                                                        |
| raytrace                | 298 ms                                                       | 307 ms: 1.03x slower                                                         |
| meteor_contest          | 128 ms                                                       | 132 ms: 1.03x slower                                                         |
| tornado_http            | 121 ms                                                       | 125 ms: 1.03x slower                                                         |
| chameleon               | 7.23 ms                                                      | 7.50 ms: 1.04x slower                                                        |
| django_template         | 38.2 ms                                                      | 39.7 ms: 1.04x slower                                                        |
| deepcopy_reduce         | 3.37 us                                                      | 3.51 us: 1.04x slower                                                        |
| spectral_norm           | 91.6 ms                                                      | 95.5 ms: 1.04x slower                                                        |
| gc_traversal            | 3.48 ms                                                      | 3.63 ms: 1.04x slower                                                        |
| create_gc_cycles        | 1.59 ms                                                      | 1.66 ms: 1.04x slower                                                        |
| sqlglot_normalize       | 116 ms                                                       | 121 ms: 1.05x slower                                                         |
| crypto_pyaes            | 80.3 ms                                                      | 84.3 ms: 1.05x slower                                                        |
| bench_thread_pool       | 950 us                                                       | 1.00 ms: 1.06x slower                                                        |
| mdp                     | 2.57 sec                                                     | 2.72 sec: 1.06x slower                                                       |
| sqlalchemy_imperative   | 18.7 ms                                                      | 19.9 ms: 1.06x slower                                                        |
| dulwich_log             | 65.4 ms                                                      | 69.6 ms: 1.06x slower                                                        |
| logging_silent          | 94.4 ns                                                      | 101 ns: 1.07x slower                                                         |
| dask                    | 392 ms                                                       | 420 ms: 1.07x slower                                                         |
| async_tree_cpu_io_mixed | 696 ms                                                       | 746 ms: 1.07x slower                                                         |
| logging_format          | 7.48 us                                                      | 8.03 us: 1.07x slower                                                        |
| sqlglot_transpile       | 1.78 ms                                                      | 1.92 ms: 1.08x slower                                                        |
| sympy_integrate         | 23.9 ms                                                      | 25.9 ms: 1.08x slower                                                        |
| pycparser               | 1.23 sec                                                     | 1.34 sec: 1.08x slower                                                       |
| json                    | 5.12 ms                                                      | 5.57 ms: 1.09x slower                                                        |
| mako                    | 10.0 ms                                                      | 10.9 ms: 1.09x slower                                                        |
| regex_compile           | 144 ms                                                       | 157 ms: 1.09x slower                                                         |
| deepcopy                | 368 us                                                       | 407 us: 1.11x slower                                                         |
| logging_simple          | 6.71 us                                                      | 7.43 us: 1.11x slower                                                        |
| xml_etree_parse         | 144 ms                                                       | 160 ms: 1.11x slower                                                         |
| deepcopy_memo           | 36.8 us                                                      | 41.0 us: 1.11x slower                                                        |
| sympy_str               | 302 ms                                                       | 337 ms: 1.12x slower                                                         |
| nqueens                 | 89.9 ms                                                      | 101 ms: 1.13x slower                                                         |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.13x slower                                                       |
| sympy_sum               | 162 ms                                                       | 183 ms: 1.13x slower                                                         |
| sqlglot_parse           | 1.38 ms                                                      | 1.56 ms: 1.13x slower                                                        |
| sympy_expand            | 484 ms                                                       | 553 ms: 1.14x slower                                                         |
| async_tree_none         | 452 ms                                                       | 517 ms: 1.14x slower                                                         |
| go                      | 150 ms                                                       | 172 ms: 1.15x slower                                                         |
| scimark_lu              | 98.8 ms                                                      | 114 ms: 1.15x slower                                                         |
| comprehensions          | 21.9 us                                                      | 25.5 us: 1.16x slower                                                        |
| json_loads              | 24.4 us                                                      | 28.4 us: 1.17x slower                                                        |
| async_tree_memoization  | 544 ms                                                       | 636 ms: 1.17x slower                                                         |
| richards                | 45.7 ms                                                      | 53.5 ms: 1.17x slower                                                        |
| unpickle_pure_python    | 210 us                                                       | 250 us: 1.19x slower                                                         |
| hexiom                  | 5.96 ms                                                      | 7.12 ms: 1.20x slower                                                        |
| coroutines              | 23.0 ms                                                      | 27.9 ms: 1.21x slower                                                        |
| fannkuch                | 350 ms                                                       | 441 ms: 1.26x slower                                                         |
| deltablue               | 3.24 ms                                                      | 4.09 ms: 1.27x slower                                                        |
| chaos                   | 64.0 ms                                                      | 81.4 ms: 1.27x slower                                                        |
| json_dumps              | 10.2 ms                                                      | 13.5 ms: 1.32x slower                                                        |
| generators              | 37.4 ms                                                      | 54.2 ms: 1.45x slower                                                        |
| asyncio_tcp             | 378 ms                                                       | 752 ms: 1.99x slower                                                         |
| Geometric mean          | (ref)                                                        | 1.05x slower                                                                 |

Benchmark hidden because not significant (3): scimark_monte_carlo, docutils, unpickle_list
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20220911-3.11.0rc2-ed7c3ff/bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.91x