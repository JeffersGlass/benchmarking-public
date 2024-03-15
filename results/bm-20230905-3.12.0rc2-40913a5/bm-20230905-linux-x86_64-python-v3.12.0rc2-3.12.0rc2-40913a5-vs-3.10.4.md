
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0rc2
- machine: linux-x86_64
- commit hash: 40913a5
- commit date: 2023-09-05
- overall geometric mean: 1.35x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 268 ms: 1.30x faster                                         |
| docutils       | 3.30 sec                                               | 2.71 sec: 1.22x faster                                       |
| tornado_http   | 136 ms                                                 | 102 ms: 1.34x faster                                         |
| Geometric mean | (ref)                                                  | 1.28x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 465 ms: 1.57x faster                                         |
| async_tree_io           | 1.77 sec                                               | 1.14 sec: 1.55x faster                                       |
| async_tree_memoization  | 870 ms                                                 | 571 ms: 1.52x faster                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 708 ms: 1.44x faster                                         |
| Geometric mean          | (ref)                                                  | 1.52x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 93.4 ms: 1.64x faster                                        |
| float          | 117 ms                                                 | 80.1 ms: 1.46x faster                                        |
| pidigits       | 191 ms                                                 | 212 ms: 1.11x slower                                         |
| Geometric mean | (ref)                                                  | 1.29x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 144 ms: 1.31x faster                                         |
| regex_v8       | 27.8 ms                                                | 22.3 ms: 1.24x faster                                        |
| regex_dna      | 227 ms                                                 | 213 ms: 1.06x faster                                         |
| Geometric mean | (ref)                                                  | 1.15x faster                                                 |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 314 us: 1.54x faster                                         |
| unpickle_pure_python | 331 us                                                 | 219 us: 1.51x faster                                         |
| json_dumps           | 14.2 ms                                                | 9.89 ms: 1.43x faster                                        |
| tomli_loads          | 3.14 sec                                               | 2.20 sec: 1.43x faster                                       |
| xml_etree_process    | 79.1 ms                                                | 58.7 ms: 1.35x faster                                        |
| json_loads           | 31.2 us                                                | 25.1 us: 1.24x faster                                        |
| xml_etree_generate   | 99.4 ms                                                | 84.3 ms: 1.18x faster                                        |
| xml_etree_iterparse  | 115 ms                                                 | 103 ms: 1.12x faster                                         |
| xml_etree_parse      | 168 ms                                                 | 154 ms: 1.09x faster                                         |
| pickle_list          | 5.08 us                                                | 4.67 us: 1.09x faster                                        |
| unpickle_list        | 5.20 us                                                | 5.38 us: 1.03x slower                                        |
| unpickle             | 14.4 us                                                | 15.1 us: 1.05x slower                                        |
| pickle_dict          | 29.6 us                                                | 31.8 us: 1.07x slower                                        |
| Geometric mean       | (ref)                                                  | 1.19x faster                                                 |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.46 ms: 1.54x faster                                        |
| python_startup_no_site | 5.93 ms                                                | 6.88 ms: 1.16x slower                                        |
| Geometric mean         | (ref)                                                  | 1.15x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.9 ms: 1.50x faster                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230905-linux-x86_64-python-v3.12.0rc2-3.12.0rc2-40913a5 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 144 us: 3.77x faster                                         |
| generators               | 80.1 ms                                                | 30.8 ms: 2.60x faster                                        |
| deltablue                | 7.91 ms                                                | 3.49 ms: 2.27x faster                                        |
| richards_super           | 94.7 ms                                                | 48.9 ms: 1.94x faster                                        |
| logging_silent           | 190 ns                                                 | 98.5 ns: 1.93x faster                                        |
| richards                 | 79.3 ms                                                | 43.3 ms: 1.83x faster                                        |
| asyncio_tcp              | 922 ms                                                 | 505 ms: 1.83x faster                                         |
| chaos                    | 115 ms                                                 | 63.8 ms: 1.81x faster                                        |
| go                       | 240 ms                                                 | 135 ms: 1.77x faster                                         |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.77x faster                                         |
| raytrace                 | 507 ms                                                 | 293 ms: 1.73x faster                                         |
| hexiom                   | 10.4 ms                                                | 6.17 ms: 1.68x faster                                        |
| scimark_monte_carlo      | 118 ms                                                 | 71.4 ms: 1.66x faster                                        |
| nbody                    | 154 ms                                                 | 93.4 ms: 1.64x faster                                        |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                        |
| crypto_pyaes             | 128 ms                                                 | 79.6 ms: 1.61x faster                                        |
| spectral_norm            | 170 ms                                                 | 106 ms: 1.60x faster                                         |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                        |
| async_tree_none          | 728 ms                                                 | 465 ms: 1.57x faster                                         |
| sqlglot_transpile        | 2.57 ms                                                | 1.65 ms: 1.56x faster                                        |
| deepcopy_memo            | 58.5 us                                                | 37.5 us: 1.56x faster                                        |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.55x faster                                         |
| async_tree_io            | 1.77 sec                                               | 1.14 sec: 1.55x faster                                       |
| pickle_pure_python       | 484 us                                                 | 314 us: 1.54x faster                                         |
| python_startup           | 14.6 ms                                                | 9.46 ms: 1.54x faster                                        |
| pyflate                  | 716 ms                                                 | 467 ms: 1.53x faster                                         |
| async_tree_memoization   | 870 ms                                                 | 571 ms: 1.52x faster                                         |
| unpickle_pure_python     | 331 us                                                 | 219 us: 1.51x faster                                         |
| mako                     | 16.3 ms                                                | 10.9 ms: 1.50x faster                                        |
| float                    | 117 ms                                                 | 80.1 ms: 1.46x faster                                        |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 708 ms: 1.44x faster                                         |
| json_dumps               | 14.2 ms                                                | 9.89 ms: 1.43x faster                                        |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                       |
| tomli_loads              | 3.14 sec                                               | 2.20 sec: 1.43x faster                                       |
| pprint_pformat           | 2.10 sec                                               | 1.51 sec: 1.39x faster                                       |
| comprehensions           | 28.8 us                                                | 20.7 us: 1.39x faster                                        |
| pprint_safe_repr         | 1.02 sec                                               | 736 ms: 1.38x faster                                         |
| deepcopy                 | 479 us                                                 | 351 us: 1.37x faster                                         |
| pycparser                | 1.58 sec                                               | 1.16 sec: 1.36x faster                                       |
| xml_etree_process        | 79.1 ms                                                | 58.7 ms: 1.35x faster                                        |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.81 ms: 1.35x faster                                        |
| tornado_http             | 136 ms                                                 | 102 ms: 1.34x faster                                         |
| deepcopy_reduce          | 4.17 us                                                | 3.12 us: 1.34x faster                                        |
| fannkuch                 | 532 ms                                                 | 400 ms: 1.33x faster                                         |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                         |
| logging_simple           | 8.30 us                                                | 6.28 us: 1.32x faster                                        |
| unpack_sequence          | 60.0 ns                                                | 45.6 ns: 1.32x faster                                        |
| regex_compile            | 188 ms                                                 | 144 ms: 1.31x faster                                         |
| 2to3                     | 348 ms                                                 | 268 ms: 1.30x faster                                         |
| nqueens                  | 106 ms                                                 | 81.4 ms: 1.30x faster                                        |
| sqlglot_optimize         | 69.2 ms                                                | 53.5 ms: 1.29x faster                                        |
| logging_format           | 9.09 us                                                | 7.08 us: 1.28x faster                                        |
| scimark_fft              | 466 ms                                                 | 364 ms: 1.28x faster                                         |
| sqlalchemy_imperative    | 23.3 ms                                                | 18.4 ms: 1.27x faster                                        |
| regex_v8                 | 27.8 ms                                                | 22.3 ms: 1.24x faster                                        |
| json_loads               | 31.2 us                                                | 25.1 us: 1.24x faster                                        |
| dulwich_log              | 84.3 ms                                                | 68.2 ms: 1.24x faster                                        |
| docutils                 | 3.30 sec                                               | 2.71 sec: 1.22x faster                                       |
| bench_thread_pool        | 986 us                                                 | 829 us: 1.19x faster                                         |
| sqlalchemy_declarative   | 172 ms                                                 | 145 ms: 1.19x faster                                         |
| json                     | 5.69 ms                                                | 4.80 ms: 1.19x faster                                        |
| xml_etree_generate       | 99.4 ms                                                | 84.3 ms: 1.18x faster                                        |
| meteor_contest           | 120 ms                                                 | 106 ms: 1.13x faster                                         |
| xml_etree_iterparse      | 115 ms                                                 | 103 ms: 1.12x faster                                         |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                        |
| mdp                      | 2.85 sec                                               | 2.58 sec: 1.11x faster                                       |
| sqlite_synth             | 3.02 us                                                | 2.74 us: 1.10x faster                                        |
| xml_etree_parse          | 168 ms                                                 | 154 ms: 1.09x faster                                         |
| pickle_list              | 5.08 us                                                | 4.67 us: 1.09x faster                                        |
| create_gc_cycles         | 1.62 ms                                                | 1.51 ms: 1.07x faster                                        |
| telco                    | 7.27 ms                                                | 6.83 ms: 1.06x faster                                        |
| regex_dna                | 227 ms                                                 | 213 ms: 1.06x faster                                         |
| unpickle_list            | 5.20 us                                                | 5.38 us: 1.03x slower                                        |
| unpickle                 | 14.4 us                                                | 15.1 us: 1.05x slower                                        |
| gc_traversal             | 3.62 ms                                                | 3.83 ms: 1.06x slower                                        |
| pickle_dict              | 29.6 us                                                | 31.8 us: 1.07x slower                                        |
| pidigits                 | 191 ms                                                 | 212 ms: 1.11x slower                                         |
| python_startup_no_site   | 5.93 ms                                                | 6.88 ms: 1.16x slower                                        |
| coverage                 | 79.4 ms                                                | 94.7 ms: 1.19x slower                                        |
| dask                     | 441 ms                                                 | 537 ms: 1.22x slower                                         |
| Geometric mean           | (ref)                                                  | 1.35x faster                                                 |

Benchmark hidden because not significant (4): regex_effbot, pickle, bench_mp_pool, async_generators
Ignored benchmarks (17) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.17x