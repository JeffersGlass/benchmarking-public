
# Results vs. 3.10.4

- fork: python
- ref: 7c12e4835ebe52287acd
- machine: linux-x86_64
- commit hash: 7c12e48
- commit date: 2021-10-05
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 329 ms: 1.07x faster                                                        |
| chameleon      | 9.44 ms                                                      | 8.97 ms: 1.05x faster                                                       |
| docutils       | 3.41 sec                                                     | 3.22 sec: 1.06x faster                                                      |
| html5lib       | 94.6 ms                                                      | 83.0 ms: 1.14x faster                                                       |
| tornado_http   | 157 ms                                                       | 136 ms: 1.15x faster                                                        |
| Geometric mean | (ref)                                                        | 1.09x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 515 ms: 1.34x faster                                                        |
| async_tree_io           | 1.60 sec                                                     | 1.24 sec: 1.29x faster                                                      |
| async_tree_memoization  | 819 ms                                                       | 660 ms: 1.24x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 796 ms: 1.18x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.26x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 86.6 ms: 1.28x faster                                                       |
| pidigits       | 271 ms                                                       | 266 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                        | 1.10x faster                                                                |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 169 ms: 1.13x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 25.6 ms: 1.06x faster                                                       |
| regex_effbot   | 3.09 ms                                                      | 3.05 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| xml_etree_process    | 75.9 ms                                                      | 64.1 ms: 1.18x faster                                                       |
| pickle_pure_python   | 455 us                                                       | 394 us: 1.16x faster                                                        |
| json_loads           | 30.3 us                                                      | 27.0 us: 1.12x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 86.0 ms: 1.07x faster                                                       |
| json_dumps           | 14.5 ms                                                      | 13.6 ms: 1.07x faster                                                       |
| unpickle_pure_python | 312 us                                                       | 293 us: 1.07x faster                                                        |
| unpickle_list        | 4.65 us                                                      | 4.54 us: 1.02x faster                                                       |
| xml_etree_parse      | 160 ms                                                       | 158 ms: 1.01x faster                                                        |
| unpickle             | 13.5 us                                                      | 13.7 us: 1.01x slower                                                       |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                       |
| pickle_dict          | 29.5 us                                                      | 31.5 us: 1.07x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.04x faster                                                                |

Benchmark hidden because not significant (2): pickle_list, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 11.8 ms: 1.02x slower                                                       |
| python_startup_no_site | 7.33 ms                                                      | 7.57 ms: 1.03x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.03x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 13.1 ms: 1.13x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 28.3 ms: 1.11x faster                                                       |
| django_template | 50.2 ms                                                      | 47.5 ms: 1.06x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 59.9 ms: 1.06x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.09x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 515 ms: 1.34x faster                                                        |
| logging_simple          | 8.88 us                                                      | 6.69 us: 1.33x faster                                                       |
| logging_format          | 9.64 us                                                      | 7.28 us: 1.32x faster                                                       |
| raytrace                | 489 ms                                                       | 371 ms: 1.32x faster                                                        |
| deltablue               | 7.50 ms                                                      | 5.73 ms: 1.31x faster                                                       |
| unpack_sequence         | 59.9 ns                                                      | 46.5 ns: 1.29x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.24 sec: 1.29x faster                                                      |
| float                   | 111 ms                                                       | 86.6 ms: 1.28x faster                                                       |
| logging_silent          | 167 ns                                                       | 134 ns: 1.25x faster                                                        |
| chaos                   | 109 ms                                                       | 87.5 ms: 1.24x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 660 ms: 1.24x faster                                                        |
| bench_mp_pool           | 6.37 ms                                                      | 5.14 ms: 1.24x faster                                                       |
| go                      | 262 ms                                                       | 211 ms: 1.24x faster                                                        |
| scimark_monte_carlo     | 107 ms                                                       | 87.3 ms: 1.23x faster                                                       |
| scimark_sor             | 180 ms                                                       | 147 ms: 1.23x faster                                                        |
| pprint_safe_repr        | 1.05 sec                                                     | 879 ms: 1.19x faster                                                        |
| pyflate                 | 733 ms                                                       | 615 ms: 1.19x faster                                                        |
| pycparser               | 1.67 sec                                                     | 1.41 sec: 1.18x faster                                                      |
| xml_etree_process       | 75.9 ms                                                      | 64.1 ms: 1.18x faster                                                       |
| async_generators        | 421 ms                                                       | 356 ms: 1.18x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 796 ms: 1.18x faster                                                        |
| pprint_pformat          | 2.15 sec                                                     | 1.83 sec: 1.18x faster                                                      |
| gunicorn                | 1.16 ms                                                      | 988 us: 1.17x faster                                                        |
| crypto_pyaes            | 119 ms                                                       | 102 ms: 1.17x faster                                                        |
| spectral_norm           | 139 ms                                                       | 120 ms: 1.16x faster                                                        |
| richards                | 75.1 ms                                                      | 64.9 ms: 1.16x faster                                                       |
| pickle_pure_python      | 455 us                                                       | 394 us: 1.16x faster                                                        |
| thrift                  | 1.18 ms                                                      | 1.02 ms: 1.16x faster                                                       |
| hexiom                  | 9.42 ms                                                      | 8.15 ms: 1.16x faster                                                       |
| tornado_http            | 157 ms                                                       | 136 ms: 1.15x faster                                                        |
| scimark_lu              | 167 ms                                                       | 145 ms: 1.15x faster                                                        |
| html5lib                | 94.6 ms                                                      | 83.0 ms: 1.14x faster                                                       |
| mako                    | 14.7 ms                                                      | 13.1 ms: 1.13x faster                                                       |
| regex_compile           | 190 ms                                                       | 169 ms: 1.13x faster                                                        |
| json_loads              | 30.3 us                                                      | 27.0 us: 1.12x faster                                                       |
| nqueens                 | 115 ms                                                       | 103 ms: 1.12x faster                                                        |
| deepcopy_memo           | 49.8 us                                                      | 44.7 us: 1.11x faster                                                       |
| genshi_text             | 31.4 ms                                                      | 28.3 ms: 1.11x faster                                                       |
| deepcopy                | 468 us                                                       | 427 us: 1.10x faster                                                        |
| dulwich_log             | 81.1 ms                                                      | 74.2 ms: 1.09x faster                                                       |
| generators              | 57.3 ms                                                      | 52.5 ms: 1.09x faster                                                       |
| dask                    | 472 ms                                                       | 433 ms: 1.09x faster                                                        |
| json                    | 5.86 ms                                                      | 5.40 ms: 1.09x faster                                                       |
| telco                   | 7.23 ms                                                      | 6.66 ms: 1.09x faster                                                       |
| scimark_fft             | 361 ms                                                       | 333 ms: 1.09x faster                                                        |
| sqlite_synth            | 2.99 us                                                      | 2.76 us: 1.08x faster                                                       |
| deepcopy_reduce         | 4.01 us                                                      | 3.70 us: 1.08x faster                                                       |
| xml_etree_generate      | 92.3 ms                                                      | 86.0 ms: 1.07x faster                                                       |
| bench_thread_pool       | 1.14 ms                                                      | 1.07 ms: 1.07x faster                                                       |
| json_dumps              | 14.5 ms                                                      | 13.6 ms: 1.07x faster                                                       |
| 2to3                    | 350 ms                                                       | 329 ms: 1.07x faster                                                        |
| unpickle_pure_python    | 312 us                                                       | 293 us: 1.07x faster                                                        |
| sqlglot_normalize       | 144 ms                                                       | 135 ms: 1.06x faster                                                        |
| coroutines              | 30.3 ms                                                      | 28.5 ms: 1.06x faster                                                       |
| docutils                | 3.41 sec                                                     | 3.22 sec: 1.06x faster                                                      |
| regex_v8                | 27.2 ms                                                      | 25.6 ms: 1.06x faster                                                       |
| django_template         | 50.2 ms                                                      | 47.5 ms: 1.06x faster                                                       |
| mdp                     | 3.01 sec                                                     | 2.84 sec: 1.06x faster                                                      |
| genshi_xml              | 63.3 ms                                                      | 59.9 ms: 1.06x faster                                                       |
| sqlglot_optimize        | 70.1 ms                                                      | 66.6 ms: 1.05x faster                                                       |
| chameleon               | 9.44 ms                                                      | 8.97 ms: 1.05x faster                                                       |
| sympy_integrate         | 28.2 ms                                                      | 26.8 ms: 1.05x faster                                                       |
| sympy_str               | 360 ms                                                       | 343 ms: 1.05x faster                                                        |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 4.84 ms: 1.05x faster                                                       |
| sympy_expand            | 600 ms                                                       | 573 ms: 1.05x faster                                                        |
| sympy_sum               | 193 ms                                                       | 184 ms: 1.05x faster                                                        |
| meteor_contest          | 138 ms                                                       | 133 ms: 1.04x faster                                                        |
| unpickle_list           | 4.65 us                                                      | 4.54 us: 1.02x faster                                                       |
| fannkuch                | 483 ms                                                       | 472 ms: 1.02x faster                                                        |
| pathlib                 | 21.4 ms                                                      | 20.9 ms: 1.02x faster                                                       |
| pidigits                | 271 ms                                                       | 266 ms: 1.02x faster                                                        |
| xml_etree_parse         | 160 ms                                                       | 158 ms: 1.01x faster                                                        |
| regex_effbot            | 3.09 ms                                                      | 3.05 ms: 1.01x faster                                                       |
| unpickle                | 13.5 us                                                      | 13.7 us: 1.01x slower                                                       |
| python_startup          | 11.5 ms                                                      | 11.8 ms: 1.02x slower                                                       |
| sqlglot_transpile       | 2.68 ms                                                      | 2.76 ms: 1.03x slower                                                       |
| python_startup_no_site  | 7.33 ms                                                      | 7.57 ms: 1.03x slower                                                       |
| gc_traversal            | 3.42 ms                                                      | 3.55 ms: 1.04x slower                                                       |
| pickle                  | 9.89 us                                                      | 10.4 us: 1.05x slower                                                       |
| sqlglot_parse           | 2.24 ms                                                      | 2.37 ms: 1.06x slower                                                       |
| pickle_dict             | 29.5 us                                                      | 31.5 us: 1.07x slower                                                       |
| create_gc_cycles        | 1.76 ms                                                      | 1.90 ms: 1.08x slower                                                       |
| comprehensions          | 26.7 us                                                      | 29.5 us: 1.10x slower                                                       |
| flaskblogging           | 4.39 ms                                                      | 4.88 ms: 1.11x slower                                                       |
| coverage                | 63.3 ms                                                      | 72.0 ms: 1.14x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.10x faster                                                                |

Benchmark hidden because not significant (4): nbody, regex_dna, pickle_list, xml_etree_iterparse
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.06x


# Memory

- memory change: 1.06x