
# Results vs. 3.10.4

- fork: faster-cpython
- ref: split_on_oparg_1
- machine: linux-x86_64
- commit hash: 2e5a158
- commit date: 2024-02-14
- overall geometric mean: 1.31x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 277 ms: 1.26x faster                                                         |
| chameleon      | 9.68 ms                                                | 6.88 ms: 1.41x faster                                                        |
| docutils       | 3.30 sec                                               | 2.65 sec: 1.24x faster                                                       |
| tornado_http   | 136 ms                                                 | 96.6 ms: 1.41x faster                                                        |
| Geometric mean | (ref)                                                  | 1.33x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 445 ms: 1.64x faster                                                         |
| async_tree_memoization  | 870 ms                                                 | 571 ms: 1.52x faster                                                         |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 717 ms: 1.42x faster                                                         |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 104 ms: 1.47x faster                                                         |
| float          | 117 ms                                                 | 85.0 ms: 1.38x faster                                                        |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                  | 1.27x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 140 ms: 1.34x faster                                                         |
| regex_v8       | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                        |
| regex_dna      | 227 ms                                                 | 222 ms: 1.02x faster                                                         |
| regex_effbot   | 3.63 ms                                                | 3.70 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 299 us: 1.62x faster                                                         |
| unpickle_pure_python | 331 us                                                 | 229 us: 1.44x faster                                                         |
| tomli_loads          | 3.14 sec                                               | 2.21 sec: 1.42x faster                                                       |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                        |
| xml_etree_process    | 79.1 ms                                                | 58.5 ms: 1.35x faster                                                        |
| xml_etree_generate   | 99.4 ms                                                | 85.7 ms: 1.16x faster                                                        |
| json_loads           | 31.2 us                                                | 27.7 us: 1.13x faster                                                        |
| xml_etree_parse      | 168 ms                                                 | 155 ms: 1.08x faster                                                         |
| xml_etree_iterparse  | 115 ms                                                 | 107 ms: 1.08x faster                                                         |
| unpickle_list        | 5.20 us                                                | 5.05 us: 1.03x faster                                                        |
| unpickle             | 14.4 us                                                | 15.1 us: 1.05x slower                                                        |
| pickle               | 10.7 us                                                | 11.3 us: 1.06x slower                                                        |
| pickle_dict          | 29.6 us                                                | 33.6 us: 1.14x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                                 |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.3 ms: 1.42x faster                                                        |
| python_startup_no_site | 5.93 ms                                                | 8.91 ms: 1.50x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.03x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.2 ms: 1.34x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.92x faster                                                         |
| generators               | 80.1 ms                                                | 29.2 ms: 2.75x faster                                                        |
| deltablue                | 7.91 ms                                                | 3.39 ms: 2.34x faster                                                        |
| asyncio_tcp              | 922 ms                                                 | 489 ms: 1.88x faster                                                         |
| logging_silent           | 190 ns                                                 | 103 ns: 1.84x faster                                                         |
| richards_super           | 94.7 ms                                                | 51.4 ms: 1.84x faster                                                        |
| scimark_sor              | 220 ms                                                 | 121 ms: 1.81x faster                                                         |
| raytrace                 | 507 ms                                                 | 283 ms: 1.79x faster                                                         |
| richards                 | 79.3 ms                                                | 45.1 ms: 1.76x faster                                                        |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.68x faster                                                        |
| chaos                    | 115 ms                                                 | 70.5 ms: 1.64x faster                                                        |
| async_tree_none          | 728 ms                                                 | 445 ms: 1.64x faster                                                         |
| crypto_pyaes             | 128 ms                                                 | 78.7 ms: 1.62x faster                                                        |
| pickle_pure_python       | 484 us                                                 | 299 us: 1.62x faster                                                         |
| go                       | 240 ms                                                 | 149 ms: 1.61x faster                                                         |
| sqlglot_transpile        | 2.57 ms                                                | 1.63 ms: 1.58x faster                                                        |
| comprehensions           | 28.8 us                                                | 18.2 us: 1.58x faster                                                        |
| scimark_monte_carlo      | 118 ms                                                 | 75.5 ms: 1.57x faster                                                        |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.55x faster                                                         |
| coroutines               | 35.1 ms                                                | 22.8 ms: 1.54x faster                                                        |
| async_tree_memoization   | 870 ms                                                 | 571 ms: 1.52x faster                                                         |
| deepcopy_memo            | 58.5 us                                                | 39.2 us: 1.49x faster                                                        |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                       |
| nbody                    | 154 ms                                                 | 104 ms: 1.47x faster                                                         |
| unpickle_pure_python     | 331 us                                                 | 229 us: 1.44x faster                                                         |
| logging_simple           | 8.30 us                                                | 5.77 us: 1.44x faster                                                        |
| logging_format           | 9.09 us                                                | 6.34 us: 1.43x faster                                                        |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                       |
| pyflate                  | 716 ms                                                 | 504 ms: 1.42x faster                                                         |
| tomli_loads              | 3.14 sec                                               | 2.21 sec: 1.42x faster                                                       |
| python_startup           | 14.6 ms                                                | 10.3 ms: 1.42x faster                                                        |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 717 ms: 1.42x faster                                                         |
| tornado_http             | 136 ms                                                 | 96.6 ms: 1.41x faster                                                        |
| chameleon                | 9.68 ms                                                | 6.88 ms: 1.41x faster                                                        |
| float                    | 117 ms                                                 | 85.0 ms: 1.38x faster                                                        |
| deepcopy                 | 479 us                                                 | 351 us: 1.36x faster                                                         |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                        |
| xml_etree_process        | 79.1 ms                                                | 58.5 ms: 1.35x faster                                                        |
| deepcopy_reduce          | 4.17 us                                                | 3.10 us: 1.35x faster                                                        |
| regex_compile            | 188 ms                                                 | 140 ms: 1.34x faster                                                         |
| mako                     | 16.3 ms                                                | 12.2 ms: 1.34x faster                                                        |
| pycparser                | 1.58 sec                                               | 1.19 sec: 1.33x faster                                                       |
| hexiom                   | 10.4 ms                                                | 7.86 ms: 1.32x faster                                                        |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                                         |
| pprint_safe_repr         | 1.02 sec                                               | 780 ms: 1.30x faster                                                         |
| pprint_pformat           | 2.10 sec                                               | 1.63 sec: 1.29x faster                                                       |
| spectral_norm            | 170 ms                                                 | 132 ms: 1.29x faster                                                         |
| fannkuch                 | 532 ms                                                 | 418 ms: 1.27x faster                                                         |
| 2to3                     | 348 ms                                                 | 277 ms: 1.26x faster                                                         |
| sympy_integrate          | 25.8 ms                                                | 20.6 ms: 1.25x faster                                                        |
| sqlglot_optimize         | 69.2 ms                                                | 55.4 ms: 1.25x faster                                                        |
| sympy_sum                | 196 ms                                                 | 157 ms: 1.25x faster                                                         |
| scimark_fft              | 466 ms                                                 | 374 ms: 1.25x faster                                                         |
| docutils                 | 3.30 sec                                               | 2.65 sec: 1.24x faster                                                       |
| dulwich_log              | 84.3 ms                                                | 67.9 ms: 1.24x faster                                                        |
| sympy_str                | 346 ms                                                 | 282 ms: 1.23x faster                                                         |
| dask                     | 441 ms                                                 | 366 ms: 1.21x faster                                                         |
| sympy_expand             | 566 ms                                                 | 479 ms: 1.18x faster                                                         |
| nqueens                  | 106 ms                                                 | 90.2 ms: 1.17x faster                                                        |
| bench_thread_pool        | 986 us                                                 | 842 us: 1.17x faster                                                         |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.55 ms: 1.17x faster                                                        |
| xml_etree_generate       | 99.4 ms                                                | 85.7 ms: 1.16x faster                                                        |
| json_loads               | 31.2 us                                                | 27.7 us: 1.13x faster                                                        |
| mdp                      | 2.85 sec                                               | 2.57 sec: 1.11x faster                                                       |
| json                     | 5.69 ms                                                | 5.15 ms: 1.10x faster                                                        |
| regex_v8                 | 27.8 ms                                                | 25.2 ms: 1.10x faster                                                        |
| pathlib                  | 20.5 ms                                                | 18.6 ms: 1.10x faster                                                        |
| meteor_contest           | 120 ms                                                 | 110 ms: 1.09x faster                                                         |
| xml_etree_parse          | 168 ms                                                 | 155 ms: 1.08x faster                                                         |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                        |
| xml_etree_iterparse      | 115 ms                                                 | 107 ms: 1.08x faster                                                         |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                                        |
| unpack_sequence          | 60.0 ns                                                | 58.0 ns: 1.03x faster                                                        |
| unpickle_list            | 5.20 us                                                | 5.05 us: 1.03x faster                                                        |
| regex_dna                | 227 ms                                                 | 222 ms: 1.02x faster                                                         |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                                         |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                         |
| regex_effbot             | 3.63 ms                                                | 3.70 ms: 1.02x slower                                                        |
| async_generators         | 444 ms                                                 | 461 ms: 1.04x slower                                                         |
| unpickle                 | 14.4 us                                                | 15.1 us: 1.05x slower                                                        |
| gc_traversal             | 3.62 ms                                                | 3.85 ms: 1.06x slower                                                        |
| pickle                   | 10.7 us                                                | 11.3 us: 1.06x slower                                                        |
| pickle_dict              | 29.6 us                                                | 33.6 us: 1.14x slower                                                        |
| telco                    | 7.27 ms                                                | 8.65 ms: 1.19x slower                                                        |
| coverage                 | 79.4 ms                                                | 94.8 ms: 1.19x slower                                                        |
| python_startup_no_site   | 5.93 ms                                                | 8.91 ms: 1.50x slower                                                        |
| Geometric mean           | (ref)                                                  | 1.31x faster                                                                 |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, pickle_list
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240214-3.13.0a3+-2e5a158-JIT/bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-2e5a158.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.10x