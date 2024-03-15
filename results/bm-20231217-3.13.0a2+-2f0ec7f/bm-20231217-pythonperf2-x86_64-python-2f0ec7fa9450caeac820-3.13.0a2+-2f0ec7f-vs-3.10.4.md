
# Results vs. 3.10.4

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: linux-x86_64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 295 ms: 1.19x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.40 ms: 1.28x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.84 sec: 1.20x faster                                                       |
| tornado_http   | 157 ms                                                       | 118 ms: 1.33x faster                                                         |
| Geometric mean | (ref)                                                        | 1.25x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 432 ms: 1.60x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 544 ms: 1.51x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 695 ms: 1.35x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.48x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 91.2 ms: 1.47x faster                                                        |
| float          | 111 ms                                                       | 78.8 ms: 1.41x faster                                                        |
| pidigits       | 271 ms                                                       | 264 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.29x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 141 ms: 1.35x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 26.1 ms: 1.04x faster                                                        |
| regex_dna      | 261 ms                                                       | 256 ms: 1.02x faster                                                         |
| regex_effbot   | 3.09 ms                                                      | 3.64 ms: 1.18x slower                                                        |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 310 us: 1.47x faster                                                         |
| unpickle_pure_python | 312 us                                                       | 222 us: 1.41x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.5 ms: 1.39x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 57.9 ms: 1.31x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.28 sec: 1.28x faster                                                       |
| json_loads           | 30.3 us                                                      | 25.7 us: 1.18x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 148 ms: 1.08x faster                                                         |
| xml_etree_generate   | 92.3 ms                                                      | 85.4 ms: 1.08x faster                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 106 ms: 1.04x faster                                                         |
| unpickle_list        | 4.65 us                                                      | 4.69 us: 1.01x slower                                                        |
| pickle               | 9.89 us                                                      | 9.99 us: 1.01x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.19 us: 1.02x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.5 us: 1.08x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 31.8 us: 1.08x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.0 ms: 1.50x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.28x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.1 ms: 1.45x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 116 us: 4.63x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 367 ms: 2.13x faster                                                         |
| deltablue                | 7.50 ms                                                      | 3.54 ms: 2.12x faster                                                        |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                                       |
| raytrace                 | 489 ms                                                       | 259 ms: 1.89x faster                                                         |
| chaos                    | 109 ms                                                       | 60.3 ms: 1.80x faster                                                        |
| logging_silent           | 167 ns                                                       | 96.5 ns: 1.73x faster                                                        |
| scimark_lu               | 167 ms                                                       | 98.2 ms: 1.70x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 70.3 ms: 1.69x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 65.3 ms: 1.64x faster                                                        |
| comprehensions           | 26.7 us                                                      | 16.4 us: 1.62x faster                                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.39 ms: 1.61x faster                                                        |
| generators               | 57.3 ms                                                      | 35.6 ms: 1.61x faster                                                        |
| async_tree_none          | 692 ms                                                       | 432 ms: 1.60x faster                                                         |
| go                       | 262 ms                                                       | 169 ms: 1.54x faster                                                         |
| spectral_norm            | 139 ms                                                       | 91.2 ms: 1.52x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 544 ms: 1.51x faster                                                         |
| sqlglot_transpile        | 2.68 ms                                                      | 1.80 ms: 1.49x faster                                                        |
| async_tree_io            | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                       |
| hexiom                   | 9.42 ms                                                      | 6.35 ms: 1.48x faster                                                        |
| richards_super           | 90.6 ms                                                      | 61.2 ms: 1.48x faster                                                        |
| nbody                    | 134 ms                                                       | 91.2 ms: 1.47x faster                                                        |
| pickle_pure_python       | 455 us                                                       | 310 us: 1.47x faster                                                         |
| mako                     | 14.7 ms                                                      | 10.1 ms: 1.45x faster                                                        |
| pyflate                  | 733 ms                                                       | 508 ms: 1.44x faster                                                         |
| float                    | 111 ms                                                       | 78.8 ms: 1.41x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 222 us: 1.41x faster                                                         |
| bench_mp_pool            | 6.37 ms                                                      | 4.57 ms: 1.39x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.5 ms: 1.39x faster                                                        |
| richards                 | 75.1 ms                                                      | 54.8 ms: 1.37x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.3 ms: 1.36x faster                                                        |
| logging_simple           | 8.88 us                                                      | 6.56 us: 1.35x faster                                                        |
| regex_compile            | 190 ms                                                       | 141 ms: 1.35x faster                                                         |
| deepcopy_memo            | 49.8 us                                                      | 36.9 us: 1.35x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 695 ms: 1.35x faster                                                         |
| tornado_http             | 157 ms                                                       | 118 ms: 1.33x faster                                                         |
| logging_format           | 9.64 us                                                      | 7.27 us: 1.33x faster                                                        |
| nqueens                  | 115 ms                                                       | 87.4 ms: 1.32x faster                                                        |
| pprint_pformat           | 2.15 sec                                                     | 1.64 sec: 1.32x faster                                                       |
| xml_etree_process        | 75.9 ms                                                      | 57.9 ms: 1.31x faster                                                        |
| pprint_safe_repr         | 1.05 sec                                                     | 806 ms: 1.30x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.28 sec: 1.28x faster                                                       |
| chameleon                | 9.44 ms                                                      | 7.40 ms: 1.28x faster                                                        |
| sympy_sum                | 193 ms                                                       | 151 ms: 1.27x faster                                                         |
| pycparser                | 1.67 sec                                                     | 1.32 sec: 1.27x faster                                                       |
| deepcopy                 | 468 us                                                       | 369 us: 1.27x faster                                                         |
| scimark_sor              | 180 ms                                                       | 144 ms: 1.25x faster                                                         |
| unpack_sequence          | 59.9 ns                                                      | 48.2 ns: 1.24x faster                                                        |
| sqlglot_normalize        | 144 ms                                                       | 116 ms: 1.24x faster                                                         |
| sympy_str                | 360 ms                                                       | 293 ms: 1.23x faster                                                         |
| sympy_integrate          | 28.2 ms                                                      | 23.1 ms: 1.22x faster                                                        |
| fannkuch                 | 483 ms                                                       | 395 ms: 1.22x faster                                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.18 ms: 1.22x faster                                                        |
| deepcopy_reduce          | 4.01 us                                                      | 3.30 us: 1.21x faster                                                        |
| dulwich_log              | 81.1 ms                                                      | 67.2 ms: 1.21x faster                                                        |
| mdp                      | 3.01 sec                                                     | 2.49 sec: 1.21x faster                                                       |
| bench_thread_pool        | 1.14 ms                                                      | 947 us: 1.21x faster                                                         |
| docutils                 | 3.41 sec                                                     | 2.84 sec: 1.20x faster                                                       |
| sympy_expand             | 600 ms                                                       | 502 ms: 1.20x faster                                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 58.8 ms: 1.19x faster                                                        |
| 2to3                     | 350 ms                                                       | 295 ms: 1.19x faster                                                         |
| scimark_fft              | 361 ms                                                       | 305 ms: 1.18x faster                                                         |
| json_loads               | 30.3 us                                                      | 25.7 us: 1.18x faster                                                        |
| async_generators         | 421 ms                                                       | 356 ms: 1.18x faster                                                         |
| dask                     | 472 ms                                                       | 400 ms: 1.18x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 19.0 ms: 1.12x faster                                                        |
| json                     | 5.86 ms                                                      | 5.29 ms: 1.11x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.71 us: 1.10x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.62 ms: 1.09x faster                                                        |
| meteor_contest           | 138 ms                                                       | 128 ms: 1.08x faster                                                         |
| mypy2                    | 933 ms                                                       | 861 ms: 1.08x faster                                                         |
| xml_etree_parse          | 160 ms                                                       | 148 ms: 1.08x faster                                                         |
| xml_etree_generate       | 92.3 ms                                                      | 85.4 ms: 1.08x faster                                                        |
| regex_v8                 | 27.2 ms                                                      | 26.1 ms: 1.04x faster                                                        |
| xml_etree_iterparse      | 110 ms                                                       | 106 ms: 1.04x faster                                                         |
| pidigits                 | 271 ms                                                       | 264 ms: 1.03x faster                                                         |
| regex_dna                | 261 ms                                                       | 256 ms: 1.02x faster                                                         |
| unpickle_list            | 4.65 us                                                      | 4.69 us: 1.01x slower                                                        |
| pickle                   | 9.89 us                                                      | 9.99 us: 1.01x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.19 us: 1.02x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.56 ms: 1.04x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.5 us: 1.08x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 31.8 us: 1.08x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.15 ms: 1.13x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.64 ms: 1.18x slower                                                        |
| coverage                 | 63.3 ms                                                      | 78.0 ms: 1.23x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.0 ms: 1.50x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.29x faster                                                                 |

Benchmark hidden because not significant (1): asyncio_websockets
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.06x