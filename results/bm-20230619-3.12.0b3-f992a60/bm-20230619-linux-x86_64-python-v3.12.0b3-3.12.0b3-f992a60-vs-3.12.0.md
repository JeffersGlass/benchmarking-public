
# Results vs. 3.12.0

- fork: python
- ref: v3.12.0b3
- machine: linux-x86_64
- commit hash: f992a60
- commit date: 2023-06-19
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 267 ms: 1.03x faster                                       |
| docutils       | 2.77 sec                                               | 2.72 sec: 1.02x faster                                     |
| tornado_http   | 103 ms                                                 | 99.3 ms: 1.03x faster                                      |
| Geometric mean | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 713 ms: 1.02x faster                                       |
| async_tree_io           | 1.16 sec                                               | 1.16 sec: 1.00x slower                                     |
| Geometric mean          | (ref)                                                  | 1.01x faster                                               |

Benchmark hidden because not significant (2): async_tree_none, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| float          | 84.7 ms                                                | 80.4 ms: 1.05x faster                                      |
| nbody          | 97.0 ms                                                | 94.3 ms: 1.03x faster                                      |
| pidigits       | 187 ms                                                 | 197 ms: 1.05x slower                                       |
| Geometric mean | (ref)                                                  | 1.01x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_dna      | 212 ms                                                 | 200 ms: 1.06x faster                                       |
| regex_compile  | 148 ms                                                 | 144 ms: 1.03x faster                                       |
| regex_effbot   | 3.61 ms                                                | 3.56 ms: 1.01x faster                                      |
| regex_v8       | 23.1 ms                                                | 22.9 ms: 1.01x faster                                      |
| Geometric mean | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_loads           | 28.5 us                                                | 25.0 us: 1.14x faster                                      |
| pickle_list          | 5.08 us                                                | 4.49 us: 1.13x faster                                      |
| pickle_dict          | 35.5 us                                                | 31.8 us: 1.12x faster                                      |
| tomli_loads          | 2.33 sec                                               | 2.17 sec: 1.07x faster                                     |
| unpickle_pure_python | 230 us                                                 | 215 us: 1.07x faster                                       |
| unpickle_list        | 5.29 us                                                | 4.96 us: 1.07x faster                                      |
| unpickle             | 15.9 us                                                | 14.9 us: 1.07x faster                                      |
| json_dumps           | 10.4 ms                                                | 9.79 ms: 1.06x faster                                      |
| pickle               | 11.6 us                                                | 11.0 us: 1.06x faster                                      |
| xml_etree_parse      | 159 ms                                                 | 152 ms: 1.05x faster                                       |
| xml_etree_process    | 61.7 ms                                                | 59.2 ms: 1.04x faster                                      |
| xml_etree_generate   | 89.2 ms                                                | 85.4 ms: 1.04x faster                                      |
| pickle_pure_python   | 324 us                                                 | 312 us: 1.04x faster                                       |
| xml_etree_iterparse  | 107 ms                                                 | 103 ms: 1.04x faster                                       |
| Geometric mean       | (ref)                                                  | 1.07x faster                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 9.28 ms: 1.03x faster                                      |
| python_startup_no_site | 6.94 ms                                                | 6.74 ms: 1.03x faster                                      |
| Geometric mean         | (ref)                                                  | 1.03x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 11.9 ms                                                | 10.6 ms: 1.12x faster                                      |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230619-linux-x86_64-python-v3.12.0b3-3.12.0b3-f992a60 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| unpack_sequence          | 54.0 ns                                                | 47.4 ns: 1.14x faster                                      |
| json_loads               | 28.5 us                                                | 25.0 us: 1.14x faster                                      |
| pickle_list              | 5.08 us                                                | 4.49 us: 1.13x faster                                      |
| mako                     | 11.9 ms                                                | 10.6 ms: 1.12x faster                                      |
| pickle_dict              | 35.5 us                                                | 31.8 us: 1.12x faster                                      |
| json                     | 5.26 ms                                                | 4.74 ms: 1.11x faster                                      |
| spectral_norm            | 115 ms                                                 | 106 ms: 1.08x faster                                       |
| typing_runtime_protocols | 158 us                                                 | 146 us: 1.08x faster                                       |
| fannkuch                 | 417 ms                                                 | 387 ms: 1.08x faster                                       |
| tomli_loads              | 2.33 sec                                               | 2.17 sec: 1.07x faster                                     |
| deepcopy_reduce          | 3.35 us                                                | 3.12 us: 1.07x faster                                      |
| unpickle_pure_python     | 230 us                                                 | 215 us: 1.07x faster                                       |
| scimark_fft              | 382 ms                                                 | 358 ms: 1.07x faster                                       |
| unpickle_list            | 5.29 us                                                | 4.96 us: 1.07x faster                                      |
| unpickle                 | 15.9 us                                                | 14.9 us: 1.07x faster                                      |
| pyflate                  | 482 ms                                                 | 453 ms: 1.06x faster                                       |
| meteor_contest           | 112 ms                                                 | 106 ms: 1.06x faster                                       |
| deepcopy_memo            | 40.7 us                                                | 38.3 us: 1.06x faster                                      |
| pathlib                  | 19.3 ms                                                | 18.2 ms: 1.06x faster                                      |
| deltablue                | 3.72 ms                                                | 3.50 ms: 1.06x faster                                      |
| json_dumps               | 10.4 ms                                                | 9.79 ms: 1.06x faster                                      |
| regex_dna                | 212 ms                                                 | 200 ms: 1.06x faster                                       |
| pickle                   | 11.6 us                                                | 11.0 us: 1.06x faster                                      |
| pprint_safe_repr         | 776 ms                                                 | 734 ms: 1.06x faster                                       |
| scimark_monte_carlo      | 75.1 ms                                                | 71.2 ms: 1.05x faster                                      |
| float                    | 84.7 ms                                                | 80.4 ms: 1.05x faster                                      |
| xml_etree_parse          | 159 ms                                                 | 152 ms: 1.05x faster                                       |
| scimark_lu               | 118 ms                                                 | 112 ms: 1.05x faster                                       |
| comprehensions           | 21.8 us                                                | 20.7 us: 1.05x faster                                      |
| chaos                    | 67.0 ms                                                | 63.8 ms: 1.05x faster                                      |
| crypto_pyaes             | 81.9 ms                                                | 78.1 ms: 1.05x faster                                      |
| logging_silent           | 104 ns                                                 | 99.7 ns: 1.05x faster                                      |
| richards                 | 45.8 ms                                                | 43.8 ms: 1.05x faster                                      |
| richards_super           | 51.5 ms                                                | 49.2 ms: 1.05x faster                                      |
| raytrace                 | 312 ms                                                 | 298 ms: 1.05x faster                                       |
| hexiom                   | 6.41 ms                                                | 6.13 ms: 1.05x faster                                      |
| coroutines               | 23.2 ms                                                | 22.2 ms: 1.05x faster                                      |
| pprint_pformat           | 1.57 sec                                               | 1.50 sec: 1.04x faster                                     |
| async_generators         | 463 ms                                                 | 444 ms: 1.04x faster                                       |
| xml_etree_process        | 61.7 ms                                                | 59.2 ms: 1.04x faster                                      |
| xml_etree_generate       | 89.2 ms                                                | 85.4 ms: 1.04x faster                                      |
| scimark_sor              | 129 ms                                                 | 124 ms: 1.04x faster                                       |
| telco                    | 7.10 ms                                                | 6.82 ms: 1.04x faster                                      |
| pickle_pure_python       | 324 us                                                 | 312 us: 1.04x faster                                       |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.88 ms: 1.04x faster                                      |
| xml_etree_iterparse      | 107 ms                                                 | 103 ms: 1.04x faster                                       |
| logging_format           | 7.23 us                                                | 6.99 us: 1.03x faster                                      |
| nqueens                  | 83.3 ms                                                | 80.5 ms: 1.03x faster                                      |
| deepcopy                 | 371 us                                                 | 359 us: 1.03x faster                                       |
| logging_simple           | 6.46 us                                                | 6.25 us: 1.03x faster                                      |
| tornado_http             | 103 ms                                                 | 99.3 ms: 1.03x faster                                      |
| sqlite_synth             | 2.83 us                                                | 2.75 us: 1.03x faster                                      |
| generators               | 31.2 ms                                                | 30.3 ms: 1.03x faster                                      |
| python_startup           | 9.55 ms                                                | 9.28 ms: 1.03x faster                                      |
| python_startup_no_site   | 6.94 ms                                                | 6.74 ms: 1.03x faster                                      |
| nbody                    | 97.0 ms                                                | 94.3 ms: 1.03x faster                                      |
| regex_compile            | 148 ms                                                 | 144 ms: 1.03x faster                                       |
| sqlglot_parse            | 1.36 ms                                                | 1.33 ms: 1.03x faster                                      |
| 2to3                     | 274 ms                                                 | 267 ms: 1.03x faster                                       |
| sqlglot_transpile        | 1.68 ms                                                | 1.64 ms: 1.03x faster                                      |
| sqlglot_optimize         | 54.8 ms                                                | 53.5 ms: 1.02x faster                                      |
| go                       | 139 ms                                                 | 137 ms: 1.02x faster                                       |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 713 ms: 1.02x faster                                       |
| bench_thread_pool        | 842 us                                                 | 827 us: 1.02x faster                                       |
| docutils                 | 2.77 sec                                               | 2.72 sec: 1.02x faster                                     |
| sqlalchemy_imperative    | 18.7 ms                                                | 18.4 ms: 1.02x faster                                      |
| pycparser                | 1.18 sec                                               | 1.16 sec: 1.02x faster                                     |
| sqlalchemy_declarative   | 147 ms                                                 | 145 ms: 1.02x faster                                       |
| sqlglot_normalize        | 110 ms                                                 | 109 ms: 1.02x faster                                       |
| regex_effbot             | 3.61 ms                                                | 3.56 ms: 1.01x faster                                      |
| regex_v8                 | 23.1 ms                                                | 22.9 ms: 1.01x faster                                      |
| dulwich_log              | 68.5 ms                                                | 67.9 ms: 1.01x faster                                      |
| async_tree_io            | 1.16 sec                                               | 1.16 sec: 1.00x slower                                     |
| mdp                      | 2.63 sec                                               | 2.64 sec: 1.00x slower                                     |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.79 sec: 1.00x slower                                     |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.01x slower                                      |
| asyncio_tcp              | 491 ms                                                 | 513 ms: 1.04x slower                                       |
| pidigits                 | 187 ms                                                 | 197 ms: 1.05x slower                                       |
| gc_traversal             | 3.79 ms                                                | 4.07 ms: 1.07x slower                                      |
| coverage                 | 72.7 ms                                                | 95.0 ms: 1.31x slower                                      |
| dask                     | 372 ms                                                 | 536 ms: 1.44x slower                                       |
| Geometric mean           | (ref)                                                  | 1.03x faster                                               |

Benchmark hidden because not significant (3): async_tree_none, async_tree_memoization, bench_mp_pool
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, gunicorn, mypy2, sympy_expand, sympy_integrate, sympy_str, sympy_sum


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.01x