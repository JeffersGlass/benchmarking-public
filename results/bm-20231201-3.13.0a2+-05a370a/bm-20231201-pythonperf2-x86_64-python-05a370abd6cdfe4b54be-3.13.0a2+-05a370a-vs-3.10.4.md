
# Results vs. 3.10.4

- fork: python
- ref: 05a370abd6cdfe4b54be
- machine: linux-x86_64
- commit hash: 05a370a
- commit date: 2023-12-01
- overall geometric mean: 1.28x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 293 ms: 1.20x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.34 ms: 1.29x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.82 sec: 1.21x faster                                                       |
| tornado_http   | 157 ms                                                       | 119 ms: 1.32x faster                                                         |
| Geometric mean | (ref)                                                        | 1.25x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 432 ms: 1.60x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 545 ms: 1.50x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 699 ms: 1.34x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.48x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 85.9 ms: 1.56x faster                                                        |
| float          | 111 ms                                                       | 79.4 ms: 1.40x faster                                                        |
| pidigits       | 271 ms                                                       | 264 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.31x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 145 ms: 1.31x faster                                                         |
| regex_dna      | 261 ms                                                       | 236 ms: 1.11x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 24.8 ms: 1.09x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.46 ms: 1.12x slower                                                        |
| Geometric mean | (ref)                                                        | 1.09x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 213 us: 1.46x faster                                                         |
| pickle_pure_python   | 455 us                                                       | 312 us: 1.46x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.23 sec: 1.31x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 58.5 ms: 1.30x faster                                                        |
| json_loads           | 30.3 us                                                      | 25.5 us: 1.19x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| xml_etree_generate   | 92.3 ms                                                      | 85.1 ms: 1.08x faster                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 107 ms: 1.03x faster                                                         |
| unpickle_list        | 4.65 us                                                      | 4.71 us: 1.01x slower                                                        |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.5 us: 1.07x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.46 us: 1.08x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 32.8 us: 1.11x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.8 ms: 1.11x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.2 ms: 1.53x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.31x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.2 ms: 1.45x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 126 us: 4.26x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 369 ms: 2.11x faster                                                         |
| deltablue                | 7.50 ms                                                      | 3.64 ms: 2.06x faster                                                        |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                                       |
| raytrace                 | 489 ms                                                       | 278 ms: 1.76x faster                                                         |
| chaos                    | 109 ms                                                       | 62.0 ms: 1.75x faster                                                        |
| logging_silent           | 167 ns                                                       | 97.0 ns: 1.72x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 69.6 ms: 1.71x faster                                                        |
| generators               | 57.3 ms                                                      | 34.3 ms: 1.67x faster                                                        |
| scimark_lu               | 167 ms                                                       | 102 ms: 1.63x faster                                                         |
| async_tree_none          | 692 ms                                                       | 432 ms: 1.60x faster                                                         |
| scimark_monte_carlo      | 107 ms                                                       | 67.4 ms: 1.59x faster                                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.41 ms: 1.58x faster                                                        |
| comprehensions           | 26.7 us                                                      | 16.9 us: 1.58x faster                                                        |
| go                       | 262 ms                                                       | 167 ms: 1.57x faster                                                         |
| nbody                    | 134 ms                                                       | 85.9 ms: 1.56x faster                                                        |
| spectral_norm            | 139 ms                                                       | 90.5 ms: 1.54x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 545 ms: 1.50x faster                                                         |
| richards_super           | 90.6 ms                                                      | 60.4 ms: 1.50x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.82 ms: 1.48x faster                                                        |
| async_tree_io            | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                       |
| unpickle_pure_python     | 312 us                                                       | 213 us: 1.46x faster                                                         |
| pickle_pure_python       | 455 us                                                       | 312 us: 1.46x faster                                                         |
| hexiom                   | 9.42 ms                                                      | 6.47 ms: 1.46x faster                                                        |
| pyflate                  | 733 ms                                                       | 505 ms: 1.45x faster                                                         |
| mako                     | 14.7 ms                                                      | 10.2 ms: 1.45x faster                                                        |
| float                    | 111 ms                                                       | 79.4 ms: 1.40x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.57 ms: 1.40x faster                                                        |
| richards                 | 75.1 ms                                                      | 53.9 ms: 1.39x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                        |
| pprint_pformat           | 2.15 sec                                                     | 1.58 sec: 1.36x faster                                                       |
| pprint_safe_repr         | 1.05 sec                                                     | 773 ms: 1.36x faster                                                         |
| coroutines               | 30.3 ms                                                      | 22.5 ms: 1.35x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 699 ms: 1.34x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.68 us: 1.33x faster                                                        |
| tornado_http             | 157 ms                                                       | 119 ms: 1.32x faster                                                         |
| deepcopy_memo            | 49.8 us                                                      | 37.8 us: 1.32x faster                                                        |
| regex_compile            | 190 ms                                                       | 145 ms: 1.31x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.23 sec: 1.31x faster                                                       |
| nqueens                  | 115 ms                                                       | 88.3 ms: 1.30x faster                                                        |
| xml_etree_process        | 75.9 ms                                                      | 58.5 ms: 1.30x faster                                                        |
| chameleon                | 9.44 ms                                                      | 7.34 ms: 1.29x faster                                                        |
| sympy_sum                | 193 ms                                                       | 150 ms: 1.28x faster                                                         |
| logging_format           | 9.64 us                                                      | 7.51 us: 1.28x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.33 sec: 1.26x faster                                                       |
| deepcopy                 | 468 us                                                       | 373 us: 1.26x faster                                                         |
| sympy_str                | 360 ms                                                       | 290 ms: 1.24x faster                                                         |
| unpack_sequence          | 59.9 ns                                                      | 48.3 ns: 1.24x faster                                                        |
| fannkuch                 | 483 ms                                                       | 390 ms: 1.24x faster                                                         |
| sqlglot_normalize        | 144 ms                                                       | 116 ms: 1.24x faster                                                         |
| sympy_integrate          | 28.2 ms                                                      | 23.0 ms: 1.23x faster                                                        |
| sympy_expand             | 600 ms                                                       | 490 ms: 1.22x faster                                                         |
| scimark_sor              | 180 ms                                                       | 149 ms: 1.21x faster                                                         |
| bench_thread_pool        | 1.14 ms                                                      | 942 us: 1.21x faster                                                         |
| docutils                 | 3.41 sec                                                     | 2.82 sec: 1.21x faster                                                       |
| deepcopy_reduce          | 4.01 us                                                      | 3.32 us: 1.21x faster                                                        |
| dulwich_log              | 81.1 ms                                                      | 67.7 ms: 1.20x faster                                                        |
| 2to3                     | 350 ms                                                       | 293 ms: 1.20x faster                                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 58.6 ms: 1.20x faster                                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.25 ms: 1.19x faster                                                        |
| mdp                      | 3.01 sec                                                     | 2.52 sec: 1.19x faster                                                       |
| dask                     | 472 ms                                                       | 396 ms: 1.19x faster                                                         |
| json_loads               | 30.3 us                                                      | 25.5 us: 1.19x faster                                                        |
| async_generators         | 421 ms                                                       | 362 ms: 1.16x faster                                                         |
| scimark_fft              | 361 ms                                                       | 314 ms: 1.15x faster                                                         |
| json                     | 5.86 ms                                                      | 5.22 ms: 1.12x faster                                                        |
| pathlib                  | 21.4 ms                                                      | 19.0 ms: 1.12x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.59 ms: 1.11x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.70 us: 1.11x faster                                                        |
| regex_dna                | 261 ms                                                       | 236 ms: 1.11x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 24.8 ms: 1.09x faster                                                        |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 85.1 ms: 1.08x faster                                                        |
| mypy2                    | 933 ms                                                       | 861 ms: 1.08x faster                                                         |
| meteor_contest           | 138 ms                                                       | 129 ms: 1.08x faster                                                         |
| xml_etree_iterparse      | 110 ms                                                       | 107 ms: 1.03x faster                                                         |
| pidigits                 | 271 ms                                                       | 264 ms: 1.02x faster                                                         |
| asyncio_websockets       | 390 ms                                                       | 386 ms: 1.01x faster                                                         |
| unpickle_list            | 4.65 us                                                      | 4.71 us: 1.01x slower                                                        |
| pickle                   | 9.89 us                                                      | 10.3 us: 1.04x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.5 us: 1.07x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.46 us: 1.08x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.75 ms: 1.10x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 32.8 us: 1.11x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.8 ms: 1.11x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.06 ms: 1.12x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.46 ms: 1.12x slower                                                        |
| coverage                 | 63.3 ms                                                      | 80.6 ms: 1.27x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.2 ms: 1.53x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.28x faster                                                                 |
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-pythonperf2-x86_64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.06x