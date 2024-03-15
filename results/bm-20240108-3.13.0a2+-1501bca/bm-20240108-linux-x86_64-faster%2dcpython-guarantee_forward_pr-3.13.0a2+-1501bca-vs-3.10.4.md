
# Results vs. 3.10.4

- fork: faster-cpython
- ref: guarantee_forward_pr
- machine: linux-x86_64
- commit hash: 1501bca
- commit date: 2024-01-08
- overall geometric mean: 1.36x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 263 ms: 1.32x faster                                                             |
| chameleon      | 9.68 ms                                                | 6.89 ms: 1.41x faster                                                            |
| docutils       | 3.30 sec                                               | 2.58 sec: 1.28x faster                                                           |
| tornado_http   | 136 ms                                                 | 93.8 ms: 1.45x faster                                                            |
| Geometric mean | (ref)                                                  | 1.36x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 435 ms: 1.67x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 556 ms: 1.56x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 704 ms: 1.44x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.55x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.8 ms: 1.73x faster                                                            |
| float          | 117 ms                                                 | 80.1 ms: 1.46x faster                                                            |
| pidigits       | 191 ms                                                 | 195 ms: 1.02x slower                                                             |
| Geometric mean | (ref)                                                  | 1.35x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 129 ms: 1.46x faster                                                             |
| regex_v8       | 27.8 ms                                                | 26.0 ms: 1.07x faster                                                            |
| regex_dna      | 227 ms                                                 | 219 ms: 1.04x faster                                                             |
| Geometric mean | (ref)                                                  | 1.13x faster                                                                     |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 299 us: 1.62x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 214 us: 1.55x faster                                                             |
| tomli_loads          | 3.14 sec                                               | 2.12 sec: 1.48x faster                                                           |
| xml_etree_process    | 79.1 ms                                                | 59.4 ms: 1.33x faster                                                            |
| json_dumps           | 14.2 ms                                                | 10.7 ms: 1.32x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 86.0 ms: 1.16x faster                                                            |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                                             |
| json_loads           | 31.2 us                                                | 28.7 us: 1.09x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                                             |
| pickle_list          | 5.08 us                                                | 4.89 us: 1.04x faster                                                            |
| unpickle_list        | 5.20 us                                                | 5.11 us: 1.02x faster                                                            |
| unpickle             | 14.4 us                                                | 14.9 us: 1.03x slower                                                            |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                                            |
| pickle_dict          | 29.6 us                                                | 35.1 us: 1.19x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.73 ms: 1.47x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.1 ms: 1.47x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.97x faster                                                             |
| generators               | 80.1 ms                                                | 29.2 ms: 2.74x faster                                                            |
| deltablue                | 7.91 ms                                                | 3.20 ms: 2.47x faster                                                            |
| chaos                    | 115 ms                                                 | 58.7 ms: 1.97x faster                                                            |
| raytrace                 | 507 ms                                                 | 261 ms: 1.94x faster                                                             |
| asyncio_tcp              | 922 ms                                                 | 481 ms: 1.92x faster                                                             |
| logging_silent           | 190 ns                                                 | 104 ns: 1.83x faster                                                             |
| crypto_pyaes             | 128 ms                                                 | 70.6 ms: 1.81x faster                                                            |
| comprehensions           | 28.8 us                                                | 16.1 us: 1.79x faster                                                            |
| go                       | 240 ms                                                 | 137 ms: 1.75x faster                                                             |
| sqlglot_parse            | 2.17 ms                                                | 1.24 ms: 1.74x faster                                                            |
| scimark_monte_carlo      | 118 ms                                                 | 68.0 ms: 1.74x faster                                                            |
| richards_super           | 94.7 ms                                                | 54.5 ms: 1.74x faster                                                            |
| nbody                    | 154 ms                                                 | 88.8 ms: 1.73x faster                                                            |
| scimark_sor              | 220 ms                                                 | 127 ms: 1.73x faster                                                             |
| hexiom                   | 10.4 ms                                                | 6.09 ms: 1.71x faster                                                            |
| async_tree_none          | 728 ms                                                 | 435 ms: 1.67x faster                                                             |
| richards                 | 79.3 ms                                                | 47.6 ms: 1.67x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.56 ms: 1.65x faster                                                            |
| pickle_pure_python       | 484 us                                                 | 299 us: 1.62x faster                                                             |
| coroutines               | 35.1 ms                                                | 22.0 ms: 1.60x faster                                                            |
| pyflate                  | 716 ms                                                 | 452 ms: 1.58x faster                                                             |
| async_tree_memoization   | 870 ms                                                 | 556 ms: 1.56x faster                                                             |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.55x faster                                                             |
| unpickle_pure_python     | 331 us                                                 | 214 us: 1.55x faster                                                             |
| deepcopy_memo            | 58.5 us                                                | 38.4 us: 1.52x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                           |
| spectral_norm            | 170 ms                                                 | 112 ms: 1.51x faster                                                             |
| logging_simple           | 8.30 us                                                | 5.57 us: 1.49x faster                                                            |
| logging_format           | 9.09 us                                                | 6.13 us: 1.48x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.12 sec: 1.48x faster                                                           |
| mako                     | 16.3 ms                                                | 11.1 ms: 1.47x faster                                                            |
| regex_compile            | 188 ms                                                 | 129 ms: 1.46x faster                                                             |
| float                    | 117 ms                                                 | 80.1 ms: 1.46x faster                                                            |
| tornado_http             | 136 ms                                                 | 93.8 ms: 1.45x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.45x faster                                                           |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 704 ms: 1.44x faster                                                             |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                            |
| chameleon                | 9.68 ms                                                | 6.89 ms: 1.41x faster                                                            |
| pprint_pformat           | 2.10 sec                                               | 1.50 sec: 1.40x faster                                                           |
| deepcopy                 | 479 us                                                 | 346 us: 1.38x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 739 ms: 1.38x faster                                                             |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.35x faster                                                             |
| fannkuch                 | 532 ms                                                 | 394 ms: 1.35x faster                                                             |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.34x faster                                                             |
| sympy_integrate          | 25.8 ms                                                | 19.3 ms: 1.33x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.13 us: 1.33x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 59.4 ms: 1.33x faster                                                            |
| unpack_sequence          | 60.0 ns                                                | 45.2 ns: 1.33x faster                                                            |
| 2to3                     | 348 ms                                                 | 263 ms: 1.32x faster                                                             |
| nqueens                  | 106 ms                                                 | 80.0 ms: 1.32x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.7 ms: 1.32x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.32x faster                                                           |
| sqlglot_optimize         | 69.2 ms                                                | 53.4 ms: 1.29x faster                                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.00 ms: 1.29x faster                                                            |
| sympy_str                | 346 ms                                                 | 268 ms: 1.29x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 65.5 ms: 1.29x faster                                                            |
| scimark_fft              | 466 ms                                                 | 362 ms: 1.29x faster                                                             |
| docutils                 | 3.30 sec                                               | 2.58 sec: 1.28x faster                                                           |
| sympy_expand             | 566 ms                                                 | 454 ms: 1.25x faster                                                             |
| dask                     | 441 ms                                                 | 361 ms: 1.22x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 826 us: 1.19x faster                                                             |
| xml_etree_generate       | 99.4 ms                                                | 86.0 ms: 1.16x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                            |
| meteor_contest           | 120 ms                                                 | 108 ms: 1.11x faster                                                             |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                                             |
| mdp                      | 2.85 sec                                               | 2.60 sec: 1.09x faster                                                           |
| json_loads               | 31.2 us                                                | 28.7 us: 1.09x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                            |
| json                     | 5.69 ms                                                | 5.26 ms: 1.08x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 26.0 ms: 1.07x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.88 us: 1.05x faster                                                            |
| pickle_list              | 5.08 us                                                | 4.89 us: 1.04x faster                                                            |
| regex_dna                | 227 ms                                                 | 219 ms: 1.04x faster                                                             |
| unpickle_list            | 5.20 us                                                | 5.11 us: 1.02x faster                                                            |
| async_generators         | 444 ms                                                 | 437 ms: 1.01x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                             |
| pidigits                 | 191 ms                                                 | 195 ms: 1.02x slower                                                             |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.03x slower                                                            |
| gc_traversal             | 3.62 ms                                                | 3.81 ms: 1.05x slower                                                            |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                                            |
| telco                    | 7.27 ms                                                | 8.41 ms: 1.16x slower                                                            |
| pickle_dict              | 29.6 us                                                | 35.1 us: 1.19x slower                                                            |
| coverage                 | 79.4 ms                                                | 94.7 ms: 1.19x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.73 ms: 1.47x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                                     |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240108-3.13.0a2+-1501bca/bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.05x