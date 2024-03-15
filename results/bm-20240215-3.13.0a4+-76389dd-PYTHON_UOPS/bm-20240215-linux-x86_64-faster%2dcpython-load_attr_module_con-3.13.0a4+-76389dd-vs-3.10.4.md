
# Results vs. 3.10.4

- fork: faster-cpython
- ref: load_attr_module_con
- machine: linux-x86_64
- commit hash: 76389dd
- commit date: 2024-02-15
- overall geometric mean: 1.24x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 292 ms: 1.19x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.10 ms: 1.36x faster                                                            |
| docutils       | 3.30 sec                                               | 2.80 sec: 1.18x faster                                                           |
| tornado_http   | 136 ms                                                 | 99.0 ms: 1.38x faster                                                            |
| Geometric mean | (ref)                                                  | 1.27x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 450 ms: 1.62x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 574 ms: 1.52x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 724 ms: 1.40x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 115 ms: 1.34x faster                                                             |
| float          | 117 ms                                                 | 89.8 ms: 1.30x faster                                                            |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.21x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 25.1 ms: 1.11x faster                                                            |
| regex_compile  | 188 ms                                                 | 176 ms: 1.07x faster                                                             |
| regex_dna      | 227 ms                                                 | 221 ms: 1.02x faster                                                             |
| Geometric mean | (ref)                                                  | 1.05x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 61.0 ms: 1.30x faster                                                            |
| unpickle_pure_python | 331 us                                                 | 271 us: 1.22x faster                                                             |
| tomli_loads          | 3.14 sec                                               | 2.64 sec: 1.19x faster                                                           |
| json_loads           | 31.2 us                                                | 27.7 us: 1.13x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 89.5 ms: 1.11x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| unpickle             | 14.4 us                                                | 15.1 us: 1.05x slower                                                            |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| pickle_dict          | 29.6 us                                                | 33.6 us: 1.14x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                                     |

Benchmark hidden because not significant (2): pickle_list, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.82 ms: 1.49x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 14.0 ms: 1.16x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 114 us: 4.77x faster                                                             |
| generators               | 80.1 ms                                                | 29.4 ms: 2.72x faster                                                            |
| deltablue                | 7.91 ms                                                | 3.72 ms: 2.12x faster                                                            |
| logging_silent           | 190 ns                                                 | 100 ns: 1.89x faster                                                             |
| asyncio_tcp              | 922 ms                                                 | 491 ms: 1.88x faster                                                             |
| async_tree_none          | 728 ms                                                 | 450 ms: 1.62x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 301 us: 1.61x faster                                                             |
| chaos                    | 115 ms                                                 | 73.9 ms: 1.56x faster                                                            |
| scimark_sor              | 220 ms                                                 | 141 ms: 1.56x faster                                                             |
| coroutines               | 35.1 ms                                                | 23.0 ms: 1.53x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 83.9 ms: 1.52x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.43 ms: 1.52x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 574 ms: 1.52x faster                                                             |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| sqlglot_transpile        | 2.57 ms                                                | 1.76 ms: 1.46x faster                                                            |
| richards_super           | 94.7 ms                                                | 66.0 ms: 1.43x faster                                                            |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| raytrace                 | 507 ms                                                 | 355 ms: 1.43x faster                                                             |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.42x faster                                                           |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 724 ms: 1.40x faster                                                             |
| deepcopy_memo            | 58.5 us                                                | 41.7 us: 1.40x faster                                                            |
| scimark_monte_carlo      | 118 ms                                                 | 85.6 ms: 1.38x faster                                                            |
| tornado_http             | 136 ms                                                 | 99.0 ms: 1.38x faster                                                            |
| comprehensions           | 28.8 us                                                | 21.0 us: 1.37x faster                                                            |
| chameleon                | 9.68 ms                                                | 7.10 ms: 1.36x faster                                                            |
| go                       | 240 ms                                                 | 176 ms: 1.36x faster                                                             |
| logging_simple           | 8.30 us                                                | 6.17 us: 1.35x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.11 us: 1.34x faster                                                            |
| nbody                    | 154 ms                                                 | 115 ms: 1.34x faster                                                             |
| deepcopy                 | 479 us                                                 | 360 us: 1.33x faster                                                             |
| richards                 | 79.3 ms                                                | 59.9 ms: 1.32x faster                                                            |
| float                    | 117 ms                                                 | 89.8 ms: 1.30x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 61.0 ms: 1.30x faster                                                            |
| logging_format           | 9.09 us                                                | 7.05 us: 1.29x faster                                                            |
| sqlglot_normalize        | 143 ms                                                 | 113 ms: 1.26x faster                                                             |
| spectral_norm            | 170 ms                                                 | 136 ms: 1.25x faster                                                             |
| pycparser                | 1.58 sec                                               | 1.27 sec: 1.24x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                                            |
| pyflate                  | 716 ms                                                 | 588 ms: 1.22x faster                                                             |
| unpickle_pure_python     | 331 us                                                 | 271 us: 1.22x faster                                                             |
| sympy_sum                | 196 ms                                                 | 163 ms: 1.20x faster                                                             |
| dask                     | 441 ms                                                 | 367 ms: 1.20x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 851 ms: 1.20x faster                                                             |
| 2to3                     | 348 ms                                                 | 292 ms: 1.19x faster                                                             |
| tomli_loads              | 3.14 sec                                               | 2.64 sec: 1.19x faster                                                           |
| docutils                 | 3.30 sec                                               | 2.80 sec: 1.18x faster                                                           |
| mako                     | 16.3 ms                                                | 14.0 ms: 1.16x faster                                                            |
| sympy_str                | 346 ms                                                 | 298 ms: 1.16x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 72.7 ms: 1.16x faster                                                            |
| pprint_pformat           | 2.10 sec                                               | 1.82 sec: 1.16x faster                                                           |
| sqlglot_optimize         | 69.2 ms                                                | 60.2 ms: 1.15x faster                                                            |
| bench_thread_pool        | 986 us                                                 | 862 us: 1.14x faster                                                             |
| hexiom                   | 10.4 ms                                                | 9.15 ms: 1.14x faster                                                            |
| json                     | 5.69 ms                                                | 5.04 ms: 1.13x faster                                                            |
| json_loads               | 31.2 us                                                | 27.7 us: 1.13x faster                                                            |
| fannkuch                 | 532 ms                                                 | 473 ms: 1.12x faster                                                             |
| sympy_expand             | 566 ms                                                 | 505 ms: 1.12x faster                                                             |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.82 ms: 1.11x faster                                                            |
| scimark_fft              | 466 ms                                                 | 419 ms: 1.11x faster                                                             |
| xml_etree_generate       | 99.4 ms                                                | 89.5 ms: 1.11x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 25.1 ms: 1.11x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.08x faster                                                            |
| pathlib                  | 20.5 ms                                                | 19.1 ms: 1.07x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.66 sec: 1.07x faster                                                           |
| regex_compile            | 188 ms                                                 | 176 ms: 1.07x faster                                                             |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| nqueens                  | 106 ms                                                 | 100 ms: 1.06x faster                                                             |
| scimark_lu               | 176 ms                                                 | 167 ms: 1.06x faster                                                             |
| unpack_sequence          | 60.0 ns                                                | 57.0 ns: 1.05x faster                                                            |
| xml_etree_iterparse      | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.89 us: 1.05x faster                                                            |
| meteor_contest           | 120 ms                                                 | 116 ms: 1.03x faster                                                             |
| regex_dna                | 227 ms                                                 | 221 ms: 1.02x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                             |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| gc_traversal             | 3.62 ms                                                | 3.75 ms: 1.04x slower                                                            |
| async_generators         | 444 ms                                                 | 466 ms: 1.05x slower                                                             |
| unpickle                 | 14.4 us                                                | 15.1 us: 1.05x slower                                                            |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                            |
| pickle_dict              | 29.6 us                                                | 33.6 us: 1.14x slower                                                            |
| telco                    | 7.27 ms                                                | 8.81 ms: 1.21x slower                                                            |
| coverage                 | 79.4 ms                                                | 97.9 ms: 1.23x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.82 ms: 1.49x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.24x faster                                                                     |

Benchmark hidden because not significant (5): regex_effbot, bench_mp_pool, pickle_list, mypy2, unpickle_list
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a4+-76389dd-PYTHON_UOPS/bm-20240215-linux-x86_64-faster%2dcpython-load_attr_module_con-3.13.0a4+-76389dd.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.07x