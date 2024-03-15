# Results vs. 3.10.4

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: linux-x86_64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.36x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 310 ms: 1.13x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.45 ms: 1.27x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.96 sec: 1.15x faster                                                       |
| tornado_http   | 157 ms                                                       | 127 ms: 1.24x faster                                                         |
| Geometric mean | (ref)                                                        | 1.20x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 444 ms: 1.56x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 560 ms: 1.46x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.10 sec: 1.45x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 715 ms: 1.31x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.44x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 78.8 ms: 1.41x faster                                                        |
| nbody          | 134 ms                                                       | 102 ms: 1.31x faster                                                         |
| pidigits       | 271 ms                                                       | 262 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.24x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 154 ms: 1.23x faster                                                         |
| regex_dna      | 261 ms                                                       | 239 ms: 1.09x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 25.3 ms: 1.07x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                                        |
| Geometric mean | (ref)                                                        | 1.06x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 319 us: 1.43x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.4 ms: 1.39x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 243 us: 1.28x faster                                                         |
| xml_etree_process    | 75.9 ms                                                      | 59.5 ms: 1.28x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.39 sec: 1.22x faster                                                       |
| json_loads           | 30.3 us                                                      | 25.0 us: 1.21x faster                                                        |
| xml_etree_generate   | 92.3 ms                                                      | 86.8 ms: 1.06x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 151 ms: 1.06x faster                                                         |
| xml_etree_iterparse  | 110 ms                                                       | 106 ms: 1.05x faster                                                         |
| unpickle_list        | 4.65 us                                                      | 4.60 us: 1.01x faster                                                        |
| pickle_dict          | 29.5 us                                                      | 30.4 us: 1.03x slower                                                        |
| pickle               | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.6 us: 1.08x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.51 us: 1.10x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.11x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 15.7 ms: 1.36x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 14.1 ms: 1.93x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.62x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.7 ms: 1.37x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 120 us: 4.47x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 378 ms: 2.06x faster                                                         |
| deltablue                | 7.50 ms                                                      | 3.80 ms: 1.98x faster                                                        |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.59 sec: 1.96x faster                                                       |
| generators               | 57.3 ms                                                      | 33.4 ms: 1.72x faster                                                        |
| logging_silent           | 167 ns                                                       | 100 ns: 1.67x faster                                                         |
| raytrace                 | 489 ms                                                       | 304 ms: 1.61x faster                                                         |
| chaos                    | 109 ms                                                       | 69.2 ms: 1.57x faster                                                        |
| async_tree_none          | 692 ms                                                       | 444 ms: 1.56x faster                                                         |
| richards_super           | 90.6 ms                                                      | 58.6 ms: 1.55x faster                                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.45 ms: 1.54x faster                                                        |
| go                       | 262 ms                                                       | 176 ms: 1.48x faster                                                         |
| crypto_pyaes             | 119 ms                                                       | 80.9 ms: 1.47x faster                                                        |
| async_tree_memoization   | 819 ms                                                       | 560 ms: 1.46x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.10 sec: 1.45x faster                                                       |
| richards                 | 75.1 ms                                                      | 52.2 ms: 1.44x faster                                                        |
| sqlglot_transpile        | 2.68 ms                                                      | 1.88 ms: 1.43x faster                                                        |
| pickle_pure_python       | 455 us                                                       | 319 us: 1.43x faster                                                         |
| float                    | 111 ms                                                       | 78.8 ms: 1.41x faster                                                        |
| spectral_norm            | 139 ms                                                       | 99.6 ms: 1.40x faster                                                        |
| json_dumps               | 14.5 ms                                                      | 10.4 ms: 1.39x faster                                                        |
| comprehensions           | 26.7 us                                                      | 19.2 us: 1.39x faster                                                        |
| scimark_lu               | 167 ms                                                       | 121 ms: 1.38x faster                                                         |
| mako                     | 14.7 ms                                                      | 10.7 ms: 1.37x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.4 ms: 1.35x faster                                                        |
| logging_simple           | 8.88 us                                                      | 6.58 us: 1.35x faster                                                        |
| logging_format           | 9.64 us                                                      | 7.15 us: 1.35x faster                                                        |
| pyflate                  | 733 ms                                                       | 544 ms: 1.35x faster                                                         |
| nbody                    | 134 ms                                                       | 102 ms: 1.31x faster                                                         |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 715 ms: 1.31x faster                                                         |
| unpickle_pure_python     | 312 us                                                       | 243 us: 1.28x faster                                                         |
| xml_etree_process        | 75.9 ms                                                      | 59.5 ms: 1.28x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 84.3 ms: 1.27x faster                                                        |
| chameleon                | 9.44 ms                                                      | 7.45 ms: 1.27x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.33 sec: 1.26x faster                                                       |
| deepcopy_memo            | 49.8 us                                                      | 39.8 us: 1.25x faster                                                        |
| tornado_http             | 157 ms                                                       | 127 ms: 1.24x faster                                                         |
| regex_compile            | 190 ms                                                       | 154 ms: 1.23x faster                                                         |
| hexiom                   | 9.42 ms                                                      | 7.69 ms: 1.22x faster                                                        |
| tomli_loads              | 2.92 sec                                                     | 2.39 sec: 1.22x faster                                                       |
| json_loads               | 30.3 us                                                      | 25.0 us: 1.21x faster                                                        |
| deepcopy                 | 468 us                                                       | 388 us: 1.21x faster                                                         |
| sqlglot_normalize        | 144 ms                                                       | 120 ms: 1.19x faster                                                         |
| pprint_safe_repr         | 1.05 sec                                                     | 886 ms: 1.18x faster                                                         |
| sympy_sum                | 193 ms                                                       | 163 ms: 1.18x faster                                                         |
| pprint_pformat           | 2.15 sec                                                     | 1.83 sec: 1.18x faster                                                       |
| sympy_str                | 360 ms                                                       | 306 ms: 1.18x faster                                                         |
| scimark_sor              | 180 ms                                                       | 156 ms: 1.16x faster                                                         |
| mdp                      | 3.01 sec                                                     | 2.61 sec: 1.15x faster                                                       |
| docutils                 | 3.41 sec                                                     | 2.96 sec: 1.15x faster                                                       |
| deepcopy_reduce          | 4.01 us                                                      | 3.48 us: 1.15x faster                                                        |
| sympy_expand             | 600 ms                                                       | 523 ms: 1.15x faster                                                         |
| bench_thread_pool        | 1.14 ms                                                      | 998 us: 1.14x faster                                                         |
| dulwich_log              | 81.1 ms                                                      | 71.1 ms: 1.14x faster                                                        |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.45 ms: 1.14x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.56 ms: 1.13x faster                                                        |
| 2to3                     | 350 ms                                                       | 310 ms: 1.13x faster                                                         |
| sympy_integrate          | 28.2 ms                                                      | 25.1 ms: 1.12x faster                                                        |
| nqueens                  | 115 ms                                                       | 104 ms: 1.11x faster                                                         |
| sqlite_synth             | 2.99 us                                                      | 2.70 us: 1.11x faster                                                        |
| json                     | 5.86 ms                                                      | 5.33 ms: 1.10x faster                                                        |
| fannkuch                 | 483 ms                                                       | 440 ms: 1.10x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 19.5 ms: 1.09x faster                                                        |
| regex_dna                | 261 ms                                                       | 239 ms: 1.09x faster                                                         |
| sqlglot_optimize         | 70.1 ms                                                      | 64.3 ms: 1.09x faster                                                        |
| async_generators         | 421 ms                                                       | 388 ms: 1.08x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 25.3 ms: 1.07x faster                                                        |
| xml_etree_generate       | 92.3 ms                                                      | 86.8 ms: 1.06x faster                                                        |
| xml_etree_parse          | 160 ms                                                       | 151 ms: 1.06x faster                                                         |
| scimark_fft              | 361 ms                                                       | 341 ms: 1.06x faster                                                         |
| meteor_contest           | 138 ms                                                       | 132 ms: 1.05x faster                                                         |
| xml_etree_iterparse      | 110 ms                                                       | 106 ms: 1.05x faster                                                         |
| pidigits                 | 271 ms                                                       | 262 ms: 1.03x faster                                                         |
| asyncio_websockets       | 390 ms                                                       | 385 ms: 1.01x faster                                                         |
| unpickle_list            | 4.65 us                                                      | 4.60 us: 1.01x faster                                                        |
| pickle_dict              | 29.5 us                                                      | 30.4 us: 1.03x slower                                                        |
| pickle                   | 9.89 us                                                      | 10.2 us: 1.03x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.6 us: 1.08x slower                                                        |
| bench_mp_pool            | 6.37 ms                                                      | 6.93 ms: 1.09x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.51 us: 1.10x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.89 ms: 1.14x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.32 ms: 1.15x slower                                                        |
| coverage                 | 63.3 ms                                                      | 84.7 ms: 1.34x slower                                                        |
| unpack_sequence          | 59.9 ns                                                      | 81.5 ns: 1.36x slower                                                        |
| python_startup           | 11.5 ms                                                      | 15.7 ms: 1.36x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 14.1 ms: 1.93x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.21x faster                                                                 |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-f0df35e-JIT/bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.36x