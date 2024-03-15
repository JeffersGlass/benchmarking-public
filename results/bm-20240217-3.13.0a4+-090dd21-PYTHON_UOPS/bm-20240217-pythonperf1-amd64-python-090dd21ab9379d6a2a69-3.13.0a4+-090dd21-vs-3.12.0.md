
# Results vs. 3.12.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-amd64
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.00x faster \*
- HPT reliability: 86.90%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 220 ms: 1.01x slower                                                        |
| chameleon      | 4.98 ms                                                     | 5.12 ms: 1.03x slower                                                       |
| docutils       | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 85.4 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 270 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 458 ms: 1.07x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 471 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 353 ms: 1.04x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 274 ms: 1.04x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 763 ms: 1.01x faster                                                        |
| async_tree_memoization     | 339 ms                                                      | 346 ms: 1.02x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.03x faster                                                                |

Benchmark hidden because not significant (1): async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 147 ms: 1.03x faster                                                        |
| float          | 56.8 ms                                                     | 58.3 ms: 1.03x slower                                                       |
| nbody          | 71.9 ms                                                     | 75.6 ms: 1.05x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 119 ms: 1.07x faster                                                        |
| regex_compile  | 87.5 ms                                                     | 84.8 ms: 1.03x faster                                                       |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.7 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 184 us: 1.06x faster                                                        |
| pickle               | 7.43 us                                                     | 7.10 us: 1.05x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 54.0 ms: 1.03x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.5 us: 1.03x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.65 ms: 1.01x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 37.4 ms: 1.01x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 18.3 us: 1.01x faster                                                       |
| pickle_list          | 2.83 us                                                     | 2.85 us: 1.01x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.43 us: 1.03x slower                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 67.4 ms: 1.03x slower                                                       |
| unpickle_list        | 2.75 us                                                     | 2.86 us: 1.04x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 140 us: 1.05x slower                                                        |
| tomli_loads          | 1.37 sec                                                    | 1.51 sec: 1.11x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                                |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.0 ms: 1.03x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.0 ms: 1.11x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.67 ms: 1.08x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 74.0 us: 1.28x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.64 sec: 1.28x faster                                                      |
| mypy2                      | 509 ms                                                      | 424 ms: 1.20x faster                                                        |
| comprehensions             | 14.1 us                                                     | 12.5 us: 1.13x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.58 us: 1.12x faster                                                       |
| generators                 | 22.5 ms                                                     | 20.3 ms: 1.11x faster                                                       |
| raytrace                   | 192 ms                                                      | 174 ms: 1.11x faster                                                        |
| coroutines                 | 14.3 ms                                                     | 13.2 ms: 1.08x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 56.0 ns: 1.08x faster                                                       |
| async_tree_none            | 291 ms                                                      | 270 ms: 1.08x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 41.5 ms: 1.07x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 458 ms: 1.07x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 471 ms: 1.07x faster                                                        |
| regex_dna                  | 126 ms                                                      | 119 ms: 1.07x faster                                                        |
| pathlib                    | 80.5 ms                                                     | 75.5 ms: 1.07x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 65.1 ms: 1.06x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 184 us: 1.06x faster                                                        |
| deepcopy_reduce            | 2.09 us                                                     | 1.99 us: 1.05x faster                                                       |
| asyncio_tcp                | 487 ms                                                      | 465 ms: 1.05x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 85.4 ms: 1.05x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.10 us: 1.05x faster                                                       |
| sympy_str                  | 175 ms                                                      | 168 ms: 1.04x faster                                                        |
| docutils                   | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| async_tree_memoization_tg  | 367 ms                                                      | 353 ms: 1.04x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 274 ms: 1.04x faster                                                        |
| richards                   | 28.4 ms                                                     | 27.3 ms: 1.04x faster                                                       |
| scimark_lu                 | 58.9 ms                                                     | 56.9 ms: 1.04x faster                                                       |
| richards_super             | 32.1 ms                                                     | 31.0 ms: 1.04x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 88.4 ms: 1.04x faster                                                       |
| async_generators           | 239 ms                                                      | 231 ms: 1.03x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 54.0 ms: 1.03x faster                                                       |
| pidigits                   | 152 ms                                                      | 147 ms: 1.03x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 84.8 ms: 1.03x faster                                                       |
| deepcopy                   | 238 us                                                      | 231 us: 1.03x faster                                                        |
| json_loads                 | 13.9 us                                                     | 13.5 us: 1.03x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 182 ms: 1.02x faster                                                        |
| gc_traversal               | 1.52 ms                                                     | 1.49 ms: 1.02x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 23.2 us: 1.02x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 47.5 ms: 1.02x faster                                                       |
| dask                       | 263 ms                                                      | 257 ms: 1.02x faster                                                        |
| create_gc_cycles           | 752 us                                                      | 738 us: 1.02x faster                                                        |
| sqlglot_parse              | 804 us                                                      | 790 us: 1.02x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 763 ms: 1.01x faster                                                        |
| sqlglot_transpile          | 1.02 ms                                                     | 1.01 ms: 1.01x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.65 ms: 1.01x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 37.4 ms: 1.01x faster                                                       |
| pickle_dict                | 18.4 us                                                     | 18.3 us: 1.01x faster                                                       |
| deltablue                  | 2.16 ms                                                     | 2.15 ms: 1.01x faster                                                       |
| 2to3                       | 218 ms                                                      | 220 ms: 1.01x slower                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                                       |
| pickle_list                | 2.83 us                                                     | 2.85 us: 1.01x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 37.9 ns: 1.01x slower                                                       |
| meteor_contest             | 74.6 ms                                                     | 76.0 ms: 1.02x slower                                                       |
| pprint_safe_repr           | 513 ms                                                      | 523 ms: 1.02x slower                                                        |
| async_tree_memoization     | 339 ms                                                      | 346 ms: 1.02x slower                                                        |
| go                         | 91.6 ms                                                     | 93.7 ms: 1.02x slower                                                       |
| nqueens                    | 62.8 ms                                                     | 64.4 ms: 1.03x slower                                                       |
| float                      | 56.8 ms                                                     | 58.3 ms: 1.03x slower                                                       |
| chameleon                  | 4.98 ms                                                     | 5.12 ms: 1.03x slower                                                       |
| chaos                      | 43.3 ms                                                     | 44.5 ms: 1.03x slower                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.08 sec: 1.03x slower                                                      |
| python_startup             | 19.5 ms                                                     | 20.0 ms: 1.03x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.43 us: 1.03x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.7 ms: 1.03x slower                                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 67.4 ms: 1.03x slower                                                       |
| unpickle_list              | 2.75 us                                                     | 2.86 us: 1.04x slower                                                       |
| unpickle_pure_python       | 133 us                                                      | 140 us: 1.05x slower                                                        |
| nbody                      | 71.9 ms                                                     | 75.6 ms: 1.05x slower                                                       |
| scimark_sor                | 78.8 ms                                                     | 83.8 ms: 1.06x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.47 sec: 1.07x slower                                                      |
| fannkuch                   | 247 ms                                                      | 266 ms: 1.08x slower                                                        |
| mako                       | 7.09 ms                                                     | 7.67 ms: 1.08x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.51 sec: 1.11x slower                                                      |
| python_startup_no_site     | 16.2 ms                                                     | 18.0 ms: 1.11x slower                                                       |
| pyflate                    | 295 ms                                                      | 328 ms: 1.11x slower                                                        |
| scimark_fft                | 184 ms                                                      | 205 ms: 1.11x slower                                                        |
| scimark_monte_carlo        | 43.7 ms                                                     | 49.4 ms: 1.13x slower                                                       |
| coverage                   | 40.8 ms                                                     | 47.0 ms: 1.15x slower                                                       |
| pycparser                  | 699 ms                                                      | 823 ms: 1.18x slower                                                        |
| telco                      | 4.13 ms                                                     | 4.87 ms: 1.18x slower                                                       |
| spectral_norm              | 66.9 ms                                                     | 81.0 ms: 1.21x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 5.00 ms: 1.22x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 3.22 ms: 1.26x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.00x faster                                                                |

Benchmark hidden because not significant (8): bench_thread_pool, xml_etree_parse, sympy_expand, logging_simple, sympy_integrate, async_tree_io, logging_format, json
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 86.90% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown