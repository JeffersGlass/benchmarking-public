
# Results vs. 3.10.4

- fork: python
- ref: ae460d450ab854ca66d5
- machine: linux-x86_64
- commit hash: ae460d4
- commit date: 2024-02-15
- overall geometric mean: 1.25x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 301 ms: 1.16x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.18 ms: 1.32x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.88 sec: 1.18x faster                                                       |
| tornado_http   | 157 ms                                                       | 123 ms: 1.27x faster                                                         |
| Geometric mean | (ref)                                                        | 1.23x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 436 ms: 1.59x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 547 ms: 1.50x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 701 ms: 1.34x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.47x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 81.7 ms: 1.36x faster                                                        |
| nbody          | 134 ms                                                       | 106 ms: 1.26x faster                                                         |
| pidigits       | 271 ms                                                       | 262 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.21x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 146 ms: 1.30x faster                                                         |
| regex_dna      | 261 ms                                                       | 249 ms: 1.05x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 26.1 ms: 1.04x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.49 ms: 1.13x slower                                                        |
| Geometric mean | (ref)                                                        | 1.06x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 305 us: 1.49x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.5 ms: 1.38x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 228 us: 1.37x faster                                                         |
| xml_etree_process    | 75.9 ms                                                      | 58.5 ms: 1.30x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.30 sec: 1.27x faster                                                       |
| json_loads           | 30.3 us                                                      | 25.2 us: 1.20x faster                                                        |
| xml_etree_generate   | 92.3 ms                                                      | 84.7 ms: 1.09x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| xml_etree_iterparse  | 110 ms                                                       | 104 ms: 1.06x faster                                                         |
| unpickle_list        | 4.65 us                                                      | 4.76 us: 1.03x slower                                                        |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 30.8 us: 1.04x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.47 us: 1.09x slower                                                        |
| unpickle             | 13.5 us                                                      | 15.3 us: 1.13x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.12x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.7 ms: 1.10x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 11.9 ms: 1.24x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 120 us: 4.48x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 376 ms: 2.07x faster                                                         |
| deltablue                | 7.50 ms                                                      | 3.69 ms: 2.03x faster                                                        |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.97x faster                                                       |
| raytrace                 | 489 ms                                                       | 278 ms: 1.76x faster                                                         |
| logging_silent           | 167 ns                                                       | 96.2 ns: 1.74x faster                                                        |
| generators               | 57.3 ms                                                      | 33.6 ms: 1.71x faster                                                        |
| scimark_lu               | 167 ms                                                       | 99.4 ms: 1.68x faster                                                        |
| richards_super           | 90.6 ms                                                      | 56.4 ms: 1.61x faster                                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.40 ms: 1.60x faster                                                        |
| async_tree_none          | 692 ms                                                       | 436 ms: 1.59x faster                                                         |
| go                       | 262 ms                                                       | 167 ms: 1.57x faster                                                         |
| chaos                    | 109 ms                                                       | 69.4 ms: 1.56x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 547 ms: 1.50x faster                                                         |
| pickle_pure_python       | 455 us                                                       | 305 us: 1.49x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                       |
| richards                 | 75.1 ms                                                      | 50.6 ms: 1.48x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 81.0 ms: 1.47x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.83 ms: 1.47x faster                                                        |
| comprehensions           | 26.7 us                                                      | 19.2 us: 1.39x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 77.6 ms: 1.38x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.5 ms: 1.38x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 228 us: 1.37x faster                                                         |
| pyflate                  | 733 ms                                                       | 538 ms: 1.36x faster                                                         |
| coroutines               | 30.3 ms                                                      | 22.3 ms: 1.36x faster                                                        |
| float                    | 111 ms                                                       | 81.7 ms: 1.36x faster                                                        |
| deepcopy_memo            | 49.8 us                                                      | 37.0 us: 1.34x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.75 ms: 1.34x faster                                                        |
| unpack_sequence          | 59.9 ns                                                      | 44.8 ns: 1.34x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 701 ms: 1.34x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.66 us: 1.33x faster                                                        |
| chameleon                | 9.44 ms                                                      | 7.18 ms: 1.32x faster                                                        |
| regex_compile            | 190 ms                                                       | 146 ms: 1.30x faster                                                         |
| logging_format           | 9.64 us                                                      | 7.43 us: 1.30x faster                                                        |
| xml_etree_process        | 75.9 ms                                                      | 58.5 ms: 1.30x faster                                                        |
| scimark_sor              | 180 ms                                                       | 141 ms: 1.28x faster                                                         |
| deepcopy                 | 468 us                                                       | 367 us: 1.28x faster                                                         |
| tornado_http             | 157 ms                                                       | 123 ms: 1.27x faster                                                         |
| pycparser                | 1.67 sec                                                     | 1.32 sec: 1.27x faster                                                       |
| tomli_loads              | 2.92 sec                                                     | 2.30 sec: 1.27x faster                                                       |
| nbody                    | 134 ms                                                       | 106 ms: 1.26x faster                                                         |
| spectral_norm            | 139 ms                                                       | 111 ms: 1.26x faster                                                         |
| hexiom                   | 9.42 ms                                                      | 7.60 ms: 1.24x faster                                                        |
| mako                     | 14.7 ms                                                      | 11.9 ms: 1.24x faster                                                        |
| pprint_pformat           | 2.15 sec                                                     | 1.74 sec: 1.24x faster                                                       |
| pprint_safe_repr         | 1.05 sec                                                     | 856 ms: 1.23x faster                                                         |
| sympy_sum                | 193 ms                                                       | 158 ms: 1.22x faster                                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.31 us: 1.21x faster                                                        |
| sqlglot_normalize        | 144 ms                                                       | 119 ms: 1.21x faster                                                         |
| sympy_str                | 360 ms                                                       | 298 ms: 1.21x faster                                                         |
| json_loads               | 30.3 us                                                      | 25.2 us: 1.20x faster                                                        |
| nqueens                  | 115 ms                                                       | 96.7 ms: 1.19x faster                                                        |
| sympy_expand             | 600 ms                                                       | 505 ms: 1.19x faster                                                         |
| docutils                 | 3.41 sec                                                     | 2.88 sec: 1.18x faster                                                       |
| mdp                      | 3.01 sec                                                     | 2.54 sec: 1.18x faster                                                       |
| sympy_integrate          | 28.2 ms                                                      | 23.8 ms: 1.18x faster                                                        |
| dulwich_log              | 81.1 ms                                                      | 69.0 ms: 1.17x faster                                                        |
| fannkuch                 | 483 ms                                                       | 412 ms: 1.17x faster                                                         |
| bench_thread_pool        | 1.14 ms                                                      | 976 us: 1.17x faster                                                         |
| dask                     | 472 ms                                                       | 404 ms: 1.17x faster                                                         |
| 2to3                     | 350 ms                                                       | 301 ms: 1.16x faster                                                         |
| create_gc_cycles         | 1.76 ms                                                      | 1.54 ms: 1.14x faster                                                        |
| sqlglot_optimize         | 70.1 ms                                                      | 61.5 ms: 1.14x faster                                                        |
| pathlib                  | 21.4 ms                                                      | 18.8 ms: 1.14x faster                                                        |
| json                     | 5.86 ms                                                      | 5.31 ms: 1.11x faster                                                        |
| async_generators         | 421 ms                                                       | 382 ms: 1.10x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 84.7 ms: 1.09x faster                                                        |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| sqlite_synth             | 2.99 us                                                      | 2.78 us: 1.08x faster                                                        |
| xml_etree_iterparse      | 110 ms                                                       | 104 ms: 1.06x faster                                                         |
| regex_dna                | 261 ms                                                       | 249 ms: 1.05x faster                                                         |
| scimark_fft              | 361 ms                                                       | 345 ms: 1.05x faster                                                         |
| meteor_contest           | 138 ms                                                       | 133 ms: 1.04x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 26.1 ms: 1.04x faster                                                        |
| pidigits                 | 271 ms                                                       | 262 ms: 1.03x faster                                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.95 ms: 1.03x faster                                                        |
| asyncio_websockets       | 390 ms                                                       | 386 ms: 1.01x faster                                                         |
| unpickle_list            | 4.65 us                                                      | 4.76 us: 1.03x slower                                                        |
| pickle                   | 9.89 us                                                      | 10.3 us: 1.04x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 30.8 us: 1.04x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.71 ms: 1.09x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.47 us: 1.09x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.7 ms: 1.10x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.49 ms: 1.13x slower                                                        |
| unpickle                 | 13.5 us                                                      | 15.3 us: 1.13x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.24 ms: 1.14x slower                                                        |
| coverage                 | 63.3 ms                                                      | 79.5 ms: 1.26x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.25x faster                                                                 |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a3+-ae460d4-JIT/bm-20240215-pythonperf2-x86_64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.21x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: 1.11x