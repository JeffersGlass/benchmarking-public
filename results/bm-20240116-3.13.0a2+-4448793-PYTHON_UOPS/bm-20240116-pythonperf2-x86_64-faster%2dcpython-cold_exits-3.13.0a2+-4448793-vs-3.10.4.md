
# Results vs. 3.10.4

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 4448793
- commit date: 2024-01-16
- overall geometric mean: 1.13x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 318 ms: 1.10x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.85 ms: 1.20x faster                                                        |
| docutils       | 3.41 sec                                                     | 3.08 sec: 1.11x faster                                                       |
| tornado_http   | 157 ms                                                       | 124 ms: 1.27x faster                                                         |
| Geometric mean | (ref)                                                        | 1.17x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 450 ms: 1.54x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 562 ms: 1.46x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.10 sec: 1.46x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 712 ms: 1.31x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.44x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 106 ms: 1.05x faster                                                         |
| pidigits       | 271 ms                                                       | 265 ms: 1.02x faster                                                         |
| nbody          | 134 ms                                                       | 131 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 261 ms                                                       | 250 ms: 1.04x faster                                                         |
| regex_compile  | 190 ms                                                       | 194 ms: 1.02x slower                                                         |
| regex_effbot   | 3.09 ms                                                      | 3.48 ms: 1.13x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 310 us: 1.47x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 11.0 ms: 1.32x faster                                                        |
| json_loads           | 30.3 us                                                      | 24.6 us: 1.23x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 62.6 ms: 1.21x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| tomli_loads          | 2.92 sec                                                     | 2.89 sec: 1.01x faster                                                       |
| unpickle_pure_python | 312 us                                                       | 317 us: 1.02x slower                                                         |
| pickle               | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 114 ms: 1.03x slower                                                         |
| pickle_dict          | 29.5 us                                                      | 30.8 us: 1.04x slower                                                        |
| unpickle_list        | 4.65 us                                                      | 4.97 us: 1.07x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.50 us: 1.09x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.7 us: 1.09x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.06x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 14.9 ms: 1.02x slower                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 127 us: 4.23x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 373 ms: 2.09x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.95x faster                                                       |
| generators               | 57.3 ms                                                      | 33.6 ms: 1.70x faster                                                        |
| logging_silent           | 167 ns                                                       | 99.4 ns: 1.68x faster                                                        |
| async_tree_none          | 692 ms                                                       | 450 ms: 1.54x faster                                                         |
| raytrace                 | 489 ms                                                       | 319 ms: 1.53x faster                                                         |
| pickle_pure_python       | 455 us                                                       | 310 us: 1.47x faster                                                         |
| async_tree_memoization   | 819 ms                                                       | 562 ms: 1.46x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.10 sec: 1.46x faster                                                       |
| sqlglot_parse            | 2.24 ms                                                      | 1.54 ms: 1.45x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 85.7 ms: 1.39x faster                                                        |
| chaos                    | 109 ms                                                       | 78.5 ms: 1.38x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.1 ms: 1.37x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.96 ms: 1.37x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.73 ms: 1.35x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 11.0 ms: 1.32x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 712 ms: 1.31x faster                                                         |
| deltablue                | 7.50 ms                                                      | 5.76 ms: 1.30x faster                                                        |
| go                       | 262 ms                                                       | 202 ms: 1.30x faster                                                         |
| logging_format           | 9.64 us                                                      | 7.57 us: 1.27x faster                                                        |
| tornado_http             | 157 ms                                                       | 124 ms: 1.27x faster                                                         |
| logging_simple           | 8.88 us                                                      | 7.03 us: 1.26x faster                                                        |
| json_loads               | 30.3 us                                                      | 24.6 us: 1.23x faster                                                        |
| deepcopy                 | 468 us                                                       | 381 us: 1.23x faster                                                         |
| xml_etree_process        | 75.9 ms                                                      | 62.6 ms: 1.21x faster                                                        |
| deepcopy_memo            | 49.8 us                                                      | 41.2 us: 1.21x faster                                                        |
| chameleon                | 9.44 ms                                                      | 7.85 ms: 1.20x faster                                                        |
| deepcopy_reduce          | 4.01 us                                                      | 3.34 us: 1.20x faster                                                        |
| scimark_lu               | 167 ms                                                       | 140 ms: 1.20x faster                                                         |
| pycparser                | 1.67 sec                                                     | 1.44 sec: 1.16x faster                                                       |
| bench_thread_pool        | 1.14 ms                                                      | 990 us: 1.15x faster                                                         |
| dask                     | 472 ms                                                       | 412 ms: 1.15x faster                                                         |
| mdp                      | 3.01 sec                                                     | 2.64 sec: 1.14x faster                                                       |
| richards_super           | 90.6 ms                                                      | 80.0 ms: 1.13x faster                                                        |
| scimark_sor              | 180 ms                                                       | 160 ms: 1.13x faster                                                         |
| sqlglot_normalize        | 144 ms                                                       | 128 ms: 1.13x faster                                                         |
| json                     | 5.86 ms                                                      | 5.28 ms: 1.11x faster                                                        |
| async_generators         | 421 ms                                                       | 379 ms: 1.11x faster                                                         |
| pyflate                  | 733 ms                                                       | 660 ms: 1.11x faster                                                         |
| docutils                 | 3.41 sec                                                     | 3.08 sec: 1.11x faster                                                       |
| create_gc_cycles         | 1.76 ms                                                      | 1.59 ms: 1.11x faster                                                        |
| sympy_sum                | 193 ms                                                       | 175 ms: 1.10x faster                                                         |
| 2to3                     | 350 ms                                                       | 318 ms: 1.10x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 19.5 ms: 1.09x faster                                                        |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| sympy_integrate          | 28.2 ms                                                      | 26.0 ms: 1.09x faster                                                        |
| sympy_expand             | 600 ms                                                       | 556 ms: 1.08x faster                                                         |
| dulwich_log              | 81.1 ms                                                      | 75.7 ms: 1.07x faster                                                        |
| sympy_str                | 360 ms                                                       | 336 ms: 1.07x faster                                                         |
| sqlite_synth             | 2.99 us                                                      | 2.81 us: 1.07x faster                                                        |
| float                    | 111 ms                                                       | 106 ms: 1.05x faster                                                         |
| pprint_safe_repr         | 1.05 sec                                                     | 998 ms: 1.05x faster                                                         |
| pprint_pformat           | 2.15 sec                                                     | 2.05 sec: 1.05x faster                                                       |
| richards                 | 75.1 ms                                                      | 71.6 ms: 1.05x faster                                                        |
| regex_dna                | 261 ms                                                       | 250 ms: 1.04x faster                                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 67.3 ms: 1.04x faster                                                        |
| pidigits                 | 271 ms                                                       | 265 ms: 1.02x faster                                                         |
| nbody                    | 134 ms                                                       | 131 ms: 1.02x faster                                                         |
| scimark_monte_carlo      | 107 ms                                                       | 105 ms: 1.02x faster                                                         |
| comprehensions           | 26.7 us                                                      | 26.2 us: 1.02x faster                                                        |
| asyncio_websockets       | 390 ms                                                       | 386 ms: 1.01x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.89 sec: 1.01x faster                                                       |
| nqueens                  | 115 ms                                                       | 116 ms: 1.01x slower                                                         |
| unpickle_pure_python     | 312 us                                                       | 317 us: 1.02x slower                                                         |
| mako                     | 14.7 ms                                                      | 14.9 ms: 1.02x slower                                                        |
| meteor_contest           | 138 ms                                                       | 141 ms: 1.02x slower                                                         |
| regex_compile            | 190 ms                                                       | 194 ms: 1.02x slower                                                         |
| pickle                   | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| xml_etree_iterparse      | 110 ms                                                       | 114 ms: 1.03x slower                                                         |
| pickle_dict              | 29.5 us                                                      | 30.8 us: 1.04x slower                                                        |
| fannkuch                 | 483 ms                                                       | 516 ms: 1.07x slower                                                         |
| unpickle_list            | 4.65 us                                                      | 4.97 us: 1.07x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.50 us: 1.09x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.7 us: 1.09x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| unpack_sequence          | 59.9 ns                                                      | 66.4 ns: 1.11x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.81 ms: 1.12x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.48 ms: 1.13x slower                                                        |
| hexiom                   | 9.42 ms                                                      | 10.9 ms: 1.15x slower                                                        |
| spectral_norm            | 139 ms                                                       | 161 ms: 1.16x slower                                                         |
| telco                    | 7.23 ms                                                      | 8.51 ms: 1.18x slower                                                        |
| scimark_fft              | 361 ms                                                       | 426 ms: 1.18x slower                                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 6.23 ms: 1.23x slower                                                        |
| coverage                 | 63.3 ms                                                      | 79.1 ms: 1.25x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.13x faster                                                                 |

Benchmark hidden because not significant (3): regex_v8, mypy2, xml_etree_generate
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240116-3.13.0a2+-4448793-PYTHON_UOPS/bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: 1.07x