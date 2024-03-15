
# Results vs. 3.10.4

- fork: mdboom
- ref: force_mimalloc
- machine: linux-x86_64
- commit hash: f8250a4
- commit date: 2024-02-14
- overall geometric mean: 1.37x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.30x faster
- Memory change: 1.14x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 258 ms: 1.35x faster                                             |
| chameleon      | 9.68 ms                                                | 6.72 ms: 1.44x faster                                            |
| docutils       | 3.30 sec                                               | 2.66 sec: 1.24x faster                                           |
| tornado_http   | 136 ms                                                 | 91.7 ms: 1.49x faster                                            |
| Geometric mean | (ref)                                                  | 1.38x faster                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 473 ms: 1.54x faster                                             |
| async_tree_memoization  | 870 ms                                                 | 628 ms: 1.39x faster                                             |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 763 ms: 1.33x faster                                             |
| async_tree_io           | 1.77 sec                                               | 1.34 sec: 1.32x faster                                           |
| Geometric mean          | (ref)                                                  | 1.39x faster                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 90.1 ms: 1.70x faster                                            |
| float          | 117 ms                                                 | 80.0 ms: 1.46x faster                                            |
| pidigits       | 191 ms                                                 | 181 ms: 1.05x faster                                             |
| Geometric mean | (ref)                                                  | 1.38x faster                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 126 ms: 1.50x faster                                             |
| regex_v8       | 27.8 ms                                                | 24.5 ms: 1.13x faster                                            |
| regex_dna      | 227 ms                                                 | 218 ms: 1.04x faster                                             |
| regex_effbot   | 3.63 ms                                                | 3.50 ms: 1.04x faster                                            |
| Geometric mean | (ref)                                                  | 1.16x faster                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 292 us: 1.66x faster                                             |
| unpickle_pure_python | 331 us                                                 | 213 us: 1.55x faster                                             |
| tomli_loads          | 3.14 sec                                               | 2.08 sec: 1.51x faster                                           |
| json_dumps           | 14.2 ms                                                | 10.2 ms: 1.39x faster                                            |
| xml_etree_process    | 79.1 ms                                                | 58.5 ms: 1.35x faster                                            |
| xml_etree_generate   | 99.4 ms                                                | 84.1 ms: 1.18x faster                                            |
| json_loads           | 31.2 us                                                | 27.1 us: 1.15x faster                                            |
| xml_etree_iterparse  | 115 ms                                                 | 103 ms: 1.12x faster                                             |
| xml_etree_parse      | 168 ms                                                 | 155 ms: 1.09x faster                                             |
| unpickle_list        | 5.20 us                                                | 4.92 us: 1.06x faster                                            |
| pickle_list          | 5.08 us                                                | 5.11 us: 1.01x slower                                            |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                            |
| unpickle             | 14.4 us                                                | 16.1 us: 1.12x slower                                            |
| pickle_dict          | 29.6 us                                                | 35.0 us: 1.18x slower                                            |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.45x faster                                            |
| python_startup_no_site | 5.93 ms                                                | 8.70 ms: 1.47x slower                                            |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.2 ms: 1.61x faster                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 107 us: 5.09x faster                                             |
| generators               | 80.1 ms                                                | 29.0 ms: 2.77x faster                                            |
| deltablue                | 7.91 ms                                                | 3.17 ms: 2.49x faster                                            |
| chaos                    | 115 ms                                                 | 58.3 ms: 1.98x faster                                            |
| logging_silent           | 190 ns                                                 | 96.9 ns: 1.96x faster                                            |
| raytrace                 | 507 ms                                                 | 259 ms: 1.96x faster                                             |
| scimark_sor              | 220 ms                                                 | 117 ms: 1.87x faster                                             |
| asyncio_tcp              | 922 ms                                                 | 498 ms: 1.85x faster                                             |
| crypto_pyaes             | 128 ms                                                 | 71.1 ms: 1.80x faster                                            |
| scimark_monte_carlo      | 118 ms                                                 | 66.1 ms: 1.79x faster                                            |
| comprehensions           | 28.8 us                                                | 16.1 us: 1.79x faster                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.22 ms: 1.78x faster                                            |
| richards_super           | 94.7 ms                                                | 53.5 ms: 1.77x faster                                            |
| go                       | 240 ms                                                 | 137 ms: 1.75x faster                                             |
| hexiom                   | 10.4 ms                                                | 6.09 ms: 1.71x faster                                            |
| nbody                    | 154 ms                                                 | 90.1 ms: 1.70x faster                                            |
| richards                 | 79.3 ms                                                | 46.9 ms: 1.69x faster                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.52 ms: 1.69x faster                                            |
| spectral_norm            | 170 ms                                                 | 101 ms: 1.68x faster                                             |
| pickle_pure_python       | 484 us                                                 | 292 us: 1.66x faster                                             |
| pyflate                  | 716 ms                                                 | 438 ms: 1.64x faster                                             |
| coroutines               | 35.1 ms                                                | 21.5 ms: 1.63x faster                                            |
| mako                     | 16.3 ms                                                | 10.2 ms: 1.61x faster                                            |
| deepcopy_memo            | 58.5 us                                                | 36.5 us: 1.60x faster                                            |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.56x faster                                             |
| unpickle_pure_python     | 331 us                                                 | 213 us: 1.55x faster                                             |
| async_tree_none          | 728 ms                                                 | 473 ms: 1.54x faster                                             |
| tomli_loads              | 3.14 sec                                               | 2.08 sec: 1.51x faster                                           |
| regex_compile            | 188 ms                                                 | 126 ms: 1.50x faster                                             |
| tornado_http             | 136 ms                                                 | 91.7 ms: 1.49x faster                                            |
| logging_simple           | 8.30 us                                                | 5.62 us: 1.48x faster                                            |
| logging_format           | 9.09 us                                                | 6.17 us: 1.47x faster                                            |
| unpack_sequence          | 60.0 ns                                                | 40.8 ns: 1.47x faster                                            |
| float                    | 117 ms                                                 | 80.0 ms: 1.46x faster                                            |
| pprint_pformat           | 2.10 sec                                               | 1.44 sec: 1.46x faster                                           |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.45x faster                                            |
| chameleon                | 9.68 ms                                                | 6.72 ms: 1.44x faster                                            |
| deepcopy                 | 479 us                                                 | 332 us: 1.44x faster                                             |
| pprint_safe_repr         | 1.02 sec                                               | 710 ms: 1.43x faster                                             |
| pycparser                | 1.58 sec                                               | 1.10 sec: 1.43x faster                                           |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.82 sec: 1.41x faster                                           |
| deepcopy_reduce          | 4.17 us                                                | 2.97 us: 1.41x faster                                            |
| sqlglot_normalize        | 143 ms                                                 | 102 ms: 1.40x faster                                             |
| json_dumps               | 14.2 ms                                                | 10.2 ms: 1.39x faster                                            |
| async_tree_memoization   | 870 ms                                                 | 628 ms: 1.39x faster                                             |
| fannkuch                 | 532 ms                                                 | 388 ms: 1.37x faster                                             |
| sympy_sum                | 196 ms                                                 | 145 ms: 1.36x faster                                             |
| xml_etree_process        | 79.1 ms                                                | 58.5 ms: 1.35x faster                                            |
| 2to3                     | 348 ms                                                 | 258 ms: 1.35x faster                                             |
| nqueens                  | 106 ms                                                 | 78.5 ms: 1.35x faster                                            |
| sympy_integrate          | 25.8 ms                                                | 19.2 ms: 1.34x faster                                            |
| sqlglot_optimize         | 69.2 ms                                                | 51.5 ms: 1.34x faster                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 763 ms: 1.33x faster                                             |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.86 ms: 1.33x faster                                            |
| dulwich_log              | 84.3 ms                                                | 63.4 ms: 1.33x faster                                            |
| scimark_fft              | 466 ms                                                 | 350 ms: 1.33x faster                                             |
| sympy_str                | 346 ms                                                 | 260 ms: 1.33x faster                                             |
| async_tree_io            | 1.77 sec                                               | 1.34 sec: 1.32x faster                                           |
| sympy_expand             | 566 ms                                                 | 448 ms: 1.26x faster                                             |
| docutils                 | 3.30 sec                                               | 2.66 sec: 1.24x faster                                           |
| dask                     | 441 ms                                                 | 366 ms: 1.20x faster                                             |
| pathlib                  | 20.5 ms                                                | 17.3 ms: 1.18x faster                                            |
| xml_etree_generate       | 99.4 ms                                                | 84.1 ms: 1.18x faster                                            |
| json_loads               | 31.2 us                                                | 27.1 us: 1.15x faster                                            |
| json                     | 5.69 ms                                                | 4.98 ms: 1.14x faster                                            |
| regex_v8                 | 27.8 ms                                                | 24.5 ms: 1.13x faster                                            |
| xml_etree_iterparse      | 115 ms                                                 | 103 ms: 1.12x faster                                             |
| sqlite_synth             | 3.02 us                                                | 2.72 us: 1.11x faster                                            |
| mdp                      | 2.85 sec                                               | 2.59 sec: 1.10x faster                                           |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.09x faster                                             |
| xml_etree_parse          | 168 ms                                                 | 155 ms: 1.09x faster                                             |
| unpickle_list            | 5.20 us                                                | 4.92 us: 1.06x faster                                            |
| pidigits                 | 191 ms                                                 | 181 ms: 1.05x faster                                             |
| create_gc_cycles         | 1.62 ms                                                | 1.54 ms: 1.05x faster                                            |
| regex_dna                | 227 ms                                                 | 218 ms: 1.04x faster                                             |
| regex_effbot             | 3.63 ms                                                | 3.50 ms: 1.04x faster                                            |
| asyncio_websockets       | 559 ms                                                 | 543 ms: 1.03x faster                                             |
| async_generators         | 444 ms                                                 | 442 ms: 1.00x faster                                             |
| pickle_list              | 5.08 us                                                | 5.11 us: 1.01x slower                                            |
| gc_traversal             | 3.62 ms                                                | 3.75 ms: 1.03x slower                                            |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                            |
| unpickle                 | 14.4 us                                                | 16.1 us: 1.12x slower                                            |
| telco                    | 7.27 ms                                                | 8.18 ms: 1.13x slower                                            |
| pickle_dict              | 29.6 us                                                | 35.0 us: 1.18x slower                                            |
| coverage                 | 79.4 ms                                                | 95.5 ms: 1.20x slower                                            |
| bench_thread_pool        | 986 us                                                 | 1.20 ms: 1.22x slower                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.70 ms: 1.47x slower                                            |
| Geometric mean           | (ref)                                                  | 1.37x faster                                                     |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240214-3.13.0a3+-f8250a4/bm-20240214-linux-x86_64-mdboom-force_mimalloc-3.13.0a3+-f8250a4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.33x
- 95% likely to have a speedup of 1.33x
- 99% likely to have a speedup of 1.30x


# Memory

- memory change: 1.14x