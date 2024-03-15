
# Results vs. 3.12.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-amd64
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 210 ms: 1.04x faster                                                        |
| chameleon      | 4.98 ms                                                     | 4.88 ms: 1.02x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.55 sec: 1.07x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 84.5 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 489 ms                                                      | 456 ms: 1.07x faster                                                        |
| async_tree_none            | 291 ms                                                      | 272 ms: 1.07x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 475 ms: 1.06x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 358 ms: 1.03x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 280 ms: 1.02x faster                                                        |
| async_tree_memoization     | 339 ms                                                      | 350 ms: 1.03x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.03x faster                                                                |

Benchmark hidden because not significant (2): async_tree_io, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 53.3 ms: 1.07x faster                                                       |
| pidigits       | 152 ms                                                      | 147 ms: 1.04x faster                                                        |
| nbody          | 71.9 ms                                                     | 70.0 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 78.2 ms: 1.12x faster                                                       |
| regex_dna      | 126 ms                                                      | 116 ms: 1.09x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.55 ms: 1.04x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 183 us: 1.07x faster                                                        |
| unpickle_pure_python | 133 us                                                      | 127 us: 1.05x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 54.1 ms: 1.03x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.3 ms: 1.03x faster                                                       |
| pickle               | 7.43 us                                                     | 7.24 us: 1.03x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 90.8 ms: 1.02x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.6 us: 1.02x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.73 us: 1.01x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.65 ms: 1.01x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 37.5 ms: 1.01x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 18.6 us: 1.01x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.54 us: 1.04x slower                                                       |
| pickle_list          | 2.83 us                                                     | 2.95 us: 1.05x slower                                                       |
| tomli_loads          | 1.37 sec                                                    | 1.45 sec: 1.06x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.0 ms: 1.03x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 17.9 ms: 1.10x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.60 ms: 1.07x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 71.0 us: 1.34x faster                                                       |
| comprehensions             | 14.1 us                                                     | 10.7 us: 1.32x faster                                                       |
| mypy2                      | 509 ms                                                      | 413 ms: 1.23x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.76 sec: 1.19x faster                                                      |
| raytrace                   | 192 ms                                                      | 165 ms: 1.17x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.52 us: 1.16x faster                                                       |
| regex_compile              | 87.5 ms                                                     | 78.2 ms: 1.12x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 54.2 ns: 1.12x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 39.8 ms: 1.11x faster                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 39.5 ms: 1.11x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.0 ms: 1.10x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 83.3 ms: 1.10x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 44.1 ms: 1.10x faster                                                       |
| sympy_str                  | 175 ms                                                      | 160 ms: 1.10x faster                                                        |
| regex_dna                  | 126 ms                                                      | 116 ms: 1.09x faster                                                        |
| deltablue                  | 2.16 ms                                                     | 1.99 ms: 1.08x faster                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.36 ms: 1.08x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 63.9 ms: 1.08x faster                                                       |
| mako                       | 7.09 ms                                                     | 6.60 ms: 1.07x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 456 ms: 1.07x faster                                                        |
| pathlib                    | 80.5 ms                                                     | 75.1 ms: 1.07x faster                                                       |
| go                         | 91.6 ms                                                     | 85.5 ms: 1.07x faster                                                       |
| chaos                      | 43.3 ms                                                     | 40.5 ms: 1.07x faster                                                       |
| async_tree_none            | 291 ms                                                      | 272 ms: 1.07x faster                                                        |
| docutils                   | 1.66 sec                                                    | 1.55 sec: 1.07x faster                                                      |
| spectral_norm              | 66.9 ms                                                     | 62.6 ms: 1.07x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 183 us: 1.07x faster                                                        |
| float                      | 56.8 ms                                                     | 53.3 ms: 1.07x faster                                                       |
| scimark_fft                | 184 ms                                                      | 174 ms: 1.06x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 84.5 ms: 1.06x faster                                                       |
| hexiom                     | 4.10 ms                                                     | 3.87 ms: 1.06x faster                                                       |
| scimark_lu                 | 58.9 ms                                                     | 55.6 ms: 1.06x faster                                                       |
| deepcopy_memo              | 23.7 us                                                     | 22.4 us: 1.06x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 475 ms: 1.06x faster                                                        |
| nqueens                    | 62.8 ms                                                     | 59.4 ms: 1.06x faster                                                       |
| generators                 | 22.5 ms                                                     | 21.3 ms: 1.06x faster                                                       |
| unpickle_pure_python       | 133 us                                                      | 127 us: 1.05x faster                                                        |
| async_generators           | 239 ms                                                      | 229 ms: 1.05x faster                                                        |
| deepcopy                   | 238 us                                                      | 228 us: 1.04x faster                                                        |
| sympy_expand               | 284 ms                                                      | 272 ms: 1.04x faster                                                        |
| sympy_integrate            | 13.0 ms                                                     | 12.4 ms: 1.04x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.55 ms: 1.04x faster                                                       |
| asyncio_tcp                | 487 ms                                                      | 470 ms: 1.04x faster                                                        |
| pidigits                   | 152 ms                                                      | 147 ms: 1.04x faster                                                        |
| 2to3                       | 218 ms                                                      | 210 ms: 1.04x faster                                                        |
| pprint_safe_repr           | 513 ms                                                      | 496 ms: 1.04x faster                                                        |
| unpack_sequence            | 37.5 ns                                                     | 36.2 ns: 1.04x faster                                                       |
| logging_simple             | 6.28 us                                                     | 6.07 us: 1.03x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 181 ms: 1.03x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 54.1 ms: 1.03x faster                                                       |
| scimark_sor                | 78.8 ms                                                     | 76.3 ms: 1.03x faster                                                       |
| dask                       | 263 ms                                                      | 254 ms: 1.03x faster                                                        |
| logging_format             | 6.72 us                                                     | 6.52 us: 1.03x faster                                                       |
| bench_thread_pool          | 857 us                                                      | 831 us: 1.03x faster                                                        |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.3 ms: 1.03x faster                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.02 sec: 1.03x faster                                                      |
| deepcopy_reduce            | 2.09 us                                                     | 2.04 us: 1.03x faster                                                       |
| meteor_contest             | 74.6 ms                                                     | 72.7 ms: 1.03x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.24 us: 1.03x faster                                                       |
| nbody                      | 71.9 ms                                                     | 70.0 ms: 1.03x faster                                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 358 ms: 1.03x faster                                                        |
| xml_etree_parse            | 93.0 ms                                                     | 90.8 ms: 1.02x faster                                                       |
| pyflate                    | 295 ms                                                      | 288 ms: 1.02x faster                                                        |
| chameleon                  | 4.98 ms                                                     | 4.88 ms: 1.02x faster                                                       |
| json_loads                 | 13.9 us                                                     | 13.6 us: 1.02x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 788 us: 1.02x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 280 ms: 1.02x faster                                                        |
| sqlglot_transpile          | 1.02 ms                                                     | 1.00 ms: 1.02x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.0 ms: 1.01x faster                                                       |
| richards_super             | 32.1 ms                                                     | 31.8 ms: 1.01x faster                                                       |
| richards                   | 28.4 ms                                                     | 28.1 ms: 1.01x faster                                                       |
| unpickle_list              | 2.75 us                                                     | 2.73 us: 1.01x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.65 ms: 1.01x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 37.5 ms: 1.01x faster                                                       |
| pickle_dict                | 18.4 us                                                     | 18.6 us: 1.01x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| python_startup             | 19.5 ms                                                     | 20.0 ms: 1.03x slower                                                       |
| async_tree_memoization     | 339 ms                                                      | 350 ms: 1.03x slower                                                        |
| unpickle                   | 8.18 us                                                     | 8.54 us: 1.04x slower                                                       |
| pickle_list                | 2.83 us                                                     | 2.95 us: 1.05x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.45 sec: 1.06x slower                                                      |
| mdp                        | 1.37 sec                                                    | 1.48 sec: 1.08x slower                                                      |
| json                       | 3.05 ms                                                     | 3.32 ms: 1.09x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 17.9 ms: 1.10x slower                                                       |
| coverage                   | 40.8 ms                                                     | 46.4 ms: 1.14x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.80 ms: 1.16x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (6): create_gc_cycles, gc_traversal, async_tree_io, async_tree_io_tg, fannkuch, pycparser
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown