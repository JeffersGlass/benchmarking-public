
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 303 ms: 1.06x slower                                                                   |
| chameleon      | 7.23 ms                                                      | 7.67 ms: 1.06x slower                                                                  |
| docutils       | 2.87 sec                                                     | 2.90 sec: 1.01x slower                                                                 |
| tornado_http   | 121 ms                                                       | 126 ms: 1.04x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 434 ms: 1.04x faster                                                                   |
| async_tree_memoization_tg  | 540 ms                                                       | 548 ms: 1.01x slower                                                                   |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 707 ms: 1.01x slower                                                                   |
| async_tree_none_tg         | 431 ms                                                       | 438 ms: 1.02x slower                                                                   |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                                 |
| async_tree_io              | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                                 |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                                           |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 263 ms: 1.01x faster                                                                   |
| float          | 76.6 ms                                                      | 82.1 ms: 1.07x slower                                                                  |
| nbody          | 88.0 ms                                                      | 104 ms: 1.19x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.08x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.59 ms: 1.00x slower                                                                  |
| regex_dna      | 239 ms                                                       | 241 ms: 1.01x slower                                                                   |
| regex_compile  | 144 ms                                                       | 147 ms: 1.02x slower                                                                   |
| regex_v8       | 23.6 ms                                                      | 25.6 ms: 1.08x slower                                                                  |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 31.0 us: 1.05x faster                                                                  |
| pickle_pure_python   | 318 us                                                       | 304 us: 1.05x faster                                                                   |
| pickle_list          | 4.43 us                                                      | 4.37 us: 1.01x faster                                                                  |
| xml_etree_generate   | 86.1 ms                                                      | 85.1 ms: 1.01x faster                                                                  |
| pickle               | 10.5 us                                                      | 10.4 us: 1.01x faster                                                                  |
| xml_etree_process    | 58.4 ms                                                      | 58.6 ms: 1.00x slower                                                                  |
| unpickle             | 14.8 us                                                      | 15.3 us: 1.03x slower                                                                  |
| xml_etree_parse      | 144 ms                                                       | 149 ms: 1.04x slower                                                                   |
| xml_etree_iterparse  | 103 ms                                                       | 107 ms: 1.04x slower                                                                   |
| json_loads           | 24.4 us                                                      | 25.3 us: 1.04x slower                                                                  |
| json_dumps           | 10.2 ms                                                      | 10.7 ms: 1.05x slower                                                                  |
| unpickle_list        | 4.66 us                                                      | 4.95 us: 1.06x slower                                                                  |
| unpickle_pure_python | 210 us                                                       | 224 us: 1.07x slower                                                                   |
| tomli_loads          | 2.16 sec                                                     | 2.34 sec: 1.08x slower                                                                 |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                                  |
| python_startup_no_site | 8.64 ms                                                      | 11.2 ms: 1.29x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.19x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 11.8 ms: 1.18x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 122 us: 1.25x faster                                                                   |
| unpack_sequence            | 53.2 ns                                                      | 43.7 ns: 1.22x faster                                                                  |
| generators                 | 37.4 ms                                                      | 34.4 ms: 1.09x faster                                                                  |
| raytrace                   | 298 ms                                                       | 277 ms: 1.08x faster                                                                   |
| async_generators           | 390 ms                                                       | 368 ms: 1.06x faster                                                                   |
| comprehensions             | 21.9 us                                                      | 20.8 us: 1.05x faster                                                                  |
| pickle_dict                | 32.5 us                                                      | 31.0 us: 1.05x faster                                                                  |
| pickle_pure_python         | 318 us                                                       | 304 us: 1.05x faster                                                                   |
| create_gc_cycles           | 1.59 ms                                                      | 1.52 ms: 1.04x faster                                                                  |
| async_tree_none            | 452 ms                                                       | 434 ms: 1.04x faster                                                                   |
| deepcopy_reduce            | 3.37 us                                                      | 3.28 us: 1.03x faster                                                                  |
| pathlib                    | 18.9 ms                                                      | 18.4 ms: 1.03x faster                                                                  |
| coroutines                 | 23.0 ms                                                      | 22.5 ms: 1.02x faster                                                                  |
| asyncio_tcp                | 378 ms                                                       | 370 ms: 1.02x faster                                                                   |
| gc_traversal               | 3.48 ms                                                      | 3.42 ms: 1.02x faster                                                                  |
| deepcopy                   | 368 us                                                       | 363 us: 1.01x faster                                                                   |
| pickle_list                | 4.43 us                                                      | 4.37 us: 1.01x faster                                                                  |
| xml_etree_generate         | 86.1 ms                                                      | 85.1 ms: 1.01x faster                                                                  |
| pickle                     | 10.5 us                                                      | 10.4 us: 1.01x faster                                                                  |
| asyncio_websockets         | 387 ms                                                       | 383 ms: 1.01x faster                                                                   |
| logging_simple             | 6.71 us                                                      | 6.65 us: 1.01x faster                                                                  |
| mdp                        | 2.57 sec                                                     | 2.55 sec: 1.01x faster                                                                 |
| pidigits                   | 265 ms                                                       | 263 ms: 1.01x faster                                                                   |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.58 sec: 1.01x faster                                                                 |
| xml_etree_process          | 58.4 ms                                                      | 58.6 ms: 1.00x slower                                                                  |
| regex_effbot               | 3.57 ms                                                      | 3.59 ms: 1.00x slower                                                                  |
| sympy_str                  | 302 ms                                                       | 304 ms: 1.00x slower                                                                   |
| sympy_sum                  | 162 ms                                                       | 163 ms: 1.00x slower                                                                   |
| sqlglot_transpile          | 1.78 ms                                                      | 1.79 ms: 1.01x slower                                                                  |
| regex_dna                  | 239 ms                                                       | 241 ms: 1.01x slower                                                                   |
| docutils                   | 2.87 sec                                                     | 2.90 sec: 1.01x slower                                                                 |
| async_tree_memoization_tg  | 540 ms                                                       | 548 ms: 1.01x slower                                                                   |
| logging_silent             | 94.4 ns                                                      | 95.6 ns: 1.01x slower                                                                  |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 707 ms: 1.01x slower                                                                   |
| async_tree_none_tg         | 431 ms                                                       | 438 ms: 1.02x slower                                                                   |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                                 |
| scimark_lu                 | 98.8 ms                                                      | 101 ms: 1.02x slower                                                                   |
| deepcopy_memo              | 36.8 us                                                      | 37.5 us: 1.02x slower                                                                  |
| regex_compile              | 144 ms                                                       | 147 ms: 1.02x slower                                                                   |
| crypto_pyaes               | 80.3 ms                                                      | 82.1 ms: 1.02x slower                                                                  |
| sympy_integrate            | 23.9 ms                                                      | 24.5 ms: 1.02x slower                                                                  |
| async_tree_io              | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                                 |
| pycparser                  | 1.23 sec                                                     | 1.27 sec: 1.03x slower                                                                 |
| unpickle                   | 14.8 us                                                      | 15.3 us: 1.03x slower                                                                  |
| bench_thread_pool          | 950 us                                                       | 982 us: 1.03x slower                                                                   |
| xml_etree_parse            | 144 ms                                                       | 149 ms: 1.04x slower                                                                   |
| xml_etree_iterparse        | 103 ms                                                       | 107 ms: 1.04x slower                                                                   |
| tornado_http               | 121 ms                                                       | 126 ms: 1.04x slower                                                                   |
| json_loads                 | 24.4 us                                                      | 25.3 us: 1.04x slower                                                                  |
| dask                       | 392 ms                                                       | 409 ms: 1.04x slower                                                                   |
| meteor_contest             | 128 ms                                                       | 134 ms: 1.04x slower                                                                   |
| sqlglot_normalize          | 116 ms                                                       | 121 ms: 1.04x slower                                                                   |
| json_dumps                 | 10.2 ms                                                      | 10.7 ms: 1.05x slower                                                                  |
| json                       | 5.12 ms                                                      | 5.36 ms: 1.05x slower                                                                  |
| bench_mp_pool              | 4.76 ms                                                      | 5.00 ms: 1.05x slower                                                                  |
| sympy_expand               | 484 ms                                                       | 509 ms: 1.05x slower                                                                   |
| chameleon                  | 7.23 ms                                                      | 7.67 ms: 1.06x slower                                                                  |
| 2to3                       | 285 ms                                                       | 303 ms: 1.06x slower                                                                   |
| unpickle_list              | 4.66 us                                                      | 4.95 us: 1.06x slower                                                                  |
| pprint_safe_repr           | 807 ms                                                       | 860 ms: 1.07x slower                                                                   |
| unpickle_pure_python       | 210 us                                                       | 224 us: 1.07x slower                                                                   |
| float                      | 76.6 ms                                                      | 82.1 ms: 1.07x slower                                                                  |
| pprint_pformat             | 1.65 sec                                                     | 1.78 sec: 1.07x slower                                                                 |
| dulwich_log                | 65.4 ms                                                      | 70.4 ms: 1.08x slower                                                                  |
| sqlglot_optimize           | 57.5 ms                                                      | 62.1 ms: 1.08x slower                                                                  |
| regex_v8                   | 23.6 ms                                                      | 25.6 ms: 1.08x slower                                                                  |
| tomli_loads                | 2.16 sec                                                     | 2.34 sec: 1.08x slower                                                                 |
| chaos                      | 64.0 ms                                                      | 69.8 ms: 1.09x slower                                                                  |
| python_startup             | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                                  |
| nqueens                    | 89.9 ms                                                      | 98.4 ms: 1.10x slower                                                                  |
| richards                   | 45.7 ms                                                      | 51.0 ms: 1.12x slower                                                                  |
| richards_super             | 51.3 ms                                                      | 57.4 ms: 1.12x slower                                                                  |
| go                         | 150 ms                                                       | 168 ms: 1.13x slower                                                                   |
| scimark_monte_carlo        | 69.0 ms                                                      | 79.0 ms: 1.14x slower                                                                  |
| mako                       | 10.0 ms                                                      | 11.8 ms: 1.18x slower                                                                  |
| pyflate                    | 439 ms                                                       | 517 ms: 1.18x slower                                                                   |
| telco                      | 6.96 ms                                                      | 8.22 ms: 1.18x slower                                                                  |
| nbody                      | 88.0 ms                                                      | 104 ms: 1.19x slower                                                                   |
| scimark_fft                | 301 ms                                                       | 359 ms: 1.19x slower                                                                   |
| coverage                   | 66.7 ms                                                      | 80.7 ms: 1.21x slower                                                                  |
| deltablue                  | 3.24 ms                                                      | 3.94 ms: 1.22x slower                                                                  |
| fannkuch                   | 350 ms                                                       | 430 ms: 1.23x slower                                                                   |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 5.22 ms: 1.24x slower                                                                  |
| spectral_norm              | 91.6 ms                                                      | 116 ms: 1.27x slower                                                                   |
| python_startup_no_site     | 8.64 ms                                                      | 11.2 ms: 1.29x slower                                                                  |
| scimark_sor                | 109 ms                                                       | 143 ms: 1.31x slower                                                                   |
| hexiom                     | 5.96 ms                                                      | 8.04 ms: 1.35x slower                                                                  |
| Geometric mean             | (ref)                                                        | 1.04x slower                                                                           |

Benchmark hidden because not significant (6): logging_format, sqlglot_parse, sqlite_synth, async_tree_memoization, async_tree_cpu_io_mixed, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.93x