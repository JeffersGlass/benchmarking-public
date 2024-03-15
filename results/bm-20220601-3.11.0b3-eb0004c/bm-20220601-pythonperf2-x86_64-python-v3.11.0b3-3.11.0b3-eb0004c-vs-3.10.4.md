
# Results vs. 3.10.4

- fork: python
- ref: v3.11.0b3
- machine: linux-x86_64
- commit hash: eb0004c
- commit date: 2022-06-01
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 284 ms: 1.23x faster                                             |
| chameleon      | 9.44 ms                                                      | 7.60 ms: 1.24x faster                                            |
| docutils       | 3.41 sec                                                     | 2.83 sec: 1.21x faster                                           |
| html5lib       | 94.6 ms                                                      | 71.0 ms: 1.33x faster                                            |
| tornado_http   | 157 ms                                                       | 119 ms: 1.32x faster                                             |
| Geometric mean | (ref)                                                        | 1.27x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.37x faster                                           |
| async_tree_none         | 692 ms                                                       | 513 ms: 1.35x faster                                             |
| async_tree_memoization  | 819 ms                                                       | 617 ms: 1.33x faster                                             |
| async_tree_cpu_io_mixed | 936 ms                                                       | 810 ms: 1.16x faster                                             |
| Geometric mean          | (ref)                                                        | 1.30x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| float          | 111 ms                                                       | 73.9 ms: 1.50x faster                                            |
| nbody          | 134 ms                                                       | 93.0 ms: 1.44x faster                                            |
| pidigits       | 271 ms                                                       | 252 ms: 1.08x faster                                             |
| Geometric mean | (ref)                                                        | 1.33x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 156 ms: 1.22x faster                                             |
| regex_dna      | 261 ms                                                       | 219 ms: 1.19x faster                                             |
| regex_v8       | 27.2 ms                                                      | 24.3 ms: 1.12x faster                                            |
| regex_effbot   | 3.09 ms                                                      | 3.05 ms: 1.01x faster                                            |
| Geometric mean | (ref)                                                        | 1.13x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 319 us: 1.43x faster                                             |
| xml_etree_process    | 75.9 ms                                                      | 55.9 ms: 1.36x faster                                            |
| unpickle_pure_python | 312 us                                                       | 238 us: 1.31x faster                                             |
| json_loads           | 30.3 us                                                      | 25.2 us: 1.20x faster                                            |
| xml_etree_generate   | 92.3 ms                                                      | 80.2 ms: 1.15x faster                                            |
| json_dumps           | 14.5 ms                                                      | 13.5 ms: 1.08x faster                                            |
| xml_etree_iterparse  | 110 ms                                                       | 103 ms: 1.07x faster                                             |
| pickle_list          | 4.12 us                                                      | 3.92 us: 1.05x faster                                            |
| xml_etree_parse      | 160 ms                                                       | 153 ms: 1.04x faster                                             |
| unpickle             | 13.5 us                                                      | 13.2 us: 1.02x faster                                            |
| unpickle_list        | 4.65 us                                                      | 4.58 us: 1.01x faster                                            |
| pickle               | 9.89 us                                                      | 9.80 us: 1.01x faster                                            |
| pickle_dict          | 29.5 us                                                      | 31.3 us: 1.06x slower                                            |
| Geometric mean       | (ref)                                                        | 1.12x faster                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.7 ms: 1.08x faster                                            |
| python_startup_no_site | 7.33 ms                                                      | 7.70 ms: 1.05x slower                                            |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.9 ms: 1.34x faster                                            |
| django_template | 50.2 ms                                                      | 41.4 ms: 1.21x faster                                            |
| genshi_text     | 31.4 ms                                                      | 26.3 ms: 1.19x faster                                            |
| genshi_xml      | 63.3 ms                                                      | 60.1 ms: 1.05x faster                                            |
| Geometric mean  | (ref)                                                        | 1.20x faster                                                     |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf2-x86_64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 4.20 ms: 1.78x faster                                            |
| logging_silent          | 167 ns                                                       | 99.3 ns: 1.68x faster                                            |
| pyflate                 | 733 ms                                                       | 441 ms: 1.66x faster                                             |
| scimark_sor             | 180 ms                                                       | 112 ms: 1.61x faster                                             |
| raytrace                | 489 ms                                                       | 304 ms: 1.61x faster                                             |
| go                      | 262 ms                                                       | 166 ms: 1.58x faster                                             |
| scimark_monte_carlo     | 107 ms                                                       | 69.5 ms: 1.55x faster                                            |
| richards                | 75.1 ms                                                      | 49.2 ms: 1.53x faster                                            |
| scimark_lu              | 167 ms                                                       | 110 ms: 1.52x faster                                             |
| float                   | 111 ms                                                       | 73.9 ms: 1.50x faster                                            |
| chaos                   | 109 ms                                                       | 73.6 ms: 1.48x faster                                            |
| nbody                   | 134 ms                                                       | 93.0 ms: 1.44x faster                                            |
| spectral_norm           | 139 ms                                                       | 96.8 ms: 1.44x faster                                            |
| pickle_pure_python      | 455 us                                                       | 319 us: 1.43x faster                                             |
| crypto_pyaes            | 119 ms                                                       | 84.5 ms: 1.41x faster                                            |
| bench_mp_pool           | 6.37 ms                                                      | 4.52 ms: 1.41x faster                                            |
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.37x faster                                           |
| xml_etree_process       | 75.9 ms                                                      | 55.9 ms: 1.36x faster                                            |
| pprint_safe_repr        | 1.05 sec                                                     | 774 ms: 1.36x faster                                             |
| async_tree_none         | 692 ms                                                       | 513 ms: 1.35x faster                                             |
| hexiom                  | 9.42 ms                                                      | 7.00 ms: 1.35x faster                                            |
| mako                    | 14.7 ms                                                      | 10.9 ms: 1.34x faster                                            |
| pprint_pformat          | 2.15 sec                                                     | 1.61 sec: 1.33x faster                                           |
| html5lib                | 94.6 ms                                                      | 71.0 ms: 1.33x faster                                            |
| async_tree_memoization  | 819 ms                                                       | 617 ms: 1.33x faster                                             |
| async_generators        | 421 ms                                                       | 318 ms: 1.33x faster                                             |
| tornado_http            | 157 ms                                                       | 119 ms: 1.32x faster                                             |
| deepcopy_memo           | 49.8 us                                                      | 37.7 us: 1.32x faster                                            |
| unpack_sequence         | 59.9 ns                                                      | 45.4 ns: 1.32x faster                                            |
| unpickle_pure_python    | 312 us                                                       | 238 us: 1.31x faster                                             |
| thrift                  | 1.18 ms                                                      | 909 us: 1.29x faster                                             |
| pycparser               | 1.67 sec                                                     | 1.31 sec: 1.28x faster                                           |
| scimark_fft             | 361 ms                                                       | 286 ms: 1.26x faster                                             |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 4.03 ms: 1.26x faster                                            |
| gunicorn                | 1.16 ms                                                      | 931 us: 1.24x faster                                             |
| chameleon               | 9.44 ms                                                      | 7.60 ms: 1.24x faster                                            |
| aiohttp                 | 1.19 ms                                                      | 958 us: 1.24x faster                                             |
| logging_simple          | 8.88 us                                                      | 7.16 us: 1.24x faster                                            |
| 2to3                    | 350 ms                                                       | 284 ms: 1.23x faster                                             |
| sqlalchemy_declarative  | 190 ms                                                       | 154 ms: 1.23x faster                                             |
| regex_compile           | 190 ms                                                       | 156 ms: 1.22x faster                                             |
| django_template         | 50.2 ms                                                      | 41.4 ms: 1.21x faster                                            |
| logging_format          | 9.64 us                                                      | 7.95 us: 1.21x faster                                            |
| docutils                | 3.41 sec                                                     | 2.83 sec: 1.21x faster                                           |
| json_loads              | 30.3 us                                                      | 25.2 us: 1.20x faster                                            |
| deepcopy                | 468 us                                                       | 390 us: 1.20x faster                                             |
| genshi_text             | 31.4 ms                                                      | 26.3 ms: 1.19x faster                                            |
| regex_dna               | 261 ms                                                       | 219 ms: 1.19x faster                                             |
| sqlite_synth            | 2.99 us                                                      | 2.51 us: 1.19x faster                                            |
| dulwich_log             | 81.1 ms                                                      | 68.4 ms: 1.19x faster                                            |
| sqlglot_optimize        | 70.1 ms                                                      | 59.4 ms: 1.18x faster                                            |
| nqueens                 | 115 ms                                                       | 97.6 ms: 1.18x faster                                            |
| sqlglot_normalize       | 144 ms                                                       | 123 ms: 1.17x faster                                             |
| sqlalchemy_imperative   | 22.7 ms                                                      | 19.6 ms: 1.16x faster                                            |
| async_tree_cpu_io_mixed | 936 ms                                                       | 810 ms: 1.16x faster                                             |
| sqlglot_transpile       | 2.68 ms                                                      | 2.32 ms: 1.16x faster                                            |
| deepcopy_reduce         | 4.01 us                                                      | 3.48 us: 1.15x faster                                            |
| xml_etree_generate      | 92.3 ms                                                      | 80.2 ms: 1.15x faster                                            |
| flaskblogging           | 4.39 ms                                                      | 3.82 ms: 1.15x faster                                            |
| dask                    | 472 ms                                                       | 414 ms: 1.14x faster                                             |
| sqlglot_parse           | 2.24 ms                                                      | 1.97 ms: 1.14x faster                                            |
| sympy_expand            | 600 ms                                                       | 531 ms: 1.13x faster                                             |
| json                    | 5.86 ms                                                      | 5.20 ms: 1.13x faster                                            |
| bench_thread_pool       | 1.14 ms                                                      | 1.01 ms: 1.13x faster                                            |
| sympy_integrate         | 28.2 ms                                                      | 25.2 ms: 1.12x faster                                            |
| regex_v8                | 27.2 ms                                                      | 24.3 ms: 1.12x faster                                            |
| pathlib                 | 21.4 ms                                                      | 19.2 ms: 1.11x faster                                            |
| sympy_str               | 360 ms                                                       | 327 ms: 1.10x faster                                             |
| pylint                  | 566 ms                                                       | 515 ms: 1.10x faster                                             |
| coroutines              | 30.3 ms                                                      | 27.9 ms: 1.09x faster                                            |
| sympy_sum               | 193 ms                                                       | 177 ms: 1.09x faster                                             |
| json_dumps              | 14.5 ms                                                      | 13.5 ms: 1.08x faster                                            |
| python_startup          | 11.5 ms                                                      | 10.7 ms: 1.08x faster                                            |
| pidigits                | 271 ms                                                       | 252 ms: 1.08x faster                                             |
| xml_etree_iterparse     | 110 ms                                                       | 103 ms: 1.07x faster                                             |
| telco                   | 7.23 ms                                                      | 6.75 ms: 1.07x faster                                            |
| mdp                     | 3.01 sec                                                     | 2.81 sec: 1.07x faster                                           |
| meteor_contest          | 138 ms                                                       | 131 ms: 1.06x faster                                             |
| genshi_xml              | 63.3 ms                                                      | 60.1 ms: 1.05x faster                                            |
| create_gc_cycles        | 1.76 ms                                                      | 1.68 ms: 1.05x faster                                            |
| pickle_list             | 4.12 us                                                      | 3.92 us: 1.05x faster                                            |
| xml_etree_parse         | 160 ms                                                       | 153 ms: 1.04x faster                                             |
| asyncio_tcp             | 779 ms                                                       | 751 ms: 1.04x faster                                             |
| generators              | 57.3 ms                                                      | 56.0 ms: 1.02x faster                                            |
| unpickle                | 13.5 us                                                      | 13.2 us: 1.02x faster                                            |
| unpickle_list           | 4.65 us                                                      | 4.58 us: 1.01x faster                                            |
| regex_effbot            | 3.09 ms                                                      | 3.05 ms: 1.01x faster                                            |
| pickle                  | 9.89 us                                                      | 9.80 us: 1.01x faster                                            |
| fannkuch                | 483 ms                                                       | 496 ms: 1.03x slower                                             |
| python_startup_no_site  | 7.33 ms                                                      | 7.70 ms: 1.05x slower                                            |
| comprehensions          | 26.7 us                                                      | 28.3 us: 1.06x slower                                            |
| pickle_dict             | 29.5 us                                                      | 31.3 us: 1.06x slower                                            |
| gc_traversal            | 3.42 ms                                                      | 4.03 ms: 1.18x slower                                            |
| Geometric mean          | (ref)                                                        | 1.21x faster                                                     |
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.09x