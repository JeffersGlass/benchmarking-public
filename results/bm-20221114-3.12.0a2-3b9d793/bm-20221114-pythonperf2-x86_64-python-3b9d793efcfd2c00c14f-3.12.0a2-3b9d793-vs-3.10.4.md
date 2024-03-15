
# Results vs. 3.10.4

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: linux-x86_64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.25x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 282 ms: 1.24x faster                                                        |
| chameleon      | 9.44 ms                                                      | 7.19 ms: 1.31x faster                                                       |
| docutils       | 3.41 sec                                                     | 2.77 sec: 1.23x faster                                                      |
| html5lib       | 94.6 ms                                                      | 66.7 ms: 1.42x faster                                                       |
| tornado_http   | 157 ms                                                       | 115 ms: 1.36x faster                                                        |
| Geometric mean | (ref)                                                        | 1.31x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.36x faster                                                      |
| async_tree_none         | 692 ms                                                       | 520 ms: 1.33x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 621 ms: 1.32x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 762 ms: 1.23x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.31x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 73.2 ms: 1.52x faster                                                       |
| nbody          | 134 ms                                                       | 90.9 ms: 1.48x faster                                                       |
| pidigits       | 271 ms                                                       | 252 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                        | 1.34x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 147 ms: 1.30x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 23.2 ms: 1.17x faster                                                       |
| regex_dna      | 261 ms                                                       | 227 ms: 1.15x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.45 ms: 1.12x slower                                                       |
| Geometric mean | (ref)                                                        | 1.12x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 209 us: 1.49x faster                                                        |
| pickle_pure_python   | 455 us                                                       | 314 us: 1.45x faster                                                        |
| json_dumps           | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 54.8 ms: 1.39x faster                                                       |
| json_loads           | 30.3 us                                                      | 23.7 us: 1.28x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 79.3 ms: 1.16x faster                                                       |
| pickle_list          | 4.12 us                                                      | 3.65 us: 1.13x faster                                                       |
| xml_etree_parse      | 160 ms                                                       | 143 ms: 1.12x faster                                                        |
| unpickle             | 13.5 us                                                      | 12.6 us: 1.07x faster                                                       |
| unpickle_list        | 4.65 us                                                      | 4.51 us: 1.03x faster                                                       |
| xml_etree_iterparse  | 110 ms                                                       | 108 ms: 1.03x faster                                                        |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                       |
| pickle_dict          | 29.5 us                                                      | 33.4 us: 1.13x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.17x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.8 ms: 1.06x faster                                                       |
| python_startup_no_site | 7.33 ms                                                      | 7.87 ms: 1.07x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.00x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.2 ms: 1.44x faster                                                       |
| django_template | 50.2 ms                                                      | 39.7 ms: 1.26x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 25.2 ms: 1.25x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 54.0 ms: 1.17x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.28x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 3.64 ms: 2.06x faster                                                       |
| scimark_sor             | 180 ms                                                       | 106 ms: 1.69x faster                                                        |
| logging_silent          | 167 ns                                                       | 99.2 ns: 1.69x faster                                                       |
| pyflate                 | 733 ms                                                       | 436 ms: 1.68x faster                                                        |
| richards                | 75.1 ms                                                      | 45.4 ms: 1.66x faster                                                       |
| go                      | 262 ms                                                       | 160 ms: 1.63x faster                                                        |
| scimark_monte_carlo     | 107 ms                                                       | 66.4 ms: 1.62x faster                                                       |
| raytrace                | 489 ms                                                       | 305 ms: 1.60x faster                                                        |
| float                   | 111 ms                                                       | 73.2 ms: 1.52x faster                                                       |
| scimark_lu              | 167 ms                                                       | 111 ms: 1.50x faster                                                        |
| spectral_norm           | 139 ms                                                       | 93.2 ms: 1.49x faster                                                       |
| sqlglot_parse           | 2.24 ms                                                      | 1.50 ms: 1.49x faster                                                       |
| unpickle_pure_python    | 312 us                                                       | 209 us: 1.49x faster                                                        |
| chaos                   | 109 ms                                                       | 72.9 ms: 1.49x faster                                                       |
| crypto_pyaes            | 119 ms                                                       | 80.7 ms: 1.48x faster                                                       |
| nbody                   | 134 ms                                                       | 90.9 ms: 1.48x faster                                                       |
| pickle_pure_python      | 455 us                                                       | 314 us: 1.45x faster                                                        |
| mako                    | 14.7 ms                                                      | 10.2 ms: 1.44x faster                                                       |
| sqlglot_transpile       | 2.68 ms                                                      | 1.87 ms: 1.43x faster                                                       |
| json_dumps              | 14.5 ms                                                      | 10.2 ms: 1.42x faster                                                       |
| html5lib                | 94.6 ms                                                      | 66.7 ms: 1.42x faster                                                       |
| pprint_safe_repr        | 1.05 sec                                                     | 752 ms: 1.40x faster                                                        |
| hexiom                  | 9.42 ms                                                      | 6.76 ms: 1.39x faster                                                       |
| pprint_pformat          | 2.15 sec                                                     | 1.55 sec: 1.39x faster                                                      |
| bench_mp_pool           | 6.37 ms                                                      | 4.59 ms: 1.39x faster                                                       |
| xml_etree_process       | 75.9 ms                                                      | 54.8 ms: 1.39x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.36x faster                                                      |
| tornado_http            | 157 ms                                                       | 115 ms: 1.36x faster                                                        |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 3.74 ms: 1.36x faster                                                       |
| deepcopy_memo           | 49.8 us                                                      | 36.7 us: 1.36x faster                                                       |
| pycparser               | 1.67 sec                                                     | 1.24 sec: 1.35x faster                                                      |
| async_tree_none         | 692 ms                                                       | 520 ms: 1.33x faster                                                        |
| scimark_fft             | 361 ms                                                       | 273 ms: 1.32x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 621 ms: 1.32x faster                                                        |
| aiohttp                 | 1.19 ms                                                      | 904 us: 1.31x faster                                                        |
| chameleon               | 9.44 ms                                                      | 7.19 ms: 1.31x faster                                                       |
| async_generators        | 421 ms                                                       | 321 ms: 1.31x faster                                                        |
| logging_simple          | 8.88 us                                                      | 6.78 us: 1.31x faster                                                       |
| unpack_sequence         | 59.9 ns                                                      | 45.8 ns: 1.31x faster                                                       |
| gunicorn                | 1.16 ms                                                      | 886 us: 1.31x faster                                                        |
| regex_compile           | 190 ms                                                       | 147 ms: 1.30x faster                                                        |
| thrift                  | 1.18 ms                                                      | 913 us: 1.29x faster                                                        |
| json_loads              | 30.3 us                                                      | 23.7 us: 1.28x faster                                                       |
| logging_format          | 9.64 us                                                      | 7.60 us: 1.27x faster                                                       |
| django_template         | 50.2 ms                                                      | 39.7 ms: 1.26x faster                                                       |
| genshi_text             | 31.4 ms                                                      | 25.2 ms: 1.25x faster                                                       |
| 2to3                    | 350 ms                                                       | 282 ms: 1.24x faster                                                        |
| fannkuch                | 483 ms                                                       | 391 ms: 1.23x faster                                                        |
| docutils                | 3.41 sec                                                     | 2.77 sec: 1.23x faster                                                      |
| async_tree_cpu_io_mixed | 936 ms                                                       | 762 ms: 1.23x faster                                                        |
| deepcopy                | 468 us                                                       | 387 us: 1.21x faster                                                        |
| dulwich_log             | 81.1 ms                                                      | 67.2 ms: 1.21x faster                                                       |
| sqlglot_optimize        | 70.1 ms                                                      | 58.2 ms: 1.20x faster                                                       |
| json                    | 5.86 ms                                                      | 4.95 ms: 1.19x faster                                                       |
| deepcopy_reduce         | 4.01 us                                                      | 3.39 us: 1.18x faster                                                       |
| bench_thread_pool       | 1.14 ms                                                      | 969 us: 1.18x faster                                                        |
| sqlglot_normalize       | 144 ms                                                       | 122 ms: 1.18x faster                                                        |
| genshi_xml              | 63.3 ms                                                      | 54.0 ms: 1.17x faster                                                       |
| regex_v8                | 27.2 ms                                                      | 23.2 ms: 1.17x faster                                                       |
| sqlite_synth            | 2.99 us                                                      | 2.57 us: 1.16x faster                                                       |
| xml_etree_generate      | 92.3 ms                                                      | 79.3 ms: 1.16x faster                                                       |
| regex_dna               | 261 ms                                                       | 227 ms: 1.15x faster                                                        |
| dask                    | 472 ms                                                       | 410 ms: 1.15x faster                                                        |
| pickle_list             | 4.12 us                                                      | 3.65 us: 1.13x faster                                                       |
| xml_etree_parse         | 160 ms                                                       | 143 ms: 1.12x faster                                                        |
| nqueens                 | 115 ms                                                       | 103 ms: 1.12x faster                                                        |
| pathlib                 | 21.4 ms                                                      | 19.3 ms: 1.11x faster                                                       |
| sympy_integrate         | 28.2 ms                                                      | 25.5 ms: 1.10x faster                                                       |
| create_gc_cycles        | 1.76 ms                                                      | 1.60 ms: 1.10x faster                                                       |
| mdp                     | 3.01 sec                                                     | 2.73 sec: 1.10x faster                                                      |
| telco                   | 7.23 ms                                                      | 6.58 ms: 1.10x faster                                                       |
| sympy_expand            | 600 ms                                                       | 550 ms: 1.09x faster                                                        |
| coroutines              | 30.3 ms                                                      | 27.9 ms: 1.09x faster                                                       |
| meteor_contest          | 138 ms                                                       | 129 ms: 1.08x faster                                                        |
| pidigits                | 271 ms                                                       | 252 ms: 1.08x faster                                                        |
| unpickle                | 13.5 us                                                      | 12.6 us: 1.07x faster                                                       |
| sympy_str               | 360 ms                                                       | 337 ms: 1.07x faster                                                        |
| python_startup          | 11.5 ms                                                      | 10.8 ms: 1.06x faster                                                       |
| sympy_sum               | 193 ms                                                       | 184 ms: 1.05x faster                                                        |
| asyncio_tcp             | 779 ms                                                       | 749 ms: 1.04x faster                                                        |
| unpickle_list           | 4.65 us                                                      | 4.51 us: 1.03x faster                                                       |
| xml_etree_iterparse     | 110 ms                                                       | 108 ms: 1.03x faster                                                        |
| comprehensions          | 26.7 us                                                      | 26.9 us: 1.01x slower                                                       |
| pickle                  | 9.89 us                                                      | 10.1 us: 1.02x slower                                                       |
| generators              | 57.3 ms                                                      | 61.2 ms: 1.07x slower                                                       |
| python_startup_no_site  | 7.33 ms                                                      | 7.87 ms: 1.07x slower                                                       |
| regex_effbot            | 3.09 ms                                                      | 3.45 ms: 1.12x slower                                                       |
| pickle_dict             | 29.5 us                                                      | 33.4 us: 1.13x slower                                                       |
| gc_traversal            | 3.42 ms                                                      | 3.92 ms: 1.15x slower                                                       |
| coverage                | 63.3 ms                                                      | 86.9 ms: 1.37x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.25x faster                                                                |
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.10x