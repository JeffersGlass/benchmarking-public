
# Results vs. 3.12.0

- fork: faster-cpython
- ref: guarantee_forward_pr
- machine: linux-x86_64
- commit hash: 1501bca
- commit date: 2024-01-08
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 263 ms: 1.04x faster                                                             |
| chameleon      | 7.41 ms                                                | 6.89 ms: 1.08x faster                                                            |
| docutils       | 2.77 sec                                               | 2.58 sec: 1.07x faster                                                           |
| tornado_http   | 103 ms                                                 | 93.8 ms: 1.09x faster                                                            |
| Geometric mean | (ref)                                                  | 1.07x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 435 ms: 1.08x faster                                                             |
| async_tree_memoization  | 578 ms                                                 | 556 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed | 726 ms                                                 | 704 ms: 1.03x faster                                                             |
| async_tree_none_tg      | 450 ms                                                 | 440 ms: 1.02x faster                                                             |
| async_tree_io_tg        | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                           |
| async_tree_io           | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                           |
| Geometric mean          | (ref)                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.8 ms: 1.09x faster                                                            |
| float          | 84.7 ms                                                | 80.1 ms: 1.06x faster                                                            |
| pidigits       | 187 ms                                                 | 195 ms: 1.04x slower                                                             |
| Geometric mean | (ref)                                                  | 1.04x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 129 ms: 1.15x faster                                                             |
| regex_effbot   | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                            |
| regex_dna      | 212 ms                                                 | 219 ms: 1.03x slower                                                             |
| regex_v8       | 23.1 ms                                                | 26.0 ms: 1.12x slower                                                            |
| Geometric mean | (ref)                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.12 sec: 1.10x faster                                                           |
| pickle_pure_python   | 324 us                                                 | 299 us: 1.08x faster                                                             |
| unpickle_pure_python | 230 us                                                 | 214 us: 1.08x faster                                                             |
| unpickle             | 15.9 us                                                | 14.9 us: 1.07x faster                                                            |
| pickle_list          | 5.08 us                                                | 4.89 us: 1.04x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 59.4 ms: 1.04x faster                                                            |
| xml_etree_generate   | 89.2 ms                                                | 86.0 ms: 1.04x faster                                                            |
| unpickle_list        | 5.29 us                                                | 5.11 us: 1.04x faster                                                            |
| pickle               | 11.6 us                                                | 11.4 us: 1.02x faster                                                            |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.02x faster                                                             |
| pickle_dict          | 35.5 us                                                | 35.1 us: 1.01x faster                                                            |
| json_loads           | 28.5 us                                                | 28.7 us: 1.01x slower                                                            |
| json_dumps           | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                                     |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.73 ms: 1.26x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.1 ms: 1.07x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 110 us: 1.44x faster                                                             |
| comprehensions           | 21.8 us                                                | 16.1 us: 1.35x faster                                                            |
| raytrace                 | 312 ms                                                 | 261 ms: 1.19x faster                                                             |
| unpack_sequence          | 54.0 ns                                                | 45.2 ns: 1.19x faster                                                            |
| logging_format           | 7.23 us                                                | 6.13 us: 1.18x faster                                                            |
| logging_simple           | 6.46 us                                                | 5.57 us: 1.16x faster                                                            |
| deltablue                | 3.72 ms                                                | 3.20 ms: 1.16x faster                                                            |
| crypto_pyaes             | 81.9 ms                                                | 70.6 ms: 1.16x faster                                                            |
| sympy_sum                | 169 ms                                                 | 147 ms: 1.15x faster                                                             |
| regex_compile            | 148 ms                                                 | 129 ms: 1.15x faster                                                             |
| chaos                    | 67.0 ms                                                | 58.7 ms: 1.14x faster                                                            |
| sympy_str                | 300 ms                                                 | 268 ms: 1.12x faster                                                             |
| sympy_integrate          | 21.4 ms                                                | 19.3 ms: 1.11x faster                                                            |
| scimark_monte_carlo      | 75.1 ms                                                | 68.0 ms: 1.10x faster                                                            |
| tomli_loads              | 2.33 sec                                               | 2.12 sec: 1.10x faster                                                           |
| tornado_http             | 103 ms                                                 | 93.8 ms: 1.09x faster                                                            |
| sqlglot_parse            | 1.36 ms                                                | 1.24 ms: 1.09x faster                                                            |
| nbody                    | 97.0 ms                                                | 88.8 ms: 1.09x faster                                                            |
| async_tree_none          | 472 ms                                                 | 435 ms: 1.08x faster                                                             |
| pickle_pure_python       | 324 us                                                 | 299 us: 1.08x faster                                                             |
| sqlglot_transpile        | 1.68 ms                                                | 1.56 ms: 1.08x faster                                                            |
| unpickle_pure_python     | 230 us                                                 | 214 us: 1.08x faster                                                             |
| chameleon                | 7.41 ms                                                | 6.89 ms: 1.08x faster                                                            |
| mako                     | 11.9 ms                                                | 11.1 ms: 1.07x faster                                                            |
| deepcopy                 | 371 us                                                 | 346 us: 1.07x faster                                                             |
| docutils                 | 2.77 sec                                               | 2.58 sec: 1.07x faster                                                           |
| deepcopy_reduce          | 3.35 us                                                | 3.13 us: 1.07x faster                                                            |
| generators               | 31.2 ms                                                | 29.2 ms: 1.07x faster                                                            |
| pyflate                  | 482 ms                                                 | 452 ms: 1.07x faster                                                             |
| unpickle                 | 15.9 us                                                | 14.9 us: 1.07x faster                                                            |
| deepcopy_memo            | 40.7 us                                                | 38.4 us: 1.06x faster                                                            |
| fannkuch                 | 417 ms                                                 | 394 ms: 1.06x faster                                                             |
| async_generators         | 463 ms                                                 | 437 ms: 1.06x faster                                                             |
| float                    | 84.7 ms                                                | 80.1 ms: 1.06x faster                                                            |
| scimark_fft              | 382 ms                                                 | 362 ms: 1.05x faster                                                             |
| coroutines               | 23.2 ms                                                | 22.0 ms: 1.05x faster                                                            |
| hexiom                   | 6.41 ms                                                | 6.09 ms: 1.05x faster                                                            |
| sympy_expand             | 478 ms                                                 | 454 ms: 1.05x faster                                                             |
| pathlib                  | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                            |
| pprint_safe_repr         | 776 ms                                                 | 739 ms: 1.05x faster                                                             |
| pprint_pformat           | 1.57 sec                                               | 1.50 sec: 1.05x faster                                                           |
| dulwich_log              | 68.5 ms                                                | 65.5 ms: 1.05x faster                                                            |
| sqlglot_normalize        | 110 ms                                                 | 106 ms: 1.04x faster                                                             |
| meteor_contest           | 112 ms                                                 | 108 ms: 1.04x faster                                                             |
| 2to3                     | 274 ms                                                 | 263 ms: 1.04x faster                                                             |
| nqueens                  | 83.3 ms                                                | 80.0 ms: 1.04x faster                                                            |
| scimark_lu               | 118 ms                                                 | 113 ms: 1.04x faster                                                             |
| pickle_list              | 5.08 us                                                | 4.89 us: 1.04x faster                                                            |
| xml_etree_process        | 61.7 ms                                                | 59.4 ms: 1.04x faster                                                            |
| async_tree_memoization   | 578 ms                                                 | 556 ms: 1.04x faster                                                             |
| xml_etree_generate       | 89.2 ms                                                | 86.0 ms: 1.04x faster                                                            |
| unpickle_list            | 5.29 us                                                | 5.11 us: 1.04x faster                                                            |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 704 ms: 1.03x faster                                                             |
| dask                     | 372 ms                                                 | 361 ms: 1.03x faster                                                             |
| sqlglot_optimize         | 54.8 ms                                                | 53.4 ms: 1.03x faster                                                            |
| spectral_norm            | 115 ms                                                 | 112 ms: 1.02x faster                                                             |
| async_tree_none_tg       | 450 ms                                                 | 440 ms: 1.02x faster                                                             |
| asyncio_tcp              | 491 ms                                                 | 481 ms: 1.02x faster                                                             |
| bench_thread_pool        | 842 us                                                 | 826 us: 1.02x faster                                                             |
| pickle                   | 11.6 us                                                | 11.4 us: 1.02x faster                                                            |
| go                       | 139 ms                                                 | 137 ms: 1.02x faster                                                             |
| xml_etree_iterparse      | 107 ms                                                 | 105 ms: 1.02x faster                                                             |
| scimark_sor              | 129 ms                                                 | 127 ms: 1.01x faster                                                             |
| pickle_dict              | 35.5 us                                                | 35.1 us: 1.01x faster                                                            |
| mdp                      | 2.63 sec                                               | 2.60 sec: 1.01x faster                                                           |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.00 ms: 1.01x faster                                                            |
| logging_silent           | 104 ns                                                 | 104 ns: 1.01x faster                                                             |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.78 sec: 1.00x faster                                                           |
| gc_traversal             | 3.79 ms                                                | 3.81 ms: 1.00x slower                                                            |
| async_tree_io_tg         | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                           |
| json_loads               | 28.5 us                                                | 28.7 us: 1.01x slower                                                            |
| create_gc_cycles         | 1.48 ms                                                | 1.49 ms: 1.01x slower                                                            |
| regex_effbot             | 3.61 ms                                                | 3.65 ms: 1.01x slower                                                            |
| async_tree_io            | 1.16 sec                                               | 1.17 sec: 1.01x slower                                                           |
| pycparser                | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                           |
| sqlite_synth             | 2.83 us                                                | 2.88 us: 1.02x slower                                                            |
| regex_dna                | 212 ms                                                 | 219 ms: 1.03x slower                                                             |
| json_dumps               | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                            |
| richards                 | 45.8 ms                                                | 47.6 ms: 1.04x slower                                                            |
| pidigits                 | 187 ms                                                 | 195 ms: 1.04x slower                                                             |
| richards_super           | 51.5 ms                                                | 54.5 ms: 1.06x slower                                                            |
| python_startup           | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                            |
| regex_v8                 | 23.1 ms                                                | 26.0 ms: 1.12x slower                                                            |
| telco                    | 7.10 ms                                                | 8.41 ms: 1.19x slower                                                            |
| python_startup_no_site   | 6.94 ms                                                | 8.73 ms: 1.26x slower                                                            |
| coverage                 | 72.7 ms                                                | 94.7 ms: 1.30x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.04x faster                                                                     |

Benchmark hidden because not significant (7): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, xml_etree_parse, bench_mp_pool, json, asyncio_websockets, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.93x