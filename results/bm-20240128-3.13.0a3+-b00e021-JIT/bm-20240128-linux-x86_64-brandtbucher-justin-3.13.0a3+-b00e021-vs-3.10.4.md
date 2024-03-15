
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b00e021
- commit date: 2024-01-28
- overall geometric mean: 1.31x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 276 ms: 1.26x faster                                           |
| chameleon      | 9.68 ms                                                | 7.07 ms: 1.37x faster                                          |
| docutils       | 3.30 sec                                               | 2.66 sec: 1.24x faster                                         |
| tornado_http   | 136 ms                                                 | 97.5 ms: 1.40x faster                                          |
| Geometric mean | (ref)                                                  | 1.32x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 442 ms: 1.65x faster                                           |
| async_tree_memoization  | 870 ms                                                 | 564 ms: 1.54x faster                                           |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 708 ms: 1.43x faster                                           |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 104 ms: 1.48x faster                                           |
| float          | 117 ms                                                 | 86.2 ms: 1.36x faster                                          |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                           |
| Geometric mean | (ref)                                                  | 1.27x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 140 ms: 1.35x faster                                           |
| regex_v8       | 27.8 ms                                                | 24.5 ms: 1.13x faster                                          |
| regex_dna      | 227 ms                                                 | 219 ms: 1.03x faster                                           |
| regex_effbot   | 3.63 ms                                                | 3.53 ms: 1.03x faster                                          |
| Geometric mean | (ref)                                                  | 1.13x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 292 us: 1.66x faster                                           |
| unpickle_pure_python | 331 us                                                 | 229 us: 1.44x faster                                           |
| tomli_loads          | 3.14 sec                                               | 2.21 sec: 1.42x faster                                         |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.38x faster                                          |
| xml_etree_process    | 79.1 ms                                                | 59.5 ms: 1.33x faster                                          |
| xml_etree_generate   | 99.4 ms                                                | 87.4 ms: 1.14x faster                                          |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                          |
| xml_etree_parse      | 168 ms                                                 | 155 ms: 1.08x faster                                           |
| xml_etree_iterparse  | 115 ms                                                 | 108 ms: 1.06x faster                                           |
| pickle_list          | 5.08 us                                                | 5.14 us: 1.01x slower                                          |
| unpickle             | 14.4 us                                                | 14.9 us: 1.03x slower                                          |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                          |
| pickle_dict          | 29.6 us                                                | 34.3 us: 1.16x slower                                          |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                   |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                          |
| python_startup_no_site | 5.93 ms                                                | 8.84 ms: 1.49x slower                                          |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.7 ms: 1.29x faster                                          |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.88x faster                                           |
| generators               | 80.1 ms                                                | 29.7 ms: 2.69x faster                                          |
| deltablue                | 7.91 ms                                                | 4.06 ms: 1.95x faster                                          |
| asyncio_tcp              | 922 ms                                                 | 491 ms: 1.88x faster                                           |
| logging_silent           | 190 ns                                                 | 102 ns: 1.85x faster                                           |
| raytrace                 | 507 ms                                                 | 282 ms: 1.80x faster                                           |
| richards_super           | 94.7 ms                                                | 53.0 ms: 1.79x faster                                          |
| scimark_sor              | 220 ms                                                 | 123 ms: 1.78x faster                                           |
| richards                 | 79.3 ms                                                | 46.8 ms: 1.69x faster                                          |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.68x faster                                          |
| pickle_pure_python       | 484 us                                                 | 292 us: 1.66x faster                                           |
| crypto_pyaes             | 128 ms                                                 | 77.5 ms: 1.65x faster                                          |
| async_tree_none          | 728 ms                                                 | 442 ms: 1.65x faster                                           |
| chaos                    | 115 ms                                                 | 71.8 ms: 1.61x faster                                          |
| go                       | 240 ms                                                 | 150 ms: 1.60x faster                                           |
| coroutines               | 35.1 ms                                                | 22.0 ms: 1.60x faster                                          |
| sqlglot_transpile        | 2.57 ms                                                | 1.61 ms: 1.60x faster                                          |
| scimark_monte_carlo      | 118 ms                                                 | 75.6 ms: 1.56x faster                                          |
| deepcopy_memo            | 58.5 us                                                | 37.6 us: 1.56x faster                                          |
| async_tree_memoization   | 870 ms                                                 | 564 ms: 1.54x faster                                           |
| scimark_lu               | 176 ms                                                 | 115 ms: 1.53x faster                                           |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                         |
| nbody                    | 154 ms                                                 | 104 ms: 1.48x faster                                           |
| comprehensions           | 28.8 us                                                | 19.4 us: 1.48x faster                                          |
| unpickle_pure_python     | 331 us                                                 | 229 us: 1.44x faster                                           |
| logging_simple           | 8.30 us                                                | 5.77 us: 1.44x faster                                          |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 708 ms: 1.43x faster                                           |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                          |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                         |
| unpack_sequence          | 60.0 ns                                                | 42.1 ns: 1.42x faster                                          |
| tomli_loads              | 3.14 sec                                               | 2.21 sec: 1.42x faster                                         |
| logging_format           | 9.09 us                                                | 6.44 us: 1.41x faster                                          |
| tornado_http             | 136 ms                                                 | 97.5 ms: 1.40x faster                                          |
| deepcopy                 | 479 us                                                 | 344 us: 1.39x faster                                           |
| pyflate                  | 716 ms                                                 | 517 ms: 1.39x faster                                           |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.38x faster                                          |
| deepcopy_reduce          | 4.17 us                                                | 3.03 us: 1.37x faster                                          |
| chameleon                | 9.68 ms                                                | 7.07 ms: 1.37x faster                                          |
| float                    | 117 ms                                                 | 86.2 ms: 1.36x faster                                          |
| regex_compile            | 188 ms                                                 | 140 ms: 1.35x faster                                           |
| xml_etree_process        | 79.1 ms                                                | 59.5 ms: 1.33x faster                                          |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.30x faster                                         |
| sqlglot_normalize        | 143 ms                                                 | 110 ms: 1.30x faster                                           |
| hexiom                   | 10.4 ms                                                | 8.05 ms: 1.29x faster                                          |
| mako                     | 16.3 ms                                                | 12.7 ms: 1.29x faster                                          |
| pprint_safe_repr         | 1.02 sec                                               | 798 ms: 1.28x faster                                           |
| pprint_pformat           | 2.10 sec                                               | 1.65 sec: 1.27x faster                                         |
| 2to3                     | 348 ms                                                 | 276 ms: 1.26x faster                                           |
| docutils                 | 3.30 sec                                               | 2.66 sec: 1.24x faster                                         |
| sympy_integrate          | 25.8 ms                                                | 20.9 ms: 1.24x faster                                          |
| sqlglot_optimize         | 69.2 ms                                                | 56.1 ms: 1.23x faster                                          |
| dulwich_log              | 84.3 ms                                                | 68.4 ms: 1.23x faster                                          |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                           |
| fannkuch                 | 532 ms                                                 | 432 ms: 1.23x faster                                           |
| spectral_norm            | 170 ms                                                 | 139 ms: 1.23x faster                                           |
| scimark_fft              | 466 ms                                                 | 381 ms: 1.22x faster                                           |
| sympy_str                | 346 ms                                                 | 284 ms: 1.22x faster                                           |
| dask                     | 441 ms                                                 | 365 ms: 1.21x faster                                           |
| sympy_expand             | 566 ms                                                 | 478 ms: 1.18x faster                                           |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.49 ms: 1.18x faster                                          |
| bench_thread_pool        | 986 us                                                 | 839 us: 1.18x faster                                           |
| nqueens                  | 106 ms                                                 | 91.4 ms: 1.16x faster                                          |
| xml_etree_generate       | 99.4 ms                                                | 87.4 ms: 1.14x faster                                          |
| regex_v8                 | 27.8 ms                                                | 24.5 ms: 1.13x faster                                          |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                          |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                          |
| meteor_contest           | 120 ms                                                 | 110 ms: 1.09x faster                                           |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.08x faster                                          |
| xml_etree_parse          | 168 ms                                                 | 155 ms: 1.08x faster                                           |
| sqlite_synth             | 3.02 us                                                | 2.80 us: 1.08x faster                                          |
| json                     | 5.69 ms                                                | 5.27 ms: 1.08x faster                                          |
| xml_etree_iterparse      | 115 ms                                                 | 108 ms: 1.06x faster                                           |
| mdp                      | 2.85 sec                                               | 2.71 sec: 1.05x faster                                         |
| regex_dna                | 227 ms                                                 | 219 ms: 1.03x faster                                           |
| regex_effbot             | 3.63 ms                                                | 3.53 ms: 1.03x faster                                          |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                           |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                           |
| pickle_list              | 5.08 us                                                | 5.14 us: 1.01x slower                                          |
| async_generators         | 444 ms                                                 | 454 ms: 1.02x slower                                           |
| gc_traversal             | 3.62 ms                                                | 3.71 ms: 1.02x slower                                          |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.03x slower                                          |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                          |
| pickle_dict              | 29.6 us                                                | 34.3 us: 1.16x slower                                          |
| coverage                 | 79.4 ms                                                | 93.4 ms: 1.18x slower                                          |
| telco                    | 7.27 ms                                                | 8.65 ms: 1.19x slower                                          |
| python_startup_no_site   | 5.93 ms                                                | 8.84 ms: 1.49x slower                                          |
| Geometric mean           | (ref)                                                  | 1.31x faster                                                   |

Benchmark hidden because not significant (3): mypy2, unpickle_list, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240128-3.13.0a3+-b00e021-JIT/bm-20240128-linux-x86_64-brandtbucher-justin-3.13.0a3+-b00e021.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.10x