
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.01x slower
- HPT reliability: 94.90%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 229 ms: 1.05x slower                                                                  |
| chameleon      | 4.98 ms                                                     | 5.05 ms: 1.01x slower                                                                 |
| docutils       | 1.66 sec                                                    | 1.63 sec: 1.02x faster                                                                |
| tornado_http   | 89.5 ms                                                     | 87.4 ms: 1.02x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 273 ms: 1.07x faster                                                                  |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 466 ms: 1.05x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 487 ms: 1.03x faster                                                                  |
| async_tree_none_tg         | 285 ms                                                      | 288 ms: 1.01x slower                                                                  |
| async_tree_io_tg           | 771 ms                                                      | 784 ms: 1.02x slower                                                                  |
| async_tree_io              | 731 ms                                                      | 747 ms: 1.02x slower                                                                  |
| Geometric mean             | (ref)                                                       | 1.01x faster                                                                          |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 149 ms: 1.02x faster                                                                  |
| nbody          | 71.9 ms                                                     | 77.0 ms: 1.07x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.02x slower                                                                          |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 122 ms: 1.04x faster                                                                  |
| regex_compile  | 87.5 ms                                                     | 84.6 ms: 1.03x faster                                                                 |
| regex_effbot   | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                                 |
| regex_v8       | 14.2 ms                                                     | 15.7 ms: 1.10x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.00x slower                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 186 us: 1.05x faster                                                                  |
| pickle               | 7.43 us                                                     | 7.22 us: 1.03x faster                                                                 |
| unpickle_list        | 2.75 us                                                     | 2.73 us: 1.01x faster                                                                 |
| json_dumps           | 5.70 ms                                                     | 5.66 ms: 1.01x faster                                                                 |
| json_loads           | 13.9 us                                                     | 13.8 us: 1.01x faster                                                                 |
| xml_etree_process    | 37.7 ms                                                     | 38.0 ms: 1.01x slower                                                                 |
| xml_etree_parse      | 93.0 ms                                                     | 94.1 ms: 1.01x slower                                                                 |
| unpickle             | 8.18 us                                                     | 8.30 us: 1.01x slower                                                                 |
| tomli_loads          | 1.37 sec                                                    | 1.40 sec: 1.03x slower                                                                |
| unpickle_pure_python | 133 us                                                      | 139 us: 1.05x slower                                                                  |
| pickle_list          | 2.83 us                                                     | 2.98 us: 1.06x slower                                                                 |
| xml_etree_iterparse  | 65.2 ms                                                     | 68.9 ms: 1.06x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                                          |

Benchmark hidden because not significant (2): xml_etree_generate, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.8 ms: 1.07x slower                                                                 |
| python_startup_no_site | 16.2 ms                                                     | 18.9 ms: 1.16x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.11x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.22 ms: 1.02x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 74.8 us: 1.27x faster                                                                 |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.72 sec: 1.22x faster                                                                |
| mypy2                      | 509 ms                                                      | 432 ms: 1.18x faster                                                                  |
| comprehensions             | 14.1 us                                                     | 12.5 us: 1.13x faster                                                                 |
| sqlite_synth               | 1.76 us                                                     | 1.58 us: 1.12x faster                                                                 |
| raytrace                   | 192 ms                                                      | 176 ms: 1.09x faster                                                                  |
| logging_silent             | 60.5 ns                                                     | 56.3 ns: 1.07x faster                                                                 |
| async_tree_none            | 291 ms                                                      | 273 ms: 1.07x faster                                                                  |
| pickle_pure_python         | 195 us                                                      | 186 us: 1.05x faster                                                                  |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 466 ms: 1.05x faster                                                                  |
| deepcopy                   | 238 us                                                      | 227 us: 1.05x faster                                                                  |
| sympy_str                  | 175 ms                                                      | 167 ms: 1.05x faster                                                                  |
| coroutines                 | 14.3 ms                                                     | 13.6 ms: 1.05x faster                                                                 |
| richards_super             | 32.1 ms                                                     | 30.9 ms: 1.04x faster                                                                 |
| deepcopy_reduce            | 2.09 us                                                     | 2.01 us: 1.04x faster                                                                 |
| regex_dna                  | 126 ms                                                      | 122 ms: 1.04x faster                                                                  |
| regex_compile              | 87.5 ms                                                     | 84.6 ms: 1.03x faster                                                                 |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 487 ms: 1.03x faster                                                                  |
| sqlglot_parse              | 804 us                                                      | 780 us: 1.03x faster                                                                  |
| pickle                     | 7.43 us                                                     | 7.22 us: 1.03x faster                                                                 |
| richards                   | 28.4 ms                                                     | 27.6 ms: 1.03x faster                                                                 |
| sympy_sum                  | 91.5 ms                                                     | 89.1 ms: 1.03x faster                                                                 |
| sqlglot_normalize          | 187 ms                                                      | 182 ms: 1.03x faster                                                                  |
| tornado_http               | 89.5 ms                                                     | 87.4 ms: 1.02x faster                                                                 |
| logging_simple             | 6.28 us                                                     | 6.15 us: 1.02x faster                                                                 |
| logging_format             | 6.72 us                                                     | 6.59 us: 1.02x faster                                                                 |
| pidigits                   | 152 ms                                                      | 149 ms: 1.02x faster                                                                  |
| docutils                   | 1.66 sec                                                    | 1.63 sec: 1.02x faster                                                                |
| async_generators           | 239 ms                                                      | 236 ms: 1.02x faster                                                                  |
| create_gc_cycles           | 752 us                                                      | 740 us: 1.02x faster                                                                  |
| dulwich_log                | 44.3 ms                                                     | 43.7 ms: 1.01x faster                                                                 |
| sqlglot_transpile          | 1.02 ms                                                     | 1.01 ms: 1.01x faster                                                                 |
| regex_effbot               | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                                 |
| unpickle_list              | 2.75 us                                                     | 2.73 us: 1.01x faster                                                                 |
| crypto_pyaes               | 48.5 ms                                                     | 48.1 ms: 1.01x faster                                                                 |
| json_dumps                 | 5.70 ms                                                     | 5.66 ms: 1.01x faster                                                                 |
| json_loads                 | 13.9 us                                                     | 13.8 us: 1.01x faster                                                                 |
| chaos                      | 43.3 ms                                                     | 43.5 ms: 1.00x slower                                                                 |
| xml_etree_process          | 37.7 ms                                                     | 38.0 ms: 1.01x slower                                                                 |
| xml_etree_parse            | 93.0 ms                                                     | 94.1 ms: 1.01x slower                                                                 |
| async_tree_none_tg         | 285 ms                                                      | 288 ms: 1.01x slower                                                                  |
| gc_traversal               | 1.52 ms                                                     | 1.54 ms: 1.01x slower                                                                 |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                                                 |
| chameleon                  | 4.98 ms                                                     | 5.05 ms: 1.01x slower                                                                 |
| unpickle                   | 8.18 us                                                     | 8.30 us: 1.01x slower                                                                 |
| nqueens                    | 62.8 ms                                                     | 63.8 ms: 1.02x slower                                                                 |
| async_tree_io_tg           | 771 ms                                                      | 784 ms: 1.02x slower                                                                  |
| mako                       | 7.09 ms                                                     | 7.22 ms: 1.02x slower                                                                 |
| pprint_safe_repr           | 513 ms                                                      | 523 ms: 1.02x slower                                                                  |
| async_tree_io              | 731 ms                                                      | 747 ms: 1.02x slower                                                                  |
| bench_mp_pool              | 69.2 ms                                                     | 70.8 ms: 1.02x slower                                                                 |
| go                         | 91.6 ms                                                     | 93.7 ms: 1.02x slower                                                                 |
| tomli_loads                | 1.37 sec                                                    | 1.40 sec: 1.03x slower                                                                |
| sympy_integrate            | 13.0 ms                                                     | 13.3 ms: 1.03x slower                                                                 |
| deepcopy_memo              | 23.7 us                                                     | 24.4 us: 1.03x slower                                                                 |
| pprint_pformat             | 1.05 sec                                                    | 1.08 sec: 1.03x slower                                                                |
| meteor_contest             | 74.6 ms                                                     | 77.0 ms: 1.03x slower                                                                 |
| unpack_sequence            | 37.5 ns                                                     | 39.1 ns: 1.04x slower                                                                 |
| unpickle_pure_python       | 133 us                                                      | 139 us: 1.05x slower                                                                  |
| mdp                        | 1.37 sec                                                    | 1.44 sec: 1.05x slower                                                                |
| 2to3                       | 218 ms                                                      | 229 ms: 1.05x slower                                                                  |
| pickle_list                | 2.83 us                                                     | 2.98 us: 1.06x slower                                                                 |
| xml_etree_iterparse        | 65.2 ms                                                     | 68.9 ms: 1.06x slower                                                                 |
| scimark_lu                 | 58.9 ms                                                     | 62.6 ms: 1.06x slower                                                                 |
| scimark_sor                | 78.8 ms                                                     | 83.8 ms: 1.06x slower                                                                 |
| python_startup             | 19.5 ms                                                     | 20.8 ms: 1.07x slower                                                                 |
| nbody                      | 71.9 ms                                                     | 77.0 ms: 1.07x slower                                                                 |
| scimark_fft                | 184 ms                                                      | 198 ms: 1.07x slower                                                                  |
| scimark_monte_carlo        | 43.7 ms                                                     | 48.0 ms: 1.10x slower                                                                 |
| regex_v8                   | 14.2 ms                                                     | 15.7 ms: 1.10x slower                                                                 |
| fannkuch                   | 247 ms                                                      | 272 ms: 1.10x slower                                                                  |
| pyflate                    | 295 ms                                                      | 326 ms: 1.11x slower                                                                  |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.91 ms: 1.14x slower                                                                 |
| spectral_norm              | 66.9 ms                                                     | 76.2 ms: 1.14x slower                                                                 |
| telco                      | 4.13 ms                                                     | 4.73 ms: 1.15x slower                                                                 |
| python_startup_no_site     | 16.2 ms                                                     | 18.9 ms: 1.16x slower                                                                 |
| hexiom                     | 4.10 ms                                                     | 4.78 ms: 1.17x slower                                                                 |
| coverage                   | 40.8 ms                                                     | 47.8 ms: 1.17x slower                                                                 |
| deltablue                  | 2.16 ms                                                     | 2.61 ms: 1.21x slower                                                                 |
| Geometric mean             | (ref)                                                       | 1.01x slower                                                                          |

Benchmark hidden because not significant (13): json, xml_etree_generate, async_tree_memoization_tg, float, pickle_dict, dask, sympy_expand, generators, pathlib, asyncio_tcp, async_tree_memoization, pycparser, bench_thread_pool
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 94.90% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown