
# Results vs. 3.10.4

- fork: python
- ref: ed7c3ff15680c1939fad
- machine: linux-x86_64
- commit hash: ed7c3ff
- commit date: 2022-09-11
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 287 ms: 1.22x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.50 ms: 1.26x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.86 sec: 1.19x faster                                                       |
| html5lib       | 94.6 ms                                                      | 73.2 ms: 1.29x faster                                                        |
| tornado_http   | 157 ms                                                       | 125 ms: 1.25x faster                                                         |
| Geometric mean | (ref)                                                        | 1.24x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.36x faster                                                       |
| async_tree_none         | 692 ms                                                       | 517 ms: 1.34x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 636 ms: 1.29x faster                                                         |
| async_tree_cpu_io_mixed | 936 ms                                                       | 746 ms: 1.26x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.31x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 89.6 ms: 1.50x faster                                                        |
| float          | 111 ms                                                       | 75.1 ms: 1.48x faster                                                        |
| pidigits       | 271 ms                                                       | 251 ms: 1.08x faster                                                         |
| Geometric mean | (ref)                                                        | 1.34x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 157 ms: 1.21x faster                                                         |
| regex_dna      | 261 ms                                                       | 225 ms: 1.16x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 24.3 ms: 1.12x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.29 ms: 1.07x slower                                                        |
| Geometric mean | (ref)                                                        | 1.10x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 324 us: 1.41x faster                                                         |
| xml_etree_process    | 75.9 ms                                                      | 57.0 ms: 1.33x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 250 us: 1.25x faster                                                         |
| xml_etree_generate   | 92.3 ms                                                      | 80.8 ms: 1.14x faster                                                        |
| pickle_list          | 4.12 us                                                      | 3.77 us: 1.09x faster                                                        |
| json_dumps           | 14.5 ms                                                      | 13.5 ms: 1.08x faster                                                        |
| json_loads           | 30.3 us                                                      | 28.4 us: 1.07x faster                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 104 ms: 1.07x faster                                                         |
| unpickle             | 13.5 us                                                      | 13.0 us: 1.04x faster                                                        |
| pickle               | 9.89 us                                                      | 9.61 us: 1.03x faster                                                        |
| pickle_dict          | 29.5 us                                                      | 30.7 us: 1.04x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.10x faster                                                                 |

Benchmark hidden because not significant (2): xml_etree_parse, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.7 ms: 1.07x faster                                                        |
| python_startup_no_site | 7.33 ms                                                      | 7.72 ms: 1.05x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.9 ms: 1.35x faster                                                        |
| django_template | 50.2 ms                                                      | 39.7 ms: 1.26x faster                                                        |
| genshi_text     | 31.4 ms                                                      | 26.1 ms: 1.21x faster                                                        |
| genshi_xml      | 63.3 ms                                                      | 59.2 ms: 1.07x faster                                                        |
| Geometric mean  | (ref)                                                        | 1.22x faster                                                                 |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 4.09 ms: 1.83x faster                                                        |
| logging_silent          | 167 ns                                                       | 101 ns: 1.66x faster                                                         |
| scimark_sor             | 180 ms                                                       | 110 ms: 1.64x faster                                                         |
| pyflate                 | 733 ms                                                       | 450 ms: 1.63x faster                                                         |
| raytrace                | 489 ms                                                       | 307 ms: 1.59x faster                                                         |
| scimark_monte_carlo     | 107 ms                                                       | 68.7 ms: 1.56x faster                                                        |
| go                      | 262 ms                                                       | 172 ms: 1.52x faster                                                         |
| nbody                   | 134 ms                                                       | 89.6 ms: 1.50x faster                                                        |
| float                   | 111 ms                                                       | 75.1 ms: 1.48x faster                                                        |
| scimark_lu              | 167 ms                                                       | 114 ms: 1.47x faster                                                         |
| spectral_norm           | 139 ms                                                       | 95.5 ms: 1.46x faster                                                        |
| sqlglot_parse           | 2.24 ms                                                      | 1.56 ms: 1.43x faster                                                        |
| crypto_pyaes            | 119 ms                                                       | 84.3 ms: 1.41x faster                                                        |
| bench_mp_pool           | 6.37 ms                                                      | 4.54 ms: 1.41x faster                                                        |
| pickle_pure_python      | 455 us                                                       | 324 us: 1.41x faster                                                         |
| richards                | 75.1 ms                                                      | 53.5 ms: 1.40x faster                                                        |
| sqlglot_transpile       | 2.68 ms                                                      | 1.92 ms: 1.40x faster                                                        |
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.36x faster                                                       |
| mako                    | 14.7 ms                                                      | 10.9 ms: 1.35x faster                                                        |
| async_tree_none         | 692 ms                                                       | 517 ms: 1.34x faster                                                         |
| chaos                   | 109 ms                                                       | 81.4 ms: 1.33x faster                                                        |
| xml_etree_process       | 75.9 ms                                                      | 57.0 ms: 1.33x faster                                                        |
| pprint_safe_repr        | 1.05 sec                                                     | 791 ms: 1.33x faster                                                         |
| hexiom                  | 9.42 ms                                                      | 7.12 ms: 1.32x faster                                                        |
| unpack_sequence         | 59.9 ns                                                      | 45.7 ns: 1.31x faster                                                        |
| pprint_pformat          | 2.15 sec                                                     | 1.65 sec: 1.31x faster                                                       |
| scimark_fft             | 361 ms                                                       | 277 ms: 1.30x faster                                                         |
| thrift                  | 1.18 ms                                                      | 906 us: 1.30x faster                                                         |
| html5lib                | 94.6 ms                                                      | 73.2 ms: 1.29x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 636 ms: 1.29x faster                                                         |
| async_generators        | 421 ms                                                       | 328 ms: 1.28x faster                                                         |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 4.01 ms: 1.27x faster                                                        |
| django_template         | 50.2 ms                                                      | 39.7 ms: 1.26x faster                                                        |
| chameleon               | 9.44 ms                                                      | 7.50 ms: 1.26x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 746 ms: 1.26x faster                                                         |
| tornado_http            | 157 ms                                                       | 125 ms: 1.25x faster                                                         |
| pycparser               | 1.67 sec                                                     | 1.34 sec: 1.25x faster                                                       |
| unpickle_pure_python    | 312 us                                                       | 250 us: 1.25x faster                                                         |
| gunicorn                | 1.16 ms                                                      | 941 us: 1.23x faster                                                         |
| aiohttp                 | 1.19 ms                                                      | 966 us: 1.23x faster                                                         |
| sqlalchemy_declarative  | 190 ms                                                       | 155 ms: 1.22x faster                                                         |
| 2to3                    | 350 ms                                                       | 287 ms: 1.22x faster                                                         |
| deepcopy_memo           | 49.8 us                                                      | 41.0 us: 1.21x faster                                                        |
| regex_compile           | 190 ms                                                       | 157 ms: 1.21x faster                                                         |
| genshi_text             | 31.4 ms                                                      | 26.1 ms: 1.21x faster                                                        |
| sqlite_synth            | 2.99 us                                                      | 2.48 us: 1.20x faster                                                        |
| logging_format          | 9.64 us                                                      | 8.03 us: 1.20x faster                                                        |
| docutils                | 3.41 sec                                                     | 2.86 sec: 1.19x faster                                                       |
| logging_simple          | 8.88 us                                                      | 7.43 us: 1.19x faster                                                        |
| sqlglot_optimize        | 70.1 ms                                                      | 58.8 ms: 1.19x faster                                                        |
| sqlglot_normalize       | 144 ms                                                       | 121 ms: 1.19x faster                                                         |
| dulwich_log             | 81.1 ms                                                      | 69.6 ms: 1.17x faster                                                        |
| regex_dna               | 261 ms                                                       | 225 ms: 1.16x faster                                                         |
| flaskblogging           | 4.39 ms                                                      | 3.80 ms: 1.15x faster                                                        |
| deepcopy                | 468 us                                                       | 407 us: 1.15x faster                                                         |
| deepcopy_reduce         | 4.01 us                                                      | 3.51 us: 1.14x faster                                                        |
| xml_etree_generate      | 92.3 ms                                                      | 80.8 ms: 1.14x faster                                                        |
| sqlalchemy_imperative   | 22.7 ms                                                      | 19.9 ms: 1.14x faster                                                        |
| bench_thread_pool       | 1.14 ms                                                      | 1.00 ms: 1.14x faster                                                        |
| nqueens                 | 115 ms                                                       | 101 ms: 1.14x faster                                                         |
| dask                    | 472 ms                                                       | 420 ms: 1.13x faster                                                         |
| regex_v8                | 27.2 ms                                                      | 24.3 ms: 1.12x faster                                                        |
| pathlib                 | 21.4 ms                                                      | 19.1 ms: 1.12x faster                                                        |
| mdp                     | 3.01 sec                                                     | 2.72 sec: 1.11x faster                                                       |
| fannkuch                | 483 ms                                                       | 441 ms: 1.09x faster                                                         |
| pickle_list             | 4.12 us                                                      | 3.77 us: 1.09x faster                                                        |
| pylint                  | 566 ms                                                       | 520 ms: 1.09x faster                                                         |
| coroutines              | 30.3 ms                                                      | 27.9 ms: 1.09x faster                                                        |
| sympy_integrate         | 28.2 ms                                                      | 25.9 ms: 1.09x faster                                                        |
| sympy_expand            | 600 ms                                                       | 553 ms: 1.09x faster                                                         |
| json_dumps              | 14.5 ms                                                      | 13.5 ms: 1.08x faster                                                        |
| pidigits                | 271 ms                                                       | 251 ms: 1.08x faster                                                         |
| python_startup          | 11.5 ms                                                      | 10.7 ms: 1.07x faster                                                        |
| genshi_xml              | 63.3 ms                                                      | 59.2 ms: 1.07x faster                                                        |
| json_loads              | 30.3 us                                                      | 28.4 us: 1.07x faster                                                        |
| sympy_str               | 360 ms                                                       | 337 ms: 1.07x faster                                                         |
| xml_etree_iterparse     | 110 ms                                                       | 104 ms: 1.07x faster                                                         |
| create_gc_cycles        | 1.76 ms                                                      | 1.66 ms: 1.06x faster                                                        |
| generators              | 57.3 ms                                                      | 54.2 ms: 1.06x faster                                                        |
| sympy_sum               | 193 ms                                                       | 183 ms: 1.05x faster                                                         |
| json                    | 5.86 ms                                                      | 5.57 ms: 1.05x faster                                                        |
| telco                   | 7.23 ms                                                      | 6.88 ms: 1.05x faster                                                        |
| comprehensions          | 26.7 us                                                      | 25.5 us: 1.05x faster                                                        |
| meteor_contest          | 138 ms                                                       | 132 ms: 1.05x faster                                                         |
| unpickle                | 13.5 us                                                      | 13.0 us: 1.04x faster                                                        |
| asyncio_tcp             | 779 ms                                                       | 752 ms: 1.04x faster                                                         |
| pickle                  | 9.89 us                                                      | 9.61 us: 1.03x faster                                                        |
| pickle_dict             | 29.5 us                                                      | 30.7 us: 1.04x slower                                                        |
| python_startup_no_site  | 7.33 ms                                                      | 7.72 ms: 1.05x slower                                                        |
| gc_traversal            | 3.42 ms                                                      | 3.63 ms: 1.06x slower                                                        |
| regex_effbot            | 3.09 ms                                                      | 3.29 ms: 1.07x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.21x faster                                                                 |

Benchmark hidden because not significant (2): xml_etree_parse, unpickle_list
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.10x