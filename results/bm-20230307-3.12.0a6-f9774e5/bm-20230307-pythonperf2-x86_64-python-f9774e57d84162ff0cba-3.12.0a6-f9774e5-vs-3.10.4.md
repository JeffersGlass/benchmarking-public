
# Results vs. 3.10.4

- fork: python
- ref: f9774e57d84162ff0cba
- machine: linux-x86_64
- commit hash: f9774e5
- commit date: 2023-03-07
- overall geometric mean: 1.26x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: 1.23x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 284 ms: 1.23x faster                                                        |
| chameleon      | 9.44 ms                                                      | 6.94 ms: 1.36x faster                                                       |
| docutils       | 3.41 sec                                                     | 2.79 sec: 1.22x faster                                                      |
| html5lib       | 94.6 ms                                                      | 65.9 ms: 1.44x faster                                                       |
| tornado_http   | 157 ms                                                       | 115 ms: 1.36x faster                                                        |
| Geometric mean | (ref)                                                        | 1.32x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.37x faster                                                      |
| async_tree_none         | 692 ms                                                       | 510 ms: 1.36x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 611 ms: 1.34x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 745 ms: 1.26x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.33x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 73.9 ms: 1.50x faster                                                       |
| nbody          | 134 ms                                                       | 91.0 ms: 1.47x faster                                                       |
| pidigits       | 271 ms                                                       | 251 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                        | 1.34x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 146 ms: 1.30x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 22.8 ms: 1.19x faster                                                       |
| regex_dna      | 261 ms                                                       | 225 ms: 1.16x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.36 ms: 1.09x slower                                                       |
| Geometric mean | (ref)                                                        | 1.13x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 202 us: 1.54x faster                                                        |
| pickle_pure_python   | 455 us                                                       | 306 us: 1.49x faster                                                        |
| json_dumps           | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 57.3 ms: 1.33x faster                                                       |
| json_loads           | 30.3 us                                                      | 24.4 us: 1.24x faster                                                       |
| xml_etree_parse      | 160 ms                                                       | 144 ms: 1.11x faster                                                        |
| xml_etree_generate   | 92.3 ms                                                      | 83.5 ms: 1.11x faster                                                       |
| pickle_list          | 4.12 us                                                      | 3.80 us: 1.08x faster                                                       |
| xml_etree_iterparse  | 110 ms                                                       | 103 ms: 1.07x faster                                                        |
| unpickle_list        | 4.65 us                                                      | 4.44 us: 1.05x faster                                                       |
| pickle               | 9.89 us                                                      | 10.0 us: 1.01x slower                                                       |
| pickle_dict          | 29.5 us                                                      | 31.8 us: 1.08x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.17x faster                                                                |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 11.3 ms: 1.02x faster                                                       |
| python_startup_no_site | 7.33 ms                                                      | 8.34 ms: 1.14x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.0 ms: 1.46x faster                                                       |
| django_template | 50.2 ms                                                      | 39.1 ms: 1.28x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 24.6 ms: 1.28x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 53.0 ms: 1.19x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.30x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230307-pythonperf2-x86_64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 3.33 ms: 2.25x faster                                                       |
| asyncio_tcp             | 779 ms                                                       | 382 ms: 2.04x faster                                                        |
| logging_silent          | 167 ns                                                       | 94.5 ns: 1.77x faster                                                       |
| go                      | 262 ms                                                       | 151 ms: 1.74x faster                                                        |
| scimark_sor             | 180 ms                                                       | 105 ms: 1.71x faster                                                        |
| pyflate                 | 733 ms                                                       | 432 ms: 1.70x faster                                                        |
| raytrace                | 489 ms                                                       | 290 ms: 1.69x faster                                                        |
| richards                | 75.1 ms                                                      | 46.4 ms: 1.62x faster                                                       |
| scimark_lu              | 167 ms                                                       | 105 ms: 1.59x faster                                                        |
| scimark_monte_carlo     | 107 ms                                                       | 69.5 ms: 1.54x faster                                                       |
| unpickle_pure_python    | 312 us                                                       | 202 us: 1.54x faster                                                        |
| chaos                   | 109 ms                                                       | 70.9 ms: 1.53x faster                                                       |
| float                   | 111 ms                                                       | 73.9 ms: 1.50x faster                                                       |
| generators              | 57.3 ms                                                      | 38.4 ms: 1.49x faster                                                       |
| pickle_pure_python      | 455 us                                                       | 306 us: 1.49x faster                                                        |
| nbody                   | 134 ms                                                       | 91.0 ms: 1.47x faster                                                       |
| mako                    | 14.7 ms                                                      | 10.0 ms: 1.46x faster                                                       |
| crypto_pyaes            | 119 ms                                                       | 81.5 ms: 1.46x faster                                                       |
| hexiom                  | 9.42 ms                                                      | 6.46 ms: 1.46x faster                                                       |
| spectral_norm           | 139 ms                                                       | 95.6 ms: 1.45x faster                                                       |
| html5lib                | 94.6 ms                                                      | 65.9 ms: 1.44x faster                                                       |
| json_dumps              | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                                       |
| sqlglot_parse           | 2.24 ms                                                      | 1.58 ms: 1.42x faster                                                       |
| deepcopy_memo           | 49.8 us                                                      | 35.4 us: 1.41x faster                                                       |
| pprint_pformat          | 2.15 sec                                                     | 1.55 sec: 1.39x faster                                                      |
| sqlglot_transpile       | 2.68 ms                                                      | 1.94 ms: 1.38x faster                                                       |
| pprint_safe_repr        | 1.05 sec                                                     | 762 ms: 1.38x faster                                                        |
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.37x faster                                                      |
| tornado_http            | 157 ms                                                       | 115 ms: 1.36x faster                                                        |
| chameleon               | 9.44 ms                                                      | 6.94 ms: 1.36x faster                                                       |
| pycparser               | 1.67 sec                                                     | 1.23 sec: 1.36x faster                                                      |
| async_tree_none         | 692 ms                                                       | 510 ms: 1.36x faster                                                        |
| unpack_sequence         | 59.9 ns                                                      | 44.4 ns: 1.35x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 611 ms: 1.34x faster                                                        |
| xml_etree_process       | 75.9 ms                                                      | 57.3 ms: 1.33x faster                                                       |
| bench_mp_pool           | 6.37 ms                                                      | 4.84 ms: 1.32x faster                                                       |
| logging_simple          | 8.88 us                                                      | 6.79 us: 1.31x faster                                                       |
| regex_compile           | 190 ms                                                       | 146 ms: 1.30x faster                                                        |
| scimark_fft             | 361 ms                                                       | 278 ms: 1.30x faster                                                        |
| thrift                  | 1.18 ms                                                      | 909 us: 1.29x faster                                                        |
| django_template         | 50.2 ms                                                      | 39.1 ms: 1.28x faster                                                       |
| genshi_text             | 31.4 ms                                                      | 24.6 ms: 1.28x faster                                                       |
| dulwich_log             | 81.1 ms                                                      | 63.7 ms: 1.27x faster                                                       |
| logging_format          | 9.64 us                                                      | 7.59 us: 1.27x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 745 ms: 1.26x faster                                                        |
| json_loads              | 30.3 us                                                      | 24.4 us: 1.24x faster                                                       |
| deepcopy                | 468 us                                                       | 377 us: 1.24x faster                                                        |
| 2to3                    | 350 ms                                                       | 284 ms: 1.23x faster                                                        |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 4.14 ms: 1.23x faster                                                       |
| coroutines              | 30.3 ms                                                      | 24.7 ms: 1.23x faster                                                       |
| docutils                | 3.41 sec                                                     | 2.79 sec: 1.22x faster                                                      |
| sqlglot_optimize        | 70.1 ms                                                      | 58.2 ms: 1.21x faster                                                       |
| deepcopy_reduce         | 4.01 us                                                      | 3.33 us: 1.20x faster                                                       |
| sqlglot_normalize       | 144 ms                                                       | 120 ms: 1.20x faster                                                        |
| genshi_xml              | 63.3 ms                                                      | 53.0 ms: 1.19x faster                                                       |
| regex_v8                | 27.2 ms                                                      | 22.8 ms: 1.19x faster                                                       |
| nqueens                 | 115 ms                                                       | 96.9 ms: 1.19x faster                                                       |
| fannkuch                | 483 ms                                                       | 408 ms: 1.18x faster                                                        |
| mdp                     | 3.01 sec                                                     | 2.54 sec: 1.18x faster                                                      |
| json                    | 5.86 ms                                                      | 5.00 ms: 1.17x faster                                                       |
| bench_thread_pool       | 1.14 ms                                                      | 974 us: 1.17x faster                                                        |
| regex_dna               | 261 ms                                                       | 225 ms: 1.16x faster                                                        |
| pathlib                 | 21.4 ms                                                      | 18.5 ms: 1.15x faster                                                       |
| sqlite_synth            | 2.99 us                                                      | 2.63 us: 1.14x faster                                                       |
| sympy_integrate         | 28.2 ms                                                      | 25.0 ms: 1.13x faster                                                       |
| sympy_expand            | 600 ms                                                       | 538 ms: 1.12x faster                                                        |
| xml_etree_parse         | 160 ms                                                       | 144 ms: 1.11x faster                                                        |
| xml_etree_generate      | 92.3 ms                                                      | 83.5 ms: 1.11x faster                                                       |
| sympy_str               | 360 ms                                                       | 328 ms: 1.10x faster                                                        |
| async_generators        | 421 ms                                                       | 385 ms: 1.09x faster                                                        |
| pickle_list             | 4.12 us                                                      | 3.80 us: 1.08x faster                                                       |
| create_gc_cycles        | 1.76 ms                                                      | 1.63 ms: 1.08x faster                                                       |
| pidigits                | 271 ms                                                       | 251 ms: 1.08x faster                                                        |
| meteor_contest          | 138 ms                                                       | 128 ms: 1.08x faster                                                        |
| xml_etree_iterparse     | 110 ms                                                       | 103 ms: 1.07x faster                                                        |
| telco                   | 7.23 ms                                                      | 6.90 ms: 1.05x faster                                                       |
| unpickle_list           | 4.65 us                                                      | 4.44 us: 1.05x faster                                                       |
| sympy_sum               | 193 ms                                                       | 184 ms: 1.05x faster                                                        |
| python_startup          | 11.5 ms                                                      | 11.3 ms: 1.02x faster                                                       |
| pickle                  | 9.89 us                                                      | 10.0 us: 1.01x slower                                                       |
| pickle_dict             | 29.5 us                                                      | 31.8 us: 1.08x slower                                                       |
| regex_effbot            | 3.09 ms                                                      | 3.36 ms: 1.09x slower                                                       |
| python_startup_no_site  | 7.33 ms                                                      | 8.34 ms: 1.14x slower                                                       |
| gc_traversal            | 3.42 ms                                                      | 3.99 ms: 1.17x slower                                                       |
| dask                    | 472 ms                                                       | 560 ms: 1.19x slower                                                        |
| coverage                | 63.3 ms                                                      | 82.2 ms: 1.30x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.26x faster                                                                |

Benchmark hidden because not significant (2): unpickle, comprehensions
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: 1.23x