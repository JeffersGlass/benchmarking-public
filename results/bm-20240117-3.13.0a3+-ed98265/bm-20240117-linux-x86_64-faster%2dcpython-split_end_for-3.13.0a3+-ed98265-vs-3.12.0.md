
# Results vs. 3.12.0

- fork: faster-cpython
- ref: split_end_for
- machine: linux-x86_64
- commit hash: ed98265
- commit date: 2024-01-17
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 264 ms: 1.04x faster                                                      |
| chameleon      | 7.41 ms                                                | 6.74 ms: 1.10x faster                                                     |
| docutils       | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                    |
| tornado_http   | 103 ms                                                 | 94.1 ms: 1.09x faster                                                     |
| Geometric mean | (ref)                                                  | 1.07x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 435 ms: 1.08x faster                                                      |
| async_tree_memoization  | 578 ms                                                 | 563 ms: 1.03x faster                                                      |
| async_tree_cpu_io_mixed | 726 ms                                                 | 708 ms: 1.02x faster                                                      |
| async_tree_none_tg      | 450 ms                                                 | 439 ms: 1.02x faster                                                      |
| async_tree_io_tg        | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                    |
| async_tree_io           | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                    |
| Geometric mean          | (ref)                                                  | 1.02x faster                                                              |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 86.6 ms: 1.12x faster                                                     |
| float          | 84.7 ms                                                | 79.2 ms: 1.07x faster                                                     |
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                                      |
| Geometric mean | (ref)                                                  | 1.06x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 129 ms: 1.15x faster                                                      |
| regex_effbot   | 3.61 ms                                                | 3.71 ms: 1.03x slower                                                     |
| regex_dna      | 212 ms                                                 | 223 ms: 1.05x slower                                                      |
| regex_v8       | 23.1 ms                                                | 25.5 ms: 1.10x slower                                                     |
| Geometric mean | (ref)                                                  | 1.01x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.11 sec: 1.11x faster                                                    |
| pickle_pure_python   | 324 us                                                 | 297 us: 1.09x faster                                                      |
| unpickle_pure_python | 230 us                                                 | 211 us: 1.09x faster                                                      |
| xml_etree_process    | 61.7 ms                                                | 58.5 ms: 1.05x faster                                                     |
| xml_etree_generate   | 89.2 ms                                                | 85.7 ms: 1.04x faster                                                     |
| unpickle_list        | 5.29 us                                                | 5.16 us: 1.02x faster                                                     |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.02x faster                                                      |
| pickle_dict          | 35.5 us                                                | 34.9 us: 1.02x faster                                                     |
| json_loads           | 28.5 us                                                | 28.1 us: 1.01x faster                                                     |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                      |
| json_dumps           | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                     |
| pickle               | 11.6 us                                                | 11.8 us: 1.02x slower                                                     |
| pickle_list          | 5.08 us                                                | 5.25 us: 1.03x slower                                                     |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                              |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                     |
| python_startup_no_site | 6.94 ms                                                | 8.69 ms: 1.25x slower                                                     |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.2 ms: 1.07x faster                                                     |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 110 us: 1.43x faster                                                      |
| comprehensions           | 21.8 us                                                | 16.2 us: 1.34x faster                                                     |
| unpack_sequence          | 54.0 ns                                                | 44.3 ns: 1.22x faster                                                     |
| raytrace                 | 312 ms                                                 | 258 ms: 1.21x faster                                                      |
| logging_format           | 7.23 us                                                | 6.20 us: 1.17x faster                                                     |
| deltablue                | 3.72 ms                                                | 3.22 ms: 1.15x faster                                                     |
| regex_compile            | 148 ms                                                 | 129 ms: 1.15x faster                                                      |
| sympy_sum                | 169 ms                                                 | 147 ms: 1.15x faster                                                      |
| logging_simple           | 6.46 us                                                | 5.65 us: 1.14x faster                                                     |
| crypto_pyaes             | 81.9 ms                                                | 71.7 ms: 1.14x faster                                                     |
| chaos                    | 67.0 ms                                                | 58.8 ms: 1.14x faster                                                     |
| scimark_monte_carlo      | 75.1 ms                                                | 66.2 ms: 1.13x faster                                                     |
| nbody                    | 97.0 ms                                                | 86.6 ms: 1.12x faster                                                     |
| tomli_loads              | 2.33 sec                                               | 2.11 sec: 1.11x faster                                                    |
| chameleon                | 7.41 ms                                                | 6.74 ms: 1.10x faster                                                     |
| sympy_integrate          | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                     |
| sqlglot_parse            | 1.36 ms                                                | 1.24 ms: 1.10x faster                                                     |
| gc_traversal             | 3.79 ms                                                | 3.47 ms: 1.09x faster                                                     |
| deepcopy_reduce          | 3.35 us                                                | 3.06 us: 1.09x faster                                                     |
| sympy_str                | 300 ms                                                 | 275 ms: 1.09x faster                                                      |
| tornado_http             | 103 ms                                                 | 94.1 ms: 1.09x faster                                                     |
| pickle_pure_python       | 324 us                                                 | 297 us: 1.09x faster                                                      |
| unpickle_pure_python     | 230 us                                                 | 211 us: 1.09x faster                                                      |
| async_tree_none          | 472 ms                                                 | 435 ms: 1.08x faster                                                      |
| pprint_safe_repr         | 776 ms                                                 | 717 ms: 1.08x faster                                                      |
| sqlglot_transpile        | 1.68 ms                                                | 1.56 ms: 1.08x faster                                                     |
| pyflate                  | 482 ms                                                 | 448 ms: 1.08x faster                                                      |
| deepcopy                 | 371 us                                                 | 345 us: 1.07x faster                                                      |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.71 ms: 1.07x faster                                                     |
| deepcopy_memo            | 40.7 us                                                | 37.9 us: 1.07x faster                                                     |
| hexiom                   | 6.41 ms                                                | 5.97 ms: 1.07x faster                                                     |
| float                    | 84.7 ms                                                | 79.2 ms: 1.07x faster                                                     |
| pathlib                  | 19.3 ms                                                | 18.1 ms: 1.07x faster                                                     |
| pprint_pformat           | 1.57 sec                                               | 1.47 sec: 1.07x faster                                                    |
| mako                     | 11.9 ms                                                | 11.2 ms: 1.07x faster                                                     |
| scimark_lu               | 118 ms                                                 | 111 ms: 1.06x faster                                                      |
| generators               | 31.2 ms                                                | 29.5 ms: 1.06x faster                                                     |
| docutils                 | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                    |
| dulwich_log              | 68.5 ms                                                | 64.8 ms: 1.06x faster                                                     |
| meteor_contest           | 112 ms                                                 | 106 ms: 1.06x faster                                                      |
| scimark_fft              | 382 ms                                                 | 362 ms: 1.06x faster                                                      |
| xml_etree_process        | 61.7 ms                                                | 58.5 ms: 1.05x faster                                                     |
| async_generators         | 463 ms                                                 | 443 ms: 1.04x faster                                                      |
| xml_etree_generate       | 89.2 ms                                                | 85.7 ms: 1.04x faster                                                     |
| mdp                      | 2.63 sec                                               | 2.53 sec: 1.04x faster                                                    |
| logging_silent           | 104 ns                                                 | 101 ns: 1.04x faster                                                      |
| 2to3                     | 274 ms                                                 | 264 ms: 1.04x faster                                                      |
| fannkuch                 | 417 ms                                                 | 403 ms: 1.04x faster                                                      |
| sqlglot_normalize        | 110 ms                                                 | 107 ms: 1.03x faster                                                      |
| dask                     | 372 ms                                                 | 361 ms: 1.03x faster                                                      |
| nqueens                  | 83.3 ms                                                | 80.8 ms: 1.03x faster                                                     |
| spectral_norm            | 115 ms                                                 | 112 ms: 1.03x faster                                                      |
| sympy_expand             | 478 ms                                                 | 465 ms: 1.03x faster                                                      |
| json                     | 5.26 ms                                                | 5.12 ms: 1.03x faster                                                     |
| async_tree_memoization   | 578 ms                                                 | 563 ms: 1.03x faster                                                      |
| coroutines               | 23.2 ms                                                | 22.6 ms: 1.03x faster                                                     |
| unpickle_list            | 5.29 us                                                | 5.16 us: 1.02x faster                                                     |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 708 ms: 1.02x faster                                                      |
| async_tree_none_tg       | 450 ms                                                 | 439 ms: 1.02x faster                                                      |
| bench_thread_pool        | 842 us                                                 | 823 us: 1.02x faster                                                      |
| xml_etree_iterparse      | 107 ms                                                 | 105 ms: 1.02x faster                                                      |
| go                       | 139 ms                                                 | 137 ms: 1.02x faster                                                      |
| pickle_dict              | 35.5 us                                                | 34.9 us: 1.02x faster                                                     |
| sqlglot_optimize         | 54.8 ms                                                | 53.8 ms: 1.02x faster                                                     |
| asyncio_tcp              | 491 ms                                                 | 482 ms: 1.02x faster                                                      |
| json_loads               | 28.5 us                                                | 28.1 us: 1.01x faster                                                     |
| xml_etree_parse          | 159 ms                                                 | 158 ms: 1.01x faster                                                      |
| sqlite_synth             | 2.83 us                                                | 2.80 us: 1.01x faster                                                     |
| scimark_sor              | 129 ms                                                 | 128 ms: 1.01x faster                                                      |
| create_gc_cycles         | 1.48 ms                                                | 1.47 ms: 1.00x faster                                                     |
| pidigits                 | 187 ms                                                 | 188 ms: 1.00x slower                                                      |
| json_dumps               | 10.4 ms                                                | 10.5 ms: 1.01x slower                                                     |
| async_tree_io_tg         | 1.18 sec                                               | 1.19 sec: 1.01x slower                                                    |
| pycparser                | 1.18 sec                                               | 1.20 sec: 1.01x slower                                                    |
| pickle                   | 11.6 us                                                | 11.8 us: 1.02x slower                                                     |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                                    |
| regex_effbot             | 3.61 ms                                                | 3.71 ms: 1.03x slower                                                     |
| pickle_list              | 5.08 us                                                | 5.25 us: 1.03x slower                                                     |
| richards                 | 45.8 ms                                                | 47.8 ms: 1.04x slower                                                     |
| richards_super           | 51.5 ms                                                | 53.8 ms: 1.04x slower                                                     |
| regex_dna                | 212 ms                                                 | 223 ms: 1.05x slower                                                      |
| python_startup           | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                     |
| regex_v8                 | 23.1 ms                                                | 25.5 ms: 1.10x slower                                                     |
| telco                    | 7.10 ms                                                | 8.43 ms: 1.19x slower                                                     |
| python_startup_no_site   | 6.94 ms                                                | 8.69 ms: 1.25x slower                                                     |
| coverage                 | 72.7 ms                                                | 95.5 ms: 1.31x slower                                                     |
| Geometric mean           | (ref)                                                  | 1.04x faster                                                              |

Benchmark hidden because not significant (7): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, asyncio_websockets, asyncio_tcp_ssl, bench_mp_pool, unpickle, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.93x