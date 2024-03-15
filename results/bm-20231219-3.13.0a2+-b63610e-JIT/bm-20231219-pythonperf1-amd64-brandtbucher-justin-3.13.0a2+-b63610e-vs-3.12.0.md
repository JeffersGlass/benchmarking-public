
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin
- machine: windows-amd64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.02x faster
- HPT reliability: 99.97%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 219 ms: 1.01x slower                                                |
| chameleon      | 4.98 ms                                                     | 4.86 ms: 1.03x faster                                               |
| docutils       | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                              |
| Geometric mean | (ref)                                                       | 1.02x faster                                                        |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 263 ms: 1.11x faster                                                |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 449 ms: 1.09x faster                                                |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 464 ms: 1.08x faster                                                |
| async_tree_none_tg         | 285 ms                                                      | 271 ms: 1.05x faster                                                |
| async_tree_memoization_tg  | 367 ms                                                      | 354 ms: 1.04x faster                                                |
| async_tree_io_tg           | 771 ms                                                      | 745 ms: 1.03x faster                                                |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                        |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 61.9 ms: 1.16x faster                                               |
| float          | 56.8 ms                                                     | 51.4 ms: 1.11x faster                                               |
| Geometric mean | (ref)                                                       | 1.09x faster                                                        |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 83.8 ms: 1.04x faster                                               |
| regex_dna      | 126 ms                                                      | 122 ms: 1.04x faster                                                |
| regex_effbot   | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                               |
| regex_v8       | 14.2 ms                                                     | 15.5 ms: 1.09x slower                                               |
| Geometric mean | (ref)                                                       | 1.00x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 179 us: 1.09x faster                                                |
| xml_etree_generate   | 55.8 ms                                                     | 52.8 ms: 1.06x faster                                               |
| pickle_dict          | 18.4 us                                                     | 17.6 us: 1.05x faster                                               |
| xml_etree_process    | 37.7 ms                                                     | 36.2 ms: 1.04x faster                                               |
| json_loads           | 13.9 us                                                     | 13.4 us: 1.04x faster                                               |
| tomli_loads          | 1.37 sec                                                    | 1.32 sec: 1.04x faster                                              |
| pickle               | 7.43 us                                                     | 7.20 us: 1.03x faster                                               |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.7 ms: 1.02x faster                                               |
| json_dumps           | 5.70 ms                                                     | 5.61 ms: 1.02x faster                                               |
| unpickle_list        | 2.75 us                                                     | 2.72 us: 1.01x faster                                               |
| unpickle_pure_python | 133 us                                                      | 133 us: 1.00x faster                                                |
| unpickle             | 8.18 us                                                     | 8.34 us: 1.02x slower                                               |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                        |

Benchmark hidden because not significant (2): pickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 21.0 ms: 1.08x slower                                               |
| python_startup_no_site | 16.2 ms                                                     | 19.1 ms: 1.18x slower                                               |
| Geometric mean         | (ref)                                                       | 1.13x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.59 ms: 1.08x faster                                               |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231219-pythonperf1-amd64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 72.2 us: 1.32x faster                                               |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.68 sec: 1.25x faster                                              |
| comprehensions             | 14.1 us                                                     | 11.6 us: 1.22x faster                                               |
| mypy2                      | 509 ms                                                      | 432 ms: 1.18x faster                                                |
| nbody                      | 71.9 ms                                                     | 61.9 ms: 1.16x faster                                               |
| sqlite_synth               | 1.76 us                                                     | 1.55 us: 1.13x faster                                               |
| async_tree_none            | 291 ms                                                      | 263 ms: 1.11x faster                                                |
| float                      | 56.8 ms                                                     | 51.4 ms: 1.11x faster                                               |
| coroutines                 | 14.3 ms                                                     | 12.9 ms: 1.10x faster                                               |
| logging_silent             | 60.5 ns                                                     | 55.0 ns: 1.10x faster                                               |
| deepcopy_reduce            | 2.09 us                                                     | 1.91 us: 1.10x faster                                               |
| pickle_pure_python         | 195 us                                                      | 179 us: 1.09x faster                                                |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 449 ms: 1.09x faster                                                |
| deepcopy                   | 238 us                                                      | 219 us: 1.09x faster                                                |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 464 ms: 1.08x faster                                                |
| mako                       | 7.09 ms                                                     | 6.59 ms: 1.08x faster                                               |
| richards                   | 28.4 ms                                                     | 26.6 ms: 1.07x faster                                               |
| raytrace                   | 192 ms                                                      | 180 ms: 1.07x faster                                                |
| json                       | 3.05 ms                                                     | 2.87 ms: 1.06x faster                                               |
| xml_etree_generate         | 55.8 ms                                                     | 52.8 ms: 1.06x faster                                               |
| async_tree_none_tg         | 285 ms                                                      | 271 ms: 1.05x faster                                                |
| dulwich_log                | 44.3 ms                                                     | 42.2 ms: 1.05x faster                                               |
| scimark_lu                 | 58.9 ms                                                     | 56.2 ms: 1.05x faster                                               |
| pickle_dict                | 18.4 us                                                     | 17.6 us: 1.05x faster                                               |
| sympy_sum                  | 91.5 ms                                                     | 87.4 ms: 1.05x faster                                               |
| deepcopy_memo              | 23.7 us                                                     | 22.7 us: 1.05x faster                                               |
| create_gc_cycles           | 752 us                                                      | 720 us: 1.04x faster                                                |
| regex_compile              | 87.5 ms                                                     | 83.8 ms: 1.04x faster                                               |
| docutils                   | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                              |
| sympy_str                  | 175 ms                                                      | 168 ms: 1.04x faster                                                |
| xml_etree_process          | 37.7 ms                                                     | 36.2 ms: 1.04x faster                                               |
| sqlglot_parse              | 804 us                                                      | 774 us: 1.04x faster                                                |
| bench_thread_pool          | 857 us                                                      | 825 us: 1.04x faster                                                |
| async_tree_memoization_tg  | 367 ms                                                      | 354 ms: 1.04x faster                                                |
| logging_format             | 6.72 us                                                     | 6.48 us: 1.04x faster                                               |
| json_loads                 | 13.9 us                                                     | 13.4 us: 1.04x faster                                               |
| regex_dna                  | 126 ms                                                      | 122 ms: 1.04x faster                                                |
| tomli_loads                | 1.37 sec                                                    | 1.32 sec: 1.04x faster                                              |
| crypto_pyaes               | 48.5 ms                                                     | 46.9 ms: 1.03x faster                                               |
| async_tree_io_tg           | 771 ms                                                      | 745 ms: 1.03x faster                                                |
| scimark_sor                | 78.8 ms                                                     | 76.2 ms: 1.03x faster                                               |
| asyncio_tcp                | 487 ms                                                      | 472 ms: 1.03x faster                                                |
| pickle                     | 7.43 us                                                     | 7.20 us: 1.03x faster                                               |
| nqueens                    | 62.8 ms                                                     | 60.9 ms: 1.03x faster                                               |
| logging_simple             | 6.28 us                                                     | 6.09 us: 1.03x faster                                               |
| sqlglot_transpile          | 1.02 ms                                                     | 994 us: 1.03x faster                                                |
| generators                 | 22.5 ms                                                     | 22.0 ms: 1.03x faster                                               |
| chameleon                  | 4.98 ms                                                     | 4.86 ms: 1.03x faster                                               |
| sqlglot_normalize          | 187 ms                                                      | 182 ms: 1.02x faster                                                |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.7 ms: 1.02x faster                                               |
| richards_super             | 32.1 ms                                                     | 31.4 ms: 1.02x faster                                               |
| json_dumps                 | 5.70 ms                                                     | 5.61 ms: 1.02x faster                                               |
| dask                       | 263 ms                                                      | 259 ms: 1.01x faster                                                |
| unpickle_list              | 2.75 us                                                     | 2.72 us: 1.01x faster                                               |
| pprint_safe_repr           | 513 ms                                                      | 508 ms: 1.01x faster                                                |
| regex_effbot               | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                               |
| gc_traversal               | 1.52 ms                                                     | 1.51 ms: 1.01x faster                                               |
| deltablue                  | 2.16 ms                                                     | 2.14 ms: 1.01x faster                                               |
| spectral_norm              | 66.9 ms                                                     | 66.4 ms: 1.01x faster                                               |
| chaos                      | 43.3 ms                                                     | 43.1 ms: 1.01x faster                                               |
| unpickle_pure_python       | 133 us                                                      | 133 us: 1.00x faster                                                |
| 2to3                       | 218 ms                                                      | 219 ms: 1.01x slower                                                |
| fannkuch                   | 247 ms                                                      | 249 ms: 1.01x slower                                                |
| pyflate                    | 295 ms                                                      | 298 ms: 1.01x slower                                                |
| unpickle                   | 8.18 us                                                     | 8.34 us: 1.02x slower                                               |
| sympy_integrate            | 13.0 ms                                                     | 13.3 ms: 1.02x slower                                               |
| async_generators           | 239 ms                                                      | 245 ms: 1.02x slower                                                |
| sqlglot_optimize           | 34.5 ms                                                     | 35.4 ms: 1.03x slower                                               |
| meteor_contest             | 74.6 ms                                                     | 76.6 ms: 1.03x slower                                               |
| bench_mp_pool              | 69.2 ms                                                     | 71.7 ms: 1.04x slower                                               |
| scimark_fft                | 184 ms                                                      | 193 ms: 1.05x slower                                                |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.68 ms: 1.05x slower                                               |
| scimark_monte_carlo        | 43.7 ms                                                     | 46.1 ms: 1.05x slower                                               |
| python_startup             | 19.5 ms                                                     | 21.0 ms: 1.08x slower                                               |
| regex_v8                   | 14.2 ms                                                     | 15.5 ms: 1.09x slower                                               |
| coverage                   | 40.8 ms                                                     | 45.4 ms: 1.11x slower                                               |
| telco                      | 4.13 ms                                                     | 4.59 ms: 1.11x slower                                               |
| go                         | 91.6 ms                                                     | 105 ms: 1.14x slower                                                |
| mdp                        | 1.37 sec                                                    | 1.58 sec: 1.15x slower                                              |
| python_startup_no_site     | 16.2 ms                                                     | 19.1 ms: 1.18x slower                                               |
| hexiom                     | 4.10 ms                                                     | 5.42 ms: 1.32x slower                                               |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                        |

Benchmark hidden because not significant (11): pickle_list, pycparser, async_tree_memoization, xml_etree_parse, tornado_http, pprint_pformat, sympy_expand, async_tree_io, pidigits, unpack_sequence, pathlib
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.97% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown