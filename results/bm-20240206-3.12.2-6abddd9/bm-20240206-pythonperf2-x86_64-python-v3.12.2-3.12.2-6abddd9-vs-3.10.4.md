
# Results vs. 3.10.4

- fork: python
- ref: v3.12.2
- machine: linux-x86_64
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.30x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 284 ms: 1.23x faster                                         |
| chameleon      | 9.44 ms                                                      | 7.35 ms: 1.28x faster                                        |
| docutils       | 3.41 sec                                                     | 2.85 sec: 1.20x faster                                       |
| tornado_http   | 157 ms                                                       | 119 ms: 1.32x faster                                         |
| Geometric mean | (ref)                                                        | 1.26x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 458 ms: 1.51x faster                                         |
| async_tree_io           | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                       |
| async_tree_memoization  | 819 ms                                                       | 550 ms: 1.49x faster                                         |
| async_tree_cpu_io_mixed | 936 ms                                                       | 703 ms: 1.33x faster                                         |
| Geometric mean          | (ref)                                                        | 1.46x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 87.7 ms: 1.53x faster                                        |
| float          | 111 ms                                                       | 77.7 ms: 1.43x faster                                        |
| pidigits       | 271 ms                                                       | 265 ms: 1.02x faster                                         |
| Geometric mean | (ref)                                                        | 1.31x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 140 ms: 1.36x faster                                         |
| regex_v8       | 27.2 ms                                                      | 23.7 ms: 1.14x faster                                        |
| regex_dna      | 261 ms                                                       | 236 ms: 1.11x faster                                         |
| regex_effbot   | 3.09 ms                                                      | 3.43 ms: 1.11x slower                                        |
| Geometric mean | (ref)                                                        | 1.12x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 203 us: 1.53x faster                                         |
| pickle_pure_python   | 455 us                                                       | 321 us: 1.42x faster                                         |
| json_dumps           | 14.5 ms                                                      | 10.4 ms: 1.40x faster                                        |
| tomli_loads          | 2.92 sec                                                     | 2.17 sec: 1.34x faster                                       |
| xml_etree_process    | 75.9 ms                                                      | 58.9 ms: 1.29x faster                                        |
| json_loads           | 30.3 us                                                      | 24.5 us: 1.24x faster                                        |
| xml_etree_parse      | 160 ms                                                       | 149 ms: 1.08x faster                                         |
| xml_etree_generate   | 92.3 ms                                                      | 86.1 ms: 1.07x faster                                        |
| xml_etree_iterparse  | 110 ms                                                       | 104 ms: 1.07x faster                                         |
| unpickle_list        | 4.65 us                                                      | 4.69 us: 1.01x slower                                        |
| pickle               | 9.89 us                                                      | 10.3 us: 1.05x slower                                        |
| pickle_list          | 4.12 us                                                      | 4.52 us: 1.10x slower                                        |
| pickle_dict          | 29.5 us                                                      | 32.4 us: 1.10x slower                                        |
| unpickle             | 13.5 us                                                      | 14.9 us: 1.10x slower                                        |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 11.6 ms: 1.00x slower                                        |
| python_startup_no_site | 7.33 ms                                                      | 8.50 ms: 1.16x slower                                        |
| Geometric mean         | (ref)                                                        | 1.08x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 9.97 ms: 1.47x faster                                        |
| django_template | 50.2 ms                                                      | 38.5 ms: 1.30x faster                                        |
| Geometric mean  | (ref)                                                        | 1.39x faster                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 124 us: 4.34x faster                                         |
| deltablue                | 7.50 ms                                                      | 3.24 ms: 2.31x faster                                        |
| asyncio_tcp              | 779 ms                                                       | 374 ms: 2.08x faster                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.56 sec: 1.99x faster                                       |
| richards_super           | 90.6 ms                                                      | 50.8 ms: 1.78x faster                                        |
| go                       | 262 ms                                                       | 149 ms: 1.75x faster                                         |
| chaos                    | 109 ms                                                       | 63.1 ms: 1.72x faster                                        |
| richards                 | 75.1 ms                                                      | 44.3 ms: 1.69x faster                                        |
| scimark_lu               | 167 ms                                                       | 99.7 ms: 1.67x faster                                        |
| logging_silent           | 167 ns                                                       | 100 ns: 1.67x faster                                         |
| raytrace                 | 489 ms                                                       | 298 ms: 1.64x faster                                         |
| scimark_sor              | 180 ms                                                       | 110 ms: 1.64x faster                                         |
| sqlglot_parse            | 2.24 ms                                                      | 1.40 ms: 1.60x faster                                        |
| pyflate                  | 733 ms                                                       | 461 ms: 1.59x faster                                         |
| scimark_monte_carlo      | 107 ms                                                       | 68.0 ms: 1.58x faster                                        |
| generators               | 57.3 ms                                                      | 36.7 ms: 1.56x faster                                        |
| hexiom                   | 9.42 ms                                                      | 6.07 ms: 1.55x faster                                        |
| unpickle_pure_python     | 312 us                                                       | 203 us: 1.53x faster                                         |
| nbody                    | 134 ms                                                       | 87.7 ms: 1.53x faster                                        |
| async_tree_none          | 692 ms                                                       | 458 ms: 1.51x faster                                         |
| async_tree_io            | 1.60 sec                                                     | 1.06 sec: 1.51x faster                                       |
| crypto_pyaes             | 119 ms                                                       | 79.5 ms: 1.50x faster                                        |
| spectral_norm            | 139 ms                                                       | 92.8 ms: 1.50x faster                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.80 ms: 1.49x faster                                        |
| async_tree_memoization   | 819 ms                                                       | 550 ms: 1.49x faster                                         |
| mako                     | 14.7 ms                                                      | 9.97 ms: 1.47x faster                                        |
| float                    | 111 ms                                                       | 77.7 ms: 1.43x faster                                        |
| fannkuch                 | 483 ms                                                       | 339 ms: 1.42x faster                                         |
| pickle_pure_python       | 455 us                                                       | 321 us: 1.42x faster                                         |
| json_dumps               | 14.5 ms                                                      | 10.4 ms: 1.40x faster                                        |
| regex_compile            | 190 ms                                                       | 140 ms: 1.36x faster                                         |
| deepcopy_memo            | 49.8 us                                                      | 37.1 us: 1.34x faster                                        |
| tomli_loads              | 2.92 sec                                                     | 2.17 sec: 1.34x faster                                       |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 703 ms: 1.33x faster                                         |
| pycparser                | 1.67 sec                                                     | 1.27 sec: 1.32x faster                                       |
| logging_simple           | 8.88 us                                                      | 6.72 us: 1.32x faster                                        |
| coroutines               | 30.3 ms                                                      | 22.9 ms: 1.32x faster                                        |
| tornado_http             | 157 ms                                                       | 119 ms: 1.32x faster                                         |
| logging_format           | 9.64 us                                                      | 7.40 us: 1.30x faster                                        |
| django_template          | 50.2 ms                                                      | 38.5 ms: 1.30x faster                                        |
| nqueens                  | 115 ms                                                       | 88.6 ms: 1.30x faster                                        |
| mypy2                    | 933 ms                                                       | 723 ms: 1.29x faster                                         |
| xml_etree_process        | 75.9 ms                                                      | 58.9 ms: 1.29x faster                                        |
| chameleon                | 9.44 ms                                                      | 7.35 ms: 1.28x faster                                        |
| pprint_pformat           | 2.15 sec                                                     | 1.68 sec: 1.28x faster                                       |
| bench_mp_pool            | 6.37 ms                                                      | 5.00 ms: 1.28x faster                                        |
| pprint_safe_repr         | 1.05 sec                                                     | 827 ms: 1.27x faster                                         |
| comprehensions           | 26.7 us                                                      | 21.1 us: 1.26x faster                                        |
| deepcopy                 | 468 us                                                       | 371 us: 1.26x faster                                         |
| dulwich_log              | 81.1 ms                                                      | 64.9 ms: 1.25x faster                                        |
| scimark_fft              | 361 ms                                                       | 290 ms: 1.25x faster                                         |
| json_loads               | 30.3 us                                                      | 24.5 us: 1.24x faster                                        |
| 2to3                     | 350 ms                                                       | 284 ms: 1.23x faster                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.12 ms: 1.23x faster                                        |
| sqlalchemy_imperative    | 22.7 ms                                                      | 18.6 ms: 1.22x faster                                        |
| sqlglot_normalize        | 144 ms                                                       | 119 ms: 1.21x faster                                         |
| sympy_expand             | 600 ms                                                       | 496 ms: 1.21x faster                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 58.0 ms: 1.21x faster                                        |
| dask                     | 472 ms                                                       | 392 ms: 1.21x faster                                         |
| bench_thread_pool        | 1.14 ms                                                      | 949 us: 1.20x faster                                         |
| sympy_sum                | 193 ms                                                       | 161 ms: 1.20x faster                                         |
| docutils                 | 3.41 sec                                                     | 2.85 sec: 1.20x faster                                       |
| sympy_integrate          | 28.2 ms                                                      | 23.7 ms: 1.19x faster                                        |
| sympy_str                | 360 ms                                                       | 303 ms: 1.19x faster                                         |
| sqlalchemy_declarative   | 190 ms                                                       | 160 ms: 1.18x faster                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.39 us: 1.18x faster                                        |
| mdp                      | 3.01 sec                                                     | 2.56 sec: 1.17x faster                                       |
| gunicorn                 | 1.16 ms                                                      | 996 us: 1.16x faster                                         |
| aiohttp                  | 1.19 ms                                                      | 1.02 ms: 1.16x faster                                        |
| unpack_sequence          | 59.9 ns                                                      | 52.0 ns: 1.15x faster                                        |
| regex_v8                 | 27.2 ms                                                      | 23.7 ms: 1.14x faster                                        |
| json                     | 5.86 ms                                                      | 5.18 ms: 1.13x faster                                        |
| pathlib                  | 21.4 ms                                                      | 19.1 ms: 1.12x faster                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.58 ms: 1.11x faster                                        |
| regex_dna                | 261 ms                                                       | 236 ms: 1.11x faster                                         |
| meteor_contest           | 138 ms                                                       | 126 ms: 1.10x faster                                         |
| sqlite_synth             | 2.99 us                                                      | 2.73 us: 1.10x faster                                        |
| xml_etree_parse          | 160 ms                                                       | 149 ms: 1.08x faster                                         |
| xml_etree_generate       | 92.3 ms                                                      | 86.1 ms: 1.07x faster                                        |
| async_generators         | 421 ms                                                       | 393 ms: 1.07x faster                                         |
| xml_etree_iterparse      | 110 ms                                                       | 104 ms: 1.07x faster                                         |
| pidigits                 | 271 ms                                                       | 265 ms: 1.02x faster                                         |
| asyncio_websockets       | 390 ms                                                       | 385 ms: 1.01x faster                                         |
| python_startup           | 11.5 ms                                                      | 11.6 ms: 1.00x slower                                        |
| unpickle_list            | 4.65 us                                                      | 4.69 us: 1.01x slower                                        |
| pickle                   | 9.89 us                                                      | 10.3 us: 1.05x slower                                        |
| coverage                 | 63.3 ms                                                      | 66.4 ms: 1.05x slower                                        |
| gc_traversal             | 3.42 ms                                                      | 3.74 ms: 1.10x slower                                        |
| pickle_list              | 4.12 us                                                      | 4.52 us: 1.10x slower                                        |
| pickle_dict              | 29.5 us                                                      | 32.4 us: 1.10x slower                                        |
| unpickle                 | 13.5 us                                                      | 14.9 us: 1.10x slower                                        |
| regex_effbot             | 3.09 ms                                                      | 3.43 ms: 1.11x slower                                        |
| python_startup_no_site   | 7.33 ms                                                      | 8.50 ms: 1.16x slower                                        |
| Geometric mean           | (ref)                                                        | 1.30x faster                                                 |

Benchmark hidden because not significant (1): telco
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
Ignored benchmarks (4) of results/bm-20240206-3.12.2-6abddd9/bm-20240206-pythonperf2-x86_64-python-v3.12.2-3.12.2-6abddd9.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.10x