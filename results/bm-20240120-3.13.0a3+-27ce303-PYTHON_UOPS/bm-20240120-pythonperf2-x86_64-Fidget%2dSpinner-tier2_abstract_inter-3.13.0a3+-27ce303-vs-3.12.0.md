
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 27ce303
- commit date: 2024-01-20
- overall geometric mean: 1.10x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 1.14x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 316 ms: 1.11x slower                                                                   |
| chameleon      | 7.23 ms                                                      | 8.17 ms: 1.13x slower                                                                  |
| docutils       | 2.87 sec                                                     | 2.92 sec: 1.02x slower                                                                 |
| tornado_http   | 121 ms                                                       | 123 ms: 1.02x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 444 ms: 1.02x faster                                                                   |
| async_tree_memoization_tg  | 540 ms                                                       | 549 ms: 1.02x slower                                                                   |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 713 ms: 1.02x slower                                                                   |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 716 ms: 1.03x slower                                                                   |
| async_tree_memoization     | 544 ms                                                       | 560 ms: 1.03x slower                                                                   |
| async_tree_none_tg         | 431 ms                                                       | 444 ms: 1.03x slower                                                                   |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.03x slower                                                                 |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.04x slower                                                                 |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 266 ms: 1.00x slower                                                                   |
| float          | 76.6 ms                                                      | 105 ms: 1.37x slower                                                                   |
| nbody          | 88.0 ms                                                      | 134 ms: 1.52x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.28x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.50 ms: 1.02x faster                                                                  |
| regex_dna      | 239 ms                                                       | 240 ms: 1.01x slower                                                                   |
| regex_v8       | 23.6 ms                                                      | 26.0 ms: 1.10x slower                                                                  |
| regex_compile  | 144 ms                                                       | 171 ms: 1.19x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pickle_pure_python   | 318 us                                                       | 310 us: 1.03x faster                                                                   |
| pickle               | 10.5 us                                                      | 10.4 us: 1.02x faster                                                                  |
| pickle_dict          | 32.5 us                                                      | 32.4 us: 1.00x faster                                                                  |
| unpickle_list        | 4.66 us                                                      | 4.69 us: 1.01x slower                                                                  |
| json_loads           | 24.4 us                                                      | 24.8 us: 1.02x slower                                                                  |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                                   |
| json_dumps           | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                                  |
| xml_etree_process    | 58.4 ms                                                      | 62.0 ms: 1.06x slower                                                                  |
| xml_etree_generate   | 86.1 ms                                                      | 91.7 ms: 1.06x slower                                                                  |
| xml_etree_iterparse  | 103 ms                                                       | 118 ms: 1.14x slower                                                                   |
| unpickle_pure_python | 210 us                                                       | 242 us: 1.15x slower                                                                   |
| tomli_loads          | 2.16 sec                                                     | 2.83 sec: 1.31x slower                                                                 |
| Geometric mean       | (ref)                                                        | 1.05x slower                                                                           |

Benchmark hidden because not significant (2): unpickle, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                                  |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.29x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.19x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 14.8 ms: 1.48x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf2-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 128 us: 1.19x faster                                                                   |
| unpack_sequence            | 53.2 ns                                                      | 45.5 ns: 1.17x faster                                                                  |
| generators                 | 37.4 ms                                                      | 33.9 ms: 1.10x faster                                                                  |
| async_generators           | 390 ms                                                       | 370 ms: 1.05x faster                                                                   |
| coroutines                 | 23.0 ms                                                      | 22.2 ms: 1.03x faster                                                                  |
| asyncio_websockets         | 387 ms                                                       | 376 ms: 1.03x faster                                                                   |
| pickle_pure_python         | 318 us                                                       | 310 us: 1.03x faster                                                                   |
| regex_effbot               | 3.57 ms                                                      | 3.50 ms: 1.02x faster                                                                  |
| pickle                     | 10.5 us                                                      | 10.4 us: 1.02x faster                                                                  |
| async_tree_none            | 452 ms                                                       | 444 ms: 1.02x faster                                                                   |
| logging_format             | 7.48 us                                                      | 7.42 us: 1.01x faster                                                                  |
| pickle_dict                | 32.5 us                                                      | 32.4 us: 1.00x faster                                                                  |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.59 sec: 1.00x slower                                                                 |
| pidigits                   | 265 ms                                                       | 266 ms: 1.00x slower                                                                   |
| regex_dna                  | 239 ms                                                       | 240 ms: 1.01x slower                                                                   |
| unpickle_list              | 4.66 us                                                      | 4.69 us: 1.01x slower                                                                  |
| pathlib                    | 18.9 ms                                                      | 19.0 ms: 1.01x slower                                                                  |
| deepcopy_reduce            | 3.37 us                                                      | 3.41 us: 1.01x slower                                                                  |
| gc_traversal               | 3.48 ms                                                      | 3.52 ms: 1.01x slower                                                                  |
| async_tree_memoization_tg  | 540 ms                                                       | 549 ms: 1.02x slower                                                                   |
| sqlite_synth               | 2.77 us                                                      | 2.82 us: 1.02x slower                                                                  |
| json_loads                 | 24.4 us                                                      | 24.8 us: 1.02x slower                                                                  |
| raytrace                   | 298 ms                                                       | 304 ms: 1.02x slower                                                                   |
| tornado_http               | 121 ms                                                       | 123 ms: 1.02x slower                                                                   |
| docutils                   | 2.87 sec                                                     | 2.92 sec: 1.02x slower                                                                 |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                                   |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 713 ms: 1.02x slower                                                                   |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 716 ms: 1.03x slower                                                                   |
| async_tree_memoization     | 544 ms                                                       | 560 ms: 1.03x slower                                                                   |
| async_tree_none_tg         | 431 ms                                                       | 444 ms: 1.03x slower                                                                   |
| json                       | 5.12 ms                                                      | 5.28 ms: 1.03x slower                                                                  |
| logging_simple             | 6.71 us                                                      | 6.94 us: 1.03x slower                                                                  |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.03x slower                                                                 |
| dask                       | 392 ms                                                       | 407 ms: 1.04x slower                                                                   |
| deepcopy                   | 368 us                                                       | 384 us: 1.04x slower                                                                   |
| sympy_sum                  | 162 ms                                                       | 169 ms: 1.04x slower                                                                   |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.04x slower                                                                 |
| sqlglot_parse              | 1.38 ms                                                      | 1.44 ms: 1.04x slower                                                                  |
| sqlglot_transpile          | 1.78 ms                                                      | 1.85 ms: 1.04x slower                                                                  |
| mdp                        | 2.57 sec                                                     | 2.69 sec: 1.05x slower                                                                 |
| sympy_integrate            | 23.9 ms                                                      | 25.1 ms: 1.05x slower                                                                  |
| json_dumps                 | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                                  |
| logging_silent             | 94.4 ns                                                      | 99.8 ns: 1.06x slower                                                                  |
| xml_etree_process          | 58.4 ms                                                      | 62.0 ms: 1.06x slower                                                                  |
| xml_etree_generate         | 86.1 ms                                                      | 91.7 ms: 1.06x slower                                                                  |
| scimark_lu                 | 98.8 ms                                                      | 105 ms: 1.07x slower                                                                   |
| sympy_str                  | 302 ms                                                       | 324 ms: 1.07x slower                                                                   |
| sqlglot_normalize          | 116 ms                                                       | 124 ms: 1.07x slower                                                                   |
| meteor_contest             | 128 ms                                                       | 138 ms: 1.08x slower                                                                   |
| crypto_pyaes               | 80.3 ms                                                      | 86.6 ms: 1.08x slower                                                                  |
| mypy2                      | 830 ms                                                       | 896 ms: 1.08x slower                                                                   |
| python_startup             | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                                  |
| pycparser                  | 1.23 sec                                                     | 1.36 sec: 1.10x slower                                                                 |
| dulwich_log                | 65.4 ms                                                      | 71.9 ms: 1.10x slower                                                                  |
| regex_v8                   | 23.6 ms                                                      | 26.0 ms: 1.10x slower                                                                  |
| sympy_expand               | 484 ms                                                       | 535 ms: 1.11x slower                                                                   |
| 2to3                       | 285 ms                                                       | 316 ms: 1.11x slower                                                                   |
| deepcopy_memo              | 36.8 us                                                      | 40.9 us: 1.11x slower                                                                  |
| sqlglot_optimize           | 57.5 ms                                                      | 64.2 ms: 1.12x slower                                                                  |
| chameleon                  | 7.23 ms                                                      | 8.17 ms: 1.13x slower                                                                  |
| pprint_safe_repr           | 807 ms                                                       | 920 ms: 1.14x slower                                                                   |
| xml_etree_iterparse        | 103 ms                                                       | 118 ms: 1.14x slower                                                                   |
| pprint_pformat             | 1.65 sec                                                     | 1.90 sec: 1.15x slower                                                                 |
| unpickle_pure_python       | 210 us                                                       | 242 us: 1.15x slower                                                                   |
| comprehensions             | 21.9 us                                                      | 25.7 us: 1.17x slower                                                                  |
| regex_compile              | 144 ms                                                       | 171 ms: 1.19x slower                                                                   |
| richards_super             | 51.3 ms                                                      | 61.1 ms: 1.19x slower                                                                  |
| richards                   | 45.7 ms                                                      | 54.7 ms: 1.20x slower                                                                  |
| coverage                   | 66.7 ms                                                      | 80.2 ms: 1.20x slower                                                                  |
| chaos                      | 64.0 ms                                                      | 77.9 ms: 1.22x slower                                                                  |
| telco                      | 6.96 ms                                                      | 8.54 ms: 1.23x slower                                                                  |
| nqueens                    | 89.9 ms                                                      | 111 ms: 1.23x slower                                                                   |
| go                         | 150 ms                                                       | 185 ms: 1.24x slower                                                                   |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.29x slower                                                                  |
| scimark_monte_carlo        | 69.0 ms                                                      | 90.4 ms: 1.31x slower                                                                  |
| tomli_loads                | 2.16 sec                                                     | 2.83 sec: 1.31x slower                                                                 |
| scimark_sor                | 109 ms                                                       | 146 ms: 1.34x slower                                                                   |
| pyflate                    | 439 ms                                                       | 588 ms: 1.34x slower                                                                   |
| fannkuch                   | 350 ms                                                       | 478 ms: 1.37x slower                                                                   |
| float                      | 76.6 ms                                                      | 105 ms: 1.37x slower                                                                   |
| scimark_fft                | 301 ms                                                       | 424 ms: 1.41x slower                                                                   |
| mako                       | 10.0 ms                                                      | 14.8 ms: 1.48x slower                                                                  |
| nbody                      | 88.0 ms                                                      | 134 ms: 1.52x slower                                                                   |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.58 ms: 1.56x slower                                                                  |
| spectral_norm              | 91.6 ms                                                      | 152 ms: 1.66x slower                                                                   |
| hexiom                     | 5.96 ms                                                      | 9.90 ms: 1.66x slower                                                                  |
| deltablue                  | 3.24 ms                                                      | 5.50 ms: 1.70x slower                                                                  |
| Geometric mean             | (ref)                                                        | 1.10x slower                                                                           |

Benchmark hidden because not significant (6): create_gc_cycles, asyncio_tcp, unpickle, pickle_list, bench_mp_pool, bench_thread_pool
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 1.14x