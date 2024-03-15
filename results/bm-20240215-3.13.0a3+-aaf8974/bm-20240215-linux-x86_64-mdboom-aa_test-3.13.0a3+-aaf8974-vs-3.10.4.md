
# Results vs. 3.10.4

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.37x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.30x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 262 ms: 1.33x faster                                      |
| chameleon      | 9.68 ms                                                | 6.68 ms: 1.45x faster                                     |
| docutils       | 3.30 sec                                               | 2.56 sec: 1.29x faster                                    |
| tornado_http   | 136 ms                                                 | 94.3 ms: 1.45x faster                                     |
| Geometric mean | (ref)                                                  | 1.38x faster                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 431 ms: 1.69x faster                                      |
| async_tree_memoization  | 870 ms                                                 | 555 ms: 1.57x faster                                      |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                    |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 701 ms: 1.45x faster                                      |
| Geometric mean          | (ref)                                                  | 1.55x faster                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.7 ms: 1.73x faster                                     |
| float          | 117 ms                                                 | 79.2 ms: 1.48x faster                                     |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                      |
| Geometric mean | (ref)                                                  | 1.38x faster                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 127 ms: 1.48x faster                                      |
| regex_v8       | 27.8 ms                                                | 23.8 ms: 1.17x faster                                     |
| regex_dna      | 227 ms                                                 | 223 ms: 1.02x faster                                      |
| Geometric mean | (ref)                                                  | 1.15x faster                                              |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 293 us: 1.66x faster                                      |
| unpickle_pure_python | 331 us                                                 | 210 us: 1.58x faster                                      |
| tomli_loads          | 3.14 sec                                               | 2.09 sec: 1.51x faster                                    |
| xml_etree_process    | 79.1 ms                                                | 57.8 ms: 1.37x faster                                     |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.37x faster                                     |
| xml_etree_generate   | 99.4 ms                                                | 84.5 ms: 1.18x faster                                     |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                     |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                      |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                      |
| unpickle_list        | 5.20 us                                                | 4.98 us: 1.04x faster                                     |
| pickle_list          | 5.08 us                                                | 4.92 us: 1.03x faster                                     |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                     |
| unpickle             | 14.4 us                                                | 15.8 us: 1.10x slower                                     |
| pickle_dict          | 29.6 us                                                | 34.0 us: 1.15x slower                                     |
| Geometric mean       | (ref)                                                  | 1.17x faster                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                     |
| python_startup_no_site | 5.93 ms                                                | 8.78 ms: 1.48x slower                                     |
| Geometric mean         | (ref)                                                  | 1.02x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.1 ms: 1.47x faster                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 108 us: 5.03x faster                                      |
| generators               | 80.1 ms                                                | 28.9 ms: 2.77x faster                                     |
| deltablue                | 7.91 ms                                                | 3.19 ms: 2.48x faster                                     |
| logging_silent           | 190 ns                                                 | 94.7 ns: 2.00x faster                                     |
| chaos                    | 115 ms                                                 | 58.8 ms: 1.96x faster                                     |
| raytrace                 | 507 ms                                                 | 260 ms: 1.95x faster                                      |
| asyncio_tcp              | 922 ms                                                 | 484 ms: 1.90x faster                                      |
| crypto_pyaes             | 128 ms                                                 | 70.6 ms: 1.81x faster                                     |
| comprehensions           | 28.8 us                                                | 16.0 us: 1.80x faster                                     |
| richards_super           | 94.7 ms                                                | 52.8 ms: 1.79x faster                                     |
| scimark_monte_carlo      | 118 ms                                                 | 65.9 ms: 1.79x faster                                     |
| hexiom                   | 10.4 ms                                                | 5.91 ms: 1.76x faster                                     |
| sqlglot_parse            | 2.17 ms                                                | 1.24 ms: 1.75x faster                                     |
| nbody                    | 154 ms                                                 | 88.7 ms: 1.73x faster                                     |
| go                       | 240 ms                                                 | 139 ms: 1.73x faster                                      |
| scimark_sor              | 220 ms                                                 | 129 ms: 1.71x faster                                      |
| richards                 | 79.3 ms                                                | 46.7 ms: 1.70x faster                                     |
| async_tree_none          | 728 ms                                                 | 431 ms: 1.69x faster                                      |
| sqlglot_transpile        | 2.57 ms                                                | 1.55 ms: 1.66x faster                                     |
| pickle_pure_python       | 484 us                                                 | 293 us: 1.66x faster                                      |
| deepcopy_memo            | 58.5 us                                                | 36.4 us: 1.60x faster                                     |
| scimark_lu               | 176 ms                                                 | 111 ms: 1.58x faster                                      |
| unpickle_pure_python     | 331 us                                                 | 210 us: 1.58x faster                                      |
| async_tree_memoization   | 870 ms                                                 | 555 ms: 1.57x faster                                      |
| coroutines               | 35.1 ms                                                | 22.5 ms: 1.56x faster                                     |
| spectral_norm            | 170 ms                                                 | 110 ms: 1.54x faster                                      |
| pyflate                  | 716 ms                                                 | 466 ms: 1.54x faster                                      |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                    |
| tomli_loads              | 3.14 sec                                               | 2.09 sec: 1.51x faster                                    |
| regex_compile            | 188 ms                                                 | 127 ms: 1.48x faster                                      |
| logging_simple           | 8.30 us                                                | 5.61 us: 1.48x faster                                     |
| logging_format           | 9.09 us                                                | 6.14 us: 1.48x faster                                     |
| float                    | 117 ms                                                 | 79.2 ms: 1.48x faster                                     |
| mako                     | 16.3 ms                                                | 11.1 ms: 1.47x faster                                     |
| chameleon                | 9.68 ms                                                | 6.68 ms: 1.45x faster                                     |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 701 ms: 1.45x faster                                      |
| tornado_http             | 136 ms                                                 | 94.3 ms: 1.45x faster                                     |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                    |
| pprint_pformat           | 2.10 sec                                               | 1.47 sec: 1.44x faster                                    |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                     |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.56 ms: 1.42x faster                                     |
| deepcopy                 | 479 us                                                 | 338 us: 1.42x faster                                      |
| pprint_safe_repr         | 1.02 sec                                               | 721 ms: 1.41x faster                                      |
| deepcopy_reduce          | 4.17 us                                                | 2.99 us: 1.40x faster                                     |
| pycparser                | 1.58 sec                                               | 1.15 sec: 1.38x faster                                    |
| sqlglot_normalize        | 143 ms                                                 | 104 ms: 1.37x faster                                      |
| xml_etree_process        | 79.1 ms                                                | 57.8 ms: 1.37x faster                                     |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.37x faster                                     |
| fannkuch                 | 532 ms                                                 | 390 ms: 1.36x faster                                      |
| nqueens                  | 106 ms                                                 | 77.9 ms: 1.36x faster                                     |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.34x faster                                      |
| sympy_integrate          | 25.8 ms                                                | 19.4 ms: 1.33x faster                                     |
| 2to3                     | 348 ms                                                 | 262 ms: 1.33x faster                                      |
| scimark_fft              | 466 ms                                                 | 352 ms: 1.32x faster                                      |
| sympy_str                | 346 ms                                                 | 264 ms: 1.31x faster                                      |
| sqlglot_optimize         | 69.2 ms                                                | 52.9 ms: 1.31x faster                                     |
| dulwich_log              | 84.3 ms                                                | 65.1 ms: 1.30x faster                                     |
| docutils                 | 3.30 sec                                               | 2.56 sec: 1.29x faster                                    |
| sympy_expand             | 566 ms                                                 | 447 ms: 1.27x faster                                      |
| dask                     | 441 ms                                                 | 359 ms: 1.23x faster                                      |
| bench_thread_pool        | 986 us                                                 | 816 us: 1.21x faster                                      |
| unpack_sequence          | 60.0 ns                                                | 50.1 ns: 1.20x faster                                     |
| xml_etree_generate       | 99.4 ms                                                | 84.5 ms: 1.18x faster                                     |
| regex_v8                 | 27.8 ms                                                | 23.8 ms: 1.17x faster                                     |
| pathlib                  | 20.5 ms                                                | 18.1 ms: 1.13x faster                                     |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.12x faster                                      |
| json                     | 5.69 ms                                                | 5.10 ms: 1.12x faster                                     |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                     |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                      |
| sqlite_synth             | 3.02 us                                                | 2.77 us: 1.09x faster                                     |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                     |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                      |
| mdp                      | 2.85 sec                                               | 2.72 sec: 1.05x faster                                    |
| unpickle_list            | 5.20 us                                                | 4.98 us: 1.04x faster                                     |
| pickle_list              | 5.08 us                                                | 4.92 us: 1.03x faster                                     |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                      |
| regex_dna                | 227 ms                                                 | 223 ms: 1.02x faster                                      |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                      |
| async_generators         | 444 ms                                                 | 448 ms: 1.01x slower                                      |
| gc_traversal             | 3.62 ms                                                | 3.78 ms: 1.04x slower                                     |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                     |
| unpickle                 | 14.4 us                                                | 15.8 us: 1.10x slower                                     |
| telco                    | 7.27 ms                                                | 8.23 ms: 1.13x slower                                     |
| pickle_dict              | 29.6 us                                                | 34.0 us: 1.15x slower                                     |
| coverage                 | 79.4 ms                                                | 95.2 ms: 1.20x slower                                     |
| python_startup_no_site   | 5.93 ms                                                | 8.78 ms: 1.48x slower                                     |
| Geometric mean           | (ref)                                                  | 1.37x faster                                              |

Benchmark hidden because not significant (3): mypy2, regex_effbot, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a3+-aaf8974/bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.33x
- 95% likely to have a speedup of 1.32x
- 99% likely to have a speedup of 1.30x


# Memory

- memory change: 1.06x