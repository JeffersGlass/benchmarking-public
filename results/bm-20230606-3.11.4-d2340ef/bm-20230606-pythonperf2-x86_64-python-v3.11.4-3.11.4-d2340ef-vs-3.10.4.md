
# Results vs. 3.10.4

- fork: python
- ref: v3.11.4
- machine: linux-x86_64
- commit hash: d2340ef
- commit date: 2023-06-06
- overall geometric mean: 1.22x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 285 ms: 1.23x faster                                         |
| chameleon      | 9.44 ms                                                      | 7.63 ms: 1.24x faster                                        |
| docutils       | 3.41 sec                                                     | 2.83 sec: 1.21x faster                                       |
| html5lib       | 94.6 ms                                                      | 71.5 ms: 1.32x faster                                        |
| tornado_http   | 157 ms                                                       | 121 ms: 1.30x faster                                         |
| Geometric mean | (ref)                                                        | 1.26x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.36x faster                                       |
| async_tree_none         | 692 ms                                                       | 522 ms: 1.32x faster                                         |
| async_tree_memoization  | 819 ms                                                       | 630 ms: 1.30x faster                                         |
| async_tree_cpu_io_mixed | 936 ms                                                       | 758 ms: 1.24x faster                                         |
| Geometric mean          | (ref)                                                        | 1.30x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| float          | 111 ms                                                       | 73.8 ms: 1.51x faster                                        |
| nbody          | 134 ms                                                       | 95.6 ms: 1.40x faster                                        |
| pidigits       | 271 ms                                                       | 252 ms: 1.08x faster                                         |
| Geometric mean | (ref)                                                        | 1.32x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 155 ms: 1.23x faster                                         |
| regex_dna      | 261 ms                                                       | 231 ms: 1.13x faster                                         |
| regex_v8       | 27.2 ms                                                      | 24.5 ms: 1.11x faster                                        |
| regex_effbot   | 3.09 ms                                                      | 3.46 ms: 1.12x slower                                        |
| Geometric mean | (ref)                                                        | 1.08x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 321 us: 1.42x faster                                         |
| xml_etree_process    | 75.9 ms                                                      | 56.3 ms: 1.35x faster                                        |
| tomli_loads          | 2.92 sec                                                     | 2.27 sec: 1.28x faster                                       |
| unpickle_pure_python | 312 us                                                       | 243 us: 1.28x faster                                         |
| xml_etree_generate   | 92.3 ms                                                      | 81.0 ms: 1.14x faster                                        |
| pickle_list          | 4.12 us                                                      | 3.70 us: 1.11x faster                                        |
| json_dumps           | 14.5 ms                                                      | 13.4 ms: 1.09x faster                                        |
| json_loads           | 30.3 us                                                      | 28.4 us: 1.07x faster                                        |
| xml_etree_iterparse  | 110 ms                                                       | 105 ms: 1.06x faster                                         |
| unpickle             | 13.5 us                                                      | 13.0 us: 1.04x faster                                        |
| pickle_dict          | 29.5 us                                                      | 29.7 us: 1.01x slower                                        |
| unpickle_list        | 4.65 us                                                      | 4.69 us: 1.01x slower                                        |
| Geometric mean       | (ref)                                                        | 1.12x faster                                                 |

Benchmark hidden because not significant (2): xml_etree_parse, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.7 ms: 1.08x faster                                        |
| python_startup_no_site | 7.33 ms                                                      | 7.72 ms: 1.05x slower                                        |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.8 ms: 1.36x faster                                        |
| django_template | 50.2 ms                                                      | 39.7 ms: 1.26x faster                                        |
| genshi_text     | 31.4 ms                                                      | 25.6 ms: 1.23x faster                                        |
| genshi_xml      | 63.3 ms                                                      | 57.9 ms: 1.09x faster                                        |
| Geometric mean  | (ref)                                                        | 1.23x faster                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| deltablue                | 7.50 ms                                                      | 4.06 ms: 1.85x faster                                        |
| logging_silent           | 167 ns                                                       | 101 ns: 1.66x faster                                         |
| pyflate                  | 733 ms                                                       | 458 ms: 1.60x faster                                         |
| raytrace                 | 489 ms                                                       | 311 ms: 1.57x faster                                         |
| scimark_sor              | 180 ms                                                       | 115 ms: 1.57x faster                                         |
| scimark_monte_carlo      | 107 ms                                                       | 69.5 ms: 1.55x faster                                        |
| go                       | 262 ms                                                       | 170 ms: 1.54x faster                                         |
| float                    | 111 ms                                                       | 73.8 ms: 1.51x faster                                        |
| spectral_norm            | 139 ms                                                       | 94.1 ms: 1.48x faster                                        |
| scimark_lu               | 167 ms                                                       | 113 ms: 1.47x faster                                         |
| chaos                    | 109 ms                                                       | 75.0 ms: 1.45x faster                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.55 ms: 1.45x faster                                        |
| richards                 | 75.1 ms                                                      | 52.2 ms: 1.44x faster                                        |
| crypto_pyaes             | 119 ms                                                       | 83.1 ms: 1.43x faster                                        |
| pickle_pure_python       | 455 us                                                       | 321 us: 1.42x faster                                         |
| nbody                    | 134 ms                                                       | 95.6 ms: 1.40x faster                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.91 ms: 1.40x faster                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.58 ms: 1.39x faster                                        |
| richards_super           | 90.6 ms                                                      | 65.2 ms: 1.39x faster                                        |
| mako                     | 14.7 ms                                                      | 10.8 ms: 1.36x faster                                        |
| async_tree_io            | 1.60 sec                                                     | 1.17 sec: 1.36x faster                                       |
| xml_etree_process        | 75.9 ms                                                      | 56.3 ms: 1.35x faster                                        |
| pprint_safe_repr         | 1.05 sec                                                     | 784 ms: 1.34x faster                                         |
| hexiom                   | 9.42 ms                                                      | 7.06 ms: 1.33x faster                                        |
| pprint_pformat           | 2.15 sec                                                     | 1.62 sec: 1.33x faster                                       |
| async_tree_none          | 692 ms                                                       | 522 ms: 1.32x faster                                         |
| html5lib                 | 94.6 ms                                                      | 71.5 ms: 1.32x faster                                        |
| unpack_sequence          | 59.9 ns                                                      | 45.6 ns: 1.32x faster                                        |
| deepcopy_memo            | 49.8 us                                                      | 38.1 us: 1.31x faster                                        |
| async_generators         | 421 ms                                                       | 322 ms: 1.31x faster                                         |
| pycparser                | 1.67 sec                                                     | 1.28 sec: 1.31x faster                                       |
| async_tree_memoization   | 819 ms                                                       | 630 ms: 1.30x faster                                         |
| tornado_http             | 157 ms                                                       | 121 ms: 1.30x faster                                         |
| thrift                   | 1.18 ms                                                      | 912 us: 1.29x faster                                         |
| scimark_fft              | 361 ms                                                       | 281 ms: 1.29x faster                                         |
| tomli_loads              | 2.92 sec                                                     | 2.27 sec: 1.28x faster                                       |
| unpickle_pure_python     | 312 us                                                       | 243 us: 1.28x faster                                         |
| logging_format           | 9.64 us                                                      | 7.58 us: 1.27x faster                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.01 ms: 1.27x faster                                        |
| django_template          | 50.2 ms                                                      | 39.7 ms: 1.26x faster                                        |
| logging_simple           | 8.88 us                                                      | 7.05 us: 1.26x faster                                        |
| chameleon                | 9.44 ms                                                      | 7.63 ms: 1.24x faster                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 758 ms: 1.24x faster                                         |
| sqlalchemy_declarative   | 190 ms                                                       | 154 ms: 1.23x faster                                         |
| 2to3                     | 350 ms                                                       | 285 ms: 1.23x faster                                         |
| regex_compile            | 190 ms                                                       | 155 ms: 1.23x faster                                         |
| genshi_text              | 31.4 ms                                                      | 25.6 ms: 1.23x faster                                        |
| aiohttp                  | 1.19 ms                                                      | 980 us: 1.21x faster                                         |
| deepcopy                 | 468 us                                                       | 387 us: 1.21x faster                                         |
| docutils                 | 3.41 sec                                                     | 2.83 sec: 1.21x faster                                       |
| sqlite_synth             | 2.99 us                                                      | 2.48 us: 1.20x faster                                        |
| dulwich_log              | 81.1 ms                                                      | 67.6 ms: 1.20x faster                                        |
| sqlglot_optimize         | 70.1 ms                                                      | 58.7 ms: 1.19x faster                                        |
| sqlglot_normalize        | 144 ms                                                       | 122 ms: 1.18x faster                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.39 us: 1.18x faster                                        |
| gunicorn                 | 1.16 ms                                                      | 981 us: 1.18x faster                                         |
| dask                     | 472 ms                                                       | 402 ms: 1.17x faster                                         |
| nqueens                  | 115 ms                                                       | 98.5 ms: 1.17x faster                                        |
| sqlalchemy_imperative    | 22.7 ms                                                      | 19.6 ms: 1.16x faster                                        |
| bench_thread_pool        | 1.14 ms                                                      | 995 us: 1.15x faster                                         |
| xml_etree_generate       | 92.3 ms                                                      | 81.0 ms: 1.14x faster                                        |
| flaskblogging            | 4.39 ms                                                      | 3.87 ms: 1.13x faster                                        |
| regex_dna                | 261 ms                                                       | 231 ms: 1.13x faster                                         |
| pathlib                  | 21.4 ms                                                      | 18.9 ms: 1.13x faster                                        |
| pickle_list              | 4.12 us                                                      | 3.70 us: 1.11x faster                                        |
| pylint                   | 566 ms                                                       | 510 ms: 1.11x faster                                         |
| regex_v8                 | 27.2 ms                                                      | 24.5 ms: 1.11x faster                                        |
| sympy_integrate          | 28.2 ms                                                      | 25.6 ms: 1.10x faster                                        |
| fannkuch                 | 483 ms                                                       | 441 ms: 1.10x faster                                         |
| genshi_xml               | 63.3 ms                                                      | 57.9 ms: 1.09x faster                                        |
| sympy_expand             | 600 ms                                                       | 550 ms: 1.09x faster                                         |
| coroutines               | 30.3 ms                                                      | 27.8 ms: 1.09x faster                                        |
| json_dumps               | 14.5 ms                                                      | 13.4 ms: 1.09x faster                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.63 ms: 1.08x faster                                        |
| python_startup           | 11.5 ms                                                      | 10.7 ms: 1.08x faster                                        |
| sympy_str                | 360 ms                                                       | 334 ms: 1.08x faster                                         |
| pidigits                 | 271 ms                                                       | 252 ms: 1.08x faster                                         |
| telco                    | 7.23 ms                                                      | 6.75 ms: 1.07x faster                                        |
| comprehensions           | 26.7 us                                                      | 24.9 us: 1.07x faster                                        |
| json                     | 5.86 ms                                                      | 5.48 ms: 1.07x faster                                        |
| json_loads               | 30.3 us                                                      | 28.4 us: 1.07x faster                                        |
| meteor_contest           | 138 ms                                                       | 130 ms: 1.07x faster                                         |
| xml_etree_iterparse      | 110 ms                                                       | 105 ms: 1.06x faster                                         |
| sympy_sum                | 193 ms                                                       | 183 ms: 1.05x faster                                         |
| mdp                      | 3.01 sec                                                     | 2.86 sec: 1.05x faster                                       |
| generators               | 57.3 ms                                                      | 54.7 ms: 1.05x faster                                        |
| unpickle                 | 13.5 us                                                      | 13.0 us: 1.04x faster                                        |
| asyncio_tcp              | 779 ms                                                       | 751 ms: 1.04x faster                                         |
| typing_runtime_protocols | 537 us                                                       | 525 us: 1.02x faster                                         |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 3.07 sec: 1.01x faster                                       |
| pickle_dict              | 29.5 us                                                      | 29.7 us: 1.01x slower                                        |
| unpickle_list            | 4.65 us                                                      | 4.69 us: 1.01x slower                                        |
| python_startup_no_site   | 7.33 ms                                                      | 7.72 ms: 1.05x slower                                        |
| gc_traversal             | 3.42 ms                                                      | 3.70 ms: 1.08x slower                                        |
| regex_effbot             | 3.09 ms                                                      | 3.46 ms: 1.12x slower                                        |
| Geometric mean           | (ref)                                                        | 1.22x faster                                                 |

Benchmark hidden because not significant (2): xml_etree_parse, pickle
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: 1.10x