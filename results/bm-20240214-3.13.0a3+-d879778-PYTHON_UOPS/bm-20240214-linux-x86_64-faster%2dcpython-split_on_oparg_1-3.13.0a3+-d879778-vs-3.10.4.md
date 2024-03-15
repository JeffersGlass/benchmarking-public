
# Results vs. 3.10.4

- fork: faster-cpython
- ref: split_on_oparg_1
- machine: linux-x86_64
- commit hash: d879778
- commit date: 2024-02-14
- overall geometric mean: 1.27x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 284 ms: 1.23x faster                                                         |
| chameleon      | 9.68 ms                                                | 7.01 ms: 1.38x faster                                                        |
| docutils       | 3.30 sec                                               | 2.68 sec: 1.23x faster                                                       |
| tornado_http   | 136 ms                                                 | 98.0 ms: 1.39x faster                                                        |
| Geometric mean | (ref)                                                  | 1.30x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 448 ms: 1.63x faster                                                         |
| async_tree_memoization  | 870 ms                                                 | 569 ms: 1.53x faster                                                         |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 718 ms: 1.41x faster                                                         |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 121 ms: 1.27x faster                                                         |
| float          | 117 ms                                                 | 93.5 ms: 1.25x faster                                                        |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                  | 1.17x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 150 ms: 1.26x faster                                                         |
| regex_v8       | 27.8 ms                                                | 26.3 ms: 1.06x faster                                                        |
| regex_dna      | 227 ms                                                 | 228 ms: 1.01x slower                                                         |
| regex_effbot   | 3.63 ms                                                | 3.75 ms: 1.03x slower                                                        |
| Geometric mean | (ref)                                                  | 1.06x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 299 us: 1.62x faster                                                         |
| unpickle_pure_python | 331 us                                                 | 232 us: 1.43x faster                                                         |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                        |
| xml_etree_process    | 79.1 ms                                                | 60.6 ms: 1.31x faster                                                        |
| tomli_loads          | 3.14 sec                                               | 2.61 sec: 1.20x faster                                                       |
| json_loads           | 31.2 us                                                | 27.5 us: 1.14x faster                                                        |
| xml_etree_generate   | 99.4 ms                                                | 88.8 ms: 1.12x faster                                                        |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                         |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                         |
| unpickle_list        | 5.20 us                                                | 4.97 us: 1.05x faster                                                        |
| pickle_list          | 5.08 us                                                | 5.23 us: 1.03x slower                                                        |
| unpickle             | 14.4 us                                                | 15.4 us: 1.07x slower                                                        |
| pickle               | 10.7 us                                                | 12.0 us: 1.12x slower                                                        |
| pickle_dict          | 29.6 us                                                | 34.8 us: 1.18x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.3 ms: 1.42x faster                                                        |
| python_startup_no_site | 5.93 ms                                                | 8.88 ms: 1.50x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.03x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.9 ms: 1.18x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 115 us: 4.74x faster                                                         |
| generators               | 80.1 ms                                                | 29.1 ms: 2.75x faster                                                        |
| deltablue                | 7.91 ms                                                | 3.50 ms: 2.26x faster                                                        |
| asyncio_tcp              | 922 ms                                                 | 491 ms: 1.88x faster                                                         |
| logging_silent           | 190 ns                                                 | 102 ns: 1.86x faster                                                         |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.77x faster                                                         |
| richards_super           | 94.7 ms                                                | 53.9 ms: 1.76x faster                                                        |
| raytrace                 | 507 ms                                                 | 298 ms: 1.70x faster                                                         |
| richards                 | 79.3 ms                                                | 47.8 ms: 1.66x faster                                                        |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                        |
| async_tree_none          | 728 ms                                                 | 448 ms: 1.63x faster                                                         |
| pickle_pure_python       | 484 us                                                 | 299 us: 1.62x faster                                                         |
| chaos                    | 115 ms                                                 | 72.8 ms: 1.59x faster                                                        |
| go                       | 240 ms                                                 | 155 ms: 1.55x faster                                                         |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                                        |
| coroutines               | 35.1 ms                                                | 22.9 ms: 1.53x faster                                                        |
| crypto_pyaes             | 128 ms                                                 | 83.4 ms: 1.53x faster                                                        |
| async_tree_memoization   | 870 ms                                                 | 569 ms: 1.53x faster                                                         |
| scimark_lu               | 176 ms                                                 | 119 ms: 1.49x faster                                                         |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                       |
| scimark_monte_carlo      | 118 ms                                                 | 81.3 ms: 1.45x faster                                                        |
| deepcopy_memo            | 58.5 us                                                | 40.6 us: 1.44x faster                                                        |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                       |
| unpickle_pure_python     | 331 us                                                 | 232 us: 1.43x faster                                                         |
| python_startup           | 14.6 ms                                                | 10.3 ms: 1.42x faster                                                        |
| comprehensions           | 28.8 us                                                | 20.3 us: 1.42x faster                                                        |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 718 ms: 1.41x faster                                                         |
| unpack_sequence          | 60.0 ns                                                | 42.9 ns: 1.40x faster                                                        |
| tornado_http             | 136 ms                                                 | 98.0 ms: 1.39x faster                                                        |
| pyflate                  | 716 ms                                                 | 518 ms: 1.38x faster                                                         |
| chameleon                | 9.68 ms                                                | 7.01 ms: 1.38x faster                                                        |
| logging_simple           | 8.30 us                                                | 6.05 us: 1.37x faster                                                        |
| logging_format           | 9.09 us                                                | 6.76 us: 1.34x faster                                                        |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                        |
| deepcopy                 | 479 us                                                 | 357 us: 1.34x faster                                                         |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                        |
| xml_etree_process        | 79.1 ms                                                | 60.6 ms: 1.31x faster                                                        |
| pprint_safe_repr         | 1.02 sec                                               | 799 ms: 1.27x faster                                                         |
| sqlglot_normalize        | 143 ms                                                 | 112 ms: 1.27x faster                                                         |
| pprint_pformat           | 2.10 sec                                               | 1.66 sec: 1.27x faster                                                       |
| nbody                    | 154 ms                                                 | 121 ms: 1.27x faster                                                         |
| regex_compile            | 188 ms                                                 | 150 ms: 1.26x faster                                                         |
| float                    | 117 ms                                                 | 93.5 ms: 1.25x faster                                                        |
| sympy_integrate          | 25.8 ms                                                | 20.7 ms: 1.25x faster                                                        |
| sympy_sum                | 196 ms                                                 | 159 ms: 1.24x faster                                                         |
| hexiom                   | 10.4 ms                                                | 8.40 ms: 1.24x faster                                                        |
| pycparser                | 1.58 sec                                               | 1.28 sec: 1.23x faster                                                       |
| 2to3                     | 348 ms                                                 | 284 ms: 1.23x faster                                                         |
| docutils                 | 3.30 sec                                               | 2.68 sec: 1.23x faster                                                       |
| dulwich_log              | 84.3 ms                                                | 69.0 ms: 1.22x faster                                                        |
| spectral_norm            | 170 ms                                                 | 139 ms: 1.22x faster                                                         |
| tomli_loads              | 3.14 sec                                               | 2.61 sec: 1.20x faster                                                       |
| sqlglot_optimize         | 69.2 ms                                                | 57.6 ms: 1.20x faster                                                        |
| dask                     | 441 ms                                                 | 367 ms: 1.20x faster                                                         |
| fannkuch                 | 532 ms                                                 | 444 ms: 1.20x faster                                                         |
| sympy_str                | 346 ms                                                 | 290 ms: 1.19x faster                                                         |
| mako                     | 16.3 ms                                                | 13.9 ms: 1.18x faster                                                        |
| bench_thread_pool        | 986 us                                                 | 845 us: 1.17x faster                                                         |
| sympy_expand             | 566 ms                                                 | 493 ms: 1.15x faster                                                         |
| json_loads               | 31.2 us                                                | 27.5 us: 1.14x faster                                                        |
| xml_etree_generate       | 99.4 ms                                                | 88.8 ms: 1.12x faster                                                        |
| nqueens                  | 106 ms                                                 | 94.8 ms: 1.12x faster                                                        |
| json                     | 5.69 ms                                                | 5.11 ms: 1.11x faster                                                        |
| pathlib                  | 20.5 ms                                                | 18.5 ms: 1.10x faster                                                        |
| mdp                      | 2.85 sec                                               | 2.62 sec: 1.09x faster                                                       |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                        |
| scimark_fft              | 466 ms                                                 | 433 ms: 1.08x faster                                                         |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                         |
| sqlite_synth             | 3.02 us                                                | 2.86 us: 1.06x faster                                                        |
| regex_v8                 | 27.8 ms                                                | 26.3 ms: 1.06x faster                                                        |
| meteor_contest           | 120 ms                                                 | 113 ms: 1.05x faster                                                         |
| xml_etree_iterparse      | 115 ms                                                 | 110 ms: 1.05x faster                                                         |
| unpickle_list            | 5.20 us                                                | 4.97 us: 1.05x faster                                                        |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.34 ms: 1.02x faster                                                        |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                         |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                         |
| regex_dna                | 227 ms                                                 | 228 ms: 1.01x slower                                                         |
| pickle_list              | 5.08 us                                                | 5.23 us: 1.03x slower                                                        |
| regex_effbot             | 3.63 ms                                                | 3.75 ms: 1.03x slower                                                        |
| async_generators         | 444 ms                                                 | 461 ms: 1.04x slower                                                         |
| unpickle                 | 14.4 us                                                | 15.4 us: 1.07x slower                                                        |
| gc_traversal             | 3.62 ms                                                | 3.89 ms: 1.07x slower                                                        |
| pickle                   | 10.7 us                                                | 12.0 us: 1.12x slower                                                        |
| pickle_dict              | 29.6 us                                                | 34.8 us: 1.18x slower                                                        |
| telco                    | 7.27 ms                                                | 8.71 ms: 1.20x slower                                                        |
| coverage                 | 79.4 ms                                                | 96.9 ms: 1.22x slower                                                        |
| python_startup_no_site   | 5.93 ms                                                | 8.88 ms: 1.50x slower                                                        |
| Geometric mean           | (ref)                                                  | 1.27x faster                                                                 |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240214-3.13.0a3+-d879778-PYTHON_UOPS/bm-20240214-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-d879778.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: 1.07x