
# Results vs. 3.12.0

- fork: mdboom
- ref: aa_test
- machine: windows-amd64
- commit hash: aaf8974
- commit date: 2024-02-15
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 215 ms: 1.01x faster                                           |
| chameleon      | 4.98 ms                                                     | 4.78 ms: 1.04x faster                                          |
| docutils       | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                         |
| tornado_http   | 89.5 ms                                                     | 84.9 ms: 1.05x faster                                          |
| Geometric mean | (ref)                                                       | 1.04x faster                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 262 ms: 1.11x faster                                           |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 447 ms: 1.10x faster                                           |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 464 ms: 1.08x faster                                           |
| async_tree_memoization_tg  | 367 ms                                                      | 345 ms: 1.06x faster                                           |
| async_tree_none_tg         | 285 ms                                                      | 271 ms: 1.05x faster                                           |
| async_tree_io_tg           | 771 ms                                                      | 753 ms: 1.02x faster                                           |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                   |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 60.7 ms: 1.18x faster                                          |
| float          | 56.8 ms                                                     | 50.3 ms: 1.13x faster                                          |
| pidigits       | 152 ms                                                      | 152 ms: 1.00x faster                                           |
| Geometric mean | (ref)                                                       | 1.10x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 115 ms: 1.10x faster                                           |
| regex_compile  | 87.5 ms                                                     | 80.4 ms: 1.09x faster                                          |
| regex_effbot   | 1.62 ms                                                     | 1.56 ms: 1.04x faster                                          |
| regex_v8       | 14.2 ms                                                     | 14.4 ms: 1.01x slower                                          |
| Geometric mean | (ref)                                                       | 1.05x faster                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 175 us: 1.12x faster                                           |
| xml_etree_generate   | 55.8 ms                                                     | 52.0 ms: 1.07x faster                                          |
| pickle_dict          | 18.4 us                                                     | 17.4 us: 1.06x faster                                          |
| tomli_loads          | 1.37 sec                                                    | 1.30 sec: 1.05x faster                                         |
| unpickle_pure_python | 133 us                                                      | 127 us: 1.05x faster                                           |
| xml_etree_process    | 37.7 ms                                                     | 36.1 ms: 1.05x faster                                          |
| json_dumps           | 5.70 ms                                                     | 5.55 ms: 1.03x faster                                          |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.8 ms: 1.02x faster                                          |
| pickle               | 7.43 us                                                     | 7.31 us: 1.02x faster                                          |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.02x faster                                          |
| pickle_list          | 2.83 us                                                     | 2.78 us: 1.02x faster                                          |
| unpickle             | 8.18 us                                                     | 8.63 us: 1.05x slower                                          |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                   |

Benchmark hidden because not significant (2): xml_etree_parse, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.1 ms: 1.03x slower                                          |
| python_startup_no_site | 16.2 ms                                                     | 18.1 ms: 1.11x slower                                          |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|-----------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.71 ms: 1.06x faster                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-mdboom-aa_test-3.13.0a3+-aaf8974 |
|----------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 69.8 us: 1.36x faster                                          |
| comprehensions             | 14.1 us                                                     | 10.7 us: 1.32x faster                                          |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.65 sec: 1.27x faster                                         |
| mypy2                      | 509 ms                                                      | 422 ms: 1.21x faster                                           |
| nbody                      | 71.9 ms                                                     | 60.7 ms: 1.18x faster                                          |
| sqlite_synth               | 1.76 us                                                     | 1.49 us: 1.18x faster                                          |
| raytrace                   | 192 ms                                                      | 169 ms: 1.14x faster                                           |
| float                      | 56.8 ms                                                     | 50.3 ms: 1.13x faster                                          |
| richards_super             | 32.1 ms                                                     | 28.5 ms: 1.13x faster                                          |
| logging_silent             | 60.5 ns                                                     | 54.2 ns: 1.12x faster                                          |
| pickle_pure_python         | 195 us                                                      | 175 us: 1.12x faster                                           |
| coroutines                 | 14.3 ms                                                     | 12.8 ms: 1.11x faster                                          |
| async_tree_none            | 291 ms                                                      | 262 ms: 1.11x faster                                           |
| deepcopy_memo              | 23.7 us                                                     | 21.6 us: 1.10x faster                                          |
| dulwich_log                | 44.3 ms                                                     | 40.3 ms: 1.10x faster                                          |
| deepcopy_reduce            | 2.09 us                                                     | 1.91 us: 1.10x faster                                          |
| regex_dna                  | 126 ms                                                      | 115 ms: 1.10x faster                                           |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 447 ms: 1.10x faster                                           |
| generators                 | 22.5 ms                                                     | 20.6 ms: 1.09x faster                                          |
| deltablue                  | 2.16 ms                                                     | 1.98 ms: 1.09x faster                                          |
| deepcopy                   | 238 us                                                      | 219 us: 1.09x faster                                           |
| regex_compile              | 87.5 ms                                                     | 80.4 ms: 1.09x faster                                          |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 464 ms: 1.08x faster                                           |
| richards                   | 28.4 ms                                                     | 26.4 ms: 1.08x faster                                          |
| pathlib                    | 80.5 ms                                                     | 74.8 ms: 1.08x faster                                          |
| xml_etree_generate         | 55.8 ms                                                     | 52.0 ms: 1.07x faster                                          |
| sqlglot_normalize          | 187 ms                                                      | 174 ms: 1.07x faster                                           |
| pprint_safe_repr           | 513 ms                                                      | 480 ms: 1.07x faster                                           |
| logging_simple             | 6.28 us                                                     | 5.89 us: 1.07x faster                                          |
| sympy_str                  | 175 ms                                                      | 164 ms: 1.07x faster                                           |
| async_tree_memoization_tg  | 367 ms                                                      | 345 ms: 1.06x faster                                           |
| pprint_pformat             | 1.05 sec                                                    | 983 ms: 1.06x faster                                           |
| docutils                   | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                         |
| pickle_dict                | 18.4 us                                                     | 17.4 us: 1.06x faster                                          |
| sqlglot_parse              | 804 us                                                      | 761 us: 1.06x faster                                           |
| mako                       | 7.09 ms                                                     | 6.71 ms: 1.06x faster                                          |
| fannkuch                   | 247 ms                                                      | 234 ms: 1.06x faster                                           |
| tornado_http               | 89.5 ms                                                     | 84.9 ms: 1.05x faster                                          |
| async_tree_none_tg         | 285 ms                                                      | 271 ms: 1.05x faster                                           |
| logging_format             | 6.72 us                                                     | 6.39 us: 1.05x faster                                          |
| tomli_loads                | 1.37 sec                                                    | 1.30 sec: 1.05x faster                                         |
| sqlglot_transpile          | 1.02 ms                                                     | 976 us: 1.05x faster                                           |
| unpickle_pure_python       | 133 us                                                      | 127 us: 1.05x faster                                           |
| xml_etree_process          | 37.7 ms                                                     | 36.1 ms: 1.05x faster                                          |
| asyncio_tcp                | 487 ms                                                      | 466 ms: 1.05x faster                                           |
| bench_mp_pool              | 69.2 ms                                                     | 66.2 ms: 1.04x faster                                          |
| nqueens                    | 62.8 ms                                                     | 60.2 ms: 1.04x faster                                          |
| chameleon                  | 4.98 ms                                                     | 4.78 ms: 1.04x faster                                          |
| sympy_sum                  | 91.5 ms                                                     | 87.9 ms: 1.04x faster                                          |
| regex_effbot               | 1.62 ms                                                     | 1.56 ms: 1.04x faster                                          |
| crypto_pyaes               | 48.5 ms                                                     | 46.7 ms: 1.04x faster                                          |
| dask                       | 263 ms                                                      | 254 ms: 1.04x faster                                           |
| spectral_norm              | 66.9 ms                                                     | 64.8 ms: 1.03x faster                                          |
| scimark_lu                 | 58.9 ms                                                     | 57.2 ms: 1.03x faster                                          |
| chaos                      | 43.3 ms                                                     | 42.2 ms: 1.03x faster                                          |
| json_dumps                 | 5.70 ms                                                     | 5.55 ms: 1.03x faster                                          |
| async_tree_io_tg           | 771 ms                                                      | 753 ms: 1.02x faster                                           |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.8 ms: 1.02x faster                                          |
| sqlglot_optimize           | 34.5 ms                                                     | 33.9 ms: 1.02x faster                                          |
| pickle                     | 7.43 us                                                     | 7.31 us: 1.02x faster                                          |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.02x faster                                          |
| pickle_list                | 2.83 us                                                     | 2.78 us: 1.02x faster                                          |
| create_gc_cycles           | 752 us                                                      | 741 us: 1.01x faster                                           |
| 2to3                       | 218 ms                                                      | 215 ms: 1.01x faster                                           |
| sympy_expand               | 284 ms                                                      | 281 ms: 1.01x faster                                           |
| gc_traversal               | 1.52 ms                                                     | 1.51 ms: 1.01x faster                                          |
| pidigits                   | 152 ms                                                      | 152 ms: 1.00x faster                                           |
| sympy_integrate            | 13.0 ms                                                     | 12.9 ms: 1.00x faster                                          |
| async_generators           | 239 ms                                                      | 241 ms: 1.01x slower                                           |
| regex_v8                   | 14.2 ms                                                     | 14.4 ms: 1.01x slower                                          |
| meteor_contest             | 74.6 ms                                                     | 76.3 ms: 1.02x slower                                          |
| python_startup             | 19.5 ms                                                     | 20.1 ms: 1.03x slower                                          |
| scimark_fft                | 184 ms                                                      | 191 ms: 1.04x slower                                           |
| go                         | 91.6 ms                                                     | 95.8 ms: 1.05x slower                                          |
| unpack_sequence            | 37.5 ns                                                     | 39.3 ns: 1.05x slower                                          |
| pyflate                    | 295 ms                                                      | 309 ms: 1.05x slower                                           |
| unpickle                   | 8.18 us                                                     | 8.63 us: 1.05x slower                                          |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.71 ms: 1.06x slower                                          |
| pycparser                  | 699 ms                                                      | 748 ms: 1.07x slower                                           |
| telco                      | 4.13 ms                                                     | 4.59 ms: 1.11x slower                                          |
| python_startup_no_site     | 16.2 ms                                                     | 18.1 ms: 1.11x slower                                          |
| coverage                   | 40.8 ms                                                     | 45.9 ms: 1.13x slower                                          |
| mdp                        | 1.37 sec                                                    | 1.55 sec: 1.13x slower                                         |
| hexiom                     | 4.10 ms                                                     | 5.29 ms: 1.29x slower                                          |
| scimark_monte_carlo        | 43.7 ms                                                     | 56.8 ms: 1.30x slower                                          |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                   |

Benchmark hidden because not significant (7): async_tree_io, bench_thread_pool, async_tree_memoization, xml_etree_parse, scimark_sor, unpickle_list, json
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown