
# Results vs. 3.10.4

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: linux-x86_64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.25x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 286 ms: 1.22x faster                                                        |
| chameleon      | 9.44 ms                                                      | 7.31 ms: 1.29x faster                                                       |
| docutils       | 3.41 sec                                                     | 2.78 sec: 1.23x faster                                                      |
| html5lib       | 94.6 ms                                                      | 66.8 ms: 1.42x faster                                                       |
| Geometric mean | (ref)                                                        | 1.29x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.15 sec: 1.38x faster                                                      |
| async_tree_none         | 692 ms                                                       | 505 ms: 1.37x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 608 ms: 1.35x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 742 ms: 1.26x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.34x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 72.4 ms: 1.54x faster                                                       |
| nbody          | 134 ms                                                       | 98.1 ms: 1.37x faster                                                       |
| pidigits       | 271 ms                                                       | 252 ms: 1.07x faster                                                        |
| Geometric mean | (ref)                                                        | 1.31x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 149 ms: 1.27x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 23.0 ms: 1.18x faster                                                       |
| regex_dna      | 261 ms                                                       | 229 ms: 1.14x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.43 ms: 1.11x slower                                                       |
| Geometric mean | (ref)                                                        | 1.12x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 214 us: 1.46x faster                                                        |
| pickle_pure_python   | 455 us                                                       | 313 us: 1.45x faster                                                        |
| json_dumps           | 14.5 ms                                                      | 10.1 ms: 1.44x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 55.4 ms: 1.37x faster                                                       |
| json_loads           | 30.3 us                                                      | 24.0 us: 1.26x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 80.3 ms: 1.15x faster                                                       |
| xml_etree_parse      | 160 ms                                                       | 144 ms: 1.12x faster                                                        |
| pickle_list          | 4.12 us                                                      | 3.70 us: 1.11x faster                                                       |
| xml_etree_iterparse  | 110 ms                                                       | 104 ms: 1.06x faster                                                        |
| unpickle_list        | 4.65 us                                                      | 4.48 us: 1.04x faster                                                       |
| pickle               | 9.89 us                                                      | 9.71 us: 1.02x faster                                                       |
| unpickle             | 13.5 us                                                      | 13.3 us: 1.01x faster                                                       |
| pickle_dict          | 29.5 us                                                      | 31.1 us: 1.05x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.17x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.8 ms: 1.07x faster                                                       |
| python_startup_no_site | 7.33 ms                                                      | 7.87 ms: 1.07x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.00x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.2 ms: 1.44x faster                                                       |
| django_template | 50.2 ms                                                      | 39.2 ms: 1.28x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 24.8 ms: 1.27x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 53.7 ms: 1.18x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.29x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 3.69 ms: 2.03x faster                                                       |
| asyncio_tcp             | 779 ms                                                       | 386 ms: 2.02x faster                                                        |
| go                      | 262 ms                                                       | 153 ms: 1.71x faster                                                        |
| pyflate                 | 733 ms                                                       | 433 ms: 1.69x faster                                                        |
| scimark_sor             | 180 ms                                                       | 108 ms: 1.67x faster                                                        |
| scimark_lu              | 167 ms                                                       | 101 ms: 1.65x faster                                                        |
| logging_silent          | 167 ns                                                       | 102 ns: 1.64x faster                                                        |
| raytrace                | 489 ms                                                       | 299 ms: 1.64x faster                                                        |
| scimark_monte_carlo     | 107 ms                                                       | 66.6 ms: 1.61x faster                                                       |
| richards                | 75.1 ms                                                      | 46.9 ms: 1.60x faster                                                       |
| float                   | 111 ms                                                       | 72.4 ms: 1.54x faster                                                       |
| chaos                   | 109 ms                                                       | 70.9 ms: 1.53x faster                                                       |
| crypto_pyaes            | 119 ms                                                       | 81.1 ms: 1.47x faster                                                       |
| unpickle_pure_python    | 312 us                                                       | 214 us: 1.46x faster                                                        |
| pickle_pure_python      | 455 us                                                       | 313 us: 1.45x faster                                                        |
| json_dumps              | 14.5 ms                                                      | 10.1 ms: 1.44x faster                                                       |
| mako                    | 14.7 ms                                                      | 10.2 ms: 1.44x faster                                                       |
| html5lib                | 94.6 ms                                                      | 66.8 ms: 1.42x faster                                                       |
| sqlglot_parse           | 2.24 ms                                                      | 1.59 ms: 1.41x faster                                                       |
| hexiom                  | 9.42 ms                                                      | 6.77 ms: 1.39x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.15 sec: 1.38x faster                                                      |
| spectral_norm           | 139 ms                                                       | 101 ms: 1.38x faster                                                        |
| sqlglot_transpile       | 2.68 ms                                                      | 1.95 ms: 1.37x faster                                                       |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 3.70 ms: 1.37x faster                                                       |
| xml_etree_process       | 75.9 ms                                                      | 55.4 ms: 1.37x faster                                                       |
| async_tree_none         | 692 ms                                                       | 505 ms: 1.37x faster                                                        |
| nbody                   | 134 ms                                                       | 98.1 ms: 1.37x faster                                                       |
| unpack_sequence         | 59.9 ns                                                      | 44.0 ns: 1.36x faster                                                       |
| deepcopy_memo           | 49.8 us                                                      | 36.7 us: 1.36x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 608 ms: 1.35x faster                                                        |
| pycparser               | 1.67 sec                                                     | 1.26 sec: 1.33x faster                                                      |
| pprint_pformat          | 2.15 sec                                                     | 1.63 sec: 1.32x faster                                                      |
| pprint_safe_repr        | 1.05 sec                                                     | 794 ms: 1.32x faster                                                        |
| async_generators        | 421 ms                                                       | 322 ms: 1.31x faster                                                        |
| thrift                  | 1.18 ms                                                      | 908 us: 1.29x faster                                                        |
| chameleon               | 9.44 ms                                                      | 7.31 ms: 1.29x faster                                                       |
| bench_mp_pool           | 6.37 ms                                                      | 4.94 ms: 1.29x faster                                                       |
| django_template         | 50.2 ms                                                      | 39.2 ms: 1.28x faster                                                       |
| scimark_fft             | 361 ms                                                       | 283 ms: 1.28x faster                                                        |
| logging_simple          | 8.88 us                                                      | 6.95 us: 1.28x faster                                                       |
| regex_compile           | 190 ms                                                       | 149 ms: 1.27x faster                                                        |
| fannkuch                | 483 ms                                                       | 380 ms: 1.27x faster                                                        |
| genshi_text             | 31.4 ms                                                      | 24.8 ms: 1.27x faster                                                       |
| json_loads              | 30.3 us                                                      | 24.0 us: 1.26x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 742 ms: 1.26x faster                                                        |
| logging_format          | 9.64 us                                                      | 7.66 us: 1.26x faster                                                       |
| deepcopy                | 468 us                                                       | 379 us: 1.24x faster                                                        |
| docutils                | 3.41 sec                                                     | 2.78 sec: 1.23x faster                                                      |
| 2to3                    | 350 ms                                                       | 286 ms: 1.22x faster                                                        |
| nqueens                 | 115 ms                                                       | 94.0 ms: 1.22x faster                                                       |
| deepcopy_reduce         | 4.01 us                                                      | 3.33 us: 1.20x faster                                                       |
| dulwich_log             | 81.1 ms                                                      | 67.5 ms: 1.20x faster                                                       |
| sqlglot_optimize        | 70.1 ms                                                      | 59.3 ms: 1.18x faster                                                       |
| regex_v8                | 27.2 ms                                                      | 23.0 ms: 1.18x faster                                                       |
| genshi_xml              | 63.3 ms                                                      | 53.7 ms: 1.18x faster                                                       |
| sqlglot_normalize       | 144 ms                                                       | 123 ms: 1.17x faster                                                        |
| sqlite_synth            | 2.99 us                                                      | 2.56 us: 1.17x faster                                                       |
| bench_thread_pool       | 1.14 ms                                                      | 987 us: 1.16x faster                                                        |
| dask                    | 472 ms                                                       | 408 ms: 1.16x faster                                                        |
| xml_etree_generate      | 92.3 ms                                                      | 80.3 ms: 1.15x faster                                                       |
| regex_dna               | 261 ms                                                       | 229 ms: 1.14x faster                                                        |
| json                    | 5.86 ms                                                      | 5.24 ms: 1.12x faster                                                       |
| sympy_expand            | 600 ms                                                       | 537 ms: 1.12x faster                                                        |
| xml_etree_parse         | 160 ms                                                       | 144 ms: 1.12x faster                                                        |
| pickle_list             | 4.12 us                                                      | 3.70 us: 1.11x faster                                                       |
| create_gc_cycles        | 1.76 ms                                                      | 1.58 ms: 1.11x faster                                                       |
| sympy_integrate         | 28.2 ms                                                      | 25.6 ms: 1.10x faster                                                       |
| pathlib                 | 21.4 ms                                                      | 19.4 ms: 1.10x faster                                                       |
| mdp                     | 3.01 sec                                                     | 2.75 sec: 1.09x faster                                                      |
| coroutines              | 30.3 ms                                                      | 27.9 ms: 1.09x faster                                                       |
| telco                   | 7.23 ms                                                      | 6.70 ms: 1.08x faster                                                       |
| sympy_str               | 360 ms                                                       | 335 ms: 1.08x faster                                                        |
| pidigits                | 271 ms                                                       | 252 ms: 1.07x faster                                                        |
| python_startup          | 11.5 ms                                                      | 10.8 ms: 1.07x faster                                                       |
| xml_etree_iterparse     | 110 ms                                                       | 104 ms: 1.06x faster                                                        |
| meteor_contest          | 138 ms                                                       | 131 ms: 1.06x faster                                                        |
| unpickle_list           | 4.65 us                                                      | 4.48 us: 1.04x faster                                                       |
| sympy_sum               | 193 ms                                                       | 186 ms: 1.03x faster                                                        |
| pickle                  | 9.89 us                                                      | 9.71 us: 1.02x faster                                                       |
| unpickle                | 13.5 us                                                      | 13.3 us: 1.01x faster                                                       |
| comprehensions          | 26.7 us                                                      | 27.1 us: 1.01x slower                                                       |
| gc_traversal            | 3.42 ms                                                      | 3.54 ms: 1.04x slower                                                       |
| pickle_dict             | 29.5 us                                                      | 31.1 us: 1.05x slower                                                       |
| generators              | 57.3 ms                                                      | 60.5 ms: 1.06x slower                                                       |
| python_startup_no_site  | 7.33 ms                                                      | 7.87 ms: 1.07x slower                                                       |
| regex_effbot            | 3.09 ms                                                      | 3.43 ms: 1.11x slower                                                       |
| coverage                | 63.3 ms                                                      | 89.3 ms: 1.41x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.25x faster                                                                |
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: 1.09x