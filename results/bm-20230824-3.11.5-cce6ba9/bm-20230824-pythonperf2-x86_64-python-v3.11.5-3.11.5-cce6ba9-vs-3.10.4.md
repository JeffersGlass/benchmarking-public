
# Results vs. 3.10.4

- fork: python
- ref: v3.11.5
- machine: linux-x86_64
- commit hash: cce6ba9
- commit date: 2023-08-24
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 285 ms: 1.23x faster                                         |
| chameleon      | 9.44 ms                                                      | 7.28 ms: 1.30x faster                                        |
| docutils       | 3.41 sec                                                     | 2.84 sec: 1.20x faster                                       |
| html5lib       | 94.6 ms                                                      | 71.4 ms: 1.33x faster                                        |
| tornado_http   | 157 ms                                                       | 124 ms: 1.27x faster                                         |
| Geometric mean | (ref)                                                        | 1.26x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.36x faster                                       |
| async_tree_none         | 692 ms                                                       | 518 ms: 1.34x faster                                         |
| async_tree_memoization  | 819 ms                                                       | 624 ms: 1.31x faster                                         |
| async_tree_cpu_io_mixed | 936 ms                                                       | 765 ms: 1.22x faster                                         |
| Geometric mean          | (ref)                                                        | 1.31x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| float          | 111 ms                                                       | 74.3 ms: 1.50x faster                                        |
| nbody          | 134 ms                                                       | 90.5 ms: 1.48x faster                                        |
| pidigits       | 271 ms                                                       | 251 ms: 1.08x faster                                         |
| Geometric mean | (ref)                                                        | 1.34x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 155 ms: 1.22x faster                                         |
| regex_dna      | 261 ms                                                       | 227 ms: 1.15x faster                                         |
| regex_v8       | 27.2 ms                                                      | 24.2 ms: 1.12x faster                                        |
| regex_effbot   | 3.09 ms                                                      | 3.31 ms: 1.07x slower                                        |
| Geometric mean | (ref)                                                        | 1.10x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 320 us: 1.42x faster                                         |
| xml_etree_process    | 75.9 ms                                                      | 56.1 ms: 1.35x faster                                        |
| unpickle_pure_python | 312 us                                                       | 241 us: 1.30x faster                                         |
| tomli_loads          | 2.92 sec                                                     | 2.30 sec: 1.27x faster                                       |
| xml_etree_generate   | 92.3 ms                                                      | 80.8 ms: 1.14x faster                                        |
| json_loads           | 30.3 us                                                      | 27.9 us: 1.09x faster                                        |
| json_dumps           | 14.5 ms                                                      | 13.5 ms: 1.08x faster                                        |
| xml_etree_iterparse  | 110 ms                                                       | 103 ms: 1.07x faster                                         |
| pickle_list          | 4.12 us                                                      | 3.94 us: 1.04x faster                                        |
| xml_etree_parse      | 160 ms                                                       | 157 ms: 1.02x faster                                         |
| unpickle             | 13.5 us                                                      | 13.3 us: 1.02x faster                                        |
| pickle               | 9.89 us                                                      | 9.98 us: 1.01x slower                                        |
| pickle_dict          | 29.5 us                                                      | 33.1 us: 1.12x slower                                        |
| Geometric mean       | (ref)                                                        | 1.11x faster                                                 |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.8 ms: 1.07x faster                                        |
| python_startup_no_site | 7.33 ms                                                      | 7.79 ms: 1.06x slower                                        |
| Geometric mean         | (ref)                                                        | 1.00x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.6 ms: 1.38x faster                                        |
| django_template | 50.2 ms                                                      | 40.7 ms: 1.23x faster                                        |
| genshi_text     | 31.4 ms                                                      | 25.5 ms: 1.23x faster                                        |
| genshi_xml      | 63.3 ms                                                      | 55.7 ms: 1.14x faster                                        |
| Geometric mean  | (ref)                                                        | 1.24x faster                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf2-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| deltablue                | 7.50 ms                                                      | 4.03 ms: 1.86x faster                                        |
| logging_silent           | 167 ns                                                       | 100 ns: 1.67x faster                                         |
| pyflate                  | 733 ms                                                       | 441 ms: 1.66x faster                                         |
| scimark_sor              | 180 ms                                                       | 111 ms: 1.62x faster                                         |
| go                       | 262 ms                                                       | 163 ms: 1.61x faster                                         |
| scimark_monte_carlo      | 107 ms                                                       | 69.0 ms: 1.56x faster                                        |
| raytrace                 | 489 ms                                                       | 318 ms: 1.54x faster                                         |
| float                    | 111 ms                                                       | 74.3 ms: 1.50x faster                                        |
| spectral_norm            | 139 ms                                                       | 93.3 ms: 1.49x faster                                        |
| nbody                    | 134 ms                                                       | 90.5 ms: 1.48x faster                                        |
| scimark_lu               | 167 ms                                                       | 113 ms: 1.47x faster                                         |
| crypto_pyaes             | 119 ms                                                       | 81.7 ms: 1.46x faster                                        |
| richards                 | 75.1 ms                                                      | 51.6 ms: 1.46x faster                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.54 ms: 1.45x faster                                        |
| pickle_pure_python       | 455 us                                                       | 320 us: 1.42x faster                                         |
| richards_super           | 90.6 ms                                                      | 64.3 ms: 1.41x faster                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.91 ms: 1.40x faster                                        |
| mako                     | 14.7 ms                                                      | 10.6 ms: 1.38x faster                                        |
| chaos                    | 109 ms                                                       | 79.1 ms: 1.37x faster                                        |
| async_tree_io            | 1.60 sec                                                     | 1.17 sec: 1.36x faster                                       |
| pprint_safe_repr         | 1.05 sec                                                     | 775 ms: 1.35x faster                                         |
| xml_etree_process        | 75.9 ms                                                      | 56.1 ms: 1.35x faster                                        |
| bench_mp_pool            | 6.37 ms                                                      | 4.75 ms: 1.34x faster                                        |
| pprint_pformat           | 2.15 sec                                                     | 1.61 sec: 1.34x faster                                       |
| async_tree_none          | 692 ms                                                       | 518 ms: 1.34x faster                                         |
| deepcopy_memo            | 49.8 us                                                      | 37.4 us: 1.33x faster                                        |
| html5lib                 | 94.6 ms                                                      | 71.4 ms: 1.33x faster                                        |
| async_generators         | 421 ms                                                       | 318 ms: 1.32x faster                                         |
| async_tree_memoization   | 819 ms                                                       | 624 ms: 1.31x faster                                         |
| hexiom                   | 9.42 ms                                                      | 7.21 ms: 1.31x faster                                        |
| chameleon                | 9.44 ms                                                      | 7.28 ms: 1.30x faster                                        |
| unpickle_pure_python     | 312 us                                                       | 241 us: 1.30x faster                                         |
| scimark_fft              | 361 ms                                                       | 280 ms: 1.29x faster                                         |
| unpack_sequence          | 59.9 ns                                                      | 46.9 ns: 1.28x faster                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.00 ms: 1.27x faster                                        |
| tornado_http             | 157 ms                                                       | 124 ms: 1.27x faster                                         |
| tomli_loads              | 2.92 sec                                                     | 2.30 sec: 1.27x faster                                       |
| pycparser                | 1.67 sec                                                     | 1.32 sec: 1.27x faster                                       |
| dulwich_log              | 81.1 ms                                                      | 65.3 ms: 1.24x faster                                        |
| django_template          | 50.2 ms                                                      | 40.7 ms: 1.23x faster                                        |
| genshi_text              | 31.4 ms                                                      | 25.5 ms: 1.23x faster                                        |
| logging_format           | 9.64 us                                                      | 7.83 us: 1.23x faster                                        |
| sqlalchemy_declarative   | 190 ms                                                       | 154 ms: 1.23x faster                                         |
| 2to3                     | 350 ms                                                       | 285 ms: 1.23x faster                                         |
| regex_compile            | 190 ms                                                       | 155 ms: 1.22x faster                                         |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 765 ms: 1.22x faster                                         |
| logging_simple           | 8.88 us                                                      | 7.33 us: 1.21x faster                                        |
| docutils                 | 3.41 sec                                                     | 2.84 sec: 1.20x faster                                       |
| aiohttp                  | 1.19 ms                                                      | 991 us: 1.20x faster                                         |
| thrift                   | 1.18 ms                                                      | 986 us: 1.19x faster                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 58.9 ms: 1.19x faster                                        |
| deepcopy                 | 468 us                                                       | 396 us: 1.18x faster                                         |
| deepcopy_reduce          | 4.01 us                                                      | 3.40 us: 1.18x faster                                        |
| sqlite_synth             | 2.99 us                                                      | 2.55 us: 1.17x faster                                        |
| sqlalchemy_imperative    | 22.7 ms                                                      | 19.5 ms: 1.16x faster                                        |
| gunicorn                 | 1.16 ms                                                      | 999 us: 1.16x faster                                         |
| sqlglot_normalize        | 144 ms                                                       | 124 ms: 1.16x faster                                         |
| dask                     | 472 ms                                                       | 409 ms: 1.15x faster                                         |
| bench_thread_pool        | 1.14 ms                                                      | 989 us: 1.15x faster                                         |
| regex_dna                | 261 ms                                                       | 227 ms: 1.15x faster                                         |
| flaskblogging            | 4.39 ms                                                      | 3.83 ms: 1.15x faster                                        |
| xml_etree_generate       | 92.3 ms                                                      | 80.8 ms: 1.14x faster                                        |
| genshi_xml               | 63.3 ms                                                      | 55.7 ms: 1.14x faster                                        |
| nqueens                  | 115 ms                                                       | 102 ms: 1.13x faster                                         |
| pathlib                  | 21.4 ms                                                      | 19.0 ms: 1.12x faster                                        |
| regex_v8                 | 27.2 ms                                                      | 24.2 ms: 1.12x faster                                        |
| sympy_integrate          | 28.2 ms                                                      | 25.6 ms: 1.10x faster                                        |
| pylint                   | 566 ms                                                       | 517 ms: 1.09x faster                                         |
| coroutines               | 30.3 ms                                                      | 27.7 ms: 1.09x faster                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.62 ms: 1.09x faster                                        |
| json_loads               | 30.3 us                                                      | 27.9 us: 1.09x faster                                        |
| mdp                      | 3.01 sec                                                     | 2.78 sec: 1.08x faster                                       |
| sympy_expand             | 600 ms                                                       | 555 ms: 1.08x faster                                         |
| pidigits                 | 271 ms                                                       | 251 ms: 1.08x faster                                         |
| json_dumps               | 14.5 ms                                                      | 13.5 ms: 1.08x faster                                        |
| xml_etree_iterparse      | 110 ms                                                       | 103 ms: 1.07x faster                                         |
| telco                    | 7.23 ms                                                      | 6.75 ms: 1.07x faster                                        |
| sympy_str                | 360 ms                                                       | 336 ms: 1.07x faster                                         |
| python_startup           | 11.5 ms                                                      | 10.8 ms: 1.07x faster                                        |
| comprehensions           | 26.7 us                                                      | 25.0 us: 1.07x faster                                        |
| json                     | 5.86 ms                                                      | 5.55 ms: 1.06x faster                                        |
| meteor_contest           | 138 ms                                                       | 131 ms: 1.06x faster                                         |
| sympy_sum                | 193 ms                                                       | 184 ms: 1.05x faster                                         |
| pickle_list              | 4.12 us                                                      | 3.94 us: 1.04x faster                                        |
| typing_runtime_protocols | 537 us                                                       | 518 us: 1.03x faster                                         |
| asyncio_tcp              | 779 ms                                                       | 753 ms: 1.03x faster                                         |
| generators               | 57.3 ms                                                      | 55.4 ms: 1.03x faster                                        |
| fannkuch                 | 483 ms                                                       | 470 ms: 1.03x faster                                         |
| xml_etree_parse          | 160 ms                                                       | 157 ms: 1.02x faster                                         |
| unpickle                 | 13.5 us                                                      | 13.3 us: 1.02x faster                                        |
| pickle                   | 9.89 us                                                      | 9.98 us: 1.01x slower                                        |
| python_startup_no_site   | 7.33 ms                                                      | 7.79 ms: 1.06x slower                                        |
| regex_effbot             | 3.09 ms                                                      | 3.31 ms: 1.07x slower                                        |
| gc_traversal             | 3.42 ms                                                      | 3.77 ms: 1.11x slower                                        |
| pickle_dict              | 29.5 us                                                      | 33.1 us: 1.12x slower                                        |
| Geometric mean           | (ref)                                                        | 1.21x faster                                                 |

Benchmark hidden because not significant (2): asyncio_tcp_ssl, unpickle_list
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.10x