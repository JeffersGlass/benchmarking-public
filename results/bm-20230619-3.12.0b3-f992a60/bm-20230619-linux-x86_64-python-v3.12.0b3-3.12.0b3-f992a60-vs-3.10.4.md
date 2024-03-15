
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b3
- machine: linux-x86_64
- commit hash: f992a60
- commit date: 2023-06-19
- overall geometric mean: 1.35x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 267 ms: 1.30x faster                                       |
| docutils       | 3.30 sec                                               | 2.72 sec: 1.21x faster                                     |
| tornado_http   | 136 ms                                                 | 99.3 ms: 1.37x faster                                      |
| Geometric mean | (ref)                                                  | 1.29x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 469 ms: 1.55x faster                                       |
| async_tree_io           | 1.77 sec                                               | 1.16 sec: 1.52x faster                                     |
| async_tree_memoization  | 870 ms                                                 | 575 ms: 1.51x faster                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 713 ms: 1.43x faster                                       |
| Geometric mean          | (ref)                                                  | 1.50x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 154 ms                                                 | 94.3 ms: 1.63x faster                                      |
| float          | 117 ms                                                 | 80.4 ms: 1.46x faster                                      |
| pidigits       | 191 ms                                                 | 197 ms: 1.03x slower                                       |
| Geometric mean | (ref)                                                  | 1.32x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 144 ms: 1.31x faster                                       |
| regex_v8       | 27.8 ms                                                | 22.9 ms: 1.21x faster                                      |
| regex_dna      | 227 ms                                                 | 200 ms: 1.13x faster                                       |
| regex_effbot   | 3.63 ms                                                | 3.56 ms: 1.02x faster                                      |
| Geometric mean | (ref)                                                  | 1.16x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 312 us: 1.55x faster                                       |
| unpickle_pure_python | 331 us                                                 | 215 us: 1.54x faster                                       |
| tomli_loads          | 3.14 sec                                               | 2.17 sec: 1.45x faster                                     |
| json_dumps           | 14.2 ms                                                | 9.79 ms: 1.45x faster                                      |
| xml_etree_process    | 79.1 ms                                                | 59.2 ms: 1.34x faster                                      |
| json_loads           | 31.2 us                                                | 25.0 us: 1.25x faster                                      |
| xml_etree_generate   | 99.4 ms                                                | 85.4 ms: 1.16x faster                                      |
| pickle_list          | 5.08 us                                                | 4.49 us: 1.13x faster                                      |
| xml_etree_iterparse  | 115 ms                                                 | 103 ms: 1.12x faster                                       |
| xml_etree_parse      | 168 ms                                                 | 152 ms: 1.11x faster                                       |
| unpickle_list        | 5.20 us                                                | 4.96 us: 1.05x faster                                      |
| pickle               | 10.7 us                                                | 11.0 us: 1.03x slower                                      |
| unpickle             | 14.4 us                                                | 14.9 us: 1.03x slower                                      |
| pickle_dict          | 29.6 us                                                | 31.8 us: 1.07x slower                                      |
| Geometric mean       | (ref)                                                  | 1.20x faster                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.28 ms: 1.57x faster                                      |
| python_startup_no_site | 5.93 ms                                                | 6.74 ms: 1.14x slower                                      |
| Geometric mean         | (ref)                                                  | 1.18x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.6 ms: 1.54x faster                                      |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 146 us: 3.73x faster                                       |
| generators               | 80.1 ms                                                | 30.3 ms: 2.64x faster                                      |
| deltablue                | 7.91 ms                                                | 3.50 ms: 2.26x faster                                      |
| richards_super           | 94.7 ms                                                | 49.2 ms: 1.93x faster                                      |
| logging_silent           | 190 ns                                                 | 99.7 ns: 1.90x faster                                      |
| richards                 | 79.3 ms                                                | 43.8 ms: 1.81x faster                                      |
| chaos                    | 115 ms                                                 | 63.8 ms: 1.81x faster                                      |
| asyncio_tcp              | 922 ms                                                 | 513 ms: 1.80x faster                                       |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.77x faster                                       |
| go                       | 240 ms                                                 | 137 ms: 1.76x faster                                       |
| raytrace                 | 507 ms                                                 | 298 ms: 1.70x faster                                       |
| hexiom                   | 10.4 ms                                                | 6.13 ms: 1.70x faster                                      |
| scimark_monte_carlo      | 118 ms                                                 | 71.2 ms: 1.66x faster                                      |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.64x faster                                      |
| crypto_pyaes             | 128 ms                                                 | 78.1 ms: 1.64x faster                                      |
| nbody                    | 154 ms                                                 | 94.3 ms: 1.63x faster                                      |
| spectral_norm            | 170 ms                                                 | 106 ms: 1.60x faster                                       |
| coroutines               | 35.1 ms                                                | 22.2 ms: 1.58x faster                                      |
| pyflate                  | 716 ms                                                 | 453 ms: 1.58x faster                                       |
| python_startup           | 14.6 ms                                                | 9.28 ms: 1.57x faster                                      |
| scimark_lu               | 176 ms                                                 | 112 ms: 1.57x faster                                       |
| sqlglot_transpile        | 2.57 ms                                                | 1.64 ms: 1.57x faster                                      |
| pickle_pure_python       | 484 us                                                 | 312 us: 1.55x faster                                       |
| async_tree_none          | 728 ms                                                 | 469 ms: 1.55x faster                                       |
| mako                     | 16.3 ms                                                | 10.6 ms: 1.54x faster                                      |
| unpickle_pure_python     | 331 us                                                 | 215 us: 1.54x faster                                       |
| deepcopy_memo            | 58.5 us                                                | 38.3 us: 1.53x faster                                      |
| async_tree_io            | 1.77 sec                                               | 1.16 sec: 1.52x faster                                     |
| async_tree_memoization   | 870 ms                                                 | 575 ms: 1.51x faster                                       |
| float                    | 117 ms                                                 | 80.4 ms: 1.46x faster                                      |
| tomli_loads              | 3.14 sec                                               | 2.17 sec: 1.45x faster                                     |
| json_dumps               | 14.2 ms                                                | 9.79 ms: 1.45x faster                                      |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.43x faster                                     |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 713 ms: 1.43x faster                                       |
| pprint_pformat           | 2.10 sec                                               | 1.50 sec: 1.40x faster                                     |
| pprint_safe_repr         | 1.02 sec                                               | 734 ms: 1.39x faster                                       |
| comprehensions           | 28.8 us                                                | 20.7 us: 1.39x faster                                      |
| tornado_http             | 136 ms                                                 | 99.3 ms: 1.37x faster                                      |
| fannkuch                 | 532 ms                                                 | 387 ms: 1.37x faster                                       |
| pycparser                | 1.58 sec                                               | 1.16 sec: 1.36x faster                                     |
| xml_etree_process        | 79.1 ms                                                | 59.2 ms: 1.34x faster                                      |
| deepcopy                 | 479 us                                                 | 359 us: 1.34x faster                                       |
| deepcopy_reduce          | 4.17 us                                                | 3.12 us: 1.33x faster                                      |
| logging_simple           | 8.30 us                                                | 6.25 us: 1.33x faster                                      |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.88 ms: 1.33x faster                                      |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.32x faster                                       |
| nqueens                  | 106 ms                                                 | 80.5 ms: 1.31x faster                                      |
| regex_compile            | 188 ms                                                 | 144 ms: 1.31x faster                                       |
| 2to3                     | 348 ms                                                 | 267 ms: 1.30x faster                                       |
| logging_format           | 9.09 us                                                | 6.99 us: 1.30x faster                                      |
| scimark_fft              | 466 ms                                                 | 358 ms: 1.30x faster                                       |
| sqlglot_optimize         | 69.2 ms                                                | 53.5 ms: 1.29x faster                                      |
| sqlalchemy_imperative    | 23.3 ms                                                | 18.4 ms: 1.27x faster                                      |
| unpack_sequence          | 60.0 ns                                                | 47.4 ns: 1.27x faster                                      |
| json_loads               | 31.2 us                                                | 25.0 us: 1.25x faster                                      |
| dulwich_log              | 84.3 ms                                                | 67.9 ms: 1.24x faster                                      |
| docutils                 | 3.30 sec                                               | 2.72 sec: 1.21x faster                                     |
| regex_v8                 | 27.8 ms                                                | 22.9 ms: 1.21x faster                                      |
| json                     | 5.69 ms                                                | 4.74 ms: 1.20x faster                                      |
| bench_thread_pool        | 986 us                                                 | 827 us: 1.19x faster                                       |
| sqlalchemy_declarative   | 172 ms                                                 | 145 ms: 1.19x faster                                       |
| xml_etree_generate       | 99.4 ms                                                | 85.4 ms: 1.16x faster                                      |
| meteor_contest           | 120 ms                                                 | 106 ms: 1.13x faster                                       |
| regex_dna                | 227 ms                                                 | 200 ms: 1.13x faster                                       |
| pickle_list              | 5.08 us                                                | 4.49 us: 1.13x faster                                      |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.12x faster                                      |
| xml_etree_iterparse      | 115 ms                                                 | 103 ms: 1.12x faster                                       |
| xml_etree_parse          | 168 ms                                                 | 152 ms: 1.11x faster                                       |
| sqlite_synth             | 3.02 us                                                | 2.75 us: 1.10x faster                                      |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                      |
| mdp                      | 2.85 sec                                               | 2.64 sec: 1.08x faster                                     |
| telco                    | 7.27 ms                                                | 6.82 ms: 1.06x faster                                      |
| unpickle_list            | 5.20 us                                                | 4.96 us: 1.05x faster                                      |
| regex_effbot             | 3.63 ms                                                | 3.56 ms: 1.02x faster                                      |
| pickle                   | 10.7 us                                                | 11.0 us: 1.03x slower                                      |
| pidigits                 | 191 ms                                                 | 197 ms: 1.03x slower                                       |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.03x slower                                      |
| pickle_dict              | 29.6 us                                                | 31.8 us: 1.07x slower                                      |
| gc_traversal             | 3.62 ms                                                | 4.07 ms: 1.12x slower                                      |
| python_startup_no_site   | 5.93 ms                                                | 6.74 ms: 1.14x slower                                      |
| coverage                 | 79.4 ms                                                | 95.0 ms: 1.20x slower                                      |
| dask                     | 441 ms                                                 | 536 ms: 1.22x slower                                       |
| Geometric mean           | (ref)                                                  | 1.35x faster                                               |

Benchmark hidden because not significant (2): bench_mp_pool, async_generators
Ignored benchmarks (17) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.31x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.17x