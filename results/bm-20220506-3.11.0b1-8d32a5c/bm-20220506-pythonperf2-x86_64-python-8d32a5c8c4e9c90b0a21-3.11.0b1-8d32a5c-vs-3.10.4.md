
# Results vs. 3.10.4

- fork: python
- ref: 8d32a5c8c4e9c90b0a21
- machine: linux-x86_64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 281 ms: 1.24x faster                                                        |
| chameleon      | 9.44 ms                                                      | 7.53 ms: 1.25x faster                                                       |
| docutils       | 3.41 sec                                                     | 2.82 sec: 1.21x faster                                                      |
| html5lib       | 94.6 ms                                                      | 69.0 ms: 1.37x faster                                                       |
| tornado_http   | 157 ms                                                       | 121 ms: 1.30x faster                                                        |
| Geometric mean | (ref)                                                        | 1.27x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.37x faster                                                      |
| async_tree_none         | 692 ms                                                       | 516 ms: 1.34x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 624 ms: 1.31x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 748 ms: 1.25x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.32x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 74.7 ms: 1.49x faster                                                       |
| nbody          | 134 ms                                                       | 100 ms: 1.34x faster                                                        |
| pidigits       | 271 ms                                                       | 251 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                        | 1.29x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 153 ms: 1.25x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 22.8 ms: 1.19x faster                                                       |
| regex_dna      | 261 ms                                                       | 232 ms: 1.13x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 2.97 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                        | 1.15x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 320 us: 1.42x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 56.1 ms: 1.35x faster                                                       |
| unpickle_pure_python | 312 us                                                       | 233 us: 1.34x faster                                                        |
| json_loads           | 30.3 us                                                      | 24.6 us: 1.23x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 80.3 ms: 1.15x faster                                                       |
| pickle_list          | 4.12 us                                                      | 3.81 us: 1.08x faster                                                       |
| json_dumps           | 14.5 ms                                                      | 13.5 ms: 1.08x faster                                                       |
| xml_etree_iterparse  | 110 ms                                                       | 105 ms: 1.06x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 155 ms: 1.03x faster                                                        |
| pickle               | 9.89 us                                                      | 9.62 us: 1.03x faster                                                       |
| unpickle_list        | 4.65 us                                                      | 4.56 us: 1.02x faster                                                       |
| unpickle             | 13.5 us                                                      | 13.3 us: 1.02x faster                                                       |
| pickle_dict          | 29.5 us                                                      | 29.9 us: 1.01x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.5 ms: 1.09x faster                                                       |
| python_startup_no_site | 7.33 ms                                                      | 7.68 ms: 1.05x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.9 ms: 1.35x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 25.4 ms: 1.24x faster                                                       |
| django_template | 50.2 ms                                                      | 41.3 ms: 1.22x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 56.7 ms: 1.12x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.23x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 3.93 ms: 1.91x faster                                                       |
| pyflate                 | 733 ms                                                       | 433 ms: 1.69x faster                                                        |
| logging_silent          | 167 ns                                                       | 99.8 ns: 1.68x faster                                                       |
| go                      | 262 ms                                                       | 156 ms: 1.67x faster                                                        |
| scimark_sor             | 180 ms                                                       | 110 ms: 1.64x faster                                                        |
| raytrace                | 489 ms                                                       | 309 ms: 1.58x faster                                                        |
| scimark_monte_carlo     | 107 ms                                                       | 69.2 ms: 1.55x faster                                                       |
| chaos                   | 109 ms                                                       | 72.4 ms: 1.50x faster                                                       |
| richards                | 75.1 ms                                                      | 50.1 ms: 1.50x faster                                                       |
| spectral_norm           | 139 ms                                                       | 93.1 ms: 1.49x faster                                                       |
| float                   | 111 ms                                                       | 74.7 ms: 1.49x faster                                                       |
| scimark_lu              | 167 ms                                                       | 114 ms: 1.46x faster                                                        |
| crypto_pyaes            | 119 ms                                                       | 82.3 ms: 1.45x faster                                                       |
| pickle_pure_python      | 455 us                                                       | 320 us: 1.42x faster                                                        |
| bench_mp_pool           | 6.37 ms                                                      | 4.56 ms: 1.40x faster                                                       |
| pprint_safe_repr        | 1.05 sec                                                     | 755 ms: 1.39x faster                                                        |
| pprint_pformat          | 2.15 sec                                                     | 1.57 sec: 1.37x faster                                                      |
| html5lib                | 94.6 ms                                                      | 69.0 ms: 1.37x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.37x faster                                                      |
| hexiom                  | 9.42 ms                                                      | 6.91 ms: 1.36x faster                                                       |
| xml_etree_process       | 75.9 ms                                                      | 56.1 ms: 1.35x faster                                                       |
| mako                    | 14.7 ms                                                      | 10.9 ms: 1.35x faster                                                       |
| nbody                   | 134 ms                                                       | 100 ms: 1.34x faster                                                        |
| async_tree_none         | 692 ms                                                       | 516 ms: 1.34x faster                                                        |
| unpickle_pure_python    | 312 us                                                       | 233 us: 1.34x faster                                                        |
| pycparser               | 1.67 sec                                                     | 1.26 sec: 1.33x faster                                                      |
| deepcopy_memo           | 49.8 us                                                      | 37.6 us: 1.32x faster                                                       |
| async_generators        | 421 ms                                                       | 318 ms: 1.32x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 624 ms: 1.31x faster                                                        |
| unpack_sequence         | 59.9 ns                                                      | 46.2 ns: 1.30x faster                                                       |
| tornado_http            | 157 ms                                                       | 121 ms: 1.30x faster                                                        |
| thrift                  | 1.18 ms                                                      | 913 us: 1.29x faster                                                        |
| logging_simple          | 8.88 us                                                      | 6.90 us: 1.29x faster                                                       |
| aiohttp                 | 1.19 ms                                                      | 945 us: 1.26x faster                                                        |
| logging_format          | 9.64 us                                                      | 7.67 us: 1.26x faster                                                       |
| chameleon               | 9.44 ms                                                      | 7.53 ms: 1.25x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 748 ms: 1.25x faster                                                        |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 4.06 ms: 1.25x faster                                                       |
| gunicorn                | 1.16 ms                                                      | 928 us: 1.25x faster                                                        |
| regex_compile           | 190 ms                                                       | 153 ms: 1.25x faster                                                        |
| 2to3                    | 350 ms                                                       | 281 ms: 1.24x faster                                                        |
| genshi_text             | 31.4 ms                                                      | 25.4 ms: 1.24x faster                                                       |
| sqlalchemy_declarative  | 190 ms                                                       | 153 ms: 1.24x faster                                                        |
| json_loads              | 30.3 us                                                      | 24.6 us: 1.23x faster                                                       |
| scimark_fft             | 361 ms                                                       | 294 ms: 1.23x faster                                                        |
| django_template         | 50.2 ms                                                      | 41.3 ms: 1.22x faster                                                       |
| sqlglot_normalize       | 144 ms                                                       | 119 ms: 1.21x faster                                                        |
| docutils                | 3.41 sec                                                     | 2.82 sec: 1.21x faster                                                      |
| nqueens                 | 115 ms                                                       | 95.8 ms: 1.20x faster                                                       |
| dulwich_log             | 81.1 ms                                                      | 68.0 ms: 1.19x faster                                                       |
| regex_v8                | 27.2 ms                                                      | 22.8 ms: 1.19x faster                                                       |
| sqlglot_optimize        | 70.1 ms                                                      | 58.9 ms: 1.19x faster                                                       |
| sqlite_synth            | 2.99 us                                                      | 2.51 us: 1.19x faster                                                       |
| deepcopy                | 468 us                                                       | 394 us: 1.19x faster                                                        |
| deepcopy_reduce         | 4.01 us                                                      | 3.42 us: 1.17x faster                                                       |
| sqlalchemy_imperative   | 22.7 ms                                                      | 19.5 ms: 1.16x faster                                                       |
| sqlglot_transpile       | 2.68 ms                                                      | 2.30 ms: 1.16x faster                                                       |
| fannkuch                | 483 ms                                                       | 418 ms: 1.15x faster                                                        |
| flaskblogging           | 4.39 ms                                                      | 3.82 ms: 1.15x faster                                                       |
| sqlglot_parse           | 2.24 ms                                                      | 1.95 ms: 1.15x faster                                                       |
| xml_etree_generate      | 92.3 ms                                                      | 80.3 ms: 1.15x faster                                                       |
| json                    | 5.86 ms                                                      | 5.14 ms: 1.14x faster                                                       |
| pathlib                 | 21.4 ms                                                      | 18.8 ms: 1.14x faster                                                       |
| dask                    | 472 ms                                                       | 418 ms: 1.13x faster                                                        |
| regex_dna               | 261 ms                                                       | 232 ms: 1.13x faster                                                        |
| pylint                  | 566 ms                                                       | 505 ms: 1.12x faster                                                        |
| sympy_integrate         | 28.2 ms                                                      | 25.2 ms: 1.12x faster                                                       |
| bench_thread_pool       | 1.14 ms                                                      | 1.02 ms: 1.12x faster                                                       |
| genshi_xml              | 63.3 ms                                                      | 56.7 ms: 1.12x faster                                                       |
| sympy_expand            | 600 ms                                                       | 540 ms: 1.11x faster                                                        |
| sympy_str               | 360 ms                                                       | 329 ms: 1.09x faster                                                        |
| python_startup          | 11.5 ms                                                      | 10.5 ms: 1.09x faster                                                       |
| coroutines              | 30.3 ms                                                      | 28.0 ms: 1.08x faster                                                       |
| pickle_list             | 4.12 us                                                      | 3.81 us: 1.08x faster                                                       |
| sympy_sum               | 193 ms                                                       | 178 ms: 1.08x faster                                                        |
| mdp                     | 3.01 sec                                                     | 2.78 sec: 1.08x faster                                                      |
| json_dumps              | 14.5 ms                                                      | 13.5 ms: 1.08x faster                                                       |
| pidigits                | 271 ms                                                       | 251 ms: 1.08x faster                                                        |
| create_gc_cycles        | 1.76 ms                                                      | 1.64 ms: 1.07x faster                                                       |
| xml_etree_iterparse     | 110 ms                                                       | 105 ms: 1.06x faster                                                        |
| meteor_contest          | 138 ms                                                       | 131 ms: 1.05x faster                                                        |
| regex_effbot            | 3.09 ms                                                      | 2.97 ms: 1.04x faster                                                       |
| asyncio_tcp             | 779 ms                                                       | 749 ms: 1.04x faster                                                        |
| telco                   | 7.23 ms                                                      | 6.99 ms: 1.03x faster                                                       |
| generators              | 57.3 ms                                                      | 55.5 ms: 1.03x faster                                                       |
| xml_etree_parse         | 160 ms                                                       | 155 ms: 1.03x faster                                                        |
| pickle                  | 9.89 us                                                      | 9.62 us: 1.03x faster                                                       |
| unpickle_list           | 4.65 us                                                      | 4.56 us: 1.02x faster                                                       |
| unpickle                | 13.5 us                                                      | 13.3 us: 1.02x faster                                                       |
| pickle_dict             | 29.5 us                                                      | 29.9 us: 1.01x slower                                                       |
| python_startup_no_site  | 7.33 ms                                                      | 7.68 ms: 1.05x slower                                                       |
| comprehensions          | 26.7 us                                                      | 28.2 us: 1.06x slower                                                       |
| gc_traversal            | 3.42 ms                                                      | 3.85 ms: 1.13x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.23x faster                                                                |
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.09x