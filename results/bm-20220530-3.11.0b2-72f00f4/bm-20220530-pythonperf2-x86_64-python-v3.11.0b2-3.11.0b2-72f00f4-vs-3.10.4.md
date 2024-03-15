
# Results vs. 3.10.4

- fork: python
- ref: v3.11.0b2
- machine: linux-x86_64
- commit hash: 72f00f4
- commit date: 2022-05-30
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 282 ms: 1.24x faster                                             |
| chameleon      | 9.44 ms                                                      | 7.52 ms: 1.26x faster                                            |
| docutils       | 3.41 sec                                                     | 2.83 sec: 1.21x faster                                           |
| html5lib       | 94.6 ms                                                      | 70.5 ms: 1.34x faster                                            |
| tornado_http   | 157 ms                                                       | 117 ms: 1.34x faster                                             |
| Geometric mean | (ref)                                                        | 1.28x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.16 sec: 1.37x faster                                           |
| async_tree_none         | 692 ms                                                       | 511 ms: 1.35x faster                                             |
| async_tree_memoization  | 819 ms                                                       | 609 ms: 1.35x faster                                             |
| async_tree_cpu_io_mixed | 936 ms                                                       | 740 ms: 1.26x faster                                             |
| Geometric mean          | (ref)                                                        | 1.33x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| float          | 111 ms                                                       | 73.8 ms: 1.51x faster                                            |
| nbody          | 134 ms                                                       | 96.9 ms: 1.38x faster                                            |
| pidigits       | 271 ms                                                       | 251 ms: 1.08x faster                                             |
| Geometric mean | (ref)                                                        | 1.31x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 157 ms: 1.21x faster                                             |
| regex_dna      | 261 ms                                                       | 227 ms: 1.15x faster                                             |
| regex_v8       | 27.2 ms                                                      | 24.1 ms: 1.12x faster                                            |
| regex_effbot   | 3.09 ms                                                      | 3.11 ms: 1.01x slower                                            |
| Geometric mean | (ref)                                                        | 1.12x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 320 us: 1.42x faster                                             |
| xml_etree_process    | 75.9 ms                                                      | 55.8 ms: 1.36x faster                                            |
| unpickle_pure_python | 312 us                                                       | 234 us: 1.33x faster                                             |
| json_loads           | 30.3 us                                                      | 25.1 us: 1.21x faster                                            |
| xml_etree_generate   | 92.3 ms                                                      | 79.0 ms: 1.17x faster                                            |
| json_dumps           | 14.5 ms                                                      | 13.3 ms: 1.09x faster                                            |
| pickle_list          | 4.12 us                                                      | 3.86 us: 1.07x faster                                            |
| xml_etree_parse      | 160 ms                                                       | 153 ms: 1.04x faster                                             |
| xml_etree_iterparse  | 110 ms                                                       | 106 ms: 1.04x faster                                             |
| unpickle             | 13.5 us                                                      | 13.3 us: 1.02x faster                                            |
| unpickle_list        | 4.65 us                                                      | 4.57 us: 1.02x faster                                            |
| pickle               | 9.89 us                                                      | 9.77 us: 1.01x faster                                            |
| pickle_dict          | 29.5 us                                                      | 30.4 us: 1.03x slower                                            |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.7 ms: 1.08x faster                                            |
| python_startup_no_site | 7.33 ms                                                      | 7.70 ms: 1.05x slower                                            |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-----------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.9 ms: 1.34x faster                                            |
| genshi_text     | 31.4 ms                                                      | 24.4 ms: 1.29x faster                                            |
| django_template | 50.2 ms                                                      | 39.5 ms: 1.27x faster                                            |
| genshi_xml      | 63.3 ms                                                      | 56.0 ms: 1.13x faster                                            |
| Geometric mean  | (ref)                                                        | 1.26x faster                                                     |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf2-x86_64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 3.98 ms: 1.88x faster                                            |
| pyflate                 | 733 ms                                                       | 431 ms: 1.70x faster                                             |
| go                      | 262 ms                                                       | 154 ms: 1.70x faster                                             |
| logging_silent          | 167 ns                                                       | 98.9 ns: 1.69x faster                                            |
| scimark_sor             | 180 ms                                                       | 108 ms: 1.67x faster                                             |
| raytrace                | 489 ms                                                       | 305 ms: 1.60x faster                                             |
| scimark_monte_carlo     | 107 ms                                                       | 67.5 ms: 1.59x faster                                            |
| richards                | 75.1 ms                                                      | 48.5 ms: 1.55x faster                                            |
| float                   | 111 ms                                                       | 73.8 ms: 1.51x faster                                            |
| chaos                   | 109 ms                                                       | 72.1 ms: 1.51x faster                                            |
| scimark_lu              | 167 ms                                                       | 111 ms: 1.50x faster                                             |
| spectral_norm           | 139 ms                                                       | 93.4 ms: 1.49x faster                                            |
| crypto_pyaes            | 119 ms                                                       | 83.5 ms: 1.43x faster                                            |
| pickle_pure_python      | 455 us                                                       | 320 us: 1.42x faster                                             |
| bench_mp_pool           | 6.37 ms                                                      | 4.55 ms: 1.40x faster                                            |
| nbody                   | 134 ms                                                       | 96.9 ms: 1.38x faster                                            |
| pprint_safe_repr        | 1.05 sec                                                     | 759 ms: 1.38x faster                                             |
| async_tree_io           | 1.60 sec                                                     | 1.16 sec: 1.37x faster                                           |
| pprint_pformat          | 2.15 sec                                                     | 1.57 sec: 1.37x faster                                           |
| xml_etree_process       | 75.9 ms                                                      | 55.8 ms: 1.36x faster                                            |
| async_tree_none         | 692 ms                                                       | 511 ms: 1.35x faster                                             |
| deepcopy_memo           | 49.8 us                                                      | 36.9 us: 1.35x faster                                            |
| hexiom                  | 9.42 ms                                                      | 6.99 ms: 1.35x faster                                            |
| async_tree_memoization  | 819 ms                                                       | 609 ms: 1.35x faster                                             |
| mako                    | 14.7 ms                                                      | 10.9 ms: 1.34x faster                                            |
| async_generators        | 421 ms                                                       | 313 ms: 1.34x faster                                             |
| html5lib                | 94.6 ms                                                      | 70.5 ms: 1.34x faster                                            |
| tornado_http            | 157 ms                                                       | 117 ms: 1.34x faster                                             |
| unpickle_pure_python    | 312 us                                                       | 234 us: 1.33x faster                                             |
| unpack_sequence         | 59.9 ns                                                      | 45.1 ns: 1.33x faster                                            |
| genshi_text             | 31.4 ms                                                      | 24.4 ms: 1.29x faster                                            |
| pycparser               | 1.67 sec                                                     | 1.30 sec: 1.29x faster                                           |
| scimark_fft             | 361 ms                                                       | 284 ms: 1.27x faster                                             |
| django_template         | 50.2 ms                                                      | 39.5 ms: 1.27x faster                                            |
| async_tree_cpu_io_mixed | 936 ms                                                       | 740 ms: 1.26x faster                                             |
| aiohttp                 | 1.19 ms                                                      | 944 us: 1.26x faster                                             |
| thrift                  | 1.18 ms                                                      | 935 us: 1.26x faster                                             |
| chameleon               | 9.44 ms                                                      | 7.52 ms: 1.26x faster                                            |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 4.05 ms: 1.25x faster                                            |
| gunicorn                | 1.16 ms                                                      | 929 us: 1.25x faster                                             |
| 2to3                    | 350 ms                                                       | 282 ms: 1.24x faster                                             |
| sqlalchemy_declarative  | 190 ms                                                       | 153 ms: 1.24x faster                                             |
| logging_format          | 9.64 us                                                      | 7.81 us: 1.23x faster                                            |
| logging_simple          | 8.88 us                                                      | 7.21 us: 1.23x faster                                            |
| deepcopy                | 468 us                                                       | 385 us: 1.21x faster                                             |
| regex_compile           | 190 ms                                                       | 157 ms: 1.21x faster                                             |
| docutils                | 3.41 sec                                                     | 2.83 sec: 1.21x faster                                           |
| json_loads              | 30.3 us                                                      | 25.1 us: 1.21x faster                                            |
| dulwich_log             | 81.1 ms                                                      | 67.2 ms: 1.21x faster                                            |
| nqueens                 | 115 ms                                                       | 97.7 ms: 1.18x faster                                            |
| sqlite_synth            | 2.99 us                                                      | 2.54 us: 1.18x faster                                            |
| sqlglot_optimize        | 70.1 ms                                                      | 59.7 ms: 1.17x faster                                            |
| sqlalchemy_imperative   | 22.7 ms                                                      | 19.4 ms: 1.17x faster                                            |
| sqlglot_transpile       | 2.68 ms                                                      | 2.29 ms: 1.17x faster                                            |
| xml_etree_generate      | 92.3 ms                                                      | 79.0 ms: 1.17x faster                                            |
| sqlglot_normalize       | 144 ms                                                       | 124 ms: 1.16x faster                                             |
| deepcopy_reduce         | 4.01 us                                                      | 3.47 us: 1.16x faster                                            |
| dask                    | 472 ms                                                       | 410 ms: 1.15x faster                                             |
| regex_dna               | 261 ms                                                       | 227 ms: 1.15x faster                                             |
| sqlglot_parse           | 2.24 ms                                                      | 1.95 ms: 1.15x faster                                            |
| bench_thread_pool       | 1.14 ms                                                      | 1.00 ms: 1.14x faster                                            |
| json                    | 5.86 ms                                                      | 5.16 ms: 1.14x faster                                            |
| genshi_xml              | 63.3 ms                                                      | 56.0 ms: 1.13x faster                                            |
| sympy_integrate         | 28.2 ms                                                      | 25.0 ms: 1.13x faster                                            |
| sympy_expand            | 600 ms                                                       | 533 ms: 1.12x faster                                             |
| regex_v8                | 27.2 ms                                                      | 24.1 ms: 1.12x faster                                            |
| pathlib                 | 21.4 ms                                                      | 19.1 ms: 1.12x faster                                            |
| pylint                  | 566 ms                                                       | 510 ms: 1.11x faster                                             |
| sympy_str               | 360 ms                                                       | 327 ms: 1.10x faster                                             |
| json_dumps              | 14.5 ms                                                      | 13.3 ms: 1.09x faster                                            |
| sympy_sum               | 193 ms                                                       | 177 ms: 1.09x faster                                             |
| coroutines              | 30.3 ms                                                      | 27.9 ms: 1.09x faster                                            |
| python_startup          | 11.5 ms                                                      | 10.7 ms: 1.08x faster                                            |
| fannkuch                | 483 ms                                                       | 447 ms: 1.08x faster                                             |
| pidigits                | 271 ms                                                       | 251 ms: 1.08x faster                                             |
| create_gc_cycles        | 1.76 ms                                                      | 1.64 ms: 1.07x faster                                            |
| meteor_contest          | 138 ms                                                       | 129 ms: 1.07x faster                                             |
| pickle_list             | 4.12 us                                                      | 3.86 us: 1.07x faster                                            |
| mdp                     | 3.01 sec                                                     | 2.85 sec: 1.06x faster                                           |
| xml_etree_parse         | 160 ms                                                       | 153 ms: 1.04x faster                                             |
| asyncio_tcp             | 779 ms                                                       | 746 ms: 1.04x faster                                             |
| xml_etree_iterparse     | 110 ms                                                       | 106 ms: 1.04x faster                                             |
| generators              | 57.3 ms                                                      | 55.2 ms: 1.04x faster                                            |
| telco                   | 7.23 ms                                                      | 6.99 ms: 1.03x faster                                            |
| unpickle                | 13.5 us                                                      | 13.3 us: 1.02x faster                                            |
| unpickle_list           | 4.65 us                                                      | 4.57 us: 1.02x faster                                            |
| pickle                  | 9.89 us                                                      | 9.77 us: 1.01x faster                                            |
| regex_effbot            | 3.09 ms                                                      | 3.11 ms: 1.01x slower                                            |
| pickle_dict             | 29.5 us                                                      | 30.4 us: 1.03x slower                                            |
| comprehensions          | 26.7 us                                                      | 27.9 us: 1.05x slower                                            |
| python_startup_no_site  | 7.33 ms                                                      | 7.70 ms: 1.05x slower                                            |
| gc_traversal            | 3.42 ms                                                      | 3.94 ms: 1.15x slower                                            |
| Geometric mean          | (ref)                                                        | 1.23x faster                                                     |
Ignored benchmarks (8) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, coverage, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: 1.09x