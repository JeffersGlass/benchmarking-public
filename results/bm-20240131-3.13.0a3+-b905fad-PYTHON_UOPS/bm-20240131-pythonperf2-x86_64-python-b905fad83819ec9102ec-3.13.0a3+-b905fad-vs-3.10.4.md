
# Results vs. 3.10.4

- fork: python
- ref: b905fad83819ec9102ec
- machine: linux-x86_64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 308 ms: 1.14x faster                                                         |
| chameleon      | 9.44 ms                                                      | 8.14 ms: 1.16x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.95 sec: 1.16x faster                                                       |
| tornado_http   | 157 ms                                                       | 126 ms: 1.24x faster                                                         |
| Geometric mean | (ref)                                                        | 1.17x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 443 ms: 1.56x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 555 ms: 1.48x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 708 ms: 1.32x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.46x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 104 ms: 1.07x faster                                                         |
| nbody          | 134 ms                                                       | 129 ms: 1.04x faster                                                         |
| pidigits       | 271 ms                                                       | 266 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                        | 1.04x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 169 ms: 1.12x faster                                                         |
| regex_dna      | 261 ms                                                       | 243 ms: 1.08x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 25.7 ms: 1.06x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.49 ms: 1.13x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 312 us: 1.46x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 242 us: 1.29x faster                                                         |
| xml_etree_process    | 75.9 ms                                                      | 62.2 ms: 1.22x faster                                                        |
| json_loads           | 30.3 us                                                      | 24.9 us: 1.22x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| tomli_loads          | 2.92 sec                                                     | 2.81 sec: 1.04x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 89.9 ms: 1.03x faster                                                        |
| unpickle_list        | 4.65 us                                                      | 4.80 us: 1.03x slower                                                        |
| pickle               | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 116 ms: 1.05x slower                                                         |
| pickle_dict          | 29.5 us                                                      | 31.1 us: 1.05x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.40 us: 1.07x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.9 us: 1.11x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.08x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 15.0 ms: 1.02x slower                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 128 us: 4.20x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 374 ms: 2.08x faster                                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.60 sec: 1.93x faster                                                       |
| logging_silent           | 167 ns                                                       | 97.0 ns: 1.73x faster                                                        |
| generators               | 57.3 ms                                                      | 34.1 ms: 1.68x faster                                                        |
| raytrace                 | 489 ms                                                       | 298 ms: 1.64x faster                                                         |
| scimark_lu               | 167 ms                                                       | 104 ms: 1.61x faster                                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.43 ms: 1.56x faster                                                        |
| async_tree_none          | 692 ms                                                       | 443 ms: 1.56x faster                                                         |
| richards_super           | 90.6 ms                                                      | 60.1 ms: 1.51x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 555 ms: 1.48x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                       |
| pickle_pure_python       | 455 us                                                       | 312 us: 1.46x faster                                                         |
| go                       | 262 ms                                                       | 180 ms: 1.46x faster                                                         |
| sqlglot_transpile        | 2.68 ms                                                      | 1.86 ms: 1.44x faster                                                        |
| chaos                    | 109 ms                                                       | 78.0 ms: 1.39x faster                                                        |
| richards                 | 75.1 ms                                                      | 54.1 ms: 1.39x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 86.0 ms: 1.39x faster                                                        |
| unpack_sequence          | 59.9 ns                                                      | 43.3 ns: 1.38x faster                                                        |
| deltablue                | 7.50 ms                                                      | 5.43 ms: 1.38x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.4 ms: 1.35x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.75 ms: 1.34x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 708 ms: 1.32x faster                                                         |
| logging_simple           | 8.88 us                                                      | 6.85 us: 1.30x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 242 us: 1.29x faster                                                         |
| logging_format           | 9.64 us                                                      | 7.54 us: 1.28x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.33 sec: 1.26x faster                                                       |
| pyflate                  | 733 ms                                                       | 586 ms: 1.25x faster                                                         |
| tornado_http             | 157 ms                                                       | 126 ms: 1.24x faster                                                         |
| deepcopy                 | 468 us                                                       | 380 us: 1.23x faster                                                         |
| scimark_sor              | 180 ms                                                       | 147 ms: 1.23x faster                                                         |
| scimark_monte_carlo      | 107 ms                                                       | 87.5 ms: 1.23x faster                                                        |
| xml_etree_process        | 75.9 ms                                                      | 62.2 ms: 1.22x faster                                                        |
| json_loads               | 30.3 us                                                      | 24.9 us: 1.22x faster                                                        |
| deepcopy_memo            | 49.8 us                                                      | 41.2 us: 1.21x faster                                                        |
| deepcopy_reduce          | 4.01 us                                                      | 3.42 us: 1.17x faster                                                        |
| sqlglot_normalize        | 144 ms                                                       | 123 ms: 1.17x faster                                                         |
| chameleon                | 9.44 ms                                                      | 8.14 ms: 1.16x faster                                                        |
| bench_thread_pool        | 1.14 ms                                                      | 984 us: 1.16x faster                                                         |
| docutils                 | 3.41 sec                                                     | 2.95 sec: 1.16x faster                                                       |
| dask                     | 472 ms                                                       | 411 ms: 1.15x faster                                                         |
| mdp                      | 3.01 sec                                                     | 2.62 sec: 1.15x faster                                                       |
| sympy_sum                | 193 ms                                                       | 168 ms: 1.15x faster                                                         |
| 2to3                     | 350 ms                                                       | 308 ms: 1.14x faster                                                         |
| sympy_integrate          | 28.2 ms                                                      | 24.8 ms: 1.14x faster                                                        |
| async_generators         | 421 ms                                                       | 372 ms: 1.13x faster                                                         |
| sympy_expand             | 600 ms                                                       | 532 ms: 1.13x faster                                                         |
| pprint_safe_repr         | 1.05 sec                                                     | 931 ms: 1.13x faster                                                         |
| regex_compile            | 190 ms                                                       | 169 ms: 1.12x faster                                                         |
| dulwich_log              | 81.1 ms                                                      | 72.5 ms: 1.12x faster                                                        |
| sympy_str                | 360 ms                                                       | 322 ms: 1.12x faster                                                         |
| pprint_pformat           | 2.15 sec                                                     | 1.93 sec: 1.12x faster                                                       |
| json                     | 5.86 ms                                                      | 5.25 ms: 1.12x faster                                                        |
| sqlglot_optimize         | 70.1 ms                                                      | 63.3 ms: 1.11x faster                                                        |
| pathlib                  | 21.4 ms                                                      | 19.3 ms: 1.11x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.60 ms: 1.10x faster                                                        |
| xml_etree_parse          | 160 ms                                                       | 147 ms: 1.09x faster                                                         |
| regex_dna                | 261 ms                                                       | 243 ms: 1.08x faster                                                         |
| sqlite_synth             | 2.99 us                                                      | 2.79 us: 1.07x faster                                                        |
| float                    | 111 ms                                                       | 104 ms: 1.07x faster                                                         |
| comprehensions           | 26.7 us                                                      | 25.1 us: 1.06x faster                                                        |
| regex_v8                 | 27.2 ms                                                      | 25.7 ms: 1.06x faster                                                        |
| nqueens                  | 115 ms                                                       | 109 ms: 1.06x faster                                                         |
| nbody                    | 134 ms                                                       | 129 ms: 1.04x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.81 sec: 1.04x faster                                                       |
| xml_etree_generate       | 92.3 ms                                                      | 89.9 ms: 1.03x faster                                                        |
| pidigits                 | 271 ms                                                       | 266 ms: 1.02x faster                                                         |
| fannkuch                 | 483 ms                                                       | 474 ms: 1.02x faster                                                         |
| asyncio_websockets       | 390 ms                                                       | 386 ms: 1.01x faster                                                         |
| meteor_contest           | 138 ms                                                       | 137 ms: 1.01x faster                                                         |
| mako                     | 14.7 ms                                                      | 15.0 ms: 1.02x slower                                                        |
| unpickle_list            | 4.65 us                                                      | 4.80 us: 1.03x slower                                                        |
| pickle                   | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| hexiom                   | 9.42 ms                                                      | 9.82 ms: 1.04x slower                                                        |
| xml_etree_iterparse      | 110 ms                                                       | 116 ms: 1.05x slower                                                         |
| pickle_dict              | 29.5 us                                                      | 31.1 us: 1.05x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.40 us: 1.07x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.73 ms: 1.09x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.9 us: 1.11x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.49 ms: 1.13x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.24 ms: 1.14x slower                                                        |
| spectral_norm            | 139 ms                                                       | 162 ms: 1.17x slower                                                         |
| scimark_fft              | 361 ms                                                       | 434 ms: 1.20x slower                                                         |
| coverage                 | 63.3 ms                                                      | 78.8 ms: 1.25x slower                                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 6.71 ms: 1.32x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.18x faster                                                                 |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: 1.07x