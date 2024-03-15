
# Results vs. 3.10.4

- fork: faster-cpython
- ref: split_on_oparg_1
- machine: linux-x86_64
- commit hash: 472a3d6
- commit date: 2024-02-15
- overall geometric mean: 1.32x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 277 ms: 1.26x faster                                                         |
| chameleon      | 9.68 ms                                                | 6.84 ms: 1.42x faster                                                        |
| docutils       | 3.30 sec                                               | 2.64 sec: 1.25x faster                                                       |
| tornado_http   | 136 ms                                                 | 96.7 ms: 1.41x faster                                                        |
| Geometric mean | (ref)                                                  | 1.33x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 439 ms: 1.66x faster                                                         |
| async_tree_memoization  | 870 ms                                                 | 559 ms: 1.56x faster                                                         |
| async_tree_io           | 1.77 sec                                               | 1.16 sec: 1.52x faster                                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 706 ms: 1.44x faster                                                         |
| Geometric mean          | (ref)                                                  | 1.54x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 101 ms: 1.51x faster                                                         |
| float          | 117 ms                                                 | 83.0 ms: 1.41x faster                                                        |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                  | 1.30x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 138 ms: 1.37x faster                                                         |
| regex_v8       | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                        |
| regex_dna      | 227 ms                                                 | 219 ms: 1.04x faster                                                         |
| Geometric mean | (ref)                                                  | 1.12x faster                                                                 |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 299 us: 1.62x faster                                                         |
| unpickle_pure_python | 331 us                                                 | 225 us: 1.47x faster                                                         |
| tomli_loads          | 3.14 sec                                               | 2.18 sec: 1.44x faster                                                       |
| xml_etree_process    | 79.1 ms                                                | 58.1 ms: 1.36x faster                                                        |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.36x faster                                                        |
| xml_etree_generate   | 99.4 ms                                                | 85.2 ms: 1.17x faster                                                        |
| json_loads           | 31.2 us                                                | 27.6 us: 1.13x faster                                                        |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                         |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                                         |
| pickle_list          | 5.08 us                                                | 4.91 us: 1.03x faster                                                        |
| unpickle             | 14.4 us                                                | 15.1 us: 1.05x slower                                                        |
| pickle               | 10.7 us                                                | 11.3 us: 1.06x slower                                                        |
| pickle_dict          | 29.6 us                                                | 33.4 us: 1.13x slower                                                        |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                                 |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                        |
| python_startup_no_site | 5.93 ms                                                | 8.84 ms: 1.49x slower                                                        |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.1 ms: 1.35x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.94x faster                                                         |
| generators               | 80.1 ms                                                | 29.9 ms: 2.67x faster                                                        |
| deltablue                | 7.91 ms                                                | 3.31 ms: 2.39x faster                                                        |
| asyncio_tcp              | 922 ms                                                 | 487 ms: 1.89x faster                                                         |
| logging_silent           | 190 ns                                                 | 101 ns: 1.87x faster                                                         |
| richards_super           | 94.7 ms                                                | 51.3 ms: 1.85x faster                                                        |
| scimark_sor              | 220 ms                                                 | 119 ms: 1.84x faster                                                         |
| raytrace                 | 507 ms                                                 | 280 ms: 1.81x faster                                                         |
| richards                 | 79.3 ms                                                | 45.2 ms: 1.75x faster                                                        |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.69x faster                                                        |
| async_tree_none          | 728 ms                                                 | 439 ms: 1.66x faster                                                         |
| chaos                    | 115 ms                                                 | 70.6 ms: 1.64x faster                                                        |
| crypto_pyaes             | 128 ms                                                 | 78.5 ms: 1.63x faster                                                        |
| go                       | 240 ms                                                 | 148 ms: 1.63x faster                                                         |
| pickle_pure_python       | 484 us                                                 | 299 us: 1.62x faster                                                         |
| scimark_monte_carlo      | 118 ms                                                 | 73.5 ms: 1.61x faster                                                        |
| comprehensions           | 28.8 us                                                | 18.0 us: 1.59x faster                                                        |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                                        |
| async_tree_memoization   | 870 ms                                                 | 559 ms: 1.56x faster                                                         |
| scimark_lu               | 176 ms                                                 | 114 ms: 1.54x faster                                                         |
| coroutines               | 35.1 ms                                                | 22.8 ms: 1.54x faster                                                        |
| deepcopy_memo            | 58.5 us                                                | 38.3 us: 1.53x faster                                                        |
| async_tree_io            | 1.77 sec                                               | 1.16 sec: 1.52x faster                                                       |
| nbody                    | 154 ms                                                 | 101 ms: 1.51x faster                                                         |
| unpickle_pure_python     | 331 us                                                 | 225 us: 1.47x faster                                                         |
| logging_simple           | 8.30 us                                                | 5.71 us: 1.45x faster                                                        |
| pyflate                  | 716 ms                                                 | 497 ms: 1.44x faster                                                         |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 706 ms: 1.44x faster                                                         |
| tomli_loads              | 3.14 sec                                               | 2.18 sec: 1.44x faster                                                       |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.43x faster                                                       |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                        |
| logging_format           | 9.09 us                                                | 6.39 us: 1.42x faster                                                        |
| chameleon                | 9.68 ms                                                | 6.84 ms: 1.42x faster                                                        |
| tornado_http             | 136 ms                                                 | 96.7 ms: 1.41x faster                                                        |
| float                    | 117 ms                                                 | 83.0 ms: 1.41x faster                                                        |
| deepcopy                 | 479 us                                                 | 349 us: 1.37x faster                                                         |
| hexiom                   | 10.4 ms                                                | 7.61 ms: 1.37x faster                                                        |
| regex_compile            | 188 ms                                                 | 138 ms: 1.37x faster                                                         |
| xml_etree_process        | 79.1 ms                                                | 58.1 ms: 1.36x faster                                                        |
| deepcopy_reduce          | 4.17 us                                                | 3.07 us: 1.36x faster                                                        |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.36x faster                                                        |
| mako                     | 16.3 ms                                                | 12.1 ms: 1.35x faster                                                        |
| spectral_norm            | 170 ms                                                 | 126 ms: 1.35x faster                                                         |
| pycparser                | 1.58 sec                                               | 1.18 sec: 1.33x faster                                                       |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.32x faster                                                         |
| pprint_safe_repr         | 1.02 sec                                               | 785 ms: 1.30x faster                                                         |
| pprint_pformat           | 2.10 sec                                               | 1.63 sec: 1.29x faster                                                       |
| fannkuch                 | 532 ms                                                 | 417 ms: 1.27x faster                                                         |
| scimark_fft              | 466 ms                                                 | 367 ms: 1.27x faster                                                         |
| sympy_integrate          | 25.8 ms                                                | 20.4 ms: 1.26x faster                                                        |
| 2to3                     | 348 ms                                                 | 277 ms: 1.26x faster                                                         |
| sqlglot_optimize         | 69.2 ms                                                | 55.3 ms: 1.25x faster                                                        |
| docutils                 | 3.30 sec                                               | 2.64 sec: 1.25x faster                                                       |
| sympy_sum                | 196 ms                                                 | 158 ms: 1.25x faster                                                         |
| dulwich_log              | 84.3 ms                                                | 67.7 ms: 1.25x faster                                                        |
| sympy_str                | 346 ms                                                 | 281 ms: 1.23x faster                                                         |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.27 ms: 1.23x faster                                                        |
| dask                     | 441 ms                                                 | 365 ms: 1.21x faster                                                         |
| nqueens                  | 106 ms                                                 | 89.1 ms: 1.19x faster                                                        |
| sympy_expand             | 566 ms                                                 | 478 ms: 1.18x faster                                                         |
| bench_thread_pool        | 986 us                                                 | 840 us: 1.17x faster                                                         |
| xml_etree_generate       | 99.4 ms                                                | 85.2 ms: 1.17x faster                                                        |
| unpack_sequence          | 60.0 ns                                                | 52.0 ns: 1.15x faster                                                        |
| regex_v8                 | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                        |
| json_loads               | 31.2 us                                                | 27.6 us: 1.13x faster                                                        |
| json                     | 5.69 ms                                                | 5.06 ms: 1.12x faster                                                        |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                                        |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                                        |
| mdp                      | 2.85 sec                                               | 2.59 sec: 1.10x faster                                                       |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                                         |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                         |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                                         |
| sqlite_synth             | 3.02 us                                                | 2.83 us: 1.07x faster                                                        |
| gc_traversal             | 3.62 ms                                                | 3.47 ms: 1.04x faster                                                        |
| regex_dna                | 227 ms                                                 | 219 ms: 1.04x faster                                                         |
| pickle_list              | 5.08 us                                                | 4.91 us: 1.03x faster                                                        |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                         |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                         |
| async_generators         | 444 ms                                                 | 458 ms: 1.03x slower                                                         |
| unpickle                 | 14.4 us                                                | 15.1 us: 1.05x slower                                                        |
| pickle                   | 10.7 us                                                | 11.3 us: 1.06x slower                                                        |
| pickle_dict              | 29.6 us                                                | 33.4 us: 1.13x slower                                                        |
| telco                    | 7.27 ms                                                | 8.61 ms: 1.19x slower                                                        |
| coverage                 | 79.4 ms                                                | 95.4 ms: 1.20x slower                                                        |
| python_startup_no_site   | 5.93 ms                                                | 8.84 ms: 1.49x slower                                                        |
| Geometric mean           | (ref)                                                  | 1.32x faster                                                                 |

Benchmark hidden because not significant (4): mypy2, unpickle_list, regex_effbot, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a3+-472a3d6-JIT/bm-20240215-linux-x86_64-faster%2dcpython-split_on_oparg_1-3.13.0a3+-472a3d6.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.10x