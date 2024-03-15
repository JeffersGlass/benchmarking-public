
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.00x slower
- HPT reliability: 76.67%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 224 ms: 1.03x slower                                                                  |
| chameleon      | 4.98 ms                                                     | 5.05 ms: 1.01x slower                                                                 |
| docutils       | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                                                |
| tornado_http   | 89.5 ms                                                     | 88.1 ms: 1.02x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.00x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 276 ms: 1.05x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 481 ms: 1.04x faster                                                                  |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 473 ms: 1.03x faster                                                                  |
| async_tree_io              | 731 ms                                                      | 756 ms: 1.03x slower                                                                  |
| async_tree_memoization     | 339 ms                                                      | 355 ms: 1.05x slower                                                                  |
| Geometric mean             | (ref)                                                       | 1.01x faster                                                                          |

Benchmark hidden because not significant (3): async_tree_none_tg, async_tree_memoization_tg, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 148 ms: 1.03x faster                                                                  |
| nbody          | 71.9 ms                                                     | 76.8 ms: 1.07x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                          |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 84.6 ms: 1.03x faster                                                                 |
| regex_dna      | 126 ms                                                      | 123 ms: 1.03x faster                                                                  |
| regex_effbot   | 1.62 ms                                                     | 1.61 ms: 1.01x faster                                                                 |
| regex_v8       | 14.2 ms                                                     | 15.7 ms: 1.10x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 181 us: 1.08x faster                                                                  |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.01x faster                                                                 |
| pickle               | 7.43 us                                                     | 7.37 us: 1.01x faster                                                                 |
| unpickle_list        | 2.75 us                                                     | 2.78 us: 1.01x slower                                                                 |
| xml_etree_parse      | 93.0 ms                                                     | 94.1 ms: 1.01x slower                                                                 |
| json_dumps           | 5.70 ms                                                     | 5.76 ms: 1.01x slower                                                                 |
| unpickle_pure_python | 133 us                                                      | 135 us: 1.02x slower                                                                  |
| pickle_dict          | 18.4 us                                                     | 18.8 us: 1.02x slower                                                                 |
| unpickle             | 8.18 us                                                     | 8.48 us: 1.04x slower                                                                 |
| tomli_loads          | 1.37 sec                                                    | 1.43 sec: 1.04x slower                                                                |
| xml_etree_iterparse  | 65.2 ms                                                     | 68.4 ms: 1.05x slower                                                                 |
| pickle_list          | 2.83 us                                                     | 2.99 us: 1.06x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                                          |

Benchmark hidden because not significant (2): xml_etree_generate, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.8 ms: 1.07x slower                                                                 |
| python_startup_no_site | 16.2 ms                                                     | 18.8 ms: 1.16x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.11x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.53 ms: 1.06x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.52 sec: 1.38x faster                                                                |
| typing_runtime_protocols   | 95.1 us                                                     | 75.3 us: 1.26x faster                                                                 |
| mypy2                      | 509 ms                                                      | 437 ms: 1.16x faster                                                                  |
| raytrace                   | 192 ms                                                      | 174 ms: 1.11x faster                                                                  |
| sqlite_synth               | 1.76 us                                                     | 1.59 us: 1.10x faster                                                                 |
| comprehensions             | 14.1 us                                                     | 12.8 us: 1.10x faster                                                                 |
| coroutines                 | 14.3 ms                                                     | 13.0 ms: 1.10x faster                                                                 |
| logging_silent             | 60.5 ns                                                     | 55.2 ns: 1.10x faster                                                                 |
| pickle_pure_python         | 195 us                                                      | 181 us: 1.08x faster                                                                  |
| deepcopy                   | 238 us                                                      | 226 us: 1.06x faster                                                                  |
| async_tree_none            | 291 ms                                                      | 276 ms: 1.05x faster                                                                  |
| sympy_str                  | 175 ms                                                      | 166 ms: 1.05x faster                                                                  |
| async_generators           | 239 ms                                                      | 228 ms: 1.05x faster                                                                  |
| richards_super             | 32.1 ms                                                     | 30.6 ms: 1.05x faster                                                                 |
| deepcopy_reduce            | 2.09 us                                                     | 2.00 us: 1.05x faster                                                                 |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 481 ms: 1.04x faster                                                                  |
| richards                   | 28.4 ms                                                     | 27.3 ms: 1.04x faster                                                                 |
| regex_compile              | 87.5 ms                                                     | 84.6 ms: 1.03x faster                                                                 |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 473 ms: 1.03x faster                                                                  |
| pidigits                   | 152 ms                                                      | 148 ms: 1.03x faster                                                                  |
| regex_dna                  | 126 ms                                                      | 123 ms: 1.03x faster                                                                  |
| docutils                   | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                                                |
| sympy_sum                  | 91.5 ms                                                     | 89.1 ms: 1.03x faster                                                                 |
| generators                 | 22.5 ms                                                     | 22.0 ms: 1.03x faster                                                                 |
| dulwich_log                | 44.3 ms                                                     | 43.2 ms: 1.03x faster                                                                 |
| sqlglot_parse              | 804 us                                                      | 787 us: 1.02x faster                                                                  |
| create_gc_cycles           | 752 us                                                      | 737 us: 1.02x faster                                                                  |
| pycparser                  | 699 ms                                                      | 687 ms: 1.02x faster                                                                  |
| scimark_lu                 | 58.9 ms                                                     | 57.9 ms: 1.02x faster                                                                 |
| tornado_http               | 89.5 ms                                                     | 88.1 ms: 1.02x faster                                                                 |
| logging_simple             | 6.28 us                                                     | 6.20 us: 1.01x faster                                                                 |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.01x faster                                                                 |
| pickle                     | 7.43 us                                                     | 7.37 us: 1.01x faster                                                                 |
| logging_format             | 6.72 us                                                     | 6.66 us: 1.01x faster                                                                 |
| crypto_pyaes               | 48.5 ms                                                     | 48.1 ms: 1.01x faster                                                                 |
| regex_effbot               | 1.62 ms                                                     | 1.61 ms: 1.01x faster                                                                 |
| chaos                      | 43.3 ms                                                     | 43.1 ms: 1.01x faster                                                                 |
| pathlib                    | 80.5 ms                                                     | 81.1 ms: 1.01x slower                                                                 |
| unpickle_list              | 2.75 us                                                     | 2.78 us: 1.01x slower                                                                 |
| xml_etree_parse            | 93.0 ms                                                     | 94.1 ms: 1.01x slower                                                                 |
| json_dumps                 | 5.70 ms                                                     | 5.76 ms: 1.01x slower                                                                 |
| chameleon                  | 4.98 ms                                                     | 5.05 ms: 1.01x slower                                                                 |
| go                         | 91.6 ms                                                     | 93.0 ms: 1.02x slower                                                                 |
| unpickle_pure_python       | 133 us                                                      | 135 us: 1.02x slower                                                                  |
| pickle_dict                | 18.4 us                                                     | 18.8 us: 1.02x slower                                                                 |
| pprint_safe_repr           | 513 ms                                                      | 523 ms: 1.02x slower                                                                  |
| pprint_pformat             | 1.05 sec                                                    | 1.07 sec: 1.02x slower                                                                |
| meteor_contest             | 74.6 ms                                                     | 76.5 ms: 1.02x slower                                                                 |
| 2to3                       | 218 ms                                                      | 224 ms: 1.03x slower                                                                  |
| sympy_integrate            | 13.0 ms                                                     | 13.3 ms: 1.03x slower                                                                 |
| nqueens                    | 62.8 ms                                                     | 64.7 ms: 1.03x slower                                                                 |
| async_tree_io              | 731 ms                                                      | 756 ms: 1.03x slower                                                                  |
| sqlglot_optimize           | 34.5 ms                                                     | 35.7 ms: 1.03x slower                                                                 |
| unpickle                   | 8.18 us                                                     | 8.48 us: 1.04x slower                                                                 |
| unpack_sequence            | 37.5 ns                                                     | 39.0 ns: 1.04x slower                                                                 |
| tomli_loads                | 1.37 sec                                                    | 1.43 sec: 1.04x slower                                                                |
| mdp                        | 1.37 sec                                                    | 1.43 sec: 1.05x slower                                                                |
| async_tree_memoization     | 339 ms                                                      | 355 ms: 1.05x slower                                                                  |
| xml_etree_iterparse        | 65.2 ms                                                     | 68.4 ms: 1.05x slower                                                                 |
| pickle_list                | 2.83 us                                                     | 2.99 us: 1.06x slower                                                                 |
| scimark_fft                | 184 ms                                                      | 195 ms: 1.06x slower                                                                  |
| mako                       | 7.09 ms                                                     | 7.53 ms: 1.06x slower                                                                 |
| nbody                      | 71.9 ms                                                     | 76.8 ms: 1.07x slower                                                                 |
| python_startup             | 19.5 ms                                                     | 20.8 ms: 1.07x slower                                                                 |
| scimark_monte_carlo        | 43.7 ms                                                     | 47.0 ms: 1.07x slower                                                                 |
| fannkuch                   | 247 ms                                                      | 269 ms: 1.09x slower                                                                  |
| pyflate                    | 295 ms                                                      | 322 ms: 1.09x slower                                                                  |
| regex_v8                   | 14.2 ms                                                     | 15.7 ms: 1.10x slower                                                                 |
| telco                      | 4.13 ms                                                     | 4.64 ms: 1.12x slower                                                                 |
| python_startup_no_site     | 16.2 ms                                                     | 18.8 ms: 1.16x slower                                                                 |
| coverage                   | 40.8 ms                                                     | 47.7 ms: 1.17x slower                                                                 |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 3.02 ms: 1.18x slower                                                                 |
| hexiom                     | 4.10 ms                                                     | 4.90 ms: 1.19x slower                                                                 |
| spectral_norm              | 66.9 ms                                                     | 80.1 ms: 1.20x slower                                                                 |
| deltablue                  | 2.16 ms                                                     | 2.65 ms: 1.23x slower                                                                 |
| Geometric mean             | (ref)                                                       | 1.00x slower                                                                          |

Benchmark hidden because not significant (17): xml_etree_generate, sqlglot_transpile, gc_traversal, float, async_tree_none_tg, sqlglot_normalize, async_tree_memoization_tg, async_tree_io_tg, bench_mp_pool, sympy_expand, deepcopy_memo, xml_etree_process, scimark_sor, dask, bench_thread_pool, asyncio_tcp, json
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 76.67% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown