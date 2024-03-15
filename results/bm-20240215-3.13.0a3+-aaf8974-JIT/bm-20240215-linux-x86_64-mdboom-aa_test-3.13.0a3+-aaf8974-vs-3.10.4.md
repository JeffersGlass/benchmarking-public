
# Results vs. 3.10.4

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.32x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 275 ms: 1.27x faster                                      |
| chameleon      | 9.68 ms                                                | 6.82 ms: 1.42x faster                                     |
| docutils       | 3.30 sec                                               | 2.63 sec: 1.25x faster                                    |
| tornado_http   | 136 ms                                                 | 96.4 ms: 1.41x faster                                     |
| Geometric mean | (ref)                                                  | 1.34x faster                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 440 ms: 1.65x faster                                      |
| async_tree_memoization  | 870 ms                                                 | 567 ms: 1.53x faster                                      |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.49x faster                                    |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 717 ms: 1.42x faster                                      |
| Geometric mean          | (ref)                                                  | 1.52x faster                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| nbody          | 154 ms                                                 | 103 ms: 1.50x faster                                      |
| float          | 117 ms                                                 | 85.3 ms: 1.37x faster                                     |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                      |
| Geometric mean | (ref)                                                  | 1.28x faster                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 140 ms: 1.35x faster                                      |
| regex_v8       | 27.8 ms                                                | 25.4 ms: 1.09x faster                                     |
| regex_dna      | 227 ms                                                 | 218 ms: 1.04x faster                                      |
| Geometric mean | (ref)                                                  | 1.11x faster                                              |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 294 us: 1.65x faster                                      |
| unpickle_pure_python | 331 us                                                 | 228 us: 1.45x faster                                      |
| tomli_loads          | 3.14 sec                                               | 2.21 sec: 1.42x faster                                    |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.37x faster                                     |
| xml_etree_process    | 79.1 ms                                                | 58.2 ms: 1.36x faster                                     |
| xml_etree_generate   | 99.4 ms                                                | 85.7 ms: 1.16x faster                                     |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                     |
| xml_etree_parse      | 168 ms                                                 | 154 ms: 1.09x faster                                      |
| xml_etree_iterparse  | 115 ms                                                 | 107 ms: 1.08x faster                                      |
| unpickle_list        | 5.20 us                                                | 5.14 us: 1.01x faster                                     |
| pickle_list          | 5.08 us                                                | 5.04 us: 1.01x faster                                     |
| unpickle             | 14.4 us                                                | 15.0 us: 1.05x slower                                     |
| pickle               | 10.7 us                                                | 11.3 us: 1.06x slower                                     |
| pickle_dict          | 29.6 us                                                | 34.0 us: 1.15x slower                                     |
| Geometric mean       | (ref)                                                  | 1.16x faster                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                     |
| python_startup_no_site | 5.93 ms                                                | 8.81 ms: 1.48x slower                                     |
| Geometric mean         | (ref)                                                  | 1.02x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.1 ms: 1.35x faster                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 113 us: 4.82x faster                                      |
| generators               | 80.1 ms                                                | 29.3 ms: 2.74x faster                                     |
| deltablue                | 7.91 ms                                                | 3.34 ms: 2.37x faster                                     |
| logging_silent           | 190 ns                                                 | 99.6 ns: 1.90x faster                                     |
| richards_super           | 94.7 ms                                                | 51.4 ms: 1.84x faster                                     |
| asyncio_tcp              | 922 ms                                                 | 502 ms: 1.84x faster                                      |
| scimark_sor              | 220 ms                                                 | 120 ms: 1.83x faster                                      |
| raytrace                 | 507 ms                                                 | 282 ms: 1.80x faster                                      |
| richards                 | 79.3 ms                                                | 45.1 ms: 1.76x faster                                     |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.68x faster                                     |
| async_tree_none          | 728 ms                                                 | 440 ms: 1.65x faster                                      |
| pickle_pure_python       | 484 us                                                 | 294 us: 1.65x faster                                      |
| crypto_pyaes             | 128 ms                                                 | 78.4 ms: 1.63x faster                                     |
| chaos                    | 115 ms                                                 | 71.4 ms: 1.62x faster                                     |
| go                       | 240 ms                                                 | 149 ms: 1.61x faster                                      |
| sqlglot_transpile        | 2.57 ms                                                | 1.61 ms: 1.60x faster                                     |
| comprehensions           | 28.8 us                                                | 18.1 us: 1.59x faster                                     |
| scimark_monte_carlo      | 118 ms                                                 | 74.5 ms: 1.59x faster                                     |
| scimark_lu               | 176 ms                                                 | 114 ms: 1.55x faster                                      |
| async_tree_memoization   | 870 ms                                                 | 567 ms: 1.53x faster                                      |
| coroutines               | 35.1 ms                                                | 23.0 ms: 1.52x faster                                     |
| deepcopy_memo            | 58.5 us                                                | 38.4 us: 1.52x faster                                     |
| nbody                    | 154 ms                                                 | 103 ms: 1.50x faster                                      |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.49x faster                                    |
| logging_format           | 9.09 us                                                | 6.22 us: 1.46x faster                                     |
| logging_simple           | 8.30 us                                                | 5.71 us: 1.45x faster                                     |
| unpickle_pure_python     | 331 us                                                 | 228 us: 1.45x faster                                      |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                     |
| chameleon                | 9.68 ms                                                | 6.82 ms: 1.42x faster                                     |
| tomli_loads              | 3.14 sec                                               | 2.21 sec: 1.42x faster                                    |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.81 sec: 1.42x faster                                    |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 717 ms: 1.42x faster                                      |
| pyflate                  | 716 ms                                                 | 506 ms: 1.42x faster                                      |
| tornado_http             | 136 ms                                                 | 96.4 ms: 1.41x faster                                     |
| deepcopy                 | 479 us                                                 | 346 us: 1.38x faster                                      |
| float                    | 117 ms                                                 | 85.3 ms: 1.37x faster                                     |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.37x faster                                     |
| deepcopy_reduce          | 4.17 us                                                | 3.05 us: 1.37x faster                                     |
| xml_etree_process        | 79.1 ms                                                | 58.2 ms: 1.36x faster                                     |
| hexiom                   | 10.4 ms                                                | 7.68 ms: 1.35x faster                                     |
| regex_compile            | 188 ms                                                 | 140 ms: 1.35x faster                                      |
| mako                     | 16.3 ms                                                | 12.1 ms: 1.35x faster                                     |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.34x faster                                      |
| pycparser                | 1.58 sec                                               | 1.18 sec: 1.33x faster                                    |
| pprint_safe_repr         | 1.02 sec                                               | 769 ms: 1.32x faster                                      |
| pprint_pformat           | 2.10 sec                                               | 1.60 sec: 1.32x faster                                    |
| spectral_norm            | 170 ms                                                 | 132 ms: 1.29x faster                                      |
| sympy_integrate          | 25.8 ms                                                | 20.3 ms: 1.27x faster                                     |
| 2to3                     | 348 ms                                                 | 275 ms: 1.27x faster                                      |
| sqlglot_optimize         | 69.2 ms                                                | 54.7 ms: 1.27x faster                                     |
| fannkuch                 | 532 ms                                                 | 422 ms: 1.26x faster                                      |
| scimark_fft              | 466 ms                                                 | 371 ms: 1.26x faster                                      |
| docutils                 | 3.30 sec                                               | 2.63 sec: 1.25x faster                                    |
| sympy_sum                | 196 ms                                                 | 157 ms: 1.25x faster                                      |
| dulwich_log              | 84.3 ms                                                | 67.9 ms: 1.24x faster                                     |
| sympy_str                | 346 ms                                                 | 281 ms: 1.23x faster                                      |
| dask                     | 441 ms                                                 | 364 ms: 1.21x faster                                      |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.36 ms: 1.21x faster                                     |
| sympy_expand             | 566 ms                                                 | 474 ms: 1.19x faster                                      |
| nqueens                  | 106 ms                                                 | 89.4 ms: 1.18x faster                                     |
| bench_thread_pool        | 986 us                                                 | 835 us: 1.18x faster                                      |
| xml_etree_generate       | 99.4 ms                                                | 85.7 ms: 1.16x faster                                     |
| unpack_sequence          | 60.0 ns                                                | 52.7 ns: 1.14x faster                                     |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.13x faster                                     |
| json                     | 5.69 ms                                                | 5.13 ms: 1.11x faster                                     |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                     |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                     |
| mdp                      | 2.85 sec                                               | 2.59 sec: 1.10x faster                                    |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                      |
| regex_v8                 | 27.8 ms                                                | 25.4 ms: 1.09x faster                                     |
| xml_etree_parse          | 168 ms                                                 | 154 ms: 1.09x faster                                      |
| xml_etree_iterparse      | 115 ms                                                 | 107 ms: 1.08x faster                                      |
| sqlite_synth             | 3.02 us                                                | 2.81 us: 1.08x faster                                     |
| regex_dna                | 227 ms                                                 | 218 ms: 1.04x faster                                      |
| gc_traversal             | 3.62 ms                                                | 3.53 ms: 1.03x faster                                     |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                      |
| unpickle_list            | 5.20 us                                                | 5.14 us: 1.01x faster                                     |
| asyncio_websockets       | 559 ms                                                 | 553 ms: 1.01x faster                                      |
| pickle_list              | 5.08 us                                                | 5.04 us: 1.01x faster                                     |
| async_generators         | 444 ms                                                 | 456 ms: 1.03x slower                                      |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.05x slower                                     |
| pickle                   | 10.7 us                                                | 11.3 us: 1.06x slower                                     |
| pickle_dict              | 29.6 us                                                | 34.0 us: 1.15x slower                                     |
| telco                    | 7.27 ms                                                | 8.50 ms: 1.17x slower                                     |
| coverage                 | 79.4 ms                                                | 96.8 ms: 1.22x slower                                     |
| python_startup_no_site   | 5.93 ms                                                | 8.81 ms: 1.48x slower                                     |
| Geometric mean           | (ref)                                                  | 1.32x faster                                              |

Benchmark hidden because not significant (3): mypy2, regex_effbot, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a3+-aaf8974-JIT/bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.10x