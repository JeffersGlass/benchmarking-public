
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin
- machine: windows-amd64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.02x faster
- HPT reliability: 99.85%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 220 ms: 1.01x slower                                                |
| chameleon      | 4.98 ms                                                     | 4.91 ms: 1.01x faster                                               |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                              |
| tornado_http   | 89.5 ms                                                     | 86.0 ms: 1.04x faster                                               |
| Geometric mean | (ref)                                                       | 1.02x faster                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 273 ms: 1.07x faster                                                |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 459 ms: 1.07x faster                                                |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 485 ms: 1.03x faster                                                |
| async_tree_none_tg         | 285 ms                                                      | 280 ms: 1.02x faster                                                |
| async_tree_memoization     | 339 ms                                                      | 346 ms: 1.02x slower                                                |
| Geometric mean             | (ref)                                                       | 1.03x faster                                                        |

Benchmark hidden because not significant (2): async_tree_io_tg, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 60.8 ms: 1.18x faster                                               |
| float          | 56.8 ms                                                     | 50.4 ms: 1.13x faster                                               |
| pidigits       | 152 ms                                                      | 154 ms: 1.01x slower                                                |
| Geometric mean | (ref)                                                       | 1.10x faster                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 82.3 ms: 1.06x faster                                               |
| regex_dna      | 126 ms                                                      | 119 ms: 1.06x faster                                                |
| regex_effbot   | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                               |
| regex_v8       | 14.2 ms                                                     | 16.9 ms: 1.19x slower                                               |
| Geometric mean | (ref)                                                       | 1.01x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 176 us: 1.11x faster                                                |
| xml_etree_generate   | 55.8 ms                                                     | 52.5 ms: 1.06x faster                                               |
| xml_etree_process    | 37.7 ms                                                     | 36.6 ms: 1.03x faster                                               |
| json_dumps           | 5.70 ms                                                     | 5.56 ms: 1.03x faster                                               |
| json_loads           | 13.9 us                                                     | 13.6 us: 1.02x faster                                               |
| unpickle_pure_python | 133 us                                                      | 131 us: 1.02x faster                                                |
| pickle               | 7.43 us                                                     | 7.35 us: 1.01x faster                                               |
| xml_etree_iterparse  | 65.2 ms                                                     | 64.6 ms: 1.01x faster                                               |
| pickle_dict          | 18.4 us                                                     | 18.6 us: 1.01x slower                                               |
| xml_etree_parse      | 93.0 ms                                                     | 94.6 ms: 1.02x slower                                               |
| pickle_list          | 2.83 us                                                     | 2.96 us: 1.05x slower                                               |
| unpickle             | 8.18 us                                                     | 8.61 us: 1.05x slower                                               |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                        |

Benchmark hidden because not significant (2): tomli_loads, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 21.0 ms: 1.08x slower                                               |
| python_startup_no_site | 16.2 ms                                                     | 19.1 ms: 1.17x slower                                               |
| Geometric mean         | (ref)                                                       | 1.13x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.98 ms: 1.02x faster                                               |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 72.1 us: 1.32x faster                                               |
| comprehensions             | 14.1 us                                                     | 11.4 us: 1.24x faster                                               |
| nbody                      | 71.9 ms                                                     | 60.8 ms: 1.18x faster                                               |
| mypy2                      | 509 ms                                                      | 436 ms: 1.17x faster                                                |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.82 sec: 1.15x faster                                              |
| sqlite_synth               | 1.76 us                                                     | 1.56 us: 1.13x faster                                               |
| float                      | 56.8 ms                                                     | 50.4 ms: 1.13x faster                                               |
| generators                 | 22.5 ms                                                     | 20.1 ms: 1.12x faster                                               |
| richards_super             | 32.1 ms                                                     | 28.8 ms: 1.12x faster                                               |
| richards                   | 28.4 ms                                                     | 25.5 ms: 1.11x faster                                               |
| logging_silent             | 60.5 ns                                                     | 54.5 ns: 1.11x faster                                               |
| pickle_pure_python         | 195 us                                                      | 176 us: 1.11x faster                                                |
| raytrace                   | 192 ms                                                      | 175 ms: 1.10x faster                                                |
| coroutines                 | 14.3 ms                                                     | 13.0 ms: 1.10x faster                                               |
| deepcopy                   | 238 us                                                      | 221 us: 1.08x faster                                                |
| deepcopy_memo              | 23.7 us                                                     | 22.1 us: 1.07x faster                                               |
| deepcopy_reduce            | 2.09 us                                                     | 1.95 us: 1.07x faster                                               |
| async_tree_none            | 291 ms                                                      | 273 ms: 1.07x faster                                                |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 459 ms: 1.07x faster                                                |
| nqueens                    | 62.8 ms                                                     | 59.1 ms: 1.06x faster                                               |
| xml_etree_generate         | 55.8 ms                                                     | 52.5 ms: 1.06x faster                                               |
| regex_compile              | 87.5 ms                                                     | 82.3 ms: 1.06x faster                                               |
| regex_dna                  | 126 ms                                                      | 119 ms: 1.06x faster                                                |
| json                       | 3.05 ms                                                     | 2.88 ms: 1.06x faster                                               |
| scimark_lu                 | 58.9 ms                                                     | 55.9 ms: 1.05x faster                                               |
| sympy_str                  | 175 ms                                                      | 168 ms: 1.04x faster                                                |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                |
| deltablue                  | 2.16 ms                                                     | 2.08 ms: 1.04x faster                                               |
| sqlglot_normalize          | 187 ms                                                      | 180 ms: 1.04x faster                                                |
| tornado_http               | 89.5 ms                                                     | 86.0 ms: 1.04x faster                                               |
| logging_simple             | 6.28 us                                                     | 6.03 us: 1.04x faster                                               |
| logging_format             | 6.72 us                                                     | 6.47 us: 1.04x faster                                               |
| docutils                   | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                              |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 485 ms: 1.03x faster                                                |
| xml_etree_process          | 37.7 ms                                                     | 36.6 ms: 1.03x faster                                               |
| sympy_sum                  | 91.5 ms                                                     | 88.9 ms: 1.03x faster                                               |
| crypto_pyaes               | 48.5 ms                                                     | 47.2 ms: 1.03x faster                                               |
| sqlglot_parse              | 804 us                                                      | 784 us: 1.03x faster                                                |
| json_dumps                 | 5.70 ms                                                     | 5.56 ms: 1.03x faster                                               |
| spectral_norm              | 66.9 ms                                                     | 65.3 ms: 1.02x faster                                               |
| dulwich_log                | 44.3 ms                                                     | 43.2 ms: 1.02x faster                                               |
| json_loads                 | 13.9 us                                                     | 13.6 us: 1.02x faster                                               |
| regex_effbot               | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                               |
| unpickle_pure_python       | 133 us                                                      | 131 us: 1.02x faster                                                |
| pprint_safe_repr           | 513 ms                                                      | 504 ms: 1.02x faster                                                |
| async_tree_none_tg         | 285 ms                                                      | 280 ms: 1.02x faster                                                |
| mako                       | 7.09 ms                                                     | 6.98 ms: 1.02x faster                                               |
| chameleon                  | 4.98 ms                                                     | 4.91 ms: 1.01x faster                                               |
| sympy_expand               | 284 ms                                                      | 280 ms: 1.01x faster                                                |
| sqlglot_transpile          | 1.02 ms                                                     | 1.01 ms: 1.01x faster                                               |
| pickle                     | 7.43 us                                                     | 7.35 us: 1.01x faster                                               |
| xml_etree_iterparse        | 65.2 ms                                                     | 64.6 ms: 1.01x faster                                               |
| async_generators           | 239 ms                                                      | 241 ms: 1.01x slower                                                |
| 2to3                       | 218 ms                                                      | 220 ms: 1.01x slower                                                |
| pickle_dict                | 18.4 us                                                     | 18.6 us: 1.01x slower                                               |
| gc_traversal               | 1.52 ms                                                     | 1.54 ms: 1.01x slower                                               |
| pidigits                   | 152 ms                                                      | 154 ms: 1.01x slower                                                |
| xml_etree_parse            | 93.0 ms                                                     | 94.6 ms: 1.02x slower                                               |
| async_tree_memoization     | 339 ms                                                      | 346 ms: 1.02x slower                                                |
| sympy_integrate            | 13.0 ms                                                     | 13.3 ms: 1.02x slower                                               |
| pickle_list                | 2.83 us                                                     | 2.96 us: 1.05x slower                                               |
| unpickle                   | 8.18 us                                                     | 8.61 us: 1.05x slower                                               |
| unpack_sequence            | 37.5 ns                                                     | 39.5 ns: 1.05x slower                                               |
| meteor_contest             | 74.6 ms                                                     | 78.7 ms: 1.05x slower                                               |
| scimark_fft                | 184 ms                                                      | 196 ms: 1.06x slower                                                |
| go                         | 91.6 ms                                                     | 97.4 ms: 1.06x slower                                               |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.72 ms: 1.06x slower                                               |
| python_startup             | 19.5 ms                                                     | 21.0 ms: 1.08x slower                                               |
| pyflate                    | 295 ms                                                      | 320 ms: 1.08x slower                                                |
| telco                      | 4.13 ms                                                     | 4.58 ms: 1.11x slower                                               |
| coverage                   | 40.8 ms                                                     | 45.7 ms: 1.12x slower                                               |
| mdp                        | 1.37 sec                                                    | 1.55 sec: 1.13x slower                                              |
| python_startup_no_site     | 16.2 ms                                                     | 19.1 ms: 1.17x slower                                               |
| regex_v8                   | 14.2 ms                                                     | 16.9 ms: 1.19x slower                                               |
| hexiom                     | 4.10 ms                                                     | 5.29 ms: 1.29x slower                                               |
| scimark_monte_carlo        | 43.7 ms                                                     | 58.7 ms: 1.34x slower                                               |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                        |

Benchmark hidden because not significant (16): tomli_loads, pathlib, async_tree_io_tg, async_tree_io, asyncio_tcp, fannkuch, scimark_sor, bench_mp_pool, unpickle_list, pprint_pformat, create_gc_cycles, sqlglot_optimize, bench_thread_pool, pycparser, dask, chaos
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.85% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown