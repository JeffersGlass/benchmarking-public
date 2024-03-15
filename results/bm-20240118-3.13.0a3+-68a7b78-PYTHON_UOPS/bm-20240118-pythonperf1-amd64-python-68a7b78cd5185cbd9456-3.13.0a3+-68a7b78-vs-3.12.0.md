
# Results vs. 3.12.0

- fork: python
- ref: 68a7b78cd5185cbd9456
- machine: windows-amd64
- commit hash: 68a7b78
- commit date: 2024-01-18
- overall geometric mean: 1.00x faster
- HPT reliability: 96.70%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| chameleon      | 4.98 ms                                                     | 4.90 ms: 1.02x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 88.2 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 268 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 455 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 471 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 350 ms: 1.05x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 747 ms: 1.03x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 276 ms: 1.03x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 147 ms: 1.03x faster                                                        |
| nbody          | 71.9 ms                                                     | 83.1 ms: 1.16x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x slower                                                                |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 121 ms: 1.05x faster                                                        |
| regex_compile  | 87.5 ms                                                     | 84.8 ms: 1.03x faster                                                       |
| regex_effbot   | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|---------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python  | 195 us                                                      | 176 us: 1.11x faster                                                        |
| json_loads          | 13.9 us                                                     | 13.4 us: 1.04x faster                                                       |
| json_dumps          | 5.70 ms                                                     | 5.55 ms: 1.03x faster                                                       |
| pickle              | 7.43 us                                                     | 7.30 us: 1.02x faster                                                       |
| xml_etree_generate  | 55.8 ms                                                     | 55.5 ms: 1.01x faster                                                       |
| pickle_dict         | 18.4 us                                                     | 18.8 us: 1.02x slower                                                       |
| unpickle            | 8.18 us                                                     | 8.40 us: 1.03x slower                                                       |
| xml_etree_iterparse | 65.2 ms                                                     | 67.0 ms: 1.03x slower                                                       |
| tomli_loads         | 1.37 sec                                                    | 1.43 sec: 1.05x slower                                                      |
| pickle_list         | 2.83 us                                                     | 3.28 us: 1.16x slower                                                       |
| Geometric mean      | (ref)                                                       | 1.00x slower                                                                |

Benchmark hidden because not significant (4): xml_etree_parse, unpickle_pure_python, xml_etree_process, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.5 ms: 1.05x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.2 ms: 1.12x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 7.66 ms: 1.08x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.62 sec: 1.29x faster                                                      |
| typing_runtime_protocols   | 95.1 us                                                     | 74.0 us: 1.29x faster                                                       |
| mypy2                      | 509 ms                                                      | 421 ms: 1.21x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.58 us: 1.11x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 176 us: 1.11x faster                                                        |
| raytrace                   | 192 ms                                                      | 174 ms: 1.11x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 55.2 ns: 1.09x faster                                                       |
| comprehensions             | 14.1 us                                                     | 12.9 us: 1.09x faster                                                       |
| async_tree_none            | 291 ms                                                      | 268 ms: 1.09x faster                                                        |
| scimark_lu                 | 58.9 ms                                                     | 54.4 ms: 1.08x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 455 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 471 ms: 1.07x faster                                                        |
| coroutines                 | 14.3 ms                                                     | 13.4 ms: 1.06x faster                                                       |
| deepcopy                   | 238 us                                                      | 224 us: 1.06x faster                                                        |
| deepcopy_memo              | 23.7 us                                                     | 22.4 us: 1.06x faster                                                       |
| richards_super             | 32.1 ms                                                     | 30.3 ms: 1.06x faster                                                       |
| sympy_str                  | 175 ms                                                      | 166 ms: 1.06x faster                                                        |
| docutils                   | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                                      |
| regex_dna                  | 126 ms                                                      | 121 ms: 1.05x faster                                                        |
| richards                   | 28.4 ms                                                     | 27.1 ms: 1.05x faster                                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 350 ms: 1.05x faster                                                        |
| json                       | 3.05 ms                                                     | 2.91 ms: 1.05x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 2.00 us: 1.05x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 771 us: 1.04x faster                                                        |
| sympy_sum                  | 91.5 ms                                                     | 87.9 ms: 1.04x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 42.6 ms: 1.04x faster                                                       |
| json_loads                 | 13.9 us                                                     | 13.4 us: 1.04x faster                                                       |
| async_generators           | 239 ms                                                      | 232 ms: 1.03x faster                                                        |
| scimark_sor                | 78.8 ms                                                     | 76.3 ms: 1.03x faster                                                       |
| async_tree_io_tg           | 771 ms                                                      | 747 ms: 1.03x faster                                                        |
| pidigits                   | 152 ms                                                      | 147 ms: 1.03x faster                                                        |
| sqlglot_normalize          | 187 ms                                                      | 181 ms: 1.03x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 84.8 ms: 1.03x faster                                                       |
| async_tree_none_tg         | 285 ms                                                      | 276 ms: 1.03x faster                                                        |
| gc_traversal               | 1.52 ms                                                     | 1.48 ms: 1.03x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 67.2 ms: 1.03x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 994 us: 1.03x faster                                                        |
| asyncio_tcp                | 487 ms                                                      | 474 ms: 1.03x faster                                                        |
| json_dumps                 | 5.70 ms                                                     | 5.55 ms: 1.03x faster                                                       |
| generators                 | 22.5 ms                                                     | 21.9 ms: 1.03x faster                                                       |
| create_gc_cycles           | 752 us                                                      | 735 us: 1.02x faster                                                        |
| sympy_expand               | 284 ms                                                      | 278 ms: 1.02x faster                                                        |
| regex_effbot               | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                       |
| dask                       | 263 ms                                                      | 258 ms: 1.02x faster                                                        |
| pickle                     | 7.43 us                                                     | 7.30 us: 1.02x faster                                                       |
| pathlib                    | 80.5 ms                                                     | 79.1 ms: 1.02x faster                                                       |
| chameleon                  | 4.98 ms                                                     | 4.90 ms: 1.02x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 88.2 ms: 1.02x faster                                                       |
| go                         | 91.6 ms                                                     | 90.4 ms: 1.01x faster                                                       |
| xml_etree_generate         | 55.8 ms                                                     | 55.5 ms: 1.01x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 48.7 ms: 1.00x slower                                                       |
| logging_simple             | 6.28 us                                                     | 6.32 us: 1.01x slower                                                       |
| pprint_safe_repr           | 513 ms                                                      | 517 ms: 1.01x slower                                                        |
| chaos                      | 43.3 ms                                                     | 44.1 ms: 1.02x slower                                                       |
| pickle_dict                | 18.4 us                                                     | 18.8 us: 1.02x slower                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.07 sec: 1.02x slower                                                      |
| regex_v8                   | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.40 us: 1.03x slower                                                       |
| nqueens                    | 62.8 ms                                                     | 64.5 ms: 1.03x slower                                                       |
| meteor_contest             | 74.6 ms                                                     | 76.7 ms: 1.03x slower                                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 67.0 ms: 1.03x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 39.1 ns: 1.04x slower                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.43 sec: 1.05x slower                                                      |
| mdp                        | 1.37 sec                                                    | 1.44 sec: 1.05x slower                                                      |
| python_startup             | 19.5 ms                                                     | 20.5 ms: 1.05x slower                                                       |
| mako                       | 7.09 ms                                                     | 7.66 ms: 1.08x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 47.8 ms: 1.09x slower                                                       |
| pyflate                    | 295 ms                                                      | 324 ms: 1.10x slower                                                        |
| fannkuch                   | 247 ms                                                      | 272 ms: 1.10x slower                                                        |
| python_startup_no_site     | 16.2 ms                                                     | 18.2 ms: 1.12x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.65 ms: 1.13x slower                                                       |
| coverage                   | 40.8 ms                                                     | 47.1 ms: 1.15x slower                                                       |
| nbody                      | 71.9 ms                                                     | 83.1 ms: 1.16x slower                                                       |
| pickle_list                | 2.83 us                                                     | 3.28 us: 1.16x slower                                                       |
| scimark_fft                | 184 ms                                                      | 215 ms: 1.16x slower                                                        |
| hexiom                     | 4.10 ms                                                     | 4.92 ms: 1.20x slower                                                       |
| deltablue                  | 2.16 ms                                                     | 2.69 ms: 1.25x slower                                                       |
| spectral_norm              | 66.9 ms                                                     | 85.2 ms: 1.27x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 3.29 ms: 1.29x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.00x faster                                                                |

Benchmark hidden because not significant (13): bench_thread_pool, xml_etree_parse, async_tree_io, logging_format, float, unpickle_pure_python, xml_etree_process, unpickle_list, 2to3, sqlglot_optimize, sympy_integrate, async_tree_memoization, pycparser
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 96.70% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown