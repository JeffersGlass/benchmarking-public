
# Results vs. 3.12.0

- fork: python
- ref: 2e91dba437fe5c56c6f8
- machine: linux-x86_64
- commit hash: 2e91dba
- commit date: 2021-12-08
- overall geometric mean: 1.11x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x slower
- Memory change: 0.92x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 293 ms: 1.03x slower                                                        |
| chameleon      | 7.23 ms                                                      | 8.85 ms: 1.22x slower                                                       |
| docutils       | 2.87 sec                                                     | 3.02 sec: 1.05x slower                                                      |
| tornado_http   | 121 ms                                                       | 135 ms: 1.11x slower                                                        |
| Geometric mean | (ref)                                                        | 1.10x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 811 ms: 1.17x slower                                                        |
| async_tree_none         | 452 ms                                                       | 545 ms: 1.21x slower                                                        |
| async_tree_memoization  | 544 ms                                                       | 686 ms: 1.26x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.32 sec: 1.26x slower                                                      |
| Geometric mean          | (ref)                                                        | 1.22x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 253 ms: 1.05x faster                                                        |
| float          | 76.6 ms                                                      | 80.9 ms: 1.06x slower                                                       |
| nbody          | 88.0 ms                                                      | 109 ms: 1.23x slower                                                        |
| Geometric mean | (ref)                                                        | 1.08x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.10 ms: 1.15x faster                                                       |
| regex_compile  | 144 ms                                                       | 153 ms: 1.06x slower                                                        |
| regex_v8       | 23.6 ms                                                      | 25.7 ms: 1.09x slower                                                       |
| regex_dna      | 239 ms                                                       | 261 ms: 1.09x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle             | 14.8 us                                                      | 13.2 us: 1.12x faster                                                       |
| xml_etree_generate   | 86.1 ms                                                      | 82.8 ms: 1.04x faster                                                       |
| pickle               | 10.5 us                                                      | 10.2 us: 1.03x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.53 us: 1.03x faster                                                       |
| pickle_list          | 4.43 us                                                      | 4.32 us: 1.03x faster                                                       |
| pickle_dict          | 32.5 us                                                      | 33.0 us: 1.01x slower                                                       |
| json_loads           | 24.4 us                                                      | 25.3 us: 1.04x slower                                                       |
| xml_etree_process    | 58.4 ms                                                      | 60.9 ms: 1.04x slower                                                       |
| xml_etree_iterparse  | 103 ms                                                       | 110 ms: 1.07x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 155 ms: 1.08x slower                                                        |
| pickle_pure_python   | 318 us                                                       | 366 us: 1.15x slower                                                        |
| unpickle_pure_python | 210 us                                                       | 265 us: 1.27x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 14.1 ms: 1.37x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.06x slower                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.14 ms: 1.21x faster                                                       |
| python_startup         | 11.6 ms                                                      | 10.1 ms: 1.15x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.18x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 44.9 ms: 1.18x slower                                                       |
| mako            | 10.0 ms                                                      | 12.9 ms: 1.29x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.23x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_generators        | 390 ms                                                       | 319 ms: 1.22x faster                                                        |
| python_startup_no_site  | 8.64 ms                                                      | 7.14 ms: 1.21x faster                                                       |
| regex_effbot            | 3.57 ms                                                      | 3.10 ms: 1.15x faster                                                       |
| python_startup          | 11.6 ms                                                      | 10.1 ms: 1.15x faster                                                       |
| unpack_sequence         | 53.2 ns                                                      | 46.3 ns: 1.15x faster                                                       |
| unpickle                | 14.8 us                                                      | 13.2 us: 1.12x faster                                                       |
| pidigits                | 265 ms                                                       | 253 ms: 1.05x faster                                                        |
| xml_etree_generate      | 86.1 ms                                                      | 82.8 ms: 1.04x faster                                                       |
| pickle                  | 10.5 us                                                      | 10.2 us: 1.03x faster                                                       |
| unpickle_list           | 4.66 us                                                      | 4.53 us: 1.03x faster                                                       |
| sqlite_synth            | 2.77 us                                                      | 2.70 us: 1.03x faster                                                       |
| pickle_list             | 4.43 us                                                      | 4.32 us: 1.03x faster                                                       |
| meteor_contest          | 128 ms                                                       | 129 ms: 1.01x slower                                                        |
| pickle_dict             | 32.5 us                                                      | 33.0 us: 1.01x slower                                                       |
| telco                   | 6.96 ms                                                      | 7.11 ms: 1.02x slower                                                       |
| json                    | 5.12 ms                                                      | 5.24 ms: 1.02x slower                                                       |
| 2to3                    | 285 ms                                                       | 293 ms: 1.03x slower                                                        |
| logging_format          | 7.48 us                                                      | 7.70 us: 1.03x slower                                                       |
| pprint_safe_repr        | 807 ms                                                       | 832 ms: 1.03x slower                                                        |
| json_loads              | 24.4 us                                                      | 25.3 us: 1.04x slower                                                       |
| create_gc_cycles        | 1.59 ms                                                      | 1.66 ms: 1.04x slower                                                       |
| scimark_fft             | 301 ms                                                       | 314 ms: 1.04x slower                                                        |
| xml_etree_process       | 58.4 ms                                                      | 60.9 ms: 1.04x slower                                                       |
| logging_simple          | 6.71 us                                                      | 7.04 us: 1.05x slower                                                       |
| pprint_pformat          | 1.65 sec                                                     | 1.74 sec: 1.05x slower                                                      |
| deepcopy_reduce         | 3.37 us                                                      | 3.55 us: 1.05x slower                                                       |
| docutils                | 2.87 sec                                                     | 3.02 sec: 1.05x slower                                                      |
| pathlib                 | 18.9 ms                                                      | 19.9 ms: 1.06x slower                                                       |
| float                   | 76.6 ms                                                      | 80.9 ms: 1.06x slower                                                       |
| scimark_sor             | 109 ms                                                       | 115 ms: 1.06x slower                                                        |
| regex_compile           | 144 ms                                                       | 153 ms: 1.06x slower                                                        |
| xml_etree_iterparse     | 103 ms                                                       | 110 ms: 1.07x slower                                                        |
| mdp                     | 2.57 sec                                                     | 2.76 sec: 1.08x slower                                                      |
| xml_etree_parse         | 144 ms                                                       | 155 ms: 1.08x slower                                                        |
| coverage                | 66.7 ms                                                      | 72.1 ms: 1.08x slower                                                       |
| regex_v8                | 23.6 ms                                                      | 25.7 ms: 1.09x slower                                                       |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 4.58 ms: 1.09x slower                                                       |
| spectral_norm           | 91.6 ms                                                      | 99.9 ms: 1.09x slower                                                       |
| pycparser               | 1.23 sec                                                     | 1.35 sec: 1.09x slower                                                      |
| regex_dna               | 239 ms                                                       | 261 ms: 1.09x slower                                                        |
| sympy_integrate         | 23.9 ms                                                      | 26.5 ms: 1.11x slower                                                       |
| dask                    | 392 ms                                                       | 435 ms: 1.11x slower                                                        |
| tornado_http            | 121 ms                                                       | 135 ms: 1.11x slower                                                        |
| scimark_lu              | 98.8 ms                                                      | 110 ms: 1.11x slower                                                        |
| scimark_monte_carlo     | 69.0 ms                                                      | 76.7 ms: 1.11x slower                                                       |
| bench_thread_pool       | 950 us                                                       | 1.06 ms: 1.11x slower                                                       |
| dulwich_log             | 65.4 ms                                                      | 73.0 ms: 1.12x slower                                                       |
| gc_traversal            | 3.48 ms                                                      | 3.89 ms: 1.12x slower                                                       |
| sqlglot_optimize        | 57.5 ms                                                      | 64.7 ms: 1.13x slower                                                       |
| deepcopy_memo           | 36.8 us                                                      | 41.5 us: 1.13x slower                                                       |
| deepcopy                | 368 us                                                       | 418 us: 1.13x slower                                                        |
| sqlglot_normalize       | 116 ms                                                       | 133 ms: 1.15x slower                                                        |
| nqueens                 | 89.9 ms                                                      | 103 ms: 1.15x slower                                                        |
| pickle_pure_python      | 318 us                                                       | 366 us: 1.15x slower                                                        |
| go                      | 150 ms                                                       | 173 ms: 1.15x slower                                                        |
| sympy_str               | 302 ms                                                       | 350 ms: 1.16x slower                                                        |
| raytrace                | 298 ms                                                       | 347 ms: 1.16x slower                                                        |
| async_tree_cpu_io_mixed | 696 ms                                                       | 811 ms: 1.17x slower                                                        |
| sympy_sum               | 162 ms                                                       | 189 ms: 1.17x slower                                                        |
| coroutines              | 23.0 ms                                                      | 27.0 ms: 1.17x slower                                                       |
| django_template         | 38.2 ms                                                      | 44.9 ms: 1.18x slower                                                       |
| crypto_pyaes            | 80.3 ms                                                      | 94.7 ms: 1.18x slower                                                       |
| sympy_expand            | 484 ms                                                       | 579 ms: 1.20x slower                                                        |
| pyflate                 | 439 ms                                                       | 525 ms: 1.20x slower                                                        |
| async_tree_none         | 452 ms                                                       | 545 ms: 1.21x slower                                                        |
| fannkuch                | 350 ms                                                       | 428 ms: 1.22x slower                                                        |
| chaos                   | 64.0 ms                                                      | 78.3 ms: 1.22x slower                                                       |
| chameleon               | 7.23 ms                                                      | 8.85 ms: 1.22x slower                                                       |
| logging_silent          | 94.4 ns                                                      | 116 ns: 1.23x slower                                                        |
| nbody                   | 88.0 ms                                                      | 109 ms: 1.23x slower                                                        |
| richards                | 45.7 ms                                                      | 56.7 ms: 1.24x slower                                                       |
| hexiom                  | 5.96 ms                                                      | 7.41 ms: 1.24x slower                                                       |
| async_tree_memoization  | 544 ms                                                       | 686 ms: 1.26x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.32 sec: 1.26x slower                                                      |
| unpickle_pure_python    | 210 us                                                       | 265 us: 1.27x slower                                                        |
| mako                    | 10.0 ms                                                      | 12.9 ms: 1.29x slower                                                       |
| generators              | 37.4 ms                                                      | 50.1 ms: 1.34x slower                                                       |
| json_dumps              | 10.2 ms                                                      | 14.1 ms: 1.37x slower                                                       |
| comprehensions          | 21.9 us                                                      | 30.6 us: 1.39x slower                                                       |
| sqlglot_transpile       | 1.78 ms                                                      | 2.60 ms: 1.46x slower                                                       |
| deltablue               | 3.24 ms                                                      | 4.78 ms: 1.48x slower                                                       |
| sqlglot_parse           | 1.38 ms                                                      | 2.21 ms: 1.60x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.11x slower                                                                |

Benchmark hidden because not significant (2): gunicorn, bench_mp_pool
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (5) of results/bm-20211208-3.11.0a3-2e91dba/bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba.json: flaskblogging, genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.09x
- 95% likely to have a slowdown of 1.08x
- 99% likely to have a slowdown of 1.07x


# Memory

- memory change: 0.92x