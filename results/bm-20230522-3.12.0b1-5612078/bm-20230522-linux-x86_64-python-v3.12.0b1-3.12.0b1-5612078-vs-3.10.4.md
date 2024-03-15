
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b1
- machine: linux-x86_64
- commit hash: 5612078
- commit date: 2023-05-22
- overall geometric mean: 1.35x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.27x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 268 ms: 1.30x faster                                       |
| docutils       | 3.30 sec                                               | 2.71 sec: 1.22x faster                                     |
| tornado_http   | 136 ms                                                 | 99.2 ms: 1.37x faster                                      |
| Geometric mean | (ref)                                                  | 1.29x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 469 ms: 1.55x faster                                       |
| async_tree_io           | 1.77 sec                                               | 1.16 sec: 1.52x faster                                     |
| async_tree_memoization  | 870 ms                                                 | 572 ms: 1.52x faster                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 708 ms: 1.43x faster                                       |
| Geometric mean          | (ref)                                                  | 1.51x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.9 ms: 1.73x faster                                      |
| float          | 117 ms                                                 | 80.7 ms: 1.45x faster                                      |
| pidigits       | 191 ms                                                 | 196 ms: 1.03x slower                                       |
| Geometric mean | (ref)                                                  | 1.35x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 144 ms: 1.31x faster                                       |
| regex_v8       | 27.8 ms                                                | 21.8 ms: 1.27x faster                                      |
| regex_dna      | 227 ms                                                 | 208 ms: 1.09x faster                                       |
| regex_effbot   | 3.63 ms                                                | 3.54 ms: 1.03x faster                                      |
| Geometric mean | (ref)                                                  | 1.17x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 312 us: 1.55x faster                                       |
| unpickle_pure_python | 331 us                                                 | 216 us: 1.53x faster                                       |
| json_dumps           | 14.2 ms                                                | 9.76 ms: 1.45x faster                                      |
| tomli_loads          | 3.14 sec                                               | 2.18 sec: 1.44x faster                                     |
| xml_etree_process    | 79.1 ms                                                | 59.0 ms: 1.34x faster                                      |
| json_loads           | 31.2 us                                                | 25.1 us: 1.24x faster                                      |
| xml_etree_generate   | 99.4 ms                                                | 85.6 ms: 1.16x faster                                      |
| xml_etree_iterparse  | 115 ms                                                 | 103 ms: 1.12x faster                                       |
| xml_etree_parse      | 168 ms                                                 | 153 ms: 1.10x faster                                       |
| pickle_list          | 5.08 us                                                | 4.73 us: 1.07x faster                                      |
| pickle               | 10.7 us                                                | 10.6 us: 1.01x faster                                      |
| unpickle             | 14.4 us                                                | 14.9 us: 1.04x slower                                      |
| pickle_dict          | 29.6 us                                                | 33.3 us: 1.12x slower                                      |
| Geometric mean       | (ref)                                                  | 1.19x faster                                               |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.34 ms: 1.56x faster                                      |
| python_startup_no_site | 5.93 ms                                                | 6.78 ms: 1.14x slower                                      |
| Geometric mean         | (ref)                                                  | 1.17x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.8 ms: 1.50x faster                                      |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230522-linux-x86_64-python-v3.12.0b1-3.12.0b1-5612078 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 140 us: 3.89x faster                                       |
| generators               | 80.1 ms                                                | 31.4 ms: 2.55x faster                                      |
| deltablue                | 7.91 ms                                                | 3.44 ms: 2.30x faster                                      |
| richards_super           | 94.7 ms                                                | 49.8 ms: 1.90x faster                                      |
| logging_silent           | 190 ns                                                 | 100 ns: 1.89x faster                                       |
| richards                 | 79.3 ms                                                | 43.6 ms: 1.82x faster                                      |
| asyncio_tcp              | 922 ms                                                 | 513 ms: 1.80x faster                                       |
| chaos                    | 115 ms                                                 | 64.6 ms: 1.79x faster                                      |
| scimark_sor              | 220 ms                                                 | 123 ms: 1.79x faster                                       |
| go                       | 240 ms                                                 | 136 ms: 1.77x faster                                       |
| nbody                    | 154 ms                                                 | 88.9 ms: 1.73x faster                                      |
| raytrace                 | 507 ms                                                 | 298 ms: 1.70x faster                                       |
| hexiom                   | 10.4 ms                                                | 6.12 ms: 1.70x faster                                      |
| crypto_pyaes             | 128 ms                                                 | 77.9 ms: 1.64x faster                                      |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                      |
| scimark_monte_carlo      | 118 ms                                                 | 72.7 ms: 1.63x faster                                      |
| pyflate                  | 716 ms                                                 | 443 ms: 1.62x faster                                       |
| coroutines               | 35.1 ms                                                | 21.9 ms: 1.60x faster                                      |
| spectral_norm            | 170 ms                                                 | 108 ms: 1.57x faster                                       |
| sqlglot_transpile        | 2.57 ms                                                | 1.64 ms: 1.57x faster                                      |
| python_startup           | 14.6 ms                                                | 9.34 ms: 1.56x faster                                      |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.56x faster                                       |
| deepcopy_memo            | 58.5 us                                                | 37.6 us: 1.55x faster                                      |
| pickle_pure_python       | 484 us                                                 | 312 us: 1.55x faster                                       |
| async_tree_none          | 728 ms                                                 | 469 ms: 1.55x faster                                       |
| unpickle_pure_python     | 331 us                                                 | 216 us: 1.53x faster                                       |
| async_tree_io            | 1.77 sec                                               | 1.16 sec: 1.52x faster                                     |
| async_tree_memoization   | 870 ms                                                 | 572 ms: 1.52x faster                                       |
| mako                     | 16.3 ms                                                | 10.8 ms: 1.50x faster                                      |
| json_dumps               | 14.2 ms                                                | 9.76 ms: 1.45x faster                                      |
| float                    | 117 ms                                                 | 80.7 ms: 1.45x faster                                      |
| tomli_loads              | 3.14 sec                                               | 2.18 sec: 1.44x faster                                     |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 708 ms: 1.43x faster                                       |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                     |
| pprint_pformat           | 2.10 sec                                               | 1.50 sec: 1.41x faster                                     |
| comprehensions           | 28.8 us                                                | 20.6 us: 1.40x faster                                      |
| fannkuch                 | 532 ms                                                 | 382 ms: 1.39x faster                                       |
| pprint_safe_repr         | 1.02 sec                                               | 733 ms: 1.39x faster                                       |
| tornado_http             | 136 ms                                                 | 99.2 ms: 1.37x faster                                      |
| xml_etree_process        | 79.1 ms                                                | 59.0 ms: 1.34x faster                                      |
| deepcopy                 | 479 us                                                 | 361 us: 1.33x faster                                       |
| pycparser                | 1.58 sec                                               | 1.19 sec: 1.32x faster                                     |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.32x faster                                       |
| regex_compile            | 188 ms                                                 | 144 ms: 1.31x faster                                       |
| logging_simple           | 8.30 us                                                | 6.33 us: 1.31x faster                                      |
| scimark_fft              | 466 ms                                                 | 356 ms: 1.31x faster                                       |
| deepcopy_reduce          | 4.17 us                                                | 3.18 us: 1.31x faster                                      |
| 2to3                     | 348 ms                                                 | 268 ms: 1.30x faster                                       |
| nqueens                  | 106 ms                                                 | 81.4 ms: 1.30x faster                                      |
| logging_format           | 9.09 us                                                | 7.09 us: 1.28x faster                                      |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.05 ms: 1.28x faster                                      |
| sqlglot_optimize         | 69.2 ms                                                | 54.1 ms: 1.28x faster                                      |
| regex_v8                 | 27.8 ms                                                | 21.8 ms: 1.27x faster                                      |
| unpack_sequence          | 60.0 ns                                                | 47.3 ns: 1.27x faster                                      |
| sqlalchemy_imperative    | 23.3 ms                                                | 18.6 ms: 1.26x faster                                      |
| dulwich_log              | 84.3 ms                                                | 67.7 ms: 1.25x faster                                      |
| json_loads               | 31.2 us                                                | 25.1 us: 1.24x faster                                      |
| docutils                 | 3.30 sec                                               | 2.71 sec: 1.22x faster                                     |
| bench_thread_pool        | 986 us                                                 | 827 us: 1.19x faster                                       |
| json                     | 5.69 ms                                                | 4.77 ms: 1.19x faster                                      |
| sqlalchemy_declarative   | 172 ms                                                 | 145 ms: 1.19x faster                                       |
| xml_etree_generate       | 99.4 ms                                                | 85.6 ms: 1.16x faster                                      |
| meteor_contest           | 120 ms                                                 | 105 ms: 1.14x faster                                       |
| xml_etree_iterparse      | 115 ms                                                 | 103 ms: 1.12x faster                                       |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                      |
| sqlite_synth             | 3.02 us                                                | 2.72 us: 1.11x faster                                      |
| xml_etree_parse          | 168 ms                                                 | 153 ms: 1.10x faster                                       |
| regex_dna                | 227 ms                                                 | 208 ms: 1.09x faster                                       |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                      |
| pickle_list              | 5.08 us                                                | 4.73 us: 1.07x faster                                      |
| mdp                      | 2.85 sec                                               | 2.68 sec: 1.06x faster                                     |
| telco                    | 7.27 ms                                                | 6.84 ms: 1.06x faster                                      |
| regex_effbot             | 3.63 ms                                                | 3.54 ms: 1.03x faster                                      |
| pickle                   | 10.7 us                                                | 10.6 us: 1.01x faster                                      |
| async_generators         | 444 ms                                                 | 449 ms: 1.01x slower                                       |
| gc_traversal             | 3.62 ms                                                | 3.67 ms: 1.01x slower                                      |
| pidigits                 | 191 ms                                                 | 196 ms: 1.03x slower                                       |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.04x slower                                      |
| pickle_dict              | 29.6 us                                                | 33.3 us: 1.12x slower                                      |
| python_startup_no_site   | 5.93 ms                                                | 6.78 ms: 1.14x slower                                      |
| dask                     | 441 ms                                                 | 535 ms: 1.21x slower                                       |
| coverage                 | 79.4 ms                                                | 96.8 ms: 1.22x slower                                      |
| Geometric mean           | (ref)                                                  | 1.35x faster                                               |

Benchmark hidden because not significant (2): unpickle_list, bench_mp_pool
Ignored benchmarks (17) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.27x


# Memory

- memory change: 1.17x