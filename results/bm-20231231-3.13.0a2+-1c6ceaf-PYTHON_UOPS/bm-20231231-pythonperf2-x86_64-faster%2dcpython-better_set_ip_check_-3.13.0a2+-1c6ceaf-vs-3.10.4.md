
# Results vs. 3.10.4

- fork: faster-cpython
- ref: better_set_ip_check_
- machine: linux-x86_64
- commit hash: 1c6ceaf
- commit date: 2023-12-31
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 309 ms: 1.13x faster                                                                   |
| chameleon      | 9.44 ms                                                      | 8.09 ms: 1.17x faster                                                                  |
| docutils       | 3.41 sec                                                     | 2.94 sec: 1.16x faster                                                                 |
| tornado_http   | 157 ms                                                       | 122 ms: 1.28x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.18x faster                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 448 ms: 1.54x faster                                                                   |
| async_tree_io           | 1.60 sec                                                     | 1.09 sec: 1.46x faster                                                                 |
| async_tree_memoization  | 819 ms                                                       | 562 ms: 1.46x faster                                                                   |
| async_tree_cpu_io_mixed | 936 ms                                                       | 714 ms: 1.31x faster                                                                   |
| Geometric mean          | (ref)                                                        | 1.44x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 103 ms: 1.08x faster                                                                   |
| nbody          | 134 ms                                                       | 129 ms: 1.04x faster                                                                   |
| pidigits       | 271 ms                                                       | 263 ms: 1.03x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 170 ms: 1.12x faster                                                                   |
| regex_v8       | 27.2 ms                                                      | 25.5 ms: 1.07x faster                                                                  |
| regex_dna      | 261 ms                                                       | 245 ms: 1.07x faster                                                                   |
| regex_effbot   | 3.09 ms                                                      | 3.62 ms: 1.17x slower                                                                  |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 314 us: 1.45x faster                                                                   |
| json_dumps           | 14.5 ms                                                      | 10.9 ms: 1.34x faster                                                                  |
| unpickle_pure_python | 312 us                                                       | 242 us: 1.29x faster                                                                   |
| xml_etree_process    | 75.9 ms                                                      | 61.5 ms: 1.23x faster                                                                  |
| json_loads           | 30.3 us                                                      | 25.0 us: 1.22x faster                                                                  |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                                   |
| tomli_loads          | 2.92 sec                                                     | 2.75 sec: 1.06x faster                                                                 |
| xml_etree_generate   | 92.3 ms                                                      | 90.5 ms: 1.02x faster                                                                  |
| unpickle_list        | 4.65 us                                                      | 4.69 us: 1.01x slower                                                                  |
| pickle               | 9.89 us                                                      | 10.0 us: 1.01x slower                                                                  |
| xml_etree_iterparse  | 110 ms                                                       | 112 ms: 1.02x slower                                                                   |
| pickle_list          | 4.12 us                                                      | 4.23 us: 1.03x slower                                                                  |
| pickle_dict          | 29.5 us                                                      | 30.7 us: 1.04x slower                                                                  |
| unpickle             | 13.5 us                                                      | 15.2 us: 1.12x slower                                                                  |
| Geometric mean       | (ref)                                                        | 1.09x faster                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                                  |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 14.1 ms: 1.04x faster                                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 124 us: 4.31x faster                                                                   |
| asyncio_tcp              | 779 ms                                                       | 373 ms: 2.09x faster                                                                   |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.95x faster                                                                 |
| generators               | 57.3 ms                                                      | 33.9 ms: 1.69x faster                                                                  |
| logging_silent           | 167 ns                                                       | 100.0 ns: 1.67x faster                                                                 |
| raytrace                 | 489 ms                                                       | 300 ms: 1.63x faster                                                                   |
| scimark_lu               | 167 ms                                                       | 105 ms: 1.59x faster                                                                   |
| sqlglot_parse            | 2.24 ms                                                      | 1.44 ms: 1.55x faster                                                                  |
| async_tree_none          | 692 ms                                                       | 448 ms: 1.54x faster                                                                   |
| richards_super           | 90.6 ms                                                      | 61.3 ms: 1.48x faster                                                                  |
| async_tree_io            | 1.60 sec                                                     | 1.09 sec: 1.46x faster                                                                 |
| async_tree_memoization   | 819 ms                                                       | 562 ms: 1.46x faster                                                                   |
| pickle_pure_python       | 455 us                                                       | 314 us: 1.45x faster                                                                   |
| sqlglot_transpile        | 2.68 ms                                                      | 1.86 ms: 1.44x faster                                                                  |
| go                       | 262 ms                                                       | 182 ms: 1.44x faster                                                                   |
| chaos                    | 109 ms                                                       | 77.4 ms: 1.40x faster                                                                  |
| crypto_pyaes             | 119 ms                                                       | 85.4 ms: 1.39x faster                                                                  |
| deltablue                | 7.50 ms                                                      | 5.42 ms: 1.38x faster                                                                  |
| coroutines               | 30.3 ms                                                      | 22.0 ms: 1.38x faster                                                                  |
| richards                 | 75.1 ms                                                      | 54.7 ms: 1.37x faster                                                                  |
| bench_mp_pool            | 6.37 ms                                                      | 4.70 ms: 1.36x faster                                                                  |
| json_dumps               | 14.5 ms                                                      | 10.9 ms: 1.34x faster                                                                  |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 714 ms: 1.31x faster                                                                   |
| logging_simple           | 8.88 us                                                      | 6.84 us: 1.30x faster                                                                  |
| logging_format           | 9.64 us                                                      | 7.45 us: 1.29x faster                                                                  |
| pyflate                  | 733 ms                                                       | 567 ms: 1.29x faster                                                                   |
| unpickle_pure_python     | 312 us                                                       | 242 us: 1.29x faster                                                                   |
| unpack_sequence          | 59.9 ns                                                      | 46.7 ns: 1.28x faster                                                                  |
| tornado_http             | 157 ms                                                       | 122 ms: 1.28x faster                                                                   |
| scimark_sor              | 180 ms                                                       | 144 ms: 1.25x faster                                                                   |
| scimark_monte_carlo      | 107 ms                                                       | 86.1 ms: 1.25x faster                                                                  |
| pycparser                | 1.67 sec                                                     | 1.34 sec: 1.25x faster                                                                 |
| deepcopy_memo            | 49.8 us                                                      | 40.3 us: 1.24x faster                                                                  |
| xml_etree_process        | 75.9 ms                                                      | 61.5 ms: 1.23x faster                                                                  |
| json_loads               | 30.3 us                                                      | 25.0 us: 1.22x faster                                                                  |
| deepcopy                 | 468 us                                                       | 388 us: 1.21x faster                                                                   |
| sqlglot_normalize        | 144 ms                                                       | 122 ms: 1.18x faster                                                                   |
| bench_thread_pool        | 1.14 ms                                                      | 972 us: 1.17x faster                                                                   |
| async_generators         | 421 ms                                                       | 361 ms: 1.17x faster                                                                   |
| chameleon                | 9.44 ms                                                      | 8.09 ms: 1.17x faster                                                                  |
| docutils                 | 3.41 sec                                                     | 2.94 sec: 1.16x faster                                                                 |
| deepcopy_reduce          | 4.01 us                                                      | 3.45 us: 1.16x faster                                                                  |
| sympy_sum                | 193 ms                                                       | 167 ms: 1.15x faster                                                                   |
| dask                     | 472 ms                                                       | 411 ms: 1.15x faster                                                                   |
| mdp                      | 3.01 sec                                                     | 2.62 sec: 1.15x faster                                                                 |
| pprint_safe_repr         | 1.05 sec                                                     | 920 ms: 1.14x faster                                                                   |
| pprint_pformat           | 2.15 sec                                                     | 1.90 sec: 1.13x faster                                                                 |
| 2to3                     | 350 ms                                                       | 309 ms: 1.13x faster                                                                   |
| dulwich_log              | 81.1 ms                                                      | 71.7 ms: 1.13x faster                                                                  |
| sympy_integrate          | 28.2 ms                                                      | 25.0 ms: 1.13x faster                                                                  |
| json                     | 5.86 ms                                                      | 5.24 ms: 1.12x faster                                                                  |
| sympy_expand             | 600 ms                                                       | 538 ms: 1.12x faster                                                                   |
| regex_compile            | 190 ms                                                       | 170 ms: 1.12x faster                                                                   |
| sympy_str                | 360 ms                                                       | 323 ms: 1.11x faster                                                                   |
| sqlglot_optimize         | 70.1 ms                                                      | 63.4 ms: 1.11x faster                                                                  |
| create_gc_cycles         | 1.76 ms                                                      | 1.61 ms: 1.10x faster                                                                  |
| comprehensions           | 26.7 us                                                      | 24.5 us: 1.09x faster                                                                  |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                                   |
| float                    | 111 ms                                                       | 103 ms: 1.08x faster                                                                   |
| pathlib                  | 21.4 ms                                                      | 19.7 ms: 1.08x faster                                                                  |
| nqueens                  | 115 ms                                                       | 107 ms: 1.07x faster                                                                   |
| sqlite_synth             | 2.99 us                                                      | 2.79 us: 1.07x faster                                                                  |
| regex_v8                 | 27.2 ms                                                      | 25.5 ms: 1.07x faster                                                                  |
| regex_dna                | 261 ms                                                       | 245 ms: 1.07x faster                                                                   |
| tomli_loads              | 2.92 sec                                                     | 2.75 sec: 1.06x faster                                                                 |
| mako                     | 14.7 ms                                                      | 14.1 ms: 1.04x faster                                                                  |
| nbody                    | 134 ms                                                       | 129 ms: 1.04x faster                                                                   |
| pidigits                 | 271 ms                                                       | 263 ms: 1.03x faster                                                                   |
| xml_etree_generate       | 92.3 ms                                                      | 90.5 ms: 1.02x faster                                                                  |
| asyncio_websockets       | 390 ms                                                       | 386 ms: 1.01x faster                                                                   |
| fannkuch                 | 483 ms                                                       | 478 ms: 1.01x faster                                                                   |
| meteor_contest           | 138 ms                                                       | 138 ms: 1.00x faster                                                                   |
| unpickle_list            | 4.65 us                                                      | 4.69 us: 1.01x slower                                                                  |
| pickle                   | 9.89 us                                                      | 10.0 us: 1.01x slower                                                                  |
| xml_etree_iterparse      | 110 ms                                                       | 112 ms: 1.02x slower                                                                   |
| pickle_list              | 4.12 us                                                      | 4.23 us: 1.03x slower                                                                  |
| gc_traversal             | 3.42 ms                                                      | 3.51 ms: 1.03x slower                                                                  |
| hexiom                   | 9.42 ms                                                      | 9.70 ms: 1.03x slower                                                                  |
| pickle_dict              | 29.5 us                                                      | 30.7 us: 1.04x slower                                                                  |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                                  |
| unpickle                 | 13.5 us                                                      | 15.2 us: 1.12x slower                                                                  |
| spectral_norm            | 139 ms                                                       | 162 ms: 1.16x slower                                                                   |
| telco                    | 7.23 ms                                                      | 8.45 ms: 1.17x slower                                                                  |
| scimark_fft              | 361 ms                                                       | 423 ms: 1.17x slower                                                                   |
| regex_effbot             | 3.09 ms                                                      | 3.62 ms: 1.17x slower                                                                  |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 6.30 ms: 1.24x slower                                                                  |
| coverage                 | 63.3 ms                                                      | 83.2 ms: 1.31x slower                                                                  |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                                  |
| Geometric mean           | (ref)                                                        | 1.18x faster                                                                           |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231231-3.13.0a2+-1c6ceaf-PYTHON_UOPS/bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: 1.07x