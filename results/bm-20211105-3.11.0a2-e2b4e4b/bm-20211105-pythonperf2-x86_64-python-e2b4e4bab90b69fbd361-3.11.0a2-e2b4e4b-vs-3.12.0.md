
# Results vs. 3.12.0

- fork: python
- ref: e2b4e4bab90b69fbd361
- machine: linux-x86_64
- commit hash: e2b4e4b
- commit date: 2021-11-05
- overall geometric mean: 1.13x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 299 ms: 1.05x slower                                                        |
| chameleon      | 7.23 ms                                                      | 9.27 ms: 1.28x slower                                                       |
| docutils       | 2.87 sec                                                     | 3.05 sec: 1.06x slower                                                      |
| tornado_http   | 121 ms                                                       | 136 ms: 1.12x slower                                                        |
| Geometric mean | (ref)                                                        | 1.12x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 818 ms: 1.17x slower                                                        |
| async_tree_none         | 452 ms                                                       | 532 ms: 1.18x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.27 sec: 1.22x slower                                                      |
| async_tree_memoization  | 544 ms                                                       | 668 ms: 1.23x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.20x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 264 ms: 1.00x faster                                                        |
| float          | 76.6 ms                                                      | 86.1 ms: 1.12x slower                                                       |
| nbody          | 88.0 ms                                                      | 113 ms: 1.28x slower                                                        |
| Geometric mean | (ref)                                                        | 1.13x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.06 ms: 1.17x faster                                                       |
| regex_v8       | 23.6 ms                                                      | 25.8 ms: 1.09x slower                                                       |
| regex_dna      | 239 ms                                                       | 262 ms: 1.10x slower                                                        |
| regex_compile  | 144 ms                                                       | 158 ms: 1.10x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle             | 14.8 us                                                      | 13.4 us: 1.11x faster                                                       |
| pickle_dict          | 32.5 us                                                      | 30.2 us: 1.08x faster                                                       |
| pickle_list          | 4.43 us                                                      | 4.17 us: 1.06x faster                                                       |
| pickle               | 10.5 us                                                      | 10.3 us: 1.03x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.55 us: 1.02x faster                                                       |
| xml_etree_generate   | 86.1 ms                                                      | 85.8 ms: 1.00x faster                                                       |
| json_loads           | 24.4 us                                                      | 24.7 us: 1.01x slower                                                       |
| xml_etree_iterparse  | 103 ms                                                       | 107 ms: 1.04x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 61.7 ms: 1.06x slower                                                       |
| xml_etree_parse      | 144 ms                                                       | 157 ms: 1.09x slower                                                        |
| pickle_pure_python   | 318 us                                                       | 386 us: 1.21x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 13.4 ms: 1.31x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 277 us: 1.32x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.05x slower                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.43 ms: 1.16x faster                                                       |
| python_startup         | 11.6 ms                                                      | 11.2 ms: 1.04x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.10x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 47.4 ms: 1.24x slower                                                       |
| mako            | 10.0 ms                                                      | 12.9 ms: 1.29x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.27x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_generators        | 390 ms                                                       | 325 ms: 1.20x faster                                                        |
| regex_effbot            | 3.57 ms                                                      | 3.06 ms: 1.17x faster                                                       |
| python_startup_no_site  | 8.64 ms                                                      | 7.43 ms: 1.16x faster                                                       |
| unpack_sequence         | 53.2 ns                                                      | 46.0 ns: 1.16x faster                                                       |
| unpickle                | 14.8 us                                                      | 13.4 us: 1.11x faster                                                       |
| pickle_dict             | 32.5 us                                                      | 30.2 us: 1.08x faster                                                       |
| pickle_list             | 4.43 us                                                      | 4.17 us: 1.06x faster                                                       |
| python_startup          | 11.6 ms                                                      | 11.2 ms: 1.04x faster                                                       |
| pickle                  | 10.5 us                                                      | 10.3 us: 1.03x faster                                                       |
| unpickle_list           | 4.66 us                                                      | 4.55 us: 1.02x faster                                                       |
| telco                   | 6.96 ms                                                      | 6.81 ms: 1.02x faster                                                       |
| gunicorn                | 1.00 ms                                                      | 980 us: 1.02x faster                                                        |
| xml_etree_generate      | 86.1 ms                                                      | 85.8 ms: 1.00x faster                                                       |
| pidigits                | 265 ms                                                       | 264 ms: 1.00x faster                                                        |
| json_loads              | 24.4 us                                                      | 24.7 us: 1.01x slower                                                       |
| json                    | 5.12 ms                                                      | 5.19 ms: 1.01x slower                                                       |
| coverage                | 66.7 ms                                                      | 68.7 ms: 1.03x slower                                                       |
| scimark_fft             | 301 ms                                                       | 311 ms: 1.03x slower                                                        |
| xml_etree_iterparse     | 103 ms                                                       | 107 ms: 1.04x slower                                                        |
| 2to3                    | 285 ms                                                       | 299 ms: 1.05x slower                                                        |
| create_gc_cycles        | 1.59 ms                                                      | 1.67 ms: 1.05x slower                                                       |
| bench_mp_pool           | 4.76 ms                                                      | 5.01 ms: 1.05x slower                                                       |
| xml_etree_process       | 58.4 ms                                                      | 61.7 ms: 1.06x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 20.0 ms: 1.06x slower                                                       |
| docutils                | 2.87 sec                                                     | 3.05 sec: 1.06x slower                                                      |
| logging_format          | 7.48 us                                                      | 8.08 us: 1.08x slower                                                       |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 4.56 ms: 1.08x slower                                                       |
| gc_traversal            | 3.48 ms                                                      | 3.77 ms: 1.08x slower                                                       |
| pprint_safe_repr        | 807 ms                                                       | 877 ms: 1.09x slower                                                        |
| regex_v8                | 23.6 ms                                                      | 25.8 ms: 1.09x slower                                                       |
| xml_etree_parse         | 144 ms                                                       | 157 ms: 1.09x slower                                                        |
| logging_simple          | 6.71 us                                                      | 7.35 us: 1.09x slower                                                       |
| regex_dna               | 239 ms                                                       | 262 ms: 1.10x slower                                                        |
| regex_compile           | 144 ms                                                       | 158 ms: 1.10x slower                                                        |
| pprint_pformat          | 1.65 sec                                                     | 1.82 sec: 1.10x slower                                                      |
| bench_thread_pool       | 950 us                                                       | 1.05 ms: 1.10x slower                                                       |
| dulwich_log             | 65.4 ms                                                      | 72.4 ms: 1.11x slower                                                       |
| sympy_integrate         | 23.9 ms                                                      | 26.5 ms: 1.11x slower                                                       |
| mdp                     | 2.57 sec                                                     | 2.87 sec: 1.12x slower                                                      |
| tornado_http            | 121 ms                                                       | 136 ms: 1.12x slower                                                        |
| float                   | 76.6 ms                                                      | 86.1 ms: 1.12x slower                                                       |
| sympy_str               | 302 ms                                                       | 340 ms: 1.13x slower                                                        |
| sqlglot_optimize        | 57.5 ms                                                      | 64.9 ms: 1.13x slower                                                       |
| deepcopy_reduce         | 3.37 us                                                      | 3.81 us: 1.13x slower                                                       |
| sympy_sum               | 162 ms                                                       | 183 ms: 1.13x slower                                                        |
| nqueens                 | 89.9 ms                                                      | 102 ms: 1.13x slower                                                        |
| dask                    | 392 ms                                                       | 445 ms: 1.14x slower                                                        |
| spectral_norm           | 91.6 ms                                                      | 104 ms: 1.14x slower                                                        |
| sqlglot_normalize       | 116 ms                                                       | 132 ms: 1.14x slower                                                        |
| scimark_monte_carlo     | 69.0 ms                                                      | 79.5 ms: 1.15x slower                                                       |
| deepcopy                | 368 us                                                       | 428 us: 1.16x slower                                                        |
| sympy_expand            | 484 ms                                                       | 563 ms: 1.16x slower                                                        |
| deepcopy_memo           | 36.8 us                                                      | 42.9 us: 1.17x slower                                                       |
| raytrace                | 298 ms                                                       | 349 ms: 1.17x slower                                                        |
| async_tree_cpu_io_mixed | 696 ms                                                       | 818 ms: 1.17x slower                                                        |
| async_tree_none         | 452 ms                                                       | 532 ms: 1.18x slower                                                        |
| crypto_pyaes            | 80.3 ms                                                      | 94.9 ms: 1.18x slower                                                       |
| pycparser               | 1.23 sec                                                     | 1.48 sec: 1.20x slower                                                      |
| pickle_pure_python      | 318 us                                                       | 386 us: 1.21x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.27 sec: 1.22x slower                                                      |
| async_tree_memoization  | 544 ms                                                       | 668 ms: 1.23x slower                                                        |
| chaos                   | 64.0 ms                                                      | 79.2 ms: 1.24x slower                                                       |
| django_template         | 38.2 ms                                                      | 47.4 ms: 1.24x slower                                                       |
| logging_silent          | 94.4 ns                                                      | 121 ns: 1.28x slower                                                        |
| scimark_sor             | 109 ms                                                       | 140 ms: 1.28x slower                                                        |
| chameleon               | 7.23 ms                                                      | 9.27 ms: 1.28x slower                                                       |
| coroutines              | 23.0 ms                                                      | 29.5 ms: 1.28x slower                                                       |
| nbody                   | 88.0 ms                                                      | 113 ms: 1.28x slower                                                        |
| mako                    | 10.0 ms                                                      | 12.9 ms: 1.29x slower                                                       |
| richards                | 45.7 ms                                                      | 59.0 ms: 1.29x slower                                                       |
| go                      | 150 ms                                                       | 194 ms: 1.30x slower                                                        |
| fannkuch                | 350 ms                                                       | 458 ms: 1.31x slower                                                        |
| comprehensions          | 21.9 us                                                      | 28.8 us: 1.31x slower                                                       |
| json_dumps              | 10.2 ms                                                      | 13.4 ms: 1.31x slower                                                       |
| hexiom                  | 5.96 ms                                                      | 7.87 ms: 1.32x slower                                                       |
| unpickle_pure_python    | 210 us                                                       | 277 us: 1.32x slower                                                        |
| pyflate                 | 439 ms                                                       | 582 ms: 1.33x slower                                                        |
| scimark_lu              | 98.8 ms                                                      | 132 ms: 1.34x slower                                                        |
| generators              | 37.4 ms                                                      | 52.7 ms: 1.41x slower                                                       |
| sqlglot_transpile       | 1.78 ms                                                      | 2.63 ms: 1.48x slower                                                       |
| deltablue               | 3.24 ms                                                      | 5.07 ms: 1.57x slower                                                       |
| sqlglot_parse           | 1.38 ms                                                      | 2.24 ms: 1.63x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.13x slower                                                                |

Benchmark hidden because not significant (2): sqlite_synth, meteor_contest
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (5) of results/bm-20211105-3.11.0a2-e2b4e4b/bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b.json: flaskblogging, genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.11x
- 95% likely to have a slowdown of 1.11x
- 99% likely to have a slowdown of 1.10x


# Memory

- memory change: 0.88x