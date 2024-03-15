
# Results vs. 3.12.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.02x faster
- HPT reliability: 99.08%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 224 ms: 1.03x slower                                                                  |
| chameleon      | 4.98 ms                                                     | 4.77 ms: 1.04x faster                                                                 |
| docutils       | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                                |
| tornado_http   | 89.5 ms                                                     | 86.7 ms: 1.03x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 489 ms                                                      | 455 ms: 1.07x faster                                                                  |
| async_tree_none            | 291 ms                                                      | 272 ms: 1.07x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 483 ms: 1.04x faster                                                                  |
| async_tree_memoization_tg  | 367 ms                                                      | 356 ms: 1.03x faster                                                                  |
| async_tree_memoization     | 339 ms                                                      | 346 ms: 1.02x slower                                                                  |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                                          |

Benchmark hidden because not significant (3): async_tree_none_tg, async_tree_io, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 62.2 ms: 1.15x faster                                                                 |
| float          | 56.8 ms                                                     | 52.1 ms: 1.09x faster                                                                 |
| pidigits       | 152 ms                                                      | 154 ms: 1.01x slower                                                                  |
| Geometric mean | (ref)                                                       | 1.08x faster                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 82.7 ms: 1.06x faster                                                                 |
| regex_dna      | 126 ms                                                      | 122 ms: 1.03x faster                                                                  |
| regex_effbot   | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                                                 |
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.02x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 177 us: 1.11x faster                                                                  |
| xml_etree_generate   | 55.8 ms                                                     | 52.2 ms: 1.07x faster                                                                 |
| tomli_loads          | 1.37 sec                                                    | 1.28 sec: 1.06x faster                                                                |
| xml_etree_process    | 37.7 ms                                                     | 35.8 ms: 1.05x faster                                                                 |
| json_dumps           | 5.70 ms                                                     | 5.44 ms: 1.05x faster                                                                 |
| pickle_dict          | 18.4 us                                                     | 17.7 us: 1.04x faster                                                                 |
| json_loads           | 13.9 us                                                     | 13.5 us: 1.03x faster                                                                 |
| unpickle_pure_python | 133 us                                                      | 131 us: 1.02x faster                                                                  |
| pickle               | 7.43 us                                                     | 7.31 us: 1.02x faster                                                                 |
| xml_etree_parse      | 93.0 ms                                                     | 95.2 ms: 1.02x slower                                                                 |
| unpickle             | 8.18 us                                                     | 8.44 us: 1.03x slower                                                                 |
| unpickle_list        | 2.75 us                                                     | 2.84 us: 1.03x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                                          |

Benchmark hidden because not significant (2): xml_etree_iterparse, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 21.1 ms: 1.08x slower                                                                 |
| python_startup_no_site | 16.2 ms                                                     | 19.1 ms: 1.18x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.13x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.86 ms: 1.03x faster                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 68.1 us: 1.40x faster                                                                 |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.52 sec: 1.37x faster                                                                |
| comprehensions             | 14.1 us                                                     | 11.7 us: 1.21x faster                                                                 |
| mypy2                      | 509 ms                                                      | 435 ms: 1.17x faster                                                                  |
| logging_silent             | 60.5 ns                                                     | 52.2 ns: 1.16x faster                                                                 |
| nbody                      | 71.9 ms                                                     | 62.2 ms: 1.15x faster                                                                 |
| richards                   | 28.4 ms                                                     | 24.9 ms: 1.14x faster                                                                 |
| sqlite_synth               | 1.76 us                                                     | 1.56 us: 1.13x faster                                                                 |
| richards_super             | 32.1 ms                                                     | 28.3 ms: 1.13x faster                                                                 |
| raytrace                   | 192 ms                                                      | 172 ms: 1.12x faster                                                                  |
| deepcopy_memo              | 23.7 us                                                     | 21.2 us: 1.12x faster                                                                 |
| pickle_pure_python         | 195 us                                                      | 177 us: 1.11x faster                                                                  |
| float                      | 56.8 ms                                                     | 52.1 ms: 1.09x faster                                                                 |
| deepcopy                   | 238 us                                                      | 218 us: 1.09x faster                                                                  |
| deepcopy_reduce            | 2.09 us                                                     | 1.93 us: 1.08x faster                                                                 |
| generators                 | 22.5 ms                                                     | 20.9 ms: 1.08x faster                                                                 |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 455 ms: 1.07x faster                                                                  |
| async_tree_none            | 291 ms                                                      | 272 ms: 1.07x faster                                                                  |
| xml_etree_generate         | 55.8 ms                                                     | 52.2 ms: 1.07x faster                                                                 |
| scimark_lu                 | 58.9 ms                                                     | 55.2 ms: 1.07x faster                                                                 |
| tomli_loads                | 1.37 sec                                                    | 1.28 sec: 1.06x faster                                                                |
| spectral_norm              | 66.9 ms                                                     | 62.9 ms: 1.06x faster                                                                 |
| sqlglot_parse              | 804 us                                                      | 760 us: 1.06x faster                                                                  |
| regex_compile              | 87.5 ms                                                     | 82.7 ms: 1.06x faster                                                                 |
| xml_etree_process          | 37.7 ms                                                     | 35.8 ms: 1.05x faster                                                                 |
| coroutines                 | 14.3 ms                                                     | 13.5 ms: 1.05x faster                                                                 |
| nqueens                    | 62.8 ms                                                     | 59.7 ms: 1.05x faster                                                                 |
| dulwich_log                | 44.3 ms                                                     | 42.2 ms: 1.05x faster                                                                 |
| json_dumps                 | 5.70 ms                                                     | 5.44 ms: 1.05x faster                                                                 |
| docutils                   | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                                |
| chameleon                  | 4.98 ms                                                     | 4.77 ms: 1.04x faster                                                                 |
| logging_simple             | 6.28 us                                                     | 6.02 us: 1.04x faster                                                                 |
| pickle_dict                | 18.4 us                                                     | 17.7 us: 1.04x faster                                                                 |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 483 ms: 1.04x faster                                                                  |
| sqlglot_normalize          | 187 ms                                                      | 180 ms: 1.04x faster                                                                  |
| sqlglot_transpile          | 1.02 ms                                                     | 984 us: 1.04x faster                                                                  |
| logging_format             | 6.72 us                                                     | 6.48 us: 1.04x faster                                                                 |
| mako                       | 7.09 ms                                                     | 6.86 ms: 1.03x faster                                                                 |
| regex_dna                  | 126 ms                                                      | 122 ms: 1.03x faster                                                                  |
| tornado_http               | 89.5 ms                                                     | 86.7 ms: 1.03x faster                                                                 |
| sympy_str                  | 175 ms                                                      | 170 ms: 1.03x faster                                                                  |
| async_tree_memoization_tg  | 367 ms                                                      | 356 ms: 1.03x faster                                                                  |
| deltablue                  | 2.16 ms                                                     | 2.10 ms: 1.03x faster                                                                 |
| pprint_safe_repr           | 513 ms                                                      | 498 ms: 1.03x faster                                                                  |
| json_loads                 | 13.9 us                                                     | 13.5 us: 1.03x faster                                                                 |
| regex_effbot               | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                                                 |
| unpickle_pure_python       | 133 us                                                      | 131 us: 1.02x faster                                                                  |
| chaos                      | 43.3 ms                                                     | 42.5 ms: 1.02x faster                                                                 |
| sympy_expand               | 284 ms                                                      | 279 ms: 1.02x faster                                                                  |
| pickle                     | 7.43 us                                                     | 7.31 us: 1.02x faster                                                                 |
| scimark_sor                | 78.8 ms                                                     | 77.6 ms: 1.02x faster                                                                 |
| crypto_pyaes               | 48.5 ms                                                     | 47.9 ms: 1.01x faster                                                                 |
| sympy_sum                  | 91.5 ms                                                     | 90.7 ms: 1.01x faster                                                                 |
| pathlib                    | 80.5 ms                                                     | 79.8 ms: 1.01x faster                                                                 |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                                                 |
| async_generators           | 239 ms                                                      | 242 ms: 1.01x slower                                                                  |
| pidigits                   | 152 ms                                                      | 154 ms: 1.01x slower                                                                  |
| fannkuch                   | 247 ms                                                      | 251 ms: 1.02x slower                                                                  |
| async_tree_memoization     | 339 ms                                                      | 346 ms: 1.02x slower                                                                  |
| regex_v8                   | 14.2 ms                                                     | 14.6 ms: 1.02x slower                                                                 |
| xml_etree_parse            | 93.0 ms                                                     | 95.2 ms: 1.02x slower                                                                 |
| 2to3                       | 218 ms                                                      | 224 ms: 1.03x slower                                                                  |
| unpickle                   | 8.18 us                                                     | 8.44 us: 1.03x slower                                                                 |
| bench_mp_pool              | 69.2 ms                                                     | 71.4 ms: 1.03x slower                                                                 |
| unpickle_list              | 2.75 us                                                     | 2.84 us: 1.03x slower                                                                 |
| unpack_sequence            | 37.5 ns                                                     | 39.1 ns: 1.04x slower                                                                 |
| scimark_fft                | 184 ms                                                      | 195 ms: 1.06x slower                                                                  |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.72 ms: 1.06x slower                                                                 |
| go                         | 91.6 ms                                                     | 97.4 ms: 1.06x slower                                                                 |
| sympy_integrate            | 13.0 ms                                                     | 13.9 ms: 1.07x slower                                                                 |
| meteor_contest             | 74.6 ms                                                     | 80.1 ms: 1.07x slower                                                                 |
| pyflate                    | 295 ms                                                      | 316 ms: 1.07x slower                                                                  |
| python_startup             | 19.5 ms                                                     | 21.1 ms: 1.08x slower                                                                 |
| json                       | 3.05 ms                                                     | 3.33 ms: 1.09x slower                                                                 |
| telco                      | 4.13 ms                                                     | 4.59 ms: 1.11x slower                                                                 |
| coverage                   | 40.8 ms                                                     | 45.8 ms: 1.12x slower                                                                 |
| python_startup_no_site     | 16.2 ms                                                     | 19.1 ms: 1.18x slower                                                                 |
| mdp                        | 1.37 sec                                                    | 1.62 sec: 1.18x slower                                                                |
| hexiom                     | 4.10 ms                                                     | 5.44 ms: 1.33x slower                                                                 |
| scimark_monte_carlo        | 43.7 ms                                                     | 58.3 ms: 1.33x slower                                                                 |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                                          |

Benchmark hidden because not significant (12): pprint_pformat, asyncio_tcp, create_gc_cycles, async_tree_none_tg, xml_etree_iterparse, gc_traversal, pickle_list, async_tree_io, bench_thread_pool, async_tree_io_tg, pycparser, dask
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.08% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown