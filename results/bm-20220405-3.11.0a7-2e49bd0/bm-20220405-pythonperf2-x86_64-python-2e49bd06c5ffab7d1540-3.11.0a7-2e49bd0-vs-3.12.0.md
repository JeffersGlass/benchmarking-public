
# Results vs. 3.12.0

- fork: python
- ref: 2e49bd06c5ffab7d1540
- machine: linux-x86_64
- commit hash: 2e49bd0
- commit date: 2022-04-05
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 293 ms: 1.03x slower                                                        |
| chameleon      | 7.23 ms                                                      | 7.97 ms: 1.10x slower                                                       |
| docutils       | 2.87 sec                                                     | 2.92 sec: 1.02x slower                                                      |
| tornado_http   | 121 ms                                                       | 123 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 753 ms: 1.08x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.18 sec: 1.13x slower                                                      |
| async_tree_none         | 452 ms                                                       | 523 ms: 1.16x slower                                                        |
| async_tree_memoization  | 544 ms                                                       | 641 ms: 1.18x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.14x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 251 ms: 1.06x faster                                                        |
| float          | 76.6 ms                                                      | 78.4 ms: 1.02x slower                                                       |
| nbody          | 88.0 ms                                                      | 93.6 ms: 1.06x slower                                                       |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.13 ms: 1.14x faster                                                       |
| regex_dna      | 239 ms                                                       | 253 ms: 1.06x slower                                                        |
| regex_compile  | 144 ms                                                       | 159 ms: 1.10x slower                                                        |
| regex_v8       | 23.6 ms                                                      | 26.6 ms: 1.13x slower                                                       |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle             | 14.8 us                                                      | 13.0 us: 1.14x faster                                                       |
| pickle_list          | 4.43 us                                                      | 4.12 us: 1.08x faster                                                       |
| pickle               | 10.5 us                                                      | 9.88 us: 1.07x faster                                                       |
| pickle_dict          | 32.5 us                                                      | 31.1 us: 1.05x faster                                                       |
| xml_etree_generate   | 86.1 ms                                                      | 82.8 ms: 1.04x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.52 us: 1.03x faster                                                       |
| json_loads           | 24.4 us                                                      | 24.5 us: 1.01x slower                                                       |
| xml_etree_iterparse  | 103 ms                                                       | 106 ms: 1.03x slower                                                        |
| pickle_pure_python   | 318 us                                                       | 331 us: 1.04x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 157 ms: 1.09x slower                                                        |
| unpickle_pure_python | 210 us                                                       | 242 us: 1.16x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 13.5 ms: 1.32x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                                |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.46 ms: 1.16x faster                                                       |
| python_startup         | 11.6 ms                                                      | 10.4 ms: 1.12x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.14x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 40.7 ms: 1.07x slower                                                       |
| mako            | 10.0 ms                                                      | 11.2 ms: 1.12x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.09x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_generators        | 390 ms                                                       | 319 ms: 1.22x faster                                                        |
| python_startup_no_site  | 8.64 ms                                                      | 7.46 ms: 1.16x faster                                                       |
| regex_effbot            | 3.57 ms                                                      | 3.13 ms: 1.14x faster                                                       |
| unpickle                | 14.8 us                                                      | 13.0 us: 1.14x faster                                                       |
| unpack_sequence         | 53.2 ns                                                      | 47.3 ns: 1.12x faster                                                       |
| python_startup          | 11.6 ms                                                      | 10.4 ms: 1.12x faster                                                       |
| sqlite_synth            | 2.77 us                                                      | 2.52 us: 1.10x faster                                                       |
| pickle_list             | 4.43 us                                                      | 4.12 us: 1.08x faster                                                       |
| dask                    | 392 ms                                                       | 367 ms: 1.07x faster                                                        |
| pickle                  | 10.5 us                                                      | 9.88 us: 1.07x faster                                                       |
| pidigits                | 265 ms                                                       | 251 ms: 1.06x faster                                                        |
| pickle_dict             | 32.5 us                                                      | 31.1 us: 1.05x faster                                                       |
| xml_etree_generate      | 86.1 ms                                                      | 82.8 ms: 1.04x faster                                                       |
| aiohttp                 | 1.02 ms                                                      | 978 us: 1.04x faster                                                        |
| gunicorn                | 1.00 ms                                                      | 968 us: 1.03x faster                                                        |
| unpickle_list           | 4.66 us                                                      | 4.52 us: 1.03x faster                                                       |
| telco                   | 6.96 ms                                                      | 6.79 ms: 1.03x faster                                                       |
| scimark_fft             | 301 ms                                                       | 297 ms: 1.01x faster                                                        |
| json_loads              | 24.4 us                                                      | 24.5 us: 1.01x slower                                                       |
| json                    | 5.12 ms                                                      | 5.17 ms: 1.01x slower                                                       |
| logging_format          | 7.48 us                                                      | 7.59 us: 1.01x slower                                                       |
| pprint_safe_repr        | 807 ms                                                       | 818 ms: 1.01x slower                                                        |
| tornado_http            | 121 ms                                                       | 123 ms: 1.02x slower                                                        |
| docutils                | 2.87 sec                                                     | 2.92 sec: 1.02x slower                                                      |
| float                   | 76.6 ms                                                      | 78.4 ms: 1.02x slower                                                       |
| pprint_pformat          | 1.65 sec                                                     | 1.69 sec: 1.02x slower                                                      |
| pathlib                 | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                       |
| 2to3                    | 285 ms                                                       | 293 ms: 1.03x slower                                                        |
| xml_etree_iterparse     | 103 ms                                                       | 106 ms: 1.03x slower                                                        |
| gc_traversal            | 3.48 ms                                                      | 3.58 ms: 1.03x slower                                                       |
| deepcopy_reduce         | 3.37 us                                                      | 3.48 us: 1.03x slower                                                       |
| scimark_sor             | 109 ms                                                       | 112 ms: 1.03x slower                                                        |
| create_gc_cycles        | 1.59 ms                                                      | 1.65 ms: 1.03x slower                                                       |
| meteor_contest          | 128 ms                                                       | 133 ms: 1.04x slower                                                        |
| pickle_pure_python      | 318 us                                                       | 331 us: 1.04x slower                                                        |
| deepcopy                | 368 us                                                       | 385 us: 1.05x slower                                                        |
| deepcopy_memo           | 36.8 us                                                      | 38.8 us: 1.05x slower                                                       |
| sympy_integrate         | 23.9 ms                                                      | 25.3 ms: 1.06x slower                                                       |
| pyflate                 | 439 ms                                                       | 464 ms: 1.06x slower                                                        |
| regex_dna               | 239 ms                                                       | 253 ms: 1.06x slower                                                        |
| nbody                   | 88.0 ms                                                      | 93.6 ms: 1.06x slower                                                       |
| django_template         | 38.2 ms                                                      | 40.7 ms: 1.07x slower                                                       |
| dulwich_log             | 65.4 ms                                                      | 69.8 ms: 1.07x slower                                                       |
| bench_thread_pool       | 950 us                                                       | 1.02 ms: 1.07x slower                                                       |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 4.51 ms: 1.07x slower                                                       |
| mdp                     | 2.57 sec                                                     | 2.76 sec: 1.07x slower                                                      |
| pycparser               | 1.23 sec                                                     | 1.33 sec: 1.08x slower                                                      |
| sqlglot_optimize        | 57.5 ms                                                      | 61.9 ms: 1.08x slower                                                       |
| raytrace                | 298 ms                                                       | 322 ms: 1.08x slower                                                        |
| async_tree_cpu_io_mixed | 696 ms                                                       | 753 ms: 1.08x slower                                                        |
| xml_etree_parse         | 144 ms                                                       | 157 ms: 1.09x slower                                                        |
| sympy_str               | 302 ms                                                       | 330 ms: 1.09x slower                                                        |
| sqlglot_normalize       | 116 ms                                                       | 127 ms: 1.09x slower                                                        |
| sympy_sum               | 162 ms                                                       | 177 ms: 1.09x slower                                                        |
| sqlalchemy_imperative   | 18.7 ms                                                      | 20.5 ms: 1.10x slower                                                       |
| chameleon               | 7.23 ms                                                      | 7.97 ms: 1.10x slower                                                       |
| regex_compile           | 144 ms                                                       | 159 ms: 1.10x slower                                                        |
| logging_silent          | 94.4 ns                                                      | 105 ns: 1.11x slower                                                        |
| go                      | 150 ms                                                       | 166 ms: 1.11x slower                                                        |
| crypto_pyaes            | 80.3 ms                                                      | 89.5 ms: 1.11x slower                                                       |
| scimark_monte_carlo     | 69.0 ms                                                      | 77.1 ms: 1.12x slower                                                       |
| mako                    | 10.0 ms                                                      | 11.2 ms: 1.12x slower                                                       |
| regex_v8                | 23.6 ms                                                      | 26.6 ms: 1.13x slower                                                       |
| async_tree_io           | 1.04 sec                                                     | 1.18 sec: 1.13x slower                                                      |
| sympy_expand            | 484 ms                                                       | 549 ms: 1.13x slower                                                        |
| nqueens                 | 89.9 ms                                                      | 102 ms: 1.14x slower                                                        |
| chaos                   | 64.0 ms                                                      | 73.4 ms: 1.15x slower                                                       |
| richards                | 45.7 ms                                                      | 52.8 ms: 1.15x slower                                                       |
| unpickle_pure_python    | 210 us                                                       | 242 us: 1.16x slower                                                        |
| async_tree_none         | 452 ms                                                       | 523 ms: 1.16x slower                                                        |
| spectral_norm           | 91.6 ms                                                      | 107 ms: 1.17x slower                                                        |
| async_tree_memoization  | 544 ms                                                       | 641 ms: 1.18x slower                                                        |
| scimark_lu              | 98.8 ms                                                      | 120 ms: 1.22x slower                                                        |
| coroutines              | 23.0 ms                                                      | 29.0 ms: 1.26x slower                                                       |
| fannkuch                | 350 ms                                                       | 442 ms: 1.26x slower                                                        |
| comprehensions          | 21.9 us                                                      | 27.8 us: 1.27x slower                                                       |
| hexiom                  | 5.96 ms                                                      | 7.66 ms: 1.29x slower                                                       |
| deltablue               | 3.24 ms                                                      | 4.23 ms: 1.31x slower                                                       |
| json_dumps              | 10.2 ms                                                      | 13.5 ms: 1.32x slower                                                       |
| sqlglot_transpile       | 1.78 ms                                                      | 2.38 ms: 1.34x slower                                                       |
| generators              | 37.4 ms                                                      | 54.7 ms: 1.46x slower                                                       |
| sqlglot_parse           | 1.38 ms                                                      | 2.04 ms: 1.48x slower                                                       |
| asyncio_tcp             | 378 ms                                                       | 746 ms: 1.97x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.07x slower                                                                |

Benchmark hidden because not significant (4): bench_mp_pool, logging_simple, xml_etree_process, sqlalchemy_declarative
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20220405-3.11.0a7-2e49bd0/bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.93x