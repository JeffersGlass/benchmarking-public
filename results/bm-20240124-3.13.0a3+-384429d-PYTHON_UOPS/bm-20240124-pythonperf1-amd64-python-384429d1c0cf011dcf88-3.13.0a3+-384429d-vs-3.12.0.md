
# Results vs. 3.12.0

- fork: python
- ref: 384429d1c0cf011dcf88
- machine: windows-amd64
- commit hash: 384429d
- commit date: 2024-01-24
- overall geometric mean: 1.01x slower
- HPT reliability: 97.90%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 223 ms: 1.02x slower                                                        |
| chameleon      | 4.98 ms                                                     | 5.12 ms: 1.03x slower                                                       |
| docutils       | 1.66 sec                                                    | 1.62 sec: 1.02x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 88.3 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                       | 1.00x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 272 ms: 1.07x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 472 ms: 1.04x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 489 ms: 1.03x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 288 ms: 1.01x slower                                                        |
| async_tree_io_tg           | 771 ms                                                      | 783 ms: 1.01x slower                                                        |
| async_tree_io              | 731 ms                                                      | 742 ms: 1.01x slower                                                        |
| async_tree_memoization     | 339 ms                                                      | 349 ms: 1.03x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.01x faster                                                                |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 147 ms: 1.03x faster                                                        |
| float          | 56.8 ms                                                     | 56.3 ms: 1.01x faster                                                       |
| nbody          | 71.9 ms                                                     | 78.4 ms: 1.09x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 118 ms: 1.07x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.56 ms: 1.04x faster                                                       |
| regex_compile  | 87.5 ms                                                     | 84.4 ms: 1.04x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.7 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 183 us: 1.07x faster                                                        |
| unpickle_list        | 2.75 us                                                     | 2.65 us: 1.04x faster                                                       |
| pickle               | 7.43 us                                                     | 7.30 us: 1.02x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.8 us: 1.01x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 38.2 ms: 1.01x slower                                                       |
| pickle_dict          | 18.4 us                                                     | 18.7 us: 1.01x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.35 us: 1.02x slower                                                       |
| pickle_list          | 2.83 us                                                     | 2.89 us: 1.02x slower                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 95.2 ms: 1.02x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 137 us: 1.03x slower                                                        |
| tomli_loads          | 1.37 sec                                                    | 1.42 sec: 1.04x slower                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 68.2 ms: 1.05x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                                |

Benchmark hidden because not significant (2): json_dumps, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.5 ms: 1.05x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.3 ms: 1.12x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.24 ms: 1.02x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 75.7 us: 1.26x faster                                                       |
| mypy2                      | 509 ms                                                      | 434 ms: 1.17x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.58 us: 1.11x faster                                                       |
| raytrace                   | 192 ms                                                      | 174 ms: 1.10x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.90 sec: 1.10x faster                                                      |
| comprehensions             | 14.1 us                                                     | 13.0 us: 1.09x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.2 ms: 1.08x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 56.1 ns: 1.08x faster                                                       |
| regex_dna                  | 126 ms                                                      | 118 ms: 1.07x faster                                                        |
| async_tree_none            | 291 ms                                                      | 272 ms: 1.07x faster                                                        |
| pickle_pure_python         | 195 us                                                      | 183 us: 1.07x faster                                                        |
| sympy_str                  | 175 ms                                                      | 167 ms: 1.05x faster                                                        |
| deepcopy                   | 238 us                                                      | 228 us: 1.04x faster                                                        |
| deepcopy_reduce            | 2.09 us                                                     | 2.01 us: 1.04x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.56 ms: 1.04x faster                                                       |
| unpickle_list              | 2.75 us                                                     | 2.65 us: 1.04x faster                                                       |
| regex_compile              | 87.5 ms                                                     | 84.4 ms: 1.04x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 472 ms: 1.04x faster                                                        |
| richards_super             | 32.1 ms                                                     | 31.0 ms: 1.04x faster                                                       |
| pidigits                   | 152 ms                                                      | 147 ms: 1.03x faster                                                        |
| async_generators           | 239 ms                                                      | 232 ms: 1.03x faster                                                        |
| richards                   | 28.4 ms                                                     | 27.6 ms: 1.03x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 489 ms: 1.03x faster                                                        |
| sympy_sum                  | 91.5 ms                                                     | 89.2 ms: 1.03x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.62 sec: 1.02x faster                                                      |
| deepcopy_memo              | 23.7 us                                                     | 23.2 us: 1.02x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 183 ms: 1.02x faster                                                        |
| pickle                     | 7.43 us                                                     | 7.30 us: 1.02x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 43.5 ms: 1.02x faster                                                       |
| logging_simple             | 6.28 us                                                     | 6.18 us: 1.02x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 88.3 ms: 1.01x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 68.2 ms: 1.01x faster                                                       |
| float                      | 56.8 ms                                                     | 56.3 ms: 1.01x faster                                                       |
| json_loads                 | 13.9 us                                                     | 13.8 us: 1.01x faster                                                       |
| sympy_expand               | 284 ms                                                      | 285 ms: 1.01x slower                                                        |
| scimark_lu                 | 58.9 ms                                                     | 59.2 ms: 1.01x slower                                                       |
| sqlglot_parse              | 804 us                                                      | 810 us: 1.01x slower                                                        |
| go                         | 91.6 ms                                                     | 92.4 ms: 1.01x slower                                                       |
| meteor_contest             | 74.6 ms                                                     | 75.3 ms: 1.01x slower                                                       |
| gc_traversal               | 1.52 ms                                                     | 1.54 ms: 1.01x slower                                                       |
| async_tree_none_tg         | 285 ms                                                      | 288 ms: 1.01x slower                                                        |
| xml_etree_process          | 37.7 ms                                                     | 38.2 ms: 1.01x slower                                                       |
| pickle_dict                | 18.4 us                                                     | 18.7 us: 1.01x slower                                                       |
| async_tree_io_tg           | 771 ms                                                      | 783 ms: 1.01x slower                                                        |
| async_tree_io              | 731 ms                                                      | 742 ms: 1.01x slower                                                        |
| bench_thread_pool          | 857 us                                                      | 871 us: 1.02x slower                                                        |
| chaos                      | 43.3 ms                                                     | 44.1 ms: 1.02x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.35 us: 1.02x slower                                                       |
| 2to3                       | 218 ms                                                      | 223 ms: 1.02x slower                                                        |
| mako                       | 7.09 ms                                                     | 7.24 ms: 1.02x slower                                                       |
| pickle_list                | 2.83 us                                                     | 2.89 us: 1.02x slower                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 95.2 ms: 1.02x slower                                                       |
| pprint_safe_repr           | 513 ms                                                      | 525 ms: 1.02x slower                                                        |
| unpickle_pure_python       | 133 us                                                      | 137 us: 1.03x slower                                                        |
| chameleon                  | 4.98 ms                                                     | 5.12 ms: 1.03x slower                                                       |
| async_tree_memoization     | 339 ms                                                      | 349 ms: 1.03x slower                                                        |
| sympy_integrate            | 13.0 ms                                                     | 13.3 ms: 1.03x slower                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.08 sec: 1.03x slower                                                      |
| regex_v8                   | 14.2 ms                                                     | 14.7 ms: 1.03x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 35.6 ms: 1.03x slower                                                       |
| pycparser                  | 699 ms                                                      | 721 ms: 1.03x slower                                                        |
| nqueens                    | 62.8 ms                                                     | 64.9 ms: 1.03x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.42 sec: 1.04x slower                                                      |
| xml_etree_iterparse        | 65.2 ms                                                     | 68.2 ms: 1.05x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.44 sec: 1.05x slower                                                      |
| python_startup             | 19.5 ms                                                     | 20.5 ms: 1.05x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 39.9 ns: 1.07x slower                                                       |
| fannkuch                   | 247 ms                                                      | 264 ms: 1.07x slower                                                        |
| scimark_sor                | 78.8 ms                                                     | 84.4 ms: 1.07x slower                                                       |
| nbody                      | 71.9 ms                                                     | 78.4 ms: 1.09x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 47.8 ms: 1.09x slower                                                       |
| pyflate                    | 295 ms                                                      | 326 ms: 1.11x slower                                                        |
| scimark_fft                | 184 ms                                                      | 207 ms: 1.12x slower                                                        |
| python_startup_no_site     | 16.2 ms                                                     | 18.3 ms: 1.12x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.67 ms: 1.13x slower                                                       |
| coverage                   | 40.8 ms                                                     | 47.7 ms: 1.17x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 4.85 ms: 1.18x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 3.05 ms: 1.19x slower                                                       |
| spectral_norm              | 66.9 ms                                                     | 81.0 ms: 1.21x slower                                                       |
| deltablue                  | 2.16 ms                                                     | 2.68 ms: 1.24x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.01x slower                                                                |

Benchmark hidden because not significant (12): create_gc_cycles, logging_format, async_tree_memoization_tg, json_dumps, pathlib, crypto_pyaes, generators, xml_etree_generate, sqlglot_transpile, dask, asyncio_tcp, json
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 97.90% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown