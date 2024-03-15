
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.00x slower
- HPT reliability: 69.50%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 224 ms: 1.03x slower                                                                  |
| docutils       | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                                                |
| tornado_http   | 89.5 ms                                                     | 85.8 ms: 1.04x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                          |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 276 ms: 1.06x faster                                                                  |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 464 ms: 1.05x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 488 ms: 1.03x faster                                                                  |
| async_tree_none_tg         | 285 ms                                                      | 289 ms: 1.01x slower                                                                  |
| async_tree_io_tg           | 771 ms                                                      | 783 ms: 1.01x slower                                                                  |
| async_tree_io              | 731 ms                                                      | 744 ms: 1.02x slower                                                                  |
| async_tree_memoization     | 339 ms                                                      | 350 ms: 1.03x slower                                                                  |
| Geometric mean             | (ref)                                                       | 1.01x faster                                                                          |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 150 ms: 1.02x faster                                                                  |
| float          | 56.8 ms                                                     | 58.1 ms: 1.02x slower                                                                 |
| nbody          | 71.9 ms                                                     | 78.8 ms: 1.10x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 122 ms: 1.04x faster                                                                  |
| regex_compile  | 87.5 ms                                                     | 85.8 ms: 1.02x faster                                                                 |
| regex_effbot   | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                                 |
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.00x faster                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 179 us: 1.09x faster                                                                  |
| pickle               | 7.43 us                                                     | 7.11 us: 1.05x faster                                                                 |
| json_dumps           | 5.70 ms                                                     | 5.51 ms: 1.03x faster                                                                 |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.01x faster                                                                 |
| xml_etree_process    | 37.7 ms                                                     | 38.0 ms: 1.01x slower                                                                 |
| pickle_dict          | 18.4 us                                                     | 18.6 us: 1.01x slower                                                                 |
| unpickle_list        | 2.75 us                                                     | 2.81 us: 1.02x slower                                                                 |
| unpickle_pure_python | 133 us                                                      | 137 us: 1.03x slower                                                                  |
| pickle_list          | 2.83 us                                                     | 2.91 us: 1.03x slower                                                                 |
| unpickle             | 8.18 us                                                     | 8.45 us: 1.03x slower                                                                 |
| xml_etree_parse      | 93.0 ms                                                     | 96.9 ms: 1.04x slower                                                                 |
| xml_etree_iterparse  | 65.2 ms                                                     | 69.1 ms: 1.06x slower                                                                 |
| tomli_loads          | 1.37 sec                                                    | 1.46 sec: 1.06x slower                                                                |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                                          |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.6 ms: 1.06x slower                                                                 |
| python_startup_no_site | 16.2 ms                                                     | 18.4 ms: 1.13x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.10x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.99 ms: 1.13x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.49 sec: 1.41x faster                                                                |
| typing_runtime_protocols   | 95.1 us                                                     | 73.7 us: 1.29x faster                                                                 |
| mypy2                      | 509 ms                                                      | 431 ms: 1.18x faster                                                                  |
| logging_silent             | 60.5 ns                                                     | 55.0 ns: 1.10x faster                                                                 |
| pickle_pure_python         | 195 us                                                      | 179 us: 1.09x faster                                                                  |
| comprehensions             | 14.1 us                                                     | 13.0 us: 1.09x faster                                                                 |
| raytrace                   | 192 ms                                                      | 178 ms: 1.08x faster                                                                  |
| generators                 | 22.5 ms                                                     | 20.9 ms: 1.08x faster                                                                 |
| deepcopy_reduce            | 2.09 us                                                     | 1.94 us: 1.08x faster                                                                 |
| richards                   | 28.4 ms                                                     | 26.6 ms: 1.07x faster                                                                 |
| deepcopy                   | 238 us                                                      | 223 us: 1.07x faster                                                                  |
| richards_super             | 32.1 ms                                                     | 30.2 ms: 1.06x faster                                                                 |
| sqlite_synth               | 1.76 us                                                     | 1.66 us: 1.06x faster                                                                 |
| async_tree_none            | 291 ms                                                      | 276 ms: 1.06x faster                                                                  |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 464 ms: 1.05x faster                                                                  |
| scimark_lu                 | 58.9 ms                                                     | 55.9 ms: 1.05x faster                                                                 |
| pickle                     | 7.43 us                                                     | 7.11 us: 1.05x faster                                                                 |
| tornado_http               | 89.5 ms                                                     | 85.8 ms: 1.04x faster                                                                 |
| async_generators           | 239 ms                                                      | 230 ms: 1.04x faster                                                                  |
| regex_dna                  | 126 ms                                                      | 122 ms: 1.04x faster                                                                  |
| sympy_str                  | 175 ms                                                      | 169 ms: 1.04x faster                                                                  |
| json_dumps                 | 5.70 ms                                                     | 5.51 ms: 1.03x faster                                                                 |
| docutils                   | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                                                |
| sympy_sum                  | 91.5 ms                                                     | 88.7 ms: 1.03x faster                                                                 |
| pycparser                  | 699 ms                                                      | 678 ms: 1.03x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 488 ms: 1.03x faster                                                                  |
| coroutines                 | 14.3 ms                                                     | 13.9 ms: 1.03x faster                                                                 |
| sqlglot_parse              | 804 us                                                      | 782 us: 1.03x faster                                                                  |
| dulwich_log                | 44.3 ms                                                     | 43.1 ms: 1.03x faster                                                                 |
| crypto_pyaes               | 48.5 ms                                                     | 47.3 ms: 1.02x faster                                                                 |
| deepcopy_memo              | 23.7 us                                                     | 23.2 us: 1.02x faster                                                                 |
| regex_compile              | 87.5 ms                                                     | 85.8 ms: 1.02x faster                                                                 |
| pidigits                   | 152 ms                                                      | 150 ms: 1.02x faster                                                                  |
| sympy_expand               | 284 ms                                                      | 280 ms: 1.02x faster                                                                  |
| scimark_sor                | 78.8 ms                                                     | 77.7 ms: 1.01x faster                                                                 |
| regex_effbot               | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                                 |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.01x faster                                                                 |
| sqlglot_transpile          | 1.02 ms                                                     | 1.01 ms: 1.01x faster                                                                 |
| pathlib                    | 80.5 ms                                                     | 79.8 ms: 1.01x faster                                                                 |
| logging_format             | 6.72 us                                                     | 6.67 us: 1.01x faster                                                                 |
| logging_simple             | 6.28 us                                                     | 6.23 us: 1.01x faster                                                                 |
| bench_mp_pool              | 69.2 ms                                                     | 68.7 ms: 1.01x faster                                                                 |
| sqlglot_normalize          | 187 ms                                                      | 186 ms: 1.01x faster                                                                  |
| xml_etree_process          | 37.7 ms                                                     | 38.0 ms: 1.01x slower                                                                 |
| go                         | 91.6 ms                                                     | 92.3 ms: 1.01x slower                                                                 |
| pickle_dict                | 18.4 us                                                     | 18.6 us: 1.01x slower                                                                 |
| nqueens                    | 62.8 ms                                                     | 63.5 ms: 1.01x slower                                                                 |
| async_tree_none_tg         | 285 ms                                                      | 289 ms: 1.01x slower                                                                  |
| async_tree_io_tg           | 771 ms                                                      | 783 ms: 1.01x slower                                                                  |
| sqlglot_optimize           | 34.5 ms                                                     | 35.1 ms: 1.02x slower                                                                 |
| async_tree_io              | 731 ms                                                      | 744 ms: 1.02x slower                                                                  |
| chaos                      | 43.3 ms                                                     | 44.1 ms: 1.02x slower                                                                 |
| unpickle_list              | 2.75 us                                                     | 2.81 us: 1.02x slower                                                                 |
| float                      | 56.8 ms                                                     | 58.1 ms: 1.02x slower                                                                 |
| pprint_safe_repr           | 513 ms                                                      | 527 ms: 1.03x slower                                                                  |
| sympy_integrate            | 13.0 ms                                                     | 13.3 ms: 1.03x slower                                                                 |
| unpickle_pure_python       | 133 us                                                      | 137 us: 1.03x slower                                                                  |
| 2to3                       | 218 ms                                                      | 224 ms: 1.03x slower                                                                  |
| pickle_list                | 2.83 us                                                     | 2.91 us: 1.03x slower                                                                 |
| async_tree_memoization     | 339 ms                                                      | 350 ms: 1.03x slower                                                                  |
| unpickle                   | 8.18 us                                                     | 8.45 us: 1.03x slower                                                                 |
| unpack_sequence            | 37.5 ns                                                     | 38.7 ns: 1.03x slower                                                                 |
| xml_etree_parse            | 93.0 ms                                                     | 96.9 ms: 1.04x slower                                                                 |
| pprint_pformat             | 1.05 sec                                                    | 1.09 sec: 1.04x slower                                                                |
| mdp                        | 1.37 sec                                                    | 1.44 sec: 1.05x slower                                                                |
| meteor_contest             | 74.6 ms                                                     | 78.7 ms: 1.05x slower                                                                 |
| xml_etree_iterparse        | 65.2 ms                                                     | 69.1 ms: 1.06x slower                                                                 |
| python_startup             | 19.5 ms                                                     | 20.6 ms: 1.06x slower                                                                 |
| tomli_loads                | 1.37 sec                                                    | 1.46 sec: 1.06x slower                                                                |
| regex_v8                   | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                                 |
| fannkuch                   | 247 ms                                                      | 268 ms: 1.09x slower                                                                  |
| json                       | 3.05 ms                                                     | 3.34 ms: 1.09x slower                                                                 |
| nbody                      | 71.9 ms                                                     | 78.8 ms: 1.10x slower                                                                 |
| scimark_monte_carlo        | 43.7 ms                                                     | 48.2 ms: 1.10x slower                                                                 |
| coverage                   | 40.8 ms                                                     | 45.0 ms: 1.10x slower                                                                 |
| pyflate                    | 295 ms                                                      | 329 ms: 1.12x slower                                                                  |
| mako                       | 7.09 ms                                                     | 7.99 ms: 1.13x slower                                                                 |
| python_startup_no_site     | 16.2 ms                                                     | 18.4 ms: 1.13x slower                                                                 |
| scimark_fft                | 184 ms                                                      | 209 ms: 1.13x slower                                                                  |
| telco                      | 4.13 ms                                                     | 4.74 ms: 1.15x slower                                                                 |
| spectral_norm              | 66.9 ms                                                     | 80.3 ms: 1.20x slower                                                                 |
| hexiom                     | 4.10 ms                                                     | 5.01 ms: 1.22x slower                                                                 |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 3.19 ms: 1.25x slower                                                                 |
| deltablue                  | 2.16 ms                                                     | 2.74 ms: 1.27x slower                                                                 |
| Geometric mean             | (ref)                                                       | 1.00x slower                                                                          |

Benchmark hidden because not significant (8): async_tree_memoization_tg, xml_etree_generate, create_gc_cycles, gc_traversal, dask, bench_thread_pool, chameleon, asyncio_tcp
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 69.50% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown