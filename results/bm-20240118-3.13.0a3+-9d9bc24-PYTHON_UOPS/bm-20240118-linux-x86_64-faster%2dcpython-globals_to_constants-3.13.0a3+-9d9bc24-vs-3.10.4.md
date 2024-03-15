
# Results vs. 3.10.4

- fork: faster-cpython
- ref: globals_to_constants
- machine: linux-x86_64
- commit hash: 9d9bc24
- commit date: 2024-01-18
- overall geometric mean: 1.27x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 283 ms: 1.23x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.20 ms: 1.34x faster                                                            |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| tornado_http   | 136 ms                                                 | 101 ms: 1.35x faster                                                             |
| Geometric mean | (ref)                                                  | 1.29x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 449 ms: 1.62x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 576 ms: 1.51x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 719 ms: 1.41x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 118 ms: 1.30x faster                                                             |
| float          | 117 ms                                                 | 91.1 ms: 1.28x faster                                                            |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.19x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 151 ms: 1.25x faster                                                             |
| regex_v8       | 27.8 ms                                                | 24.8 ms: 1.12x faster                                                            |
| regex_effbot   | 3.63 ms                                                | 3.53 ms: 1.03x faster                                                            |
| regex_dna      | 227 ms                                                 | 225 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 299 us: 1.62x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 237 us: 1.40x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.33x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.39 sec: 1.32x faster                                                           |
| xml_etree_process    | 79.1 ms                                                | 61.4 ms: 1.29x faster                                                            |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 90.1 ms: 1.10x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| pickle_list          | 5.08 us                                                | 4.95 us: 1.03x faster                                                            |
| unpickle_list        | 5.20 us                                                | 5.33 us: 1.02x slower                                                            |
| unpickle             | 14.4 us                                                | 15.0 us: 1.04x slower                                                            |
| pickle               | 10.7 us                                                | 11.3 us: 1.06x slower                                                            |
| pickle_dict          | 29.6 us                                                | 33.0 us: 1.12x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.73 ms: 1.47x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 14.0 ms: 1.16x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 115 us: 4.73x faster                                                             |
| generators               | 80.1 ms                                                | 30.1 ms: 2.66x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 483 ms: 1.91x faster                                                             |
| logging_silent           | 190 ns                                                 | 107 ns: 1.78x faster                                                             |
| richards_super           | 94.7 ms                                                | 54.8 ms: 1.73x faster                                                            |
| raytrace                 | 507 ms                                                 | 300 ms: 1.69x faster                                                             |
| scimark_sor              | 220 ms                                                 | 131 ms: 1.67x faster                                                             |
| deltablue                | 7.91 ms                                                | 4.74 ms: 1.67x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.32 ms: 1.64x faster                                                            |
| richards                 | 79.3 ms                                                | 48.8 ms: 1.63x faster                                                            |
| async_tree_none          | 728 ms                                                 | 449 ms: 1.62x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 299 us: 1.62x faster                                                             |
| chaos                    | 115 ms                                                 | 73.7 ms: 1.57x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.65 ms: 1.56x faster                                                            |
| go                       | 240 ms                                                 | 155 ms: 1.54x faster                                                             |
| coroutines               | 35.1 ms                                                | 22.8 ms: 1.54x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 83.0 ms: 1.54x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 576 ms: 1.51x faster                                                             |
| unpack_sequence          | 60.0 ns                                                | 40.3 ns: 1.49x faster                                                            |
| scimark_monte_carlo      | 118 ms                                                 | 80.2 ms: 1.47x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.20 sec: 1.47x faster                                                           |
| scimark_lu               | 176 ms                                                 | 121 ms: 1.46x faster                                                             |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                           |
| deepcopy_memo            | 58.5 us                                                | 40.9 us: 1.43x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 719 ms: 1.41x faster                                                             |
| unpickle_pure_python     | 331 us                                                 | 237 us: 1.40x faster                                                             |
| logging_simple           | 8.30 us                                                | 6.08 us: 1.37x faster                                                            |
| comprehensions           | 28.8 us                                                | 21.3 us: 1.35x faster                                                            |
| tornado_http             | 136 ms                                                 | 101 ms: 1.35x faster                                                             |
| pyflate                  | 716 ms                                                 | 532 ms: 1.35x faster                                                             |
| chameleon                | 9.68 ms                                                | 7.20 ms: 1.34x faster                                                            |
| deepcopy                 | 479 us                                                 | 359 us: 1.33x faster                                                             |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.33x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                            |
| logging_format           | 9.09 us                                                | 6.90 us: 1.32x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.39 sec: 1.32x faster                                                           |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.31x faster                                                           |
| nbody                    | 154 ms                                                 | 118 ms: 1.30x faster                                                             |
| xml_etree_process        | 79.1 ms                                                | 61.4 ms: 1.29x faster                                                            |
| float                    | 117 ms                                                 | 91.1 ms: 1.28x faster                                                            |
| sqlglot_normalize        | 143 ms                                                 | 115 ms: 1.25x faster                                                             |
| regex_compile            | 188 ms                                                 | 151 ms: 1.25x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 818 ms: 1.24x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.70 sec: 1.24x faster                                                           |
| hexiom                   | 10.4 ms                                                | 8.42 ms: 1.23x faster                                                            |
| 2to3                     | 348 ms                                                 | 283 ms: 1.23x faster                                                             |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                             |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                           |
| sympy_integrate          | 25.8 ms                                                | 21.1 ms: 1.22x faster                                                            |
| dulwich_log              | 84.3 ms                                                | 69.4 ms: 1.22x faster                                                            |
| dask                     | 441 ms                                                 | 367 ms: 1.20x faster                                                             |
| sqlglot_optimize         | 69.2 ms                                                | 57.9 ms: 1.20x faster                                                            |
| sympy_str                | 346 ms                                                 | 291 ms: 1.19x faster                                                             |
| fannkuch                 | 532 ms                                                 | 455 ms: 1.17x faster                                                             |
| sympy_expand             | 566 ms                                                 | 485 ms: 1.17x faster                                                             |
| mako                     | 16.3 ms                                                | 14.0 ms: 1.16x faster                                                            |
| bench_thread_pool        | 986 us                                                 | 848 us: 1.16x faster                                                             |
| spectral_norm            | 170 ms                                                 | 147 ms: 1.16x faster                                                             |
| nqueens                  | 106 ms                                                 | 94.6 ms: 1.12x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 24.8 ms: 1.12x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                            |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 90.1 ms: 1.10x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.91 ms: 1.09x faster                                                            |
| json                     | 5.69 ms                                                | 5.22 ms: 1.09x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.63 sec: 1.08x faster                                                           |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| meteor_contest           | 120 ms                                                 | 115 ms: 1.04x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.92 us: 1.04x faster                                                            |
| regex_effbot             | 3.63 ms                                                | 3.53 ms: 1.03x faster                                                            |
| pickle_list              | 5.08 us                                                | 4.95 us: 1.03x faster                                                            |
| scimark_fft              | 466 ms                                                 | 456 ms: 1.02x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                             |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                             |
| regex_dna                | 227 ms                                                 | 225 ms: 1.01x faster                                                             |
| gc_traversal             | 3.62 ms                                                | 3.70 ms: 1.02x slower                                                            |
| unpickle_list            | 5.20 us                                                | 5.33 us: 1.02x slower                                                            |
| async_generators         | 444 ms                                                 | 457 ms: 1.03x slower                                                             |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.04x slower                                                            |
| pickle                   | 10.7 us                                                | 11.3 us: 1.06x slower                                                            |
| pickle_dict              | 29.6 us                                                | 33.0 us: 1.12x slower                                                            |
| telco                    | 7.27 ms                                                | 8.56 ms: 1.18x slower                                                            |
| coverage                 | 79.4 ms                                                | 95.5 ms: 1.20x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.73 ms: 1.47x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.27x faster                                                                     |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240118-3.13.0a3+-9d9bc24-PYTHON_UOPS/bm-20240118-linux-x86_64-faster%2dcpython-globals_to_constants-3.13.0a3+-9d9bc24.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.06x