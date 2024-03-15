
# Results vs. 3.12.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-amd64
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 216 ms: 1.01x faster                                                        |
| chameleon      | 4.98 ms                                                     | 4.74 ms: 1.05x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.56 sec: 1.07x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 84.6 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 266 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 460 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 449 ms: 1.09x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 343 ms: 1.07x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 269 ms: 1.06x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 747 ms: 1.03x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 59.8 ms: 1.20x faster                                                       |
| float          | 56.8 ms                                                     | 50.2 ms: 1.13x faster                                                       |
| pidigits       | 152 ms                                                      | 152 ms: 1.00x faster                                                        |
| Geometric mean | (ref)                                                       | 1.11x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 79.2 ms: 1.10x faster                                                       |
| regex_dna      | 126 ms                                                      | 121 ms: 1.05x faster                                                        |
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 175 us: 1.12x faster                                                        |
| unpickle_pure_python | 133 us                                                      | 126 us: 1.06x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 52.7 ms: 1.06x faster                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.29 sec: 1.06x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 17.4 us: 1.06x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 36.0 ms: 1.05x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.59 ms: 1.02x faster                                                       |
| pickle_list          | 2.83 us                                                     | 2.77 us: 1.02x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 64.0 ms: 1.02x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 91.6 ms: 1.02x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.01x faster                                                       |
| pickle               | 7.43 us                                                     | 7.47 us: 1.01x slower                                                       |
| unpickle_list        | 2.75 us                                                     | 2.81 us: 1.02x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.44 us: 1.03x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.4 ms: 1.05x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.4 ms: 1.13x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.58 ms: 1.08x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 70.0 us: 1.36x faster                                                       |
| comprehensions             | 14.1 us                                                     | 10.8 us: 1.31x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.73 sec: 1.21x faster                                                      |
| mypy2                      | 509 ms                                                      | 423 ms: 1.20x faster                                                        |
| nbody                      | 71.9 ms                                                     | 59.8 ms: 1.20x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.49 us: 1.18x faster                                                       |
| raytrace                   | 192 ms                                                      | 167 ms: 1.15x faster                                                        |
| float                      | 56.8 ms                                                     | 50.2 ms: 1.13x faster                                                       |
| richards_super             | 32.1 ms                                                     | 28.4 ms: 1.13x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 175 us: 1.12x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 54.2 ns: 1.12x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 21.4 us: 1.11x faster                                                       |
| regex_compile              | 87.5 ms                                                     | 79.2 ms: 1.10x faster                                                       |
| richards                   | 28.4 ms                                                     | 25.8 ms: 1.10x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 40.3 ms: 1.10x faster                                                       |
| async_tree_none            | 291 ms                                                      | 266 ms: 1.10x faster                                                        |
| deepcopy_reduce            | 2.09 us                                                     | 1.91 us: 1.09x faster                                                       |
| deepcopy                   | 238 us                                                      | 218 us: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 460 ms: 1.09x faster                                                        |
| generators                 | 22.5 ms                                                     | 20.7 ms: 1.09x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 449 ms: 1.09x faster                                                        |
| deltablue                  | 2.16 ms                                                     | 1.98 ms: 1.09x faster                                                       |
| pprint_safe_repr           | 513 ms                                                      | 476 ms: 1.08x faster                                                        |
| mako                       | 7.09 ms                                                     | 6.58 ms: 1.08x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 174 ms: 1.08x faster                                                        |
| pathlib                    | 80.5 ms                                                     | 74.9 ms: 1.07x faster                                                       |
| sympy_str                  | 175 ms                                                      | 163 ms: 1.07x faster                                                        |
| pprint_pformat             | 1.05 sec                                                    | 978 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 343 ms: 1.07x faster                                                        |
| crypto_pyaes               | 48.5 ms                                                     | 45.4 ms: 1.07x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.56 sec: 1.07x faster                                                      |
| nqueens                    | 62.8 ms                                                     | 59.0 ms: 1.06x faster                                                       |
| async_tree_none_tg         | 285 ms                                                      | 269 ms: 1.06x faster                                                        |
| sqlglot_parse              | 804 us                                                      | 759 us: 1.06x faster                                                        |
| scimark_sor                | 78.8 ms                                                     | 74.3 ms: 1.06x faster                                                       |
| unpickle_pure_python       | 133 us                                                      | 126 us: 1.06x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 52.7 ms: 1.06x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 84.6 ms: 1.06x faster                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.29 sec: 1.06x faster                                                      |
| pickle_dict                | 18.4 us                                                     | 17.4 us: 1.06x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.5 ms: 1.05x faster                                                       |
| scimark_lu                 | 58.9 ms                                                     | 55.9 ms: 1.05x faster                                                       |
| logging_simple             | 6.28 us                                                     | 5.96 us: 1.05x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 971 us: 1.05x faster                                                        |
| sympy_sum                  | 91.5 ms                                                     | 87.0 ms: 1.05x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.39 us: 1.05x faster                                                       |
| chameleon                  | 4.98 ms                                                     | 4.74 ms: 1.05x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 36.0 ms: 1.05x faster                                                       |
| regex_dna                  | 126 ms                                                      | 121 ms: 1.05x faster                                                        |
| spectral_norm              | 66.9 ms                                                     | 64.1 ms: 1.04x faster                                                       |
| chaos                      | 43.3 ms                                                     | 41.6 ms: 1.04x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 66.7 ms: 1.04x faster                                                       |
| asyncio_tcp                | 487 ms                                                      | 472 ms: 1.03x faster                                                        |
| dask                       | 263 ms                                                      | 254 ms: 1.03x faster                                                        |
| create_gc_cycles           | 752 us                                                      | 729 us: 1.03x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 747 ms: 1.03x faster                                                        |
| fannkuch                   | 247 ms                                                      | 240 ms: 1.03x faster                                                        |
| bench_thread_pool          | 857 us                                                      | 837 us: 1.02x faster                                                        |
| json_dumps                 | 5.70 ms                                                     | 5.59 ms: 1.02x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 33.9 ms: 1.02x faster                                                       |
| pickle_list                | 2.83 us                                                     | 2.77 us: 1.02x faster                                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 64.0 ms: 1.02x faster                                                       |
| sympy_integrate            | 13.0 ms                                                     | 12.7 ms: 1.02x faster                                                       |
| xml_etree_parse            | 93.0 ms                                                     | 91.6 ms: 1.02x faster                                                       |
| sympy_expand               | 284 ms                                                      | 280 ms: 1.01x faster                                                        |
| gc_traversal               | 1.52 ms                                                     | 1.50 ms: 1.01x faster                                                       |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.01x faster                                                       |
| 2to3                       | 218 ms                                                      | 216 ms: 1.01x faster                                                        |
| pidigits                   | 152 ms                                                      | 152 ms: 1.00x faster                                                        |
| pickle                     | 7.43 us                                                     | 7.47 us: 1.01x slower                                                       |
| scimark_fft                | 184 ms                                                      | 186 ms: 1.01x slower                                                        |
| meteor_contest             | 74.6 ms                                                     | 75.9 ms: 1.02x slower                                                       |
| unpickle_list              | 2.75 us                                                     | 2.81 us: 1.02x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 38.6 ns: 1.03x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.44 us: 1.03x slower                                                       |
| pyflate                    | 295 ms                                                      | 306 ms: 1.04x slower                                                        |
| go                         | 91.6 ms                                                     | 95.8 ms: 1.05x slower                                                       |
| python_startup             | 19.5 ms                                                     | 20.4 ms: 1.05x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.70 ms: 1.06x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                       |
| pycparser                  | 699 ms                                                      | 764 ms: 1.09x slower                                                        |
| coverage                   | 40.8 ms                                                     | 45.6 ms: 1.12x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.67 ms: 1.13x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 18.4 ms: 1.13x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.61 sec: 1.17x slower                                                      |
| hexiom                     | 4.10 ms                                                     | 5.11 ms: 1.25x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 56.4 ms: 1.29x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (5): async_tree_io, async_tree_memoization, async_generators, json, regex_effbot
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown