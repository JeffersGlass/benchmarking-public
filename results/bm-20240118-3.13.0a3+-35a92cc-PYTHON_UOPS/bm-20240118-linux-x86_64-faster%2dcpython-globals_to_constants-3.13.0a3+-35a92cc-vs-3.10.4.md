
# Results vs. 3.10.4

- fork: faster-cpython
- ref: globals_to_constants
- machine: linux-x86_64
- commit hash: 35a92cc
- commit date: 2024-01-18
- overall geometric mean: 1.28x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 281 ms: 1.24x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.22 ms: 1.34x faster                                                            |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| tornado_http   | 136 ms                                                 | 101 ms: 1.35x faster                                                             |
| Geometric mean | (ref)                                                  | 1.29x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 449 ms: 1.62x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 577 ms: 1.51x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 719 ms: 1.41x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 111 ms: 1.38x faster                                                             |
| float          | 117 ms                                                 | 90.0 ms: 1.30x faster                                                            |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.22x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 149 ms: 1.26x faster                                                             |
| regex_v8       | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                            |
| regex_dna      | 227 ms                                                 | 219 ms: 1.04x faster                                                             |
| regex_effbot   | 3.63 ms                                                | 3.52 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                  | 1.11x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 298 us: 1.63x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 231 us: 1.43x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.33x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 60.4 ms: 1.31x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.55 sec: 1.23x faster                                                           |
| xml_etree_generate   | 99.4 ms                                                | 88.0 ms: 1.13x faster                                                            |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                             |
| pickle_list          | 5.08 us                                                | 4.85 us: 1.05x faster                                                            |
| unpickle             | 14.4 us                                                | 14.8 us: 1.03x slower                                                            |
| unpickle_list        | 5.20 us                                                | 5.45 us: 1.05x slower                                                            |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                                            |
| pickle_dict          | 29.6 us                                                | 35.1 us: 1.19x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.72 ms: 1.47x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.2 ms: 1.23x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 114 us: 4.76x faster                                                             |
| generators               | 80.1 ms                                                | 29.7 ms: 2.70x faster                                                            |
| deltablue                | 7.91 ms                                                | 3.51 ms: 2.25x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 482 ms: 1.91x faster                                                             |
| logging_silent           | 190 ns                                                 | 105 ns: 1.81x faster                                                             |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.77x faster                                                             |
| richards_super           | 94.7 ms                                                | 55.2 ms: 1.72x faster                                                            |
| raytrace                 | 507 ms                                                 | 296 ms: 1.72x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 298 us: 1.63x faster                                                             |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                            |
| async_tree_none          | 728 ms                                                 | 449 ms: 1.62x faster                                                             |
| richards                 | 79.3 ms                                                | 48.8 ms: 1.62x faster                                                            |
| chaos                    | 115 ms                                                 | 71.7 ms: 1.61x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 81.6 ms: 1.57x faster                                                            |
| coroutines               | 35.1 ms                                                | 22.6 ms: 1.55x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                                            |
| scimark_monte_carlo      | 118 ms                                                 | 78.4 ms: 1.51x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 577 ms: 1.51x faster                                                             |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                           |
| scimark_lu               | 176 ms                                                 | 119 ms: 1.48x faster                                                             |
| unpack_sequence          | 60.0 ns                                                | 40.7 ns: 1.47x faster                                                            |
| deepcopy_memo            | 58.5 us                                                | 40.0 us: 1.46x faster                                                            |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.43x faster                                                           |
| unpickle_pure_python     | 331 us                                                 | 231 us: 1.43x faster                                                             |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 719 ms: 1.41x faster                                                             |
| comprehensions           | 28.8 us                                                | 20.6 us: 1.39x faster                                                            |
| nbody                    | 154 ms                                                 | 111 ms: 1.38x faster                                                             |
| go                       | 240 ms                                                 | 174 ms: 1.38x faster                                                             |
| pyflate                  | 716 ms                                                 | 521 ms: 1.37x faster                                                             |
| logging_simple           | 8.30 us                                                | 6.10 us: 1.36x faster                                                            |
| tornado_http             | 136 ms                                                 | 101 ms: 1.35x faster                                                             |
| logging_format           | 9.09 us                                                | 6.76 us: 1.34x faster                                                            |
| chameleon                | 9.68 ms                                                | 7.22 ms: 1.34x faster                                                            |
| deepcopy                 | 479 us                                                 | 358 us: 1.34x faster                                                             |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.33x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 60.4 ms: 1.31x faster                                                            |
| float                    | 117 ms                                                 | 90.0 ms: 1.30x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.22 us: 1.30x faster                                                            |
| hexiom                   | 10.4 ms                                                | 8.04 ms: 1.29x faster                                                            |
| pprint_safe_repr         | 1.02 sec                                               | 794 ms: 1.28x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.66 sec: 1.27x faster                                                           |
| regex_compile            | 188 ms                                                 | 149 ms: 1.26x faster                                                             |
| pycparser                | 1.58 sec                                               | 1.25 sec: 1.26x faster                                                           |
| sqlglot_normalize        | 143 ms                                                 | 115 ms: 1.25x faster                                                             |
| 2to3                     | 348 ms                                                 | 281 ms: 1.24x faster                                                             |
| mako                     | 16.3 ms                                                | 13.2 ms: 1.23x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.55 sec: 1.23x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.1 ms: 1.22x faster                                                            |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| sympy_sum                | 196 ms                                                 | 161 ms: 1.22x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 69.3 ms: 1.22x faster                                                            |
| spectral_norm            | 170 ms                                                 | 140 ms: 1.22x faster                                                             |
| fannkuch                 | 532 ms                                                 | 439 ms: 1.21x faster                                                             |
| sqlglot_optimize         | 69.2 ms                                                | 57.9 ms: 1.19x faster                                                            |
| dask                     | 441 ms                                                 | 369 ms: 1.19x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 841 us: 1.17x faster                                                             |
| sympy_expand             | 566 ms                                                 | 488 ms: 1.16x faster                                                             |
| sympy_str                | 346 ms                                                 | 303 ms: 1.14x faster                                                             |
| nqueens                  | 106 ms                                                 | 93.4 ms: 1.13x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 88.0 ms: 1.13x faster                                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.80 ms: 1.11x faster                                                            |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 25.0 ms: 1.11x faster                                                            |
| json                     | 5.69 ms                                                | 5.14 ms: 1.11x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.5 ms: 1.10x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| mdp                      | 2.85 sec                                               | 2.66 sec: 1.07x faster                                                           |
| scimark_fft              | 466 ms                                                 | 436 ms: 1.07x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.86 us: 1.06x faster                                                            |
| meteor_contest           | 120 ms                                                 | 114 ms: 1.05x faster                                                             |
| pickle_list              | 5.08 us                                                | 4.85 us: 1.05x faster                                                            |
| regex_dna                | 227 ms                                                 | 219 ms: 1.04x faster                                                             |
| regex_effbot             | 3.63 ms                                                | 3.52 ms: 1.03x faster                                                            |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                             |
| async_generators         | 444 ms                                                 | 451 ms: 1.02x slower                                                             |
| gc_traversal             | 3.62 ms                                                | 3.70 ms: 1.02x slower                                                            |
| unpickle                 | 14.4 us                                                | 14.8 us: 1.03x slower                                                            |
| unpickle_list            | 5.20 us                                                | 5.45 us: 1.05x slower                                                            |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                                            |
| telco                    | 7.27 ms                                                | 8.57 ms: 1.18x slower                                                            |
| pickle_dict              | 29.6 us                                                | 35.1 us: 1.19x slower                                                            |
| coverage                 | 79.4 ms                                                | 95.7 ms: 1.20x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.72 ms: 1.47x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.28x faster                                                                     |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240118-3.13.0a3+-35a92cc-PYTHON_UOPS/bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-35a92cc.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.06x