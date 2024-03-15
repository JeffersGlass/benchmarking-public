
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_continue
- machine: windows-amd64
- commit hash: 9e86002
- commit date: 2024-02-13
- overall geometric mean: 1.05x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 214 ms: 1.02x faster                                                         |
| chameleon      | 4.98 ms                                                     | 4.80 ms: 1.04x faster                                                        |
| docutils       | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                                       |
| tornado_http   | 89.5 ms                                                     | 84.9 ms: 1.06x faster                                                        |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 261 ms: 1.12x faster                                                         |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 445 ms: 1.10x faster                                                         |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 463 ms: 1.09x faster                                                         |
| async_tree_memoization_tg  | 367 ms                                                      | 340 ms: 1.08x faster                                                         |
| async_tree_none_tg         | 285 ms                                                      | 267 ms: 1.07x faster                                                         |
| async_tree_io_tg           | 771 ms                                                      | 740 ms: 1.04x faster                                                         |
| async_tree_io              | 731 ms                                                      | 720 ms: 1.02x faster                                                         |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                 |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 59.5 ms: 1.21x faster                                                        |
| float          | 56.8 ms                                                     | 50.2 ms: 1.13x faster                                                        |
| pidigits       | 152 ms                                                      | 151 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                       | 1.11x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 78.1 ms: 1.12x faster                                                        |
| regex_dna      | 126 ms                                                      | 120 ms: 1.05x faster                                                         |
| regex_effbot   | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                        |
| regex_v8       | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 174 us: 1.13x faster                                                         |
| tomli_loads          | 1.37 sec                                                    | 1.26 sec: 1.09x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 52.7 ms: 1.06x faster                                                        |
| unpickle_pure_python | 133 us                                                      | 126 us: 1.06x faster                                                         |
| pickle_dict          | 18.4 us                                                     | 17.5 us: 1.05x faster                                                        |
| xml_etree_process    | 37.7 ms                                                     | 36.0 ms: 1.05x faster                                                        |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.4 ms: 1.03x faster                                                        |
| json_dumps           | 5.70 ms                                                     | 5.61 ms: 1.02x faster                                                        |
| json_loads           | 13.9 us                                                     | 13.8 us: 1.01x faster                                                        |
| unpickle_list        | 2.75 us                                                     | 2.79 us: 1.01x slower                                                        |
| xml_etree_parse      | 93.0 ms                                                     | 94.4 ms: 1.02x slower                                                        |
| unpickle             | 8.18 us                                                     | 8.58 us: 1.05x slower                                                        |
| pickle_list          | 2.83 us                                                     | 3.09 us: 1.09x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                 |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.2 ms: 1.04x slower                                                        |
| python_startup_no_site | 16.2 ms                                                     | 18.1 ms: 1.11x slower                                                        |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-----------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.15 ms: 1.15x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 68.8 us: 1.38x faster                                                        |
| comprehensions             | 14.1 us                                                     | 11.1 us: 1.27x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.72 sec: 1.22x faster                                                       |
| mypy2                      | 509 ms                                                      | 421 ms: 1.21x faster                                                         |
| nbody                      | 71.9 ms                                                     | 59.5 ms: 1.21x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.52 us: 1.16x faster                                                        |
| mako                       | 7.09 ms                                                     | 6.15 ms: 1.15x faster                                                        |
| raytrace                   | 192 ms                                                      | 167 ms: 1.15x faster                                                         |
| logging_silent             | 60.5 ns                                                     | 53.0 ns: 1.14x faster                                                        |
| richards_super             | 32.1 ms                                                     | 28.2 ms: 1.14x faster                                                        |
| richards                   | 28.4 ms                                                     | 25.0 ms: 1.13x faster                                                        |
| float                      | 56.8 ms                                                     | 50.2 ms: 1.13x faster                                                        |
| generators                 | 22.5 ms                                                     | 19.9 ms: 1.13x faster                                                        |
| pickle_pure_python         | 195 us                                                      | 174 us: 1.13x faster                                                         |
| regex_compile              | 87.5 ms                                                     | 78.1 ms: 1.12x faster                                                        |
| deepcopy_memo              | 23.7 us                                                     | 21.2 us: 1.12x faster                                                        |
| spectral_norm              | 66.9 ms                                                     | 59.9 ms: 1.12x faster                                                        |
| async_tree_none            | 291 ms                                                      | 261 ms: 1.12x faster                                                         |
| deepcopy                   | 238 us                                                      | 216 us: 1.10x faster                                                         |
| scimark_lu                 | 58.9 ms                                                     | 53.4 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 445 ms: 1.10x faster                                                         |
| deltablue                  | 2.16 ms                                                     | 1.96 ms: 1.10x faster                                                        |
| coroutines                 | 14.3 ms                                                     | 13.0 ms: 1.09x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 40.5 ms: 1.09x faster                                                        |
| tomli_loads                | 1.37 sec                                                    | 1.26 sec: 1.09x faster                                                       |
| pprint_safe_repr           | 513 ms                                                      | 473 ms: 1.09x faster                                                         |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 463 ms: 1.09x faster                                                         |
| sqlglot_normalize          | 187 ms                                                      | 172 ms: 1.09x faster                                                         |
| pprint_pformat             | 1.05 sec                                                    | 967 ms: 1.08x faster                                                         |
| crypto_pyaes               | 48.5 ms                                                     | 44.9 ms: 1.08x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 340 ms: 1.08x faster                                                         |
| deepcopy_reduce            | 2.09 us                                                     | 1.95 us: 1.07x faster                                                        |
| fannkuch                   | 247 ms                                                      | 230 ms: 1.07x faster                                                         |
| sympy_str                  | 175 ms                                                      | 163 ms: 1.07x faster                                                         |
| async_tree_none_tg         | 285 ms                                                      | 267 ms: 1.07x faster                                                         |
| nqueens                    | 62.8 ms                                                     | 58.8 ms: 1.07x faster                                                        |
| sqlglot_parse              | 804 us                                                      | 755 us: 1.07x faster                                                         |
| docutils                   | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                                       |
| bench_thread_pool          | 857 us                                                      | 808 us: 1.06x faster                                                         |
| sympy_sum                  | 91.5 ms                                                     | 86.4 ms: 1.06x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 52.7 ms: 1.06x faster                                                        |
| sqlglot_transpile          | 1.02 ms                                                     | 965 us: 1.06x faster                                                         |
| scimark_sor                | 78.8 ms                                                     | 74.6 ms: 1.06x faster                                                        |
| unpickle_pure_python       | 133 us                                                      | 126 us: 1.06x faster                                                         |
| tornado_http               | 89.5 ms                                                     | 84.9 ms: 1.06x faster                                                        |
| pickle_dict                | 18.4 us                                                     | 17.5 us: 1.05x faster                                                        |
| regex_dna                  | 126 ms                                                      | 120 ms: 1.05x faster                                                         |
| xml_etree_process          | 37.7 ms                                                     | 36.0 ms: 1.05x faster                                                        |
| pathlib                    | 80.5 ms                                                     | 76.9 ms: 1.05x faster                                                        |
| logging_format             | 6.72 us                                                     | 6.42 us: 1.05x faster                                                        |
| logging_simple             | 6.28 us                                                     | 6.00 us: 1.05x faster                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 66.2 ms: 1.04x faster                                                        |
| asyncio_tcp                | 487 ms                                                      | 468 ms: 1.04x faster                                                         |
| chaos                      | 43.3 ms                                                     | 41.6 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 740 ms: 1.04x faster                                                         |
| pycparser                  | 699 ms                                                      | 671 ms: 1.04x faster                                                         |
| chameleon                  | 4.98 ms                                                     | 4.80 ms: 1.04x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 33.3 ms: 1.04x faster                                                        |
| create_gc_cycles           | 752 us                                                      | 728 us: 1.03x faster                                                         |
| dask                       | 263 ms                                                      | 255 ms: 1.03x faster                                                         |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.4 ms: 1.03x faster                                                        |
| sympy_expand               | 284 ms                                                      | 276 ms: 1.03x faster                                                         |
| gc_traversal               | 1.52 ms                                                     | 1.49 ms: 1.02x faster                                                        |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.51 ms: 1.02x faster                                                        |
| 2to3                       | 218 ms                                                      | 214 ms: 1.02x faster                                                         |
| async_tree_io              | 731 ms                                                      | 720 ms: 1.02x faster                                                         |
| json_dumps                 | 5.70 ms                                                     | 5.61 ms: 1.02x faster                                                        |
| regex_effbot               | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                        |
| meteor_contest             | 74.6 ms                                                     | 73.8 ms: 1.01x faster                                                        |
| pyflate                    | 295 ms                                                      | 291 ms: 1.01x faster                                                         |
| pidigits                   | 152 ms                                                      | 151 ms: 1.01x faster                                                         |
| json_loads                 | 13.9 us                                                     | 13.8 us: 1.01x faster                                                        |
| async_generators           | 239 ms                                                      | 238 ms: 1.01x faster                                                         |
| sympy_integrate            | 13.0 ms                                                     | 12.9 ms: 1.00x faster                                                        |
| unpickle_list              | 2.75 us                                                     | 2.79 us: 1.01x slower                                                        |
| xml_etree_parse            | 93.0 ms                                                     | 94.4 ms: 1.02x slower                                                        |
| scimark_fft                | 184 ms                                                      | 188 ms: 1.02x slower                                                         |
| go                         | 91.6 ms                                                     | 94.3 ms: 1.03x slower                                                        |
| unpack_sequence            | 37.5 ns                                                     | 38.8 ns: 1.03x slower                                                        |
| python_startup             | 19.5 ms                                                     | 20.2 ms: 1.04x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                        |
| unpickle                   | 8.18 us                                                     | 8.58 us: 1.05x slower                                                        |
| json                       | 3.05 ms                                                     | 3.26 ms: 1.07x slower                                                        |
| pickle_list                | 2.83 us                                                     | 3.09 us: 1.09x slower                                                        |
| telco                      | 4.13 ms                                                     | 4.58 ms: 1.11x slower                                                        |
| python_startup_no_site     | 16.2 ms                                                     | 18.1 ms: 1.11x slower                                                        |
| coverage                   | 40.8 ms                                                     | 45.6 ms: 1.12x slower                                                        |
| scimark_monte_carlo        | 43.7 ms                                                     | 49.2 ms: 1.12x slower                                                        |
| mdp                        | 1.37 sec                                                    | 1.56 sec: 1.14x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 4.82 ms: 1.18x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                 |

Benchmark hidden because not significant (2): async_tree_memoization, pickle
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown