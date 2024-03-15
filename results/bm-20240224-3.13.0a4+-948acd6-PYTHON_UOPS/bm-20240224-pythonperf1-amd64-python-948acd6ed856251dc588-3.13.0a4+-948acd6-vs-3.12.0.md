
# Results vs. 3.12.0

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-amd64
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.04x slower \*
- HPT reliability: 99.90%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 225 ms: 1.03x slower                                                        |
| chameleon      | 4.98 ms                                                     | 5.07 ms: 1.02x slower                                                       |
| tornado_http   | 89.5 ms                                                     | 86.2 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.00x slower                                                                |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 467 ms: 1.08x faster                                                        |
| async_tree_none            | 291 ms                                                      | 271 ms: 1.07x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 458 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 276 ms: 1.03x faster                                                        |
| async_tree_memoization     | 339 ms                                                      | 345 ms: 1.02x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (2): async_tree_io_tg, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 147 ms: 1.04x faster                                                        |
| float          | 56.8 ms                                                     | 59.0 ms: 1.04x slower                                                       |
| nbody          | 71.9 ms                                                     | 81.4 ms: 1.13x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 118 ms: 1.07x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 16.6 ms: 1.16x slower                                                       |
| regex_compile  | 87.5 ms                                                     | 102 ms: 1.17x slower                                                        |
| Geometric mean | (ref)                                                       | 1.05x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 7.03 us: 1.06x faster                                                       |
| pickle_pure_python   | 195 us                                                      | 186 us: 1.05x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 56.8 ms: 1.02x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.32 us: 1.02x slower                                                       |
| xml_etree_process    | 37.7 ms                                                     | 38.8 ms: 1.03x slower                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 68.6 ms: 1.05x slower                                                       |
| pickle_list          | 2.83 us                                                     | 3.20 us: 1.13x slower                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.58 sec: 1.15x slower                                                      |
| unpickle_pure_python | 133 us                                                      | 168 us: 1.26x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.04x slower                                                                |

Benchmark hidden because not significant (5): json_loads, xml_etree_parse, json_dumps, unpickle_list, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 19.9 ms: 1.02x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 17.9 ms: 1.10x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.55 ms: 1.07x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 75.3 us: 1.26x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.76 sec: 1.19x faster                                                      |
| mypy2                      | 509 ms                                                      | 445 ms: 1.15x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.60 us: 1.10x faster                                                       |
| generators                 | 22.5 ms                                                     | 20.6 ms: 1.09x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.2 ms: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 467 ms: 1.08x faster                                                        |
| async_tree_none            | 291 ms                                                      | 271 ms: 1.07x faster                                                        |
| regex_dna                  | 126 ms                                                      | 118 ms: 1.07x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 458 ms: 1.07x faster                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 65.0 ms: 1.06x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 56.9 ns: 1.06x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.03 us: 1.06x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 186 us: 1.05x faster                                                        |
| pathlib                    | 80.5 ms                                                     | 76.8 ms: 1.05x faster                                                       |
| json                       | 3.05 ms                                                     | 2.91 ms: 1.05x faster                                                       |
| asyncio_tcp                | 487 ms                                                      | 466 ms: 1.04x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                        |
| deepcopy_reduce            | 2.09 us                                                     | 2.01 us: 1.04x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 86.2 ms: 1.04x faster                                                       |
| pidigits                   | 152 ms                                                      | 147 ms: 1.04x faster                                                        |
| regex_effbot               | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| async_tree_none_tg         | 285 ms                                                      | 276 ms: 1.03x faster                                                        |
| create_gc_cycles           | 752 us                                                      | 738 us: 1.02x faster                                                        |
| deepcopy                   | 238 us                                                      | 234 us: 1.02x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 43.6 ms: 1.02x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 47.9 ms: 1.01x faster                                                       |
| async_generators           | 239 ms                                                      | 237 ms: 1.01x faster                                                        |
| gc_traversal               | 1.52 ms                                                     | 1.51 ms: 1.01x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 189 ms: 1.01x slower                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 56.8 ms: 1.02x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.32 us: 1.02x slower                                                       |
| chameleon                  | 4.98 ms                                                     | 5.07 ms: 1.02x slower                                                       |
| async_tree_memoization     | 339 ms                                                      | 345 ms: 1.02x slower                                                        |
| logging_format             | 6.72 us                                                     | 6.86 us: 1.02x slower                                                       |
| logging_simple             | 6.28 us                                                     | 6.42 us: 1.02x slower                                                       |
| sympy_str                  | 175 ms                                                      | 179 ms: 1.02x slower                                                        |
| python_startup             | 19.5 ms                                                     | 19.9 ms: 1.02x slower                                                       |
| comprehensions             | 14.1 us                                                     | 14.5 us: 1.03x slower                                                       |
| sympy_sum                  | 91.5 ms                                                     | 94.0 ms: 1.03x slower                                                       |
| xml_etree_process          | 37.7 ms                                                     | 38.8 ms: 1.03x slower                                                       |
| meteor_contest             | 74.6 ms                                                     | 76.9 ms: 1.03x slower                                                       |
| 2to3                       | 218 ms                                                      | 225 ms: 1.03x slower                                                        |
| sqlglot_parse              | 804 us                                                      | 835 us: 1.04x slower                                                        |
| float                      | 56.8 ms                                                     | 59.0 ms: 1.04x slower                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 1.06 ms: 1.04x slower                                                       |
| deepcopy_memo              | 23.7 us                                                     | 24.8 us: 1.04x slower                                                       |
| raytrace                   | 192 ms                                                      | 202 ms: 1.05x slower                                                        |
| xml_etree_iterparse        | 65.2 ms                                                     | 68.6 ms: 1.05x slower                                                       |
| chaos                      | 43.3 ms                                                     | 45.7 ms: 1.05x slower                                                       |
| sympy_expand               | 284 ms                                                      | 300 ms: 1.06x slower                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 36.6 ms: 1.06x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.46 sec: 1.07x slower                                                      |
| mako                       | 7.09 ms                                                     | 7.55 ms: 1.07x slower                                                       |
| pycparser                  | 699 ms                                                      | 746 ms: 1.07x slower                                                        |
| sympy_integrate            | 13.0 ms                                                     | 14.1 ms: 1.08x slower                                                       |
| deltablue                  | 2.16 ms                                                     | 2.35 ms: 1.09x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 17.9 ms: 1.10x slower                                                       |
| fannkuch                   | 247 ms                                                      | 273 ms: 1.11x slower                                                        |
| pprint_safe_repr           | 513 ms                                                      | 569 ms: 1.11x slower                                                        |
| richards_super             | 32.1 ms                                                     | 35.7 ms: 1.11x slower                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.17 sec: 1.12x slower                                                      |
| richards                   | 28.4 ms                                                     | 31.9 ms: 1.12x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 42.4 ns: 1.13x slower                                                       |
| nbody                      | 71.9 ms                                                     | 81.4 ms: 1.13x slower                                                       |
| pickle_list                | 2.83 us                                                     | 3.20 us: 1.13x slower                                                       |
| nqueens                    | 62.8 ms                                                     | 71.4 ms: 1.14x slower                                                       |
| go                         | 91.6 ms                                                     | 104 ms: 1.14x slower                                                        |
| tomli_loads                | 1.37 sec                                                    | 1.58 sec: 1.15x slower                                                      |
| coverage                   | 40.8 ms                                                     | 47.5 ms: 1.16x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 16.6 ms: 1.16x slower                                                       |
| regex_compile              | 87.5 ms                                                     | 102 ms: 1.17x slower                                                        |
| telco                      | 4.13 ms                                                     | 4.85 ms: 1.18x slower                                                       |
| scimark_fft                | 184 ms                                                      | 219 ms: 1.19x slower                                                        |
| scimark_sor                | 78.8 ms                                                     | 94.1 ms: 1.19x slower                                                       |
| pyflate                    | 295 ms                                                      | 352 ms: 1.20x slower                                                        |
| spectral_norm              | 66.9 ms                                                     | 83.5 ms: 1.25x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 54.7 ms: 1.25x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 3.22 ms: 1.26x slower                                                       |
| unpickle_pure_python       | 133 us                                                      | 168 us: 1.26x slower                                                        |
| hexiom                     | 4.10 ms                                                     | 5.61 ms: 1.37x slower                                                       |
| scimark_lu                 | 58.9 ms                                                     | 81.1 ms: 1.38x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.04x slower                                                                |

Benchmark hidden because not significant (9): async_tree_io_tg, json_loads, xml_etree_parse, async_tree_io, json_dumps, unpickle_list, pickle_dict, docutils, bench_thread_pool
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.90% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown