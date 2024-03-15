
# Results vs. 3.10.4

- fork: python
- ref: 2e49bd06c5ffab7d1540
- machine: linux-x86_64
- commit hash: 2e49bd0
- commit date: 2022-04-05
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: 1.13x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 293 ms: 1.20x faster                                                        |
| chameleon      | 9.44 ms                                                      | 7.97 ms: 1.18x faster                                                       |
| docutils       | 3.41 sec                                                     | 2.92 sec: 1.17x faster                                                      |
| html5lib       | 94.6 ms                                                      | 75.0 ms: 1.26x faster                                                       |
| tornado_http   | 157 ms                                                       | 123 ms: 1.27x faster                                                        |
| Geometric mean | (ref)                                                        | 1.22x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.18 sec: 1.36x faster                                                      |
| async_tree_none         | 692 ms                                                       | 523 ms: 1.32x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 641 ms: 1.28x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 753 ms: 1.24x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.30x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 93.6 ms: 1.43x faster                                                       |
| float          | 111 ms                                                       | 78.4 ms: 1.42x faster                                                       |
| pidigits       | 271 ms                                                       | 251 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                        | 1.30x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 159 ms: 1.20x faster                                                        |
| regex_dna      | 261 ms                                                       | 253 ms: 1.03x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 26.6 ms: 1.02x faster                                                       |
| regex_effbot   | 3.09 ms                                                      | 3.13 ms: 1.01x slower                                                       |
| Geometric mean | (ref)                                                        | 1.06x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 331 us: 1.37x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 58.3 ms: 1.30x faster                                                       |
| unpickle_pure_python | 312 us                                                       | 242 us: 1.29x faster                                                        |
| json_loads           | 30.3 us                                                      | 24.5 us: 1.24x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 82.8 ms: 1.12x faster                                                       |
| json_dumps           | 14.5 ms                                                      | 13.5 ms: 1.08x faster                                                       |
| xml_etree_iterparse  | 110 ms                                                       | 106 ms: 1.05x faster                                                        |
| unpickle             | 13.5 us                                                      | 13.0 us: 1.04x faster                                                       |
| unpickle_list        | 4.65 us                                                      | 4.52 us: 1.03x faster                                                       |
| xml_etree_parse      | 160 ms                                                       | 157 ms: 1.02x faster                                                        |
| pickle_dict          | 29.5 us                                                      | 31.1 us: 1.06x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.11x faster                                                                |

Benchmark hidden because not significant (2): pickle, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.4 ms: 1.11x faster                                                       |
| python_startup_no_site | 7.33 ms                                                      | 7.46 ms: 1.02x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.04x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 11.2 ms: 1.31x faster                                                       |
| django_template | 50.2 ms                                                      | 40.7 ms: 1.23x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 26.8 ms: 1.17x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 59.7 ms: 1.06x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.19x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220405-pythonperf2-x86_64-python-2e49bd06c5ffab7d1540-3.11.0a7-2e49bd0 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 4.23 ms: 1.77x faster                                                       |
| scimark_sor             | 180 ms                                                       | 112 ms: 1.60x faster                                                        |
| logging_silent          | 167 ns                                                       | 105 ns: 1.60x faster                                                        |
| pyflate                 | 733 ms                                                       | 464 ms: 1.58x faster                                                        |
| go                      | 262 ms                                                       | 166 ms: 1.57x faster                                                        |
| raytrace                | 489 ms                                                       | 322 ms: 1.52x faster                                                        |
| chaos                   | 109 ms                                                       | 73.4 ms: 1.48x faster                                                       |
| nbody                   | 134 ms                                                       | 93.6 ms: 1.43x faster                                                       |
| richards                | 75.1 ms                                                      | 52.8 ms: 1.42x faster                                                       |
| float                   | 111 ms                                                       | 78.4 ms: 1.42x faster                                                       |
| scimark_monte_carlo     | 107 ms                                                       | 77.1 ms: 1.39x faster                                                       |
| scimark_lu              | 167 ms                                                       | 120 ms: 1.39x faster                                                        |
| bench_mp_pool           | 6.37 ms                                                      | 4.60 ms: 1.39x faster                                                       |
| pickle_pure_python      | 455 us                                                       | 331 us: 1.37x faster                                                        |
| async_tree_io           | 1.60 sec                                                     | 1.18 sec: 1.36x faster                                                      |
| crypto_pyaes            | 119 ms                                                       | 89.5 ms: 1.33x faster                                                       |
| logging_simple          | 8.88 us                                                      | 6.69 us: 1.33x faster                                                       |
| async_tree_none         | 692 ms                                                       | 523 ms: 1.32x faster                                                        |
| async_generators        | 421 ms                                                       | 319 ms: 1.32x faster                                                        |
| mako                    | 14.7 ms                                                      | 11.2 ms: 1.31x faster                                                       |
| xml_etree_process       | 75.9 ms                                                      | 58.3 ms: 1.30x faster                                                       |
| spectral_norm           | 139 ms                                                       | 107 ms: 1.30x faster                                                        |
| dask                    | 472 ms                                                       | 367 ms: 1.29x faster                                                        |
| unpickle_pure_python    | 312 us                                                       | 242 us: 1.29x faster                                                        |
| deepcopy_memo           | 49.8 us                                                      | 38.8 us: 1.28x faster                                                       |
| pprint_safe_repr        | 1.05 sec                                                     | 818 ms: 1.28x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 641 ms: 1.28x faster                                                        |
| pprint_pformat          | 2.15 sec                                                     | 1.69 sec: 1.27x faster                                                      |
| tornado_http            | 157 ms                                                       | 123 ms: 1.27x faster                                                        |
| logging_format          | 9.64 us                                                      | 7.59 us: 1.27x faster                                                       |
| unpack_sequence         | 59.9 ns                                                      | 47.3 ns: 1.27x faster                                                       |
| thrift                  | 1.18 ms                                                      | 928 us: 1.27x faster                                                        |
| html5lib                | 94.6 ms                                                      | 75.0 ms: 1.26x faster                                                       |
| pycparser               | 1.67 sec                                                     | 1.33 sec: 1.26x faster                                                      |
| async_tree_cpu_io_mixed | 936 ms                                                       | 753 ms: 1.24x faster                                                        |
| json_loads              | 30.3 us                                                      | 24.5 us: 1.24x faster                                                       |
| django_template         | 50.2 ms                                                      | 40.7 ms: 1.23x faster                                                       |
| hexiom                  | 9.42 ms                                                      | 7.66 ms: 1.23x faster                                                       |
| scimark_fft             | 361 ms                                                       | 297 ms: 1.22x faster                                                        |
| aiohttp                 | 1.19 ms                                                      | 978 us: 1.21x faster                                                        |
| deepcopy                | 468 us                                                       | 385 us: 1.21x faster                                                        |
| gunicorn                | 1.16 ms                                                      | 968 us: 1.20x faster                                                        |
| 2to3                    | 350 ms                                                       | 293 ms: 1.20x faster                                                        |
| regex_compile           | 190 ms                                                       | 159 ms: 1.20x faster                                                        |
| sqlite_synth            | 2.99 us                                                      | 2.52 us: 1.19x faster                                                       |
| sqlalchemy_declarative  | 190 ms                                                       | 160 ms: 1.19x faster                                                        |
| chameleon               | 9.44 ms                                                      | 7.97 ms: 1.18x faster                                                       |
| genshi_text             | 31.4 ms                                                      | 26.8 ms: 1.17x faster                                                       |
| docutils                | 3.41 sec                                                     | 2.92 sec: 1.17x faster                                                      |
| dulwich_log             | 81.1 ms                                                      | 69.8 ms: 1.16x faster                                                       |
| deepcopy_reduce         | 4.01 us                                                      | 3.48 us: 1.15x faster                                                       |
| sqlglot_normalize       | 144 ms                                                       | 127 ms: 1.14x faster                                                        |
| json                    | 5.86 ms                                                      | 5.17 ms: 1.13x faster                                                       |
| sqlglot_optimize        | 70.1 ms                                                      | 61.9 ms: 1.13x faster                                                       |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 4.51 ms: 1.13x faster                                                       |
| nqueens                 | 115 ms                                                       | 102 ms: 1.12x faster                                                        |
| sqlglot_transpile       | 2.68 ms                                                      | 2.38 ms: 1.12x faster                                                       |
| bench_thread_pool       | 1.14 ms                                                      | 1.02 ms: 1.12x faster                                                       |
| flaskblogging           | 4.39 ms                                                      | 3.92 ms: 1.12x faster                                                       |
| xml_etree_generate      | 92.3 ms                                                      | 82.8 ms: 1.12x faster                                                       |
| sympy_integrate         | 28.2 ms                                                      | 25.3 ms: 1.11x faster                                                       |
| python_startup          | 11.5 ms                                                      | 10.4 ms: 1.11x faster                                                       |
| sqlalchemy_imperative   | 22.7 ms                                                      | 20.5 ms: 1.11x faster                                                       |
| pathlib                 | 21.4 ms                                                      | 19.3 ms: 1.10x faster                                                       |
| sqlglot_parse           | 2.24 ms                                                      | 2.04 ms: 1.10x faster                                                       |
| pylint                  | 566 ms                                                       | 517 ms: 1.09x faster                                                        |
| sympy_expand            | 600 ms                                                       | 549 ms: 1.09x faster                                                        |
| fannkuch                | 483 ms                                                       | 442 ms: 1.09x faster                                                        |
| sympy_str               | 360 ms                                                       | 330 ms: 1.09x faster                                                        |
| mdp                     | 3.01 sec                                                     | 2.76 sec: 1.09x faster                                                      |
| sympy_sum               | 193 ms                                                       | 177 ms: 1.09x faster                                                        |
| pidigits                | 271 ms                                                       | 251 ms: 1.08x faster                                                        |
| json_dumps              | 14.5 ms                                                      | 13.5 ms: 1.08x faster                                                       |
| create_gc_cycles        | 1.76 ms                                                      | 1.65 ms: 1.07x faster                                                       |
| telco                   | 7.23 ms                                                      | 6.79 ms: 1.06x faster                                                       |
| genshi_xml              | 63.3 ms                                                      | 59.7 ms: 1.06x faster                                                       |
| generators              | 57.3 ms                                                      | 54.7 ms: 1.05x faster                                                       |
| xml_etree_iterparse     | 110 ms                                                       | 106 ms: 1.05x faster                                                        |
| coroutines              | 30.3 ms                                                      | 29.0 ms: 1.04x faster                                                       |
| asyncio_tcp             | 779 ms                                                       | 746 ms: 1.04x faster                                                        |
| meteor_contest          | 138 ms                                                       | 133 ms: 1.04x faster                                                        |
| unpickle                | 13.5 us                                                      | 13.0 us: 1.04x faster                                                       |
| regex_dna               | 261 ms                                                       | 253 ms: 1.03x faster                                                        |
| unpickle_list           | 4.65 us                                                      | 4.52 us: 1.03x faster                                                       |
| xml_etree_parse         | 160 ms                                                       | 157 ms: 1.02x faster                                                        |
| regex_v8                | 27.2 ms                                                      | 26.6 ms: 1.02x faster                                                       |
| regex_effbot            | 3.09 ms                                                      | 3.13 ms: 1.01x slower                                                       |
| python_startup_no_site  | 7.33 ms                                                      | 7.46 ms: 1.02x slower                                                       |
| comprehensions          | 26.7 us                                                      | 27.8 us: 1.04x slower                                                       |
| gc_traversal            | 3.42 ms                                                      | 3.58 ms: 1.05x slower                                                       |
| pickle_dict             | 29.5 us                                                      | 31.1 us: 1.06x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.19x faster                                                                |

Benchmark hidden because not significant (2): pickle, pickle_list
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: 1.13x