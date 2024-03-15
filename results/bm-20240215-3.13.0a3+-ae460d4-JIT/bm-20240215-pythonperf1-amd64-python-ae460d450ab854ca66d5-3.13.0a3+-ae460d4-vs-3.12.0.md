
# Results vs. 3.12.0

- fork: python
- ref: ae460d450ab854ca66d5
- machine: windows-amd64
- commit hash: ae460d4
- commit date: 2024-02-15
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 216 ms: 1.01x faster                                                        |
| chameleon      | 4.98 ms                                                     | 4.80 ms: 1.04x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.56 sec: 1.07x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 85.0 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 261 ms: 1.12x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 447 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 466 ms: 1.08x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 266 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 343 ms: 1.07x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 746 ms: 1.03x faster                                                        |
| async_tree_io              | 731 ms                                                      | 709 ms: 1.03x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 61.4 ms: 1.17x faster                                                       |
| float          | 56.8 ms                                                     | 50.5 ms: 1.13x faster                                                       |
| Geometric mean | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 80.1 ms: 1.09x faster                                                       |
| regex_dna      | 126 ms                                                      | 119 ms: 1.07x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 176 us: 1.11x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 52.0 ms: 1.07x faster                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.29 sec: 1.06x faster                                                      |
| unpickle_pure_python | 133 us                                                      | 126 us: 1.05x faster                                                        |
| xml_etree_process    | 37.7 ms                                                     | 36.0 ms: 1.05x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 17.6 us: 1.05x faster                                                       |
| pickle_list          | 2.83 us                                                     | 2.73 us: 1.04x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.3 ms: 1.03x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.6 us: 1.02x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.56 ms: 1.02x faster                                                       |
| pickle               | 7.43 us                                                     | 7.31 us: 1.02x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 91.5 ms: 1.02x faster                                                       |
| unpickle             | 8.18 us                                                     | 8.46 us: 1.03x slower                                                       |
| unpickle_list        | 2.75 us                                                     | 2.92 us: 1.06x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.5 ms: 1.05x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.3 ms: 1.13x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.66 ms: 1.06x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 70.1 us: 1.36x faster                                                       |
| comprehensions             | 14.1 us                                                     | 10.8 us: 1.31x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.67 sec: 1.26x faster                                                      |
| mypy2                      | 509 ms                                                      | 422 ms: 1.21x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.49 us: 1.18x faster                                                       |
| nbody                      | 71.9 ms                                                     | 61.4 ms: 1.17x faster                                                       |
| generators                 | 22.5 ms                                                     | 19.9 ms: 1.13x faster                                                       |
| richards_super             | 32.1 ms                                                     | 28.4 ms: 1.13x faster                                                       |
| raytrace                   | 192 ms                                                      | 171 ms: 1.13x faster                                                        |
| float                      | 56.8 ms                                                     | 50.5 ms: 1.13x faster                                                       |
| async_tree_none            | 291 ms                                                      | 261 ms: 1.12x faster                                                        |
| pickle_pure_python         | 195 us                                                      | 176 us: 1.11x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 54.6 ns: 1.11x faster                                                       |
| sympy_str                  | 175 ms                                                      | 158 ms: 1.11x faster                                                        |
| richards                   | 28.4 ms                                                     | 25.8 ms: 1.10x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 170 ms: 1.10x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 40.5 ms: 1.09x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 447 ms: 1.09x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 80.1 ms: 1.09x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.1 ms: 1.09x faster                                                       |
| deltablue                  | 2.16 ms                                                     | 1.99 ms: 1.09x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.94 us: 1.08x faster                                                       |
| deepcopy                   | 238 us                                                      | 220 us: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 466 ms: 1.08x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 266 ms: 1.07x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 52.0 ms: 1.07x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 85.4 ms: 1.07x faster                                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 343 ms: 1.07x faster                                                        |
| docutils                   | 1.66 sec                                                    | 1.56 sec: 1.07x faster                                                      |
| pathlib                    | 80.5 ms                                                     | 75.4 ms: 1.07x faster                                                       |
| regex_dna                  | 126 ms                                                      | 119 ms: 1.07x faster                                                        |
| mako                       | 7.09 ms                                                     | 6.66 ms: 1.06x faster                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.29 sec: 1.06x faster                                                      |
| nqueens                    | 62.8 ms                                                     | 59.3 ms: 1.06x faster                                                       |
| pprint_pformat             | 1.05 sec                                                    | 988 ms: 1.06x faster                                                        |
| pprint_safe_repr           | 513 ms                                                      | 486 ms: 1.06x faster                                                        |
| json                       | 3.05 ms                                                     | 2.89 ms: 1.05x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 763 us: 1.05x faster                                                        |
| logging_simple             | 6.28 us                                                     | 5.95 us: 1.05x faster                                                       |
| unpickle_pure_python       | 133 us                                                      | 126 us: 1.05x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 85.0 ms: 1.05x faster                                                       |
| spectral_norm              | 66.9 ms                                                     | 63.8 ms: 1.05x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 36.0 ms: 1.05x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 975 us: 1.05x faster                                                        |
| pickle_dict                | 18.4 us                                                     | 17.6 us: 1.05x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 46.4 ms: 1.04x faster                                                       |
| scimark_lu                 | 58.9 ms                                                     | 56.4 ms: 1.04x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 66.3 ms: 1.04x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 22.8 us: 1.04x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.45 us: 1.04x faster                                                       |
| asyncio_tcp                | 487 ms                                                      | 469 ms: 1.04x faster                                                        |
| chameleon                  | 4.98 ms                                                     | 4.80 ms: 1.04x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 33.3 ms: 1.04x faster                                                       |
| pickle_list                | 2.83 us                                                     | 2.73 us: 1.04x faster                                                       |
| dask                       | 263 ms                                                      | 253 ms: 1.04x faster                                                        |
| chaos                      | 43.3 ms                                                     | 41.9 ms: 1.03x faster                                                       |
| async_tree_io_tg           | 771 ms                                                      | 746 ms: 1.03x faster                                                        |
| async_tree_io              | 731 ms                                                      | 709 ms: 1.03x faster                                                        |
| regex_effbot               | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.3 ms: 1.03x faster                                                       |
| create_gc_cycles           | 752 us                                                      | 732 us: 1.03x faster                                                        |
| json_loads                 | 13.9 us                                                     | 13.6 us: 1.02x faster                                                       |
| fannkuch                   | 247 ms                                                      | 241 ms: 1.02x faster                                                        |
| json_dumps                 | 5.70 ms                                                     | 5.56 ms: 1.02x faster                                                       |
| bench_thread_pool          | 857 us                                                      | 838 us: 1.02x faster                                                        |
| pickle                     | 7.43 us                                                     | 7.31 us: 1.02x faster                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 91.5 ms: 1.02x faster                                                       |
| async_generators           | 239 ms                                                      | 236 ms: 1.01x faster                                                        |
| scimark_sor                | 78.8 ms                                                     | 77.8 ms: 1.01x faster                                                       |
| 2to3                       | 218 ms                                                      | 216 ms: 1.01x faster                                                        |
| sympy_expand               | 284 ms                                                      | 281 ms: 1.01x faster                                                        |
| gc_traversal               | 1.52 ms                                                     | 1.51 ms: 1.01x faster                                                       |
| sympy_integrate            | 13.0 ms                                                     | 13.0 ms: 1.00x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| scimark_fft                | 184 ms                                                      | 190 ms: 1.03x slower                                                        |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.63 ms: 1.03x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.46 us: 1.03x slower                                                       |
| meteor_contest             | 74.6 ms                                                     | 77.3 ms: 1.04x slower                                                       |
| go                         | 91.6 ms                                                     | 96.0 ms: 1.05x slower                                                       |
| pyflate                    | 295 ms                                                      | 309 ms: 1.05x slower                                                        |
| python_startup             | 19.5 ms                                                     | 20.5 ms: 1.05x slower                                                       |
| unpickle_list              | 2.75 us                                                     | 2.92 us: 1.06x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 41.6 ns: 1.11x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.60 ms: 1.11x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 18.3 ms: 1.13x slower                                                       |
| coverage                   | 40.8 ms                                                     | 46.3 ms: 1.13x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.60 sec: 1.17x slower                                                      |
| hexiom                     | 4.10 ms                                                     | 5.15 ms: 1.25x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 56.9 ms: 1.30x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (3): pycparser, async_tree_memoization, pidigits
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown