
# Results vs. 3.10.4

- fork: faster-cpython
- ref: split_end_for
- machine: linux-x86_64
- commit hash: ed98265
- commit date: 2024-01-17
- overall geometric mean: 1.36x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                                      |
| chameleon      | 9.68 ms                                                | 6.74 ms: 1.44x faster                                                     |
| docutils       | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                    |
| tornado_http   | 136 ms                                                 | 94.1 ms: 1.45x faster                                                     |
| Geometric mean | (ref)                                                  | 1.36x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 435 ms: 1.67x faster                                                      |
| async_tree_memoization  | 870 ms                                                 | 563 ms: 1.55x faster                                                      |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                    |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 708 ms: 1.43x faster                                                      |
| Geometric mean          | (ref)                                                  | 1.54x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 86.6 ms: 1.77x faster                                                     |
| float          | 117 ms                                                 | 79.2 ms: 1.48x faster                                                     |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                                      |
| Geometric mean | (ref)                                                  | 1.39x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 129 ms: 1.46x faster                                                      |
| regex_v8       | 27.8 ms                                                | 25.5 ms: 1.09x faster                                                     |
| regex_dna      | 227 ms                                                 | 223 ms: 1.02x faster                                                      |
| regex_effbot   | 3.63 ms                                                | 3.71 ms: 1.02x slower                                                     |
| Geometric mean | (ref)                                                  | 1.12x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 297 us: 1.63x faster                                                      |
| unpickle_pure_python | 331 us                                                 | 211 us: 1.56x faster                                                      |
| tomli_loads          | 3.14 sec                                               | 2.11 sec: 1.49x faster                                                    |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.36x faster                                                     |
| xml_etree_process    | 79.1 ms                                                | 58.5 ms: 1.35x faster                                                     |
| xml_etree_generate   | 99.4 ms                                                | 85.7 ms: 1.16x faster                                                     |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                                     |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                                      |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                                      |
| pickle_list          | 5.08 us                                                | 5.25 us: 1.03x slower                                                     |
| unpickle             | 14.4 us                                                | 15.9 us: 1.11x slower                                                     |
| pickle               | 10.7 us                                                | 11.8 us: 1.11x slower                                                     |
| pickle_dict          | 29.6 us                                                | 34.9 us: 1.18x slower                                                     |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                              |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                     |
| python_startup_no_site | 5.93 ms                                                | 8.69 ms: 1.46x slower                                                     |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.95x faster                                                      |
| generators               | 80.1 ms                                                | 29.5 ms: 2.72x faster                                                     |
| deltablue                | 7.91 ms                                                | 3.22 ms: 2.46x faster                                                     |
| raytrace                 | 507 ms                                                 | 258 ms: 1.97x faster                                                      |
| chaos                    | 115 ms                                                 | 58.8 ms: 1.96x faster                                                     |
| asyncio_tcp              | 922 ms                                                 | 482 ms: 1.91x faster                                                      |
| logging_silent           | 190 ns                                                 | 101 ns: 1.89x faster                                                      |
| scimark_monte_carlo      | 118 ms                                                 | 66.2 ms: 1.78x faster                                                     |
| crypto_pyaes             | 128 ms                                                 | 71.7 ms: 1.78x faster                                                     |
| nbody                    | 154 ms                                                 | 86.6 ms: 1.77x faster                                                     |
| comprehensions           | 28.8 us                                                | 16.2 us: 1.77x faster                                                     |
| richards_super           | 94.7 ms                                                | 53.8 ms: 1.76x faster                                                     |
| go                       | 240 ms                                                 | 137 ms: 1.75x faster                                                      |
| sqlglot_parse            | 2.17 ms                                                | 1.24 ms: 1.75x faster                                                     |
| hexiom                   | 10.4 ms                                                | 5.97 ms: 1.74x faster                                                     |
| scimark_sor              | 220 ms                                                 | 128 ms: 1.71x faster                                                      |
| async_tree_none          | 728 ms                                                 | 435 ms: 1.67x faster                                                      |
| richards                 | 79.3 ms                                                | 47.8 ms: 1.66x faster                                                     |
| sqlglot_transpile        | 2.57 ms                                                | 1.56 ms: 1.65x faster                                                     |
| pickle_pure_python       | 484 us                                                 | 297 us: 1.63x faster                                                      |
| pyflate                  | 716 ms                                                 | 448 ms: 1.60x faster                                                      |
| scimark_lu               | 176 ms                                                 | 111 ms: 1.58x faster                                                      |
| unpickle_pure_python     | 331 us                                                 | 211 us: 1.56x faster                                                      |
| coroutines               | 35.1 ms                                                | 22.6 ms: 1.55x faster                                                     |
| async_tree_memoization   | 870 ms                                                 | 563 ms: 1.55x faster                                                      |
| deepcopy_memo            | 58.5 us                                                | 37.9 us: 1.54x faster                                                     |
| spectral_norm            | 170 ms                                                 | 112 ms: 1.52x faster                                                      |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                    |
| tomli_loads              | 3.14 sec                                               | 2.11 sec: 1.49x faster                                                    |
| float                    | 117 ms                                                 | 79.2 ms: 1.48x faster                                                     |
| logging_simple           | 8.30 us                                                | 5.65 us: 1.47x faster                                                     |
| logging_format           | 9.09 us                                                | 6.20 us: 1.47x faster                                                     |
| mako                     | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                     |
| regex_compile            | 188 ms                                                 | 129 ms: 1.46x faster                                                      |
| tornado_http             | 136 ms                                                 | 94.1 ms: 1.45x faster                                                     |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                                     |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                    |
| chameleon                | 9.68 ms                                                | 6.74 ms: 1.44x faster                                                     |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 708 ms: 1.43x faster                                                      |
| pprint_pformat           | 2.10 sec                                               | 1.47 sec: 1.43x faster                                                    |
| pprint_safe_repr         | 1.02 sec                                               | 717 ms: 1.42x faster                                                      |
| deepcopy                 | 479 us                                                 | 345 us: 1.39x faster                                                      |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.71 ms: 1.37x faster                                                     |
| deepcopy_reduce          | 4.17 us                                                | 3.06 us: 1.36x faster                                                     |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.36x faster                                                     |
| unpack_sequence          | 60.0 ns                                                | 44.3 ns: 1.35x faster                                                     |
| xml_etree_process        | 79.1 ms                                                | 58.5 ms: 1.35x faster                                                     |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                                      |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.33x faster                                                      |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                                     |
| fannkuch                 | 532 ms                                                 | 403 ms: 1.32x faster                                                      |
| 2to3                     | 348 ms                                                 | 264 ms: 1.32x faster                                                      |
| pycparser                | 1.58 sec                                               | 1.20 sec: 1.32x faster                                                    |
| nqueens                  | 106 ms                                                 | 80.8 ms: 1.31x faster                                                     |
| dulwich_log              | 84.3 ms                                                | 64.8 ms: 1.30x faster                                                     |
| scimark_fft              | 466 ms                                                 | 362 ms: 1.29x faster                                                      |
| sqlglot_optimize         | 69.2 ms                                                | 53.8 ms: 1.29x faster                                                     |
| docutils                 | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                    |
| sympy_str                | 346 ms                                                 | 275 ms: 1.26x faster                                                      |
| dask                     | 441 ms                                                 | 361 ms: 1.22x faster                                                      |
| sympy_expand             | 566 ms                                                 | 465 ms: 1.22x faster                                                      |
| bench_thread_pool        | 986 us                                                 | 823 us: 1.20x faster                                                      |
| xml_etree_generate       | 99.4 ms                                                | 85.7 ms: 1.16x faster                                                     |
| pathlib                  | 20.5 ms                                                | 18.1 ms: 1.13x faster                                                     |
| meteor_contest           | 120 ms                                                 | 106 ms: 1.13x faster                                                      |
| mdp                      | 2.85 sec                                               | 2.53 sec: 1.12x faster                                                    |
| json                     | 5.69 ms                                                | 5.12 ms: 1.11x faster                                                     |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                                     |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                                      |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                     |
| regex_v8                 | 27.8 ms                                                | 25.5 ms: 1.09x faster                                                     |
| sqlite_synth             | 3.02 us                                                | 2.80 us: 1.08x faster                                                     |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.07x faster                                                      |
| gc_traversal             | 3.62 ms                                                | 3.47 ms: 1.04x faster                                                     |
| regex_dna                | 227 ms                                                 | 223 ms: 1.02x faster                                                      |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                                      |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                      |
| regex_effbot             | 3.63 ms                                                | 3.71 ms: 1.02x slower                                                     |
| pickle_list              | 5.08 us                                                | 5.25 us: 1.03x slower                                                     |
| unpickle                 | 14.4 us                                                | 15.9 us: 1.11x slower                                                     |
| pickle                   | 10.7 us                                                | 11.8 us: 1.11x slower                                                     |
| telco                    | 7.27 ms                                                | 8.43 ms: 1.16x slower                                                     |
| pickle_dict              | 29.6 us                                                | 34.9 us: 1.18x slower                                                     |
| coverage                 | 79.4 ms                                                | 95.5 ms: 1.20x slower                                                     |
| python_startup_no_site   | 5.93 ms                                                | 8.69 ms: 1.46x slower                                                     |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                              |

Benchmark hidden because not significant (4): mypy2, unpickle_list, async_generators, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240117-3.13.0a3+-ed98265/bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.06x