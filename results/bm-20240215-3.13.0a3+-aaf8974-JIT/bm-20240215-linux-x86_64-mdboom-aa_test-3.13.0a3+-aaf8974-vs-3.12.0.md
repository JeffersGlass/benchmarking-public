
# Results vs. 3.12.0

- fork: mdboom
- ref: aa_test
- machine: linux-x86_64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.01x faster \*
- HPT reliability: 93.76%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 275 ms: 1.00x slower                                      |
| chameleon      | 7.41 ms                                                | 6.82 ms: 1.09x faster                                     |
| docutils       | 2.77 sec                                               | 2.63 sec: 1.05x faster                                    |
| tornado_http   | 103 ms                                                 | 96.4 ms: 1.06x faster                                     |
| Geometric mean | (ref)                                                  | 1.05x faster                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_none        | 472 ms                                                 | 440 ms: 1.07x faster                                      |
| async_tree_memoization | 578 ms                                                 | 567 ms: 1.02x faster                                      |
| async_tree_none_tg     | 450 ms                                                 | 451 ms: 1.00x slower                                      |
| async_tree_io_tg       | 1.18 sec                                               | 1.21 sec: 1.02x slower                                    |
| async_tree_io          | 1.16 sec                                               | 1.18 sec: 1.02x slower                                    |
| Geometric mean         | (ref)                                                  | 1.01x faster                                              |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 187 ms: 1.00x slower                                      |
| float          | 84.7 ms                                                | 85.3 ms: 1.01x slower                                     |
| nbody          | 97.0 ms                                                | 103 ms: 1.06x slower                                      |
| Geometric mean | (ref)                                                  | 1.02x slower                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 140 ms: 1.06x faster                                      |
| regex_dna      | 212 ms                                                 | 218 ms: 1.03x slower                                      |
| regex_v8       | 23.1 ms                                                | 25.4 ms: 1.10x slower                                     |
| Geometric mean | (ref)                                                  | 1.02x slower                                              |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pickle_pure_python | 324 us                                                 | 294 us: 1.10x faster                                      |
| xml_etree_process  | 61.7 ms                                                | 58.2 ms: 1.06x faster                                     |
| unpickle           | 15.9 us                                                | 15.0 us: 1.05x faster                                     |
| tomli_loads        | 2.33 sec                                               | 2.21 sec: 1.05x faster                                    |
| pickle_dict        | 35.5 us                                                | 34.0 us: 1.05x faster                                     |
| xml_etree_generate | 89.2 ms                                                | 85.7 ms: 1.04x faster                                     |
| xml_etree_parse    | 159 ms                                                 | 154 ms: 1.03x faster                                      |
| unpickle_list      | 5.29 us                                                | 5.14 us: 1.03x faster                                     |
| pickle             | 11.6 us                                                | 11.3 us: 1.02x faster                                     |
| json_loads         | 28.5 us                                                | 28.2 us: 1.01x faster                                     |
| pickle_list        | 5.08 us                                                | 5.04 us: 1.01x faster                                     |
| json_dumps         | 10.4 ms                                                | 10.3 ms: 1.01x faster                                     |
| Geometric mean     | (ref)                                                  | 1.03x faster                                              |

Benchmark hidden because not significant (2): unpickle_pure_python, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                     |
| python_startup_no_site | 6.94 ms                                                | 8.81 ms: 1.27x slower                                     |
| Geometric mean         | (ref)                                                  | 1.16x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------:|
| mako      | 11.9 ms                                                | 12.1 ms: 1.02x slower                                     |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-linux-x86_64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 113 us: 1.40x faster                                      |
| comprehensions           | 21.8 us                                                | 18.1 us: 1.20x faster                                     |
| logging_format           | 7.23 us                                                | 6.22 us: 1.16x faster                                     |
| logging_simple           | 6.46 us                                                | 5.71 us: 1.13x faster                                     |
| deltablue                | 3.72 ms                                                | 3.34 ms: 1.11x faster                                     |
| raytrace                 | 312 ms                                                 | 282 ms: 1.11x faster                                      |
| pickle_pure_python       | 324 us                                                 | 294 us: 1.10x faster                                      |
| deepcopy_reduce          | 3.35 us                                                | 3.05 us: 1.10x faster                                     |
| chameleon                | 7.41 ms                                                | 6.82 ms: 1.09x faster                                     |
| sympy_sum                | 169 ms                                                 | 157 ms: 1.08x faster                                      |
| scimark_sor              | 129 ms                                                 | 120 ms: 1.08x faster                                      |
| gc_traversal             | 3.79 ms                                                | 3.53 ms: 1.08x faster                                     |
| async_tree_none          | 472 ms                                                 | 440 ms: 1.07x faster                                      |
| deepcopy                 | 371 us                                                 | 346 us: 1.07x faster                                      |
| generators               | 31.2 ms                                                | 29.3 ms: 1.07x faster                                     |
| sympy_str                | 300 ms                                                 | 281 ms: 1.07x faster                                      |
| pathlib                  | 19.3 ms                                                | 18.2 ms: 1.07x faster                                     |
| tornado_http             | 103 ms                                                 | 96.4 ms: 1.06x faster                                     |
| regex_compile            | 148 ms                                                 | 140 ms: 1.06x faster                                      |
| xml_etree_process        | 61.7 ms                                                | 58.2 ms: 1.06x faster                                     |
| deepcopy_memo            | 40.7 us                                                | 38.4 us: 1.06x faster                                     |
| sqlglot_parse            | 1.36 ms                                                | 1.29 ms: 1.05x faster                                     |
| unpickle                 | 15.9 us                                                | 15.0 us: 1.05x faster                                     |
| docutils                 | 2.77 sec                                               | 2.63 sec: 1.05x faster                                    |
| tomli_loads              | 2.33 sec                                               | 2.21 sec: 1.05x faster                                    |
| sympy_integrate          | 21.4 ms                                                | 20.3 ms: 1.05x faster                                     |
| logging_silent           | 104 ns                                                 | 99.6 ns: 1.05x faster                                     |
| pickle_dict              | 35.5 us                                                | 34.0 us: 1.05x faster                                     |
| sqlglot_transpile        | 1.68 ms                                                | 1.61 ms: 1.05x faster                                     |
| crypto_pyaes             | 81.9 ms                                                | 78.4 ms: 1.04x faster                                     |
| xml_etree_generate       | 89.2 ms                                                | 85.7 ms: 1.04x faster                                     |
| sqlglot_normalize        | 110 ms                                                 | 106 ms: 1.04x faster                                      |
| scimark_lu               | 118 ms                                                 | 114 ms: 1.04x faster                                      |
| xml_etree_parse          | 159 ms                                                 | 154 ms: 1.03x faster                                      |
| meteor_contest           | 112 ms                                                 | 109 ms: 1.03x faster                                      |
| scimark_fft              | 382 ms                                                 | 371 ms: 1.03x faster                                      |
| unpickle_list            | 5.29 us                                                | 5.14 us: 1.03x faster                                     |
| json                     | 5.26 ms                                                | 5.13 ms: 1.02x faster                                     |
| pickle                   | 11.6 us                                                | 11.3 us: 1.02x faster                                     |
| unpack_sequence          | 54.0 ns                                                | 52.7 ns: 1.02x faster                                     |
| dask                     | 372 ms                                                 | 364 ms: 1.02x faster                                      |
| async_tree_memoization   | 578 ms                                                 | 567 ms: 1.02x faster                                      |
| richards                 | 45.8 ms                                                | 45.1 ms: 1.02x faster                                     |
| async_generators         | 463 ms                                                 | 456 ms: 1.02x faster                                      |
| mdp                      | 2.63 sec                                               | 2.59 sec: 1.02x faster                                    |
| json_loads               | 28.5 us                                                | 28.2 us: 1.01x faster                                     |
| dulwich_log              | 68.5 ms                                                | 67.9 ms: 1.01x faster                                     |
| pprint_safe_repr         | 776 ms                                                 | 769 ms: 1.01x faster                                      |
| sympy_expand             | 478 ms                                                 | 474 ms: 1.01x faster                                      |
| pickle_list              | 5.08 us                                                | 5.04 us: 1.01x faster                                     |
| create_gc_cycles         | 1.48 ms                                                | 1.46 ms: 1.01x faster                                     |
| bench_thread_pool        | 842 us                                                 | 835 us: 1.01x faster                                      |
| scimark_monte_carlo      | 75.1 ms                                                | 74.5 ms: 1.01x faster                                     |
| sqlite_synth             | 2.83 us                                                | 2.81 us: 1.01x faster                                     |
| coroutines               | 23.2 ms                                                | 23.0 ms: 1.01x faster                                     |
| json_dumps               | 10.4 ms                                                | 10.3 ms: 1.01x faster                                     |
| sqlglot_optimize         | 54.8 ms                                                | 54.7 ms: 1.00x faster                                     |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x slower                                      |
| async_tree_none_tg       | 450 ms                                                 | 451 ms: 1.00x slower                                      |
| 2to3                     | 274 ms                                                 | 275 ms: 1.00x slower                                      |
| float                    | 84.7 ms                                                | 85.3 ms: 1.01x slower                                     |
| fannkuch                 | 417 ms                                                 | 422 ms: 1.01x slower                                      |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.81 sec: 1.01x slower                                    |
| mako                     | 11.9 ms                                                | 12.1 ms: 1.02x slower                                     |
| pprint_pformat           | 1.57 sec                                               | 1.60 sec: 1.02x slower                                    |
| async_tree_io_tg         | 1.18 sec                                               | 1.21 sec: 1.02x slower                                    |
| asyncio_tcp              | 491 ms                                                 | 502 ms: 1.02x slower                                      |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                    |
| regex_dna                | 212 ms                                                 | 218 ms: 1.03x slower                                      |
| pyflate                  | 482 ms                                                 | 506 ms: 1.05x slower                                      |
| nbody                    | 97.0 ms                                                | 103 ms: 1.06x slower                                      |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.36 ms: 1.06x slower                                     |
| chaos                    | 67.0 ms                                                | 71.4 ms: 1.07x slower                                     |
| python_startup           | 9.55 ms                                                | 10.2 ms: 1.07x slower                                     |
| go                       | 139 ms                                                 | 149 ms: 1.07x slower                                      |
| nqueens                  | 83.3 ms                                                | 89.4 ms: 1.07x slower                                     |
| regex_v8                 | 23.1 ms                                                | 25.4 ms: 1.10x slower                                     |
| spectral_norm            | 115 ms                                                 | 132 ms: 1.15x slower                                      |
| hexiom                   | 6.41 ms                                                | 7.68 ms: 1.20x slower                                     |
| telco                    | 7.10 ms                                                | 8.50 ms: 1.20x slower                                     |
| python_startup_no_site   | 6.94 ms                                                | 8.81 ms: 1.27x slower                                     |
| coverage                 | 72.7 ms                                                | 96.8 ms: 1.33x slower                                     |
| Geometric mean           | (ref)                                                  | 1.01x faster                                              |

Benchmark hidden because not significant (11): async_tree_cpu_io_mixed, unpickle_pure_python, richards_super, regex_effbot, xml_etree_iterparse, bench_mp_pool, async_tree_cpu_io_mixed_tg, pycparser, asyncio_websockets, async_tree_memoization_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 93.76% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x