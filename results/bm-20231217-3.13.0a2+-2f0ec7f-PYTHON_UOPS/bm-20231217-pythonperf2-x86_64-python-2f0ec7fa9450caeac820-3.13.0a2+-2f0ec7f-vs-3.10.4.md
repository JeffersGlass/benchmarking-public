
# Results vs. 3.10.4

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: linux-x86_64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.20x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 308 ms: 1.14x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.85 ms: 1.20x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.94 sec: 1.16x faster                                                       |
| tornado_http   | 157 ms                                                       | 125 ms: 1.25x faster                                                         |
| Geometric mean | (ref)                                                        | 1.19x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 444 ms: 1.56x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 557 ms: 1.47x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.09 sec: 1.47x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 711 ms: 1.32x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.45x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 112 ms: 1.20x faster                                                         |
| float          | 111 ms                                                       | 93.7 ms: 1.19x faster                                                        |
| pidigits       | 271 ms                                                       | 265 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.13x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 168 ms: 1.13x faster                                                         |
| regex_dna      | 261 ms                                                       | 245 ms: 1.07x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 25.6 ms: 1.06x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.54 ms: 1.15x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 312 us: 1.46x faster                                                         |
| unpickle_pure_python | 312 us                                                       | 228 us: 1.37x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.7 ms: 1.36x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 60.9 ms: 1.25x faster                                                        |
| json_loads           | 30.3 us                                                      | 25.4 us: 1.19x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.67 sec: 1.09x faster                                                       |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| xml_etree_generate   | 92.3 ms                                                      | 90.1 ms: 1.02x faster                                                        |
| unpickle_list        | 4.65 us                                                      | 4.61 us: 1.01x faster                                                        |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 31.6 us: 1.07x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.5 us: 1.08x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.47 us: 1.09x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.10x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.0 ms: 1.51x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.28x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 13.6 ms: 1.08x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 127 us: 4.21x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 377 ms: 2.06x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.95x faster                                                       |
| logging_silent           | 167 ns                                                       | 97.9 ns: 1.71x faster                                                        |
| generators               | 57.3 ms                                                      | 33.8 ms: 1.70x faster                                                        |
| raytrace                 | 489 ms                                                       | 294 ms: 1.66x faster                                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.42 ms: 1.58x faster                                                        |
| scimark_lu               | 167 ms                                                       | 107 ms: 1.56x faster                                                         |
| async_tree_none          | 692 ms                                                       | 444 ms: 1.56x faster                                                         |
| deltablue                | 7.50 ms                                                      | 4.94 ms: 1.52x faster                                                        |
| richards_super           | 90.6 ms                                                      | 59.9 ms: 1.51x faster                                                        |
| chaos                    | 109 ms                                                       | 73.7 ms: 1.47x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 557 ms: 1.47x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.09 sec: 1.47x faster                                                       |
| sqlglot_transpile        | 2.68 ms                                                      | 1.83 ms: 1.47x faster                                                        |
| pickle_pure_python       | 455 us                                                       | 312 us: 1.46x faster                                                         |
| crypto_pyaes             | 119 ms                                                       | 82.1 ms: 1.45x faster                                                        |
| go                       | 262 ms                                                       | 183 ms: 1.43x faster                                                         |
| richards                 | 75.1 ms                                                      | 54.2 ms: 1.39x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.66 ms: 1.37x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 228 us: 1.37x faster                                                         |
| json_dumps               | 14.5 ms                                                      | 10.7 ms: 1.36x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.4 ms: 1.35x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 711 ms: 1.32x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.80 us: 1.31x faster                                                        |
| pyflate                  | 733 ms                                                       | 569 ms: 1.29x faster                                                         |
| logging_format           | 9.64 us                                                      | 7.51 us: 1.28x faster                                                        |
| unpack_sequence          | 59.9 ns                                                      | 46.7 ns: 1.28x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 84.6 ms: 1.27x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.33 sec: 1.26x faster                                                       |
| tornado_http             | 157 ms                                                       | 125 ms: 1.25x faster                                                         |
| xml_etree_process        | 75.9 ms                                                      | 60.9 ms: 1.25x faster                                                        |
| deepcopy_memo            | 49.8 us                                                      | 40.4 us: 1.23x faster                                                        |
| scimark_sor              | 180 ms                                                       | 148 ms: 1.21x faster                                                         |
| deepcopy                 | 468 us                                                       | 386 us: 1.21x faster                                                         |
| chameleon                | 9.44 ms                                                      | 7.85 ms: 1.20x faster                                                        |
| nbody                    | 134 ms                                                       | 112 ms: 1.20x faster                                                         |
| json_loads               | 30.3 us                                                      | 25.4 us: 1.19x faster                                                        |
| float                    | 111 ms                                                       | 93.7 ms: 1.19x faster                                                        |
| deepcopy_reduce          | 4.01 us                                                      | 3.39 us: 1.18x faster                                                        |
| sqlglot_normalize        | 144 ms                                                       | 122 ms: 1.18x faster                                                         |
| bench_thread_pool        | 1.14 ms                                                      | 974 us: 1.17x faster                                                         |
| docutils                 | 3.41 sec                                                     | 2.94 sec: 1.16x faster                                                       |
| pprint_safe_repr         | 1.05 sec                                                     | 904 ms: 1.16x faster                                                         |
| pprint_pformat           | 2.15 sec                                                     | 1.86 sec: 1.16x faster                                                       |
| comprehensions           | 26.7 us                                                      | 23.1 us: 1.15x faster                                                        |
| mdp                      | 3.01 sec                                                     | 2.61 sec: 1.15x faster                                                       |
| dask                     | 472 ms                                                       | 410 ms: 1.15x faster                                                         |
| sympy_sum                | 193 ms                                                       | 169 ms: 1.14x faster                                                         |
| 2to3                     | 350 ms                                                       | 308 ms: 1.14x faster                                                         |
| regex_compile            | 190 ms                                                       | 168 ms: 1.13x faster                                                         |
| sympy_integrate          | 28.2 ms                                                      | 25.0 ms: 1.13x faster                                                        |
| async_generators         | 421 ms                                                       | 375 ms: 1.12x faster                                                         |
| dulwich_log              | 81.1 ms                                                      | 72.6 ms: 1.12x faster                                                        |
| sqlglot_optimize         | 70.1 ms                                                      | 63.0 ms: 1.11x faster                                                        |
| nqueens                  | 115 ms                                                       | 104 ms: 1.11x faster                                                         |
| sympy_str                | 360 ms                                                       | 325 ms: 1.11x faster                                                         |
| json                     | 5.86 ms                                                      | 5.31 ms: 1.10x faster                                                        |
| sympy_expand             | 600 ms                                                       | 545 ms: 1.10x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.67 sec: 1.09x faster                                                       |
| pathlib                  | 21.4 ms                                                      | 19.5 ms: 1.09x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.62 ms: 1.09x faster                                                        |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| sqlite_synth             | 2.99 us                                                      | 2.76 us: 1.08x faster                                                        |
| fannkuch                 | 483 ms                                                       | 447 ms: 1.08x faster                                                         |
| mako                     | 14.7 ms                                                      | 13.6 ms: 1.08x faster                                                        |
| regex_dna                | 261 ms                                                       | 245 ms: 1.07x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 25.6 ms: 1.06x faster                                                        |
| xml_etree_generate       | 92.3 ms                                                      | 90.1 ms: 1.02x faster                                                        |
| pidigits                 | 271 ms                                                       | 265 ms: 1.02x faster                                                         |
| hexiom                   | 9.42 ms                                                      | 9.23 ms: 1.02x faster                                                        |
| asyncio_websockets       | 390 ms                                                       | 385 ms: 1.01x faster                                                         |
| unpickle_list            | 4.65 us                                                      | 4.61 us: 1.01x faster                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.56 ms: 1.04x slower                                                        |
| pickle                   | 9.89 us                                                      | 10.4 us: 1.05x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 31.6 us: 1.07x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.5 us: 1.08x slower                                                        |
| spectral_norm            | 139 ms                                                       | 150 ms: 1.08x slower                                                         |
| pickle_list              | 4.12 us                                                      | 4.47 us: 1.09x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| scimark_fft              | 361 ms                                                       | 396 ms: 1.10x slower                                                         |
| telco                    | 7.23 ms                                                      | 8.21 ms: 1.14x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.54 ms: 1.15x slower                                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 6.01 ms: 1.18x slower                                                        |
| coverage                 | 63.3 ms                                                      | 84.6 ms: 1.34x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.0 ms: 1.51x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.20x faster                                                                 |

Benchmark hidden because not significant (3): mypy2, meteor_contest, xml_etree_iterparse
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: 1.07x