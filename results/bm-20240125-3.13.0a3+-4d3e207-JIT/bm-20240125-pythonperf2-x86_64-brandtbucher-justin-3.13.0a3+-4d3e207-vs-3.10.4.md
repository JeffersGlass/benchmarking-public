
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.24x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 299 ms: 1.17x faster                                                 |
| chameleon      | 9.44 ms                                                      | 7.53 ms: 1.25x faster                                                |
| docutils       | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                               |
| tornado_http   | 157 ms                                                       | 124 ms: 1.27x faster                                                 |
| Geometric mean | (ref)                                                        | 1.22x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 434 ms: 1.59x faster                                                 |
| async_tree_memoization  | 819 ms                                                       | 542 ms: 1.51x faster                                                 |
| async_tree_io           | 1.60 sec                                                     | 1.07 sec: 1.50x faster                                               |
| async_tree_cpu_io_mixed | 936 ms                                                       | 694 ms: 1.35x faster                                                 |
| Geometric mean          | (ref)                                                        | 1.49x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 111 ms                                                       | 82.4 ms: 1.35x faster                                                |
| nbody          | 134 ms                                                       | 107 ms: 1.26x faster                                                 |
| pidigits       | 271 ms                                                       | 263 ms: 1.03x faster                                                 |
| Geometric mean | (ref)                                                        | 1.20x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 147 ms: 1.29x faster                                                 |
| regex_dna      | 261 ms                                                       | 246 ms: 1.06x faster                                                 |
| regex_v8       | 27.2 ms                                                      | 26.7 ms: 1.02x faster                                                |
| regex_effbot   | 3.09 ms                                                      | 3.57 ms: 1.16x slower                                                |
| Geometric mean | (ref)                                                        | 1.05x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 310 us: 1.47x faster                                                 |
| json_dumps           | 14.5 ms                                                      | 10.7 ms: 1.36x faster                                                |
| unpickle_pure_python | 312 us                                                       | 235 us: 1.33x faster                                                 |
| xml_etree_process    | 75.9 ms                                                      | 58.7 ms: 1.29x faster                                                |
| tomli_loads          | 2.92 sec                                                     | 2.30 sec: 1.27x faster                                               |
| json_loads           | 30.3 us                                                      | 24.8 us: 1.23x faster                                                |
| xml_etree_parse      | 160 ms                                                       | 144 ms: 1.12x faster                                                 |
| xml_etree_generate   | 92.3 ms                                                      | 84.9 ms: 1.09x faster                                                |
| xml_etree_iterparse  | 110 ms                                                       | 105 ms: 1.05x faster                                                 |
| pickle_list          | 4.12 us                                                      | 4.38 us: 1.06x slower                                                |
| pickle_dict          | 29.5 us                                                      | 31.4 us: 1.06x slower                                                |
| pickle               | 9.89 us                                                      | 10.6 us: 1.07x slower                                                |
| unpickle_list        | 4.65 us                                                      | 5.09 us: 1.10x slower                                                |
| unpickle             | 13.5 us                                                      | 15.5 us: 1.15x slower                                                |
| Geometric mean       | (ref)                                                        | 1.11x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.09x slower                                                |
| python_startup_no_site | 7.33 ms                                                      | 11.0 ms: 1.51x slower                                                |
| Geometric mean         | (ref)                                                        | 1.28x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 11.9 ms: 1.23x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 119 us: 4.51x faster                                                 |
| asyncio_tcp              | 779 ms                                                       | 367 ms: 2.12x faster                                                 |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.60 sec: 1.94x faster                                               |
| deltablue                | 7.50 ms                                                      | 3.99 ms: 1.88x faster                                                |
| raytrace                 | 489 ms                                                       | 278 ms: 1.76x faster                                                 |
| logging_silent           | 167 ns                                                       | 96.7 ns: 1.73x faster                                                |
| generators               | 57.3 ms                                                      | 33.7 ms: 1.70x faster                                                |
| scimark_lu               | 167 ms                                                       | 102 ms: 1.64x faster                                                 |
| sqlglot_parse            | 2.24 ms                                                      | 1.38 ms: 1.62x faster                                                |
| async_tree_none          | 692 ms                                                       | 434 ms: 1.59x faster                                                 |
| richards_super           | 90.6 ms                                                      | 58.4 ms: 1.55x faster                                                |
| chaos                    | 109 ms                                                       | 70.7 ms: 1.54x faster                                                |
| async_tree_memoization   | 819 ms                                                       | 542 ms: 1.51x faster                                                 |
| async_tree_io            | 1.60 sec                                                     | 1.07 sec: 1.50x faster                                               |
| sqlglot_transpile        | 2.68 ms                                                      | 1.79 ms: 1.49x faster                                                |
| richards                 | 75.1 ms                                                      | 50.9 ms: 1.47x faster                                                |
| go                       | 262 ms                                                       | 178 ms: 1.47x faster                                                 |
| pickle_pure_python       | 455 us                                                       | 310 us: 1.47x faster                                                 |
| crypto_pyaes             | 119 ms                                                       | 82.9 ms: 1.44x faster                                                |
| unpack_sequence          | 59.9 ns                                                      | 42.9 ns: 1.40x faster                                                |
| json_dumps               | 14.5 ms                                                      | 10.7 ms: 1.36x faster                                                |
| scimark_monte_carlo      | 107 ms                                                       | 79.3 ms: 1.35x faster                                                |
| pyflate                  | 733 ms                                                       | 542 ms: 1.35x faster                                                 |
| float                    | 111 ms                                                       | 82.4 ms: 1.35x faster                                                |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 694 ms: 1.35x faster                                                 |
| unpickle_pure_python     | 312 us                                                       | 235 us: 1.33x faster                                                 |
| coroutines               | 30.3 ms                                                      | 23.0 ms: 1.32x faster                                                |
| logging_simple           | 8.88 us                                                      | 6.73 us: 1.32x faster                                                |
| deepcopy_memo            | 49.8 us                                                      | 37.8 us: 1.32x faster                                                |
| logging_format           | 9.64 us                                                      | 7.41 us: 1.30x faster                                                |
| xml_etree_process        | 75.9 ms                                                      | 58.7 ms: 1.29x faster                                                |
| regex_compile            | 190 ms                                                       | 147 ms: 1.29x faster                                                 |
| comprehensions           | 26.7 us                                                      | 20.8 us: 1.28x faster                                                |
| deepcopy                 | 468 us                                                       | 368 us: 1.27x faster                                                 |
| tornado_http             | 157 ms                                                       | 124 ms: 1.27x faster                                                 |
| pycparser                | 1.67 sec                                                     | 1.32 sec: 1.27x faster                                               |
| tomli_loads              | 2.92 sec                                                     | 2.30 sec: 1.27x faster                                               |
| scimark_sor              | 180 ms                                                       | 142 ms: 1.27x faster                                                 |
| nbody                    | 134 ms                                                       | 107 ms: 1.26x faster                                                 |
| bench_mp_pool            | 6.37 ms                                                      | 5.07 ms: 1.26x faster                                                |
| chameleon                | 9.44 ms                                                      | 7.53 ms: 1.25x faster                                                |
| mako                     | 14.7 ms                                                      | 11.9 ms: 1.23x faster                                                |
| json_loads               | 30.3 us                                                      | 24.8 us: 1.23x faster                                                |
| sqlglot_normalize        | 144 ms                                                       | 118 ms: 1.22x faster                                                 |
| pprint_safe_repr         | 1.05 sec                                                     | 864 ms: 1.22x faster                                                 |
| sympy_sum                | 193 ms                                                       | 159 ms: 1.21x faster                                                 |
| sympy_str                | 360 ms                                                       | 298 ms: 1.21x faster                                                 |
| deepcopy_reduce          | 4.01 us                                                      | 3.33 us: 1.20x faster                                                |
| pprint_pformat           | 2.15 sec                                                     | 1.80 sec: 1.20x faster                                               |
| spectral_norm            | 139 ms                                                       | 116 ms: 1.20x faster                                                 |
| sympy_expand             | 600 ms                                                       | 501 ms: 1.20x faster                                                 |
| dulwich_log              | 81.1 ms                                                      | 67.9 ms: 1.19x faster                                                |
| hexiom                   | 9.42 ms                                                      | 7.91 ms: 1.19x faster                                                |
| docutils                 | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                               |
| mdp                      | 3.01 sec                                                     | 2.56 sec: 1.17x faster                                               |
| dask                     | 472 ms                                                       | 403 ms: 1.17x faster                                                 |
| 2to3                     | 350 ms                                                       | 299 ms: 1.17x faster                                                 |
| nqueens                  | 115 ms                                                       | 98.5 ms: 1.17x faster                                                |
| bench_thread_pool        | 1.14 ms                                                      | 982 us: 1.16x faster                                                 |
| sympy_integrate          | 28.2 ms                                                      | 24.3 ms: 1.16x faster                                                |
| fannkuch                 | 483 ms                                                       | 418 ms: 1.15x faster                                                 |
| create_gc_cycles         | 1.76 ms                                                      | 1.53 ms: 1.15x faster                                                |
| sqlglot_optimize         | 70.1 ms                                                      | 61.0 ms: 1.15x faster                                                |
| async_generators         | 421 ms                                                       | 367 ms: 1.15x faster                                                 |
| pathlib                  | 21.4 ms                                                      | 18.8 ms: 1.14x faster                                                |
| json                     | 5.86 ms                                                      | 5.24 ms: 1.12x faster                                                |
| xml_etree_parse          | 160 ms                                                       | 144 ms: 1.12x faster                                                 |
| xml_etree_generate       | 92.3 ms                                                      | 84.9 ms: 1.09x faster                                                |
| sqlite_synth             | 2.99 us                                                      | 2.75 us: 1.09x faster                                                |
| regex_dna                | 261 ms                                                       | 246 ms: 1.06x faster                                                 |
| xml_etree_iterparse      | 110 ms                                                       | 105 ms: 1.05x faster                                                 |
| meteor_contest           | 138 ms                                                       | 133 ms: 1.04x faster                                                 |
| pidigits                 | 271 ms                                                       | 263 ms: 1.03x faster                                                 |
| regex_v8                 | 27.2 ms                                                      | 26.7 ms: 1.02x faster                                                |
| asyncio_websockets       | 390 ms                                                       | 386 ms: 1.01x faster                                                 |
| scimark_fft              | 361 ms                                                       | 368 ms: 1.02x slower                                                 |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 5.24 ms: 1.03x slower                                                |
| pickle_list              | 4.12 us                                                      | 4.38 us: 1.06x slower                                                |
| pickle_dict              | 29.5 us                                                      | 31.4 us: 1.06x slower                                                |
| pickle                   | 9.89 us                                                      | 10.6 us: 1.07x slower                                                |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.09x slower                                                |
| unpickle_list            | 4.65 us                                                      | 5.09 us: 1.10x slower                                                |
| unpickle                 | 13.5 us                                                      | 15.5 us: 1.15x slower                                                |
| regex_effbot             | 3.09 ms                                                      | 3.57 ms: 1.16x slower                                                |
| telco                    | 7.23 ms                                                      | 8.37 ms: 1.16x slower                                                |
| coverage                 | 63.3 ms                                                      | 88.0 ms: 1.39x slower                                                |
| python_startup_no_site   | 7.33 ms                                                      | 11.0 ms: 1.51x slower                                                |
| Geometric mean           | (ref)                                                        | 1.24x faster                                                         |

Benchmark hidden because not significant (2): mypy2, gc_traversal
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240125-3.13.0a3+-4d3e207-JIT/bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: 1.11x