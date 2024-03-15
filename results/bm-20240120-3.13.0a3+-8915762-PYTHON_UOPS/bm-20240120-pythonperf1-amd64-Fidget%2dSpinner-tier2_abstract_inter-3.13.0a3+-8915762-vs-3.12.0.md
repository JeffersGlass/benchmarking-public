
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: 8915762
- commit date: 2024-01-20
- overall geometric mean: 1.00x faster
- HPT reliability: 96.43%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 223 ms: 1.02x slower                                                                  |
| chameleon      | 4.98 ms                                                     | 5.03 ms: 1.01x slower                                                                 |
| docutils       | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                                                |
| tornado_http   | 89.5 ms                                                     | 88.5 ms: 1.01x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 271 ms: 1.08x faster                                                                  |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 457 ms: 1.07x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 470 ms: 1.07x faster                                                                  |
| async_tree_memoization_tg  | 367 ms                                                      | 351 ms: 1.05x faster                                                                  |
| async_tree_io_tg           | 771 ms                                                      | 738 ms: 1.04x faster                                                                  |
| async_tree_none_tg         | 285 ms                                                      | 276 ms: 1.03x faster                                                                  |
| async_tree_io              | 731 ms                                                      | 722 ms: 1.01x faster                                                                  |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                          |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 148 ms: 1.03x faster                                                                  |
| nbody          | 71.9 ms                                                     | 81.4 ms: 1.13x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                          |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 118 ms: 1.07x faster                                                                  |
| regex_compile  | 87.5 ms                                                     | 84.4 ms: 1.04x faster                                                                 |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                                 |
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 180 us: 1.08x faster                                                                  |
| json_dumps           | 5.70 ms                                                     | 5.54 ms: 1.03x faster                                                                 |
| json_loads           | 13.9 us                                                     | 13.5 us: 1.03x faster                                                                 |
| xml_etree_generate   | 55.8 ms                                                     | 54.5 ms: 1.02x faster                                                                 |
| xml_etree_process    | 37.7 ms                                                     | 37.1 ms: 1.02x faster                                                                 |
| pickle_dict          | 18.4 us                                                     | 18.3 us: 1.00x faster                                                                 |
| pickle               | 7.43 us                                                     | 7.41 us: 1.00x faster                                                                 |
| xml_etree_parse      | 93.0 ms                                                     | 94.0 ms: 1.01x slower                                                                 |
| unpickle_list        | 2.75 us                                                     | 2.79 us: 1.02x slower                                                                 |
| xml_etree_iterparse  | 65.2 ms                                                     | 66.3 ms: 1.02x slower                                                                 |
| unpickle             | 8.18 us                                                     | 8.33 us: 1.02x slower                                                                 |
| unpickle_pure_python | 133 us                                                      | 137 us: 1.03x slower                                                                  |
| tomli_loads          | 1.37 sec                                                    | 1.44 sec: 1.05x slower                                                                |
| pickle_list          | 2.83 us                                                     | 3.09 us: 1.09x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.00x slower                                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 21.0 ms: 1.08x slower                                                                 |
| python_startup_no_site | 16.2 ms                                                     | 18.5 ms: 1.14x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.11x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.50 ms: 1.06x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 72.5 us: 1.31x faster                                                                 |
| mypy2                      | 509 ms                                                      | 423 ms: 1.20x faster                                                                  |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.75 sec: 1.20x faster                                                                |
| raytrace                   | 192 ms                                                      | 173 ms: 1.11x faster                                                                  |
| comprehensions             | 14.1 us                                                     | 12.7 us: 1.11x faster                                                                 |
| logging_silent             | 60.5 ns                                                     | 55.3 ns: 1.09x faster                                                                 |
| sqlite_synth               | 1.76 us                                                     | 1.61 us: 1.09x faster                                                                 |
| pickle_pure_python         | 195 us                                                      | 180 us: 1.08x faster                                                                  |
| async_tree_none            | 291 ms                                                      | 271 ms: 1.08x faster                                                                  |
| regex_dna                  | 126 ms                                                      | 118 ms: 1.07x faster                                                                  |
| coroutines                 | 14.3 ms                                                     | 13.3 ms: 1.07x faster                                                                 |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 457 ms: 1.07x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 470 ms: 1.07x faster                                                                  |
| deepcopy                   | 238 us                                                      | 223 us: 1.07x faster                                                                  |
| deepcopy_memo              | 23.7 us                                                     | 22.5 us: 1.05x faster                                                                 |
| dulwich_log                | 44.3 ms                                                     | 42.1 ms: 1.05x faster                                                                 |
| deepcopy_reduce            | 2.09 us                                                     | 1.99 us: 1.05x faster                                                                 |
| sympy_str                  | 175 ms                                                      | 167 ms: 1.05x faster                                                                  |
| docutils                   | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                                                |
| scimark_lu                 | 58.9 ms                                                     | 56.2 ms: 1.05x faster                                                                 |
| richards                   | 28.4 ms                                                     | 27.1 ms: 1.05x faster                                                                 |
| richards_super             | 32.1 ms                                                     | 30.7 ms: 1.05x faster                                                                 |
| async_tree_memoization_tg  | 367 ms                                                      | 351 ms: 1.05x faster                                                                  |
| async_tree_io_tg           | 771 ms                                                      | 738 ms: 1.04x faster                                                                  |
| generators                 | 22.5 ms                                                     | 21.6 ms: 1.04x faster                                                                 |
| asyncio_tcp                | 487 ms                                                      | 468 ms: 1.04x faster                                                                  |
| sqlglot_parse              | 804 us                                                      | 776 us: 1.04x faster                                                                  |
| regex_compile              | 87.5 ms                                                     | 84.4 ms: 1.04x faster                                                                 |
| sympy_sum                  | 91.5 ms                                                     | 88.3 ms: 1.04x faster                                                                 |
| async_tree_none_tg         | 285 ms                                                      | 276 ms: 1.03x faster                                                                  |
| regex_effbot               | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                                 |
| pidigits                   | 152 ms                                                      | 148 ms: 1.03x faster                                                                  |
| json_dumps                 | 5.70 ms                                                     | 5.54 ms: 1.03x faster                                                                 |
| json_loads                 | 13.9 us                                                     | 13.5 us: 1.03x faster                                                                 |
| sqlglot_normalize          | 187 ms                                                      | 182 ms: 1.03x faster                                                                  |
| xml_etree_generate         | 55.8 ms                                                     | 54.5 ms: 1.02x faster                                                                 |
| sqlglot_transpile          | 1.02 ms                                                     | 1.00 ms: 1.02x faster                                                                 |
| xml_etree_process          | 37.7 ms                                                     | 37.1 ms: 1.02x faster                                                                 |
| async_generators           | 239 ms                                                      | 236 ms: 1.02x faster                                                                  |
| pathlib                    | 80.5 ms                                                     | 79.3 ms: 1.01x faster                                                                 |
| create_gc_cycles           | 752 us                                                      | 742 us: 1.01x faster                                                                  |
| sympy_expand               | 284 ms                                                      | 280 ms: 1.01x faster                                                                  |
| async_tree_io              | 731 ms                                                      | 722 ms: 1.01x faster                                                                  |
| crypto_pyaes               | 48.5 ms                                                     | 47.9 ms: 1.01x faster                                                                 |
| mdp                        | 1.37 sec                                                    | 1.36 sec: 1.01x faster                                                                |
| tornado_http               | 89.5 ms                                                     | 88.5 ms: 1.01x faster                                                                 |
| gc_traversal               | 1.52 ms                                                     | 1.51 ms: 1.01x faster                                                                 |
| logging_simple             | 6.28 us                                                     | 6.23 us: 1.01x faster                                                                 |
| pickle_dict                | 18.4 us                                                     | 18.3 us: 1.00x faster                                                                 |
| pickle                     | 7.43 us                                                     | 7.41 us: 1.00x faster                                                                 |
| scimark_sor                | 78.8 ms                                                     | 79.0 ms: 1.00x slower                                                                 |
| bench_mp_pool              | 69.2 ms                                                     | 69.7 ms: 1.01x slower                                                                 |
| go                         | 91.6 ms                                                     | 92.3 ms: 1.01x slower                                                                 |
| chameleon                  | 4.98 ms                                                     | 5.03 ms: 1.01x slower                                                                 |
| chaos                      | 43.3 ms                                                     | 43.8 ms: 1.01x slower                                                                 |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                                                 |
| xml_etree_parse            | 93.0 ms                                                     | 94.0 ms: 1.01x slower                                                                 |
| pprint_safe_repr           | 513 ms                                                      | 519 ms: 1.01x slower                                                                  |
| unpickle_list              | 2.75 us                                                     | 2.79 us: 1.02x slower                                                                 |
| xml_etree_iterparse        | 65.2 ms                                                     | 66.3 ms: 1.02x slower                                                                 |
| sympy_integrate            | 13.0 ms                                                     | 13.2 ms: 1.02x slower                                                                 |
| pprint_pformat             | 1.05 sec                                                    | 1.06 sec: 1.02x slower                                                                |
| meteor_contest             | 74.6 ms                                                     | 75.9 ms: 1.02x slower                                                                 |
| unpickle                   | 8.18 us                                                     | 8.33 us: 1.02x slower                                                                 |
| 2to3                       | 218 ms                                                      | 223 ms: 1.02x slower                                                                  |
| regex_v8                   | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                                 |
| unpickle_pure_python       | 133 us                                                      | 137 us: 1.03x slower                                                                  |
| nqueens                    | 62.8 ms                                                     | 65.5 ms: 1.04x slower                                                                 |
| tomli_loads                | 1.37 sec                                                    | 1.44 sec: 1.05x slower                                                                |
| unpack_sequence            | 37.5 ns                                                     | 39.5 ns: 1.05x slower                                                                 |
| mako                       | 7.09 ms                                                     | 7.50 ms: 1.06x slower                                                                 |
| python_startup             | 19.5 ms                                                     | 21.0 ms: 1.08x slower                                                                 |
| fannkuch                   | 247 ms                                                      | 267 ms: 1.08x slower                                                                  |
| scimark_monte_carlo        | 43.7 ms                                                     | 47.7 ms: 1.09x slower                                                                 |
| pickle_list                | 2.83 us                                                     | 3.09 us: 1.09x slower                                                                 |
| scimark_fft                | 184 ms                                                      | 202 ms: 1.10x slower                                                                  |
| pyflate                    | 295 ms                                                      | 324 ms: 1.10x slower                                                                  |
| coverage                   | 40.8 ms                                                     | 45.0 ms: 1.10x slower                                                                 |
| nbody                      | 71.9 ms                                                     | 81.4 ms: 1.13x slower                                                                 |
| python_startup_no_site     | 16.2 ms                                                     | 18.5 ms: 1.14x slower                                                                 |
| telco                      | 4.13 ms                                                     | 4.80 ms: 1.16x slower                                                                 |
| spectral_norm              | 66.9 ms                                                     | 80.6 ms: 1.20x slower                                                                 |
| hexiom                     | 4.10 ms                                                     | 4.94 ms: 1.21x slower                                                                 |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 3.19 ms: 1.25x slower                                                                 |
| deltablue                  | 2.16 ms                                                     | 2.73 ms: 1.26x slower                                                                 |
| Geometric mean             | (ref)                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (7): dask, json, float, bench_thread_pool, logging_format, pycparser, async_tree_memoization
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 96.43% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown