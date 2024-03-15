
# Results vs. 3.12.0

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-amd64
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 210 ms: 1.04x faster                                                        |
| chameleon      | 4.98 ms                                                     | 4.81 ms: 1.03x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 85.8 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 275 ms: 1.06x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 465 ms: 1.05x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 477 ms: 1.05x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 279 ms: 1.02x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 359 ms: 1.02x faster                                                        |
| async_tree_io              | 731 ms                                                      | 751 ms: 1.03x slower                                                        |
| async_tree_memoization     | 339 ms                                                      | 353 ms: 1.04x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 53.5 ms: 1.06x faster                                                       |
| pidigits       | 152 ms                                                      | 149 ms: 1.02x faster                                                        |
| nbody          | 71.9 ms                                                     | 72.3 ms: 1.01x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 76.9 ms: 1.14x faster                                                       |
| regex_dna      | 126 ms                                                      | 118 ms: 1.07x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 17.1 ms: 1.20x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 185 us: 1.06x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 53.9 ms: 1.04x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.5 us: 1.03x faster                                                       |
| pickle               | 7.43 us                                                     | 7.25 us: 1.03x faster                                                       |
| unpickle_pure_python | 133 us                                                      | 130 us: 1.02x faster                                                        |
| xml_etree_process    | 37.7 ms                                                     | 37.0 ms: 1.02x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.63 ms: 1.01x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 18.6 us: 1.01x slower                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 94.1 ms: 1.01x slower                                                       |
| pickle_list          | 2.83 us                                                     | 2.88 us: 1.02x slower                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.43 sec: 1.05x slower                                                      |
| unpickle             | 8.18 us                                                     | 8.68 us: 1.06x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.00x faster                                                                |

Benchmark hidden because not significant (2): unpickle_list, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.4 ms: 1.05x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.3 ms: 1.13x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.65 ms: 1.07x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 73.1 us: 1.30x faster                                                       |
| comprehensions             | 14.1 us                                                     | 10.9 us: 1.30x faster                                                       |
| mypy2                      | 509 ms                                                      | 419 ms: 1.22x faster                                                        |
| raytrace                   | 192 ms                                                      | 166 ms: 1.16x faster                                                        |
| crypto_pyaes               | 48.5 ms                                                     | 42.3 ms: 1.15x faster                                                       |
| regex_compile              | 87.5 ms                                                     | 76.9 ms: 1.14x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.58 us: 1.12x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 83.1 ms: 1.10x faster                                                       |
| chaos                      | 43.3 ms                                                     | 39.6 ms: 1.09x faster                                                       |
| scimark_lu                 | 58.9 ms                                                     | 53.8 ms: 1.09x faster                                                       |
| sympy_str                  | 175 ms                                                      | 161 ms: 1.09x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 55.5 ns: 1.09x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.93 sec: 1.09x faster                                                      |
| spectral_norm              | 66.9 ms                                                     | 61.8 ms: 1.08x faster                                                       |
| deltablue                  | 2.16 ms                                                     | 2.01 ms: 1.07x faster                                                       |
| go                         | 91.6 ms                                                     | 85.5 ms: 1.07x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 41.4 ms: 1.07x faster                                                       |
| regex_dna                  | 126 ms                                                      | 118 ms: 1.07x faster                                                        |
| hexiom                     | 4.10 ms                                                     | 3.84 ms: 1.07x faster                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 41.0 ms: 1.07x faster                                                       |
| mako                       | 7.09 ms                                                     | 6.65 ms: 1.07x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                                      |
| coroutines                 | 14.3 ms                                                     | 13.4 ms: 1.06x faster                                                       |
| float                      | 56.8 ms                                                     | 53.5 ms: 1.06x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.97 us: 1.06x faster                                                       |
| async_tree_none            | 291 ms                                                      | 275 ms: 1.06x faster                                                        |
| generators                 | 22.5 ms                                                     | 21.3 ms: 1.06x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 185 us: 1.06x faster                                                        |
| deepcopy                   | 238 us                                                      | 226 us: 1.05x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 465 ms: 1.05x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 477 ms: 1.05x faster                                                        |
| fannkuch                   | 247 ms                                                      | 235 ms: 1.05x faster                                                        |
| deepcopy_memo              | 23.7 us                                                     | 22.6 us: 1.05x faster                                                       |
| sympy_integrate            | 13.0 ms                                                     | 12.4 ms: 1.05x faster                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.45 ms: 1.05x faster                                                       |
| scimark_fft                | 184 ms                                                      | 177 ms: 1.04x faster                                                        |
| sqlglot_normalize          | 187 ms                                                      | 179 ms: 1.04x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 85.8 ms: 1.04x faster                                                       |
| nqueens                    | 62.8 ms                                                     | 60.2 ms: 1.04x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 981 us: 1.04x faster                                                        |
| 2to3                       | 218 ms                                                      | 210 ms: 1.04x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 33.2 ms: 1.04x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.46 us: 1.04x faster                                                       |
| xml_etree_generate         | 55.8 ms                                                     | 53.9 ms: 1.04x faster                                                       |
| chameleon                  | 4.98 ms                                                     | 4.81 ms: 1.03x faster                                                       |
| richards_super             | 32.1 ms                                                     | 31.0 ms: 1.03x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 778 us: 1.03x faster                                                        |
| sympy_expand               | 284 ms                                                      | 276 ms: 1.03x faster                                                        |
| json_loads                 | 13.9 us                                                     | 13.5 us: 1.03x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.25 us: 1.03x faster                                                       |
| async_tree_none_tg         | 285 ms                                                      | 279 ms: 1.02x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 359 ms: 1.02x faster                                                        |
| unpickle_pure_python       | 133 us                                                      | 130 us: 1.02x faster                                                        |
| regex_effbot               | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 37.0 ms: 1.02x faster                                                       |
| pidigits                   | 152 ms                                                      | 149 ms: 1.02x faster                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 67.9 ms: 1.02x faster                                                       |
| logging_simple             | 6.28 us                                                     | 6.16 us: 1.02x faster                                                       |
| async_generators           | 239 ms                                                      | 235 ms: 1.02x faster                                                        |
| scimark_sor                | 78.8 ms                                                     | 77.4 ms: 1.02x faster                                                       |
| richards                   | 28.4 ms                                                     | 28.0 ms: 1.01x faster                                                       |
| dask                       | 263 ms                                                      | 259 ms: 1.01x faster                                                        |
| meteor_contest             | 74.6 ms                                                     | 73.7 ms: 1.01x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.63 ms: 1.01x faster                                                       |
| pyflate                    | 295 ms                                                      | 293 ms: 1.01x faster                                                        |
| nbody                      | 71.9 ms                                                     | 72.3 ms: 1.01x slower                                                       |
| pathlib                    | 80.5 ms                                                     | 81.0 ms: 1.01x slower                                                       |
| pickle_dict                | 18.4 us                                                     | 18.6 us: 1.01x slower                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 94.1 ms: 1.01x slower                                                       |
| pickle_list                | 2.83 us                                                     | 2.88 us: 1.02x slower                                                       |
| async_tree_io              | 731 ms                                                      | 751 ms: 1.03x slower                                                        |
| mdp                        | 1.37 sec                                                    | 1.42 sec: 1.03x slower                                                      |
| async_tree_memoization     | 339 ms                                                      | 353 ms: 1.04x slower                                                        |
| tomli_loads                | 1.37 sec                                                    | 1.43 sec: 1.05x slower                                                      |
| python_startup             | 19.5 ms                                                     | 20.4 ms: 1.05x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.68 us: 1.06x slower                                                       |
| json                       | 3.05 ms                                                     | 3.39 ms: 1.11x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 18.3 ms: 1.13x slower                                                       |
| coverage                   | 40.8 ms                                                     | 46.2 ms: 1.13x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.71 ms: 1.14x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 17.1 ms: 1.20x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.03x faster                                                                |

Benchmark hidden because not significant (11): pprint_safe_repr, async_tree_io_tg, gc_traversal, pprint_pformat, unpickle_list, unpack_sequence, bench_thread_pool, pycparser, xml_etree_iterparse, asyncio_tcp, create_gc_cycles
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown