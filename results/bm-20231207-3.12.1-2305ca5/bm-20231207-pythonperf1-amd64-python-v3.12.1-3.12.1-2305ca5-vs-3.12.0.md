
# Results vs. 3.12.0

- fork: python
- ref: v3.12.1
- machine: windows-amd64
- commit hash: 2305ca5
- commit date: 2023-12-07
- overall geometric mean: 1.02x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 215 ms: 1.02x faster                                        |
| chameleon      | 4.98 ms                                                     | 5.06 ms: 1.02x slower                                       |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                      |
| tornado_http   | 89.5 ms                                                     | 87.0 ms: 1.03x faster                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_memoization_tg  | 367 ms                                                      | 351 ms: 1.05x faster                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 490 ms: 1.02x faster                                        |
| async_tree_none_tg         | 285 ms                                                      | 279 ms: 1.02x faster                                        |
| async_tree_io_tg           | 771 ms                                                      | 762 ms: 1.01x faster                                        |
| async_tree_none            | 291 ms                                                      | 288 ms: 1.01x faster                                        |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 56.8 ms                                                     | 54.3 ms: 1.05x faster                                       |
| nbody          | 71.9 ms                                                     | 69.5 ms: 1.03x faster                                       |
| pidigits       | 152 ms                                                      | 151 ms: 1.01x faster                                        |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 121 ms: 1.04x faster                                        |
| regex_compile  | 87.5 ms                                                     | 85.0 ms: 1.03x faster                                       |
| regex_v8       | 14.2 ms                                                     | 14.1 ms: 1.01x faster                                       |
| regex_effbot   | 1.62 ms                                                     | 1.63 ms: 1.01x slower                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|---------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle              | 7.43 us                                                     | 6.95 us: 1.07x faster                                       |
| unpickle_list       | 2.75 us                                                     | 2.68 us: 1.03x faster                                       |
| xml_etree_iterparse | 65.2 ms                                                     | 64.0 ms: 1.02x faster                                       |
| json_loads          | 13.9 us                                                     | 13.7 us: 1.01x faster                                       |
| pickle_dict         | 18.4 us                                                     | 18.2 us: 1.01x faster                                       |
| pickle_pure_python  | 195 us                                                      | 193 us: 1.01x faster                                        |
| pickle_list         | 2.83 us                                                     | 2.85 us: 1.01x slower                                       |
| xml_etree_process   | 37.7 ms                                                     | 38.4 ms: 1.02x slower                                       |
| xml_etree_generate  | 55.8 ms                                                     | 57.1 ms: 1.02x slower                                       |
| Geometric mean      | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (5): unpickle, tomli_loads, xml_etree_parse, json_dumps, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup, python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 6.89 ms: 1.03x faster                                       |
| django_template | 22.9 ms                                                     | 23.7 ms: 1.03x slower                                       |
| Geometric mean  | (ref)                                                       | 1.00x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231207-pythonperf1-amd64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 76.4 us: 1.24x faster                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.86 sec: 1.13x faster                                      |
| pickle                     | 7.43 us                                                     | 6.95 us: 1.07x faster                                       |
| coverage                   | 40.8 ms                                                     | 38.2 ms: 1.07x faster                                       |
| bench_mp_pool              | 69.2 ms                                                     | 65.3 ms: 1.06x faster                                       |
| spectral_norm              | 66.9 ms                                                     | 63.2 ms: 1.06x faster                                       |
| richards                   | 28.4 ms                                                     | 26.9 ms: 1.06x faster                                       |
| richards_super             | 32.1 ms                                                     | 30.5 ms: 1.05x faster                                       |
| float                      | 56.8 ms                                                     | 54.3 ms: 1.05x faster                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 351 ms: 1.05x faster                                        |
| go                         | 91.6 ms                                                     | 87.8 ms: 1.04x faster                                       |
| crypto_pyaes               | 48.5 ms                                                     | 46.5 ms: 1.04x faster                                       |
| regex_dna                  | 126 ms                                                      | 121 ms: 1.04x faster                                        |
| json                       | 3.05 ms                                                     | 2.93 ms: 1.04x faster                                       |
| asyncio_tcp                | 487 ms                                                      | 470 ms: 1.04x faster                                        |
| docutils                   | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                      |
| nbody                      | 71.9 ms                                                     | 69.5 ms: 1.03x faster                                       |
| scimark_fft                | 184 ms                                                      | 179 ms: 1.03x faster                                        |
| create_gc_cycles           | 752 us                                                      | 730 us: 1.03x faster                                        |
| fannkuch                   | 247 ms                                                      | 239 ms: 1.03x faster                                        |
| regex_compile              | 87.5 ms                                                     | 85.0 ms: 1.03x faster                                       |
| tornado_http               | 89.5 ms                                                     | 87.0 ms: 1.03x faster                                       |
| mako                       | 7.09 ms                                                     | 6.89 ms: 1.03x faster                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.49 ms: 1.03x faster                                       |
| unpickle_list              | 2.75 us                                                     | 2.68 us: 1.03x faster                                       |
| sympy_sum                  | 91.5 ms                                                     | 89.1 ms: 1.03x faster                                       |
| gc_traversal               | 1.52 ms                                                     | 1.48 ms: 1.03x faster                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 490 ms: 1.02x faster                                        |
| dulwich_log                | 44.3 ms                                                     | 43.2 ms: 1.02x faster                                       |
| aiohttp                    | 884 us                                                      | 864 us: 1.02x faster                                        |
| async_tree_none_tg         | 285 ms                                                      | 279 ms: 1.02x faster                                        |
| deepcopy                   | 238 us                                                      | 233 us: 1.02x faster                                        |
| sqlalchemy_declarative     | 86.4 ms                                                     | 84.7 ms: 1.02x faster                                       |
| hexiom                     | 4.10 ms                                                     | 4.03 ms: 1.02x faster                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 64.0 ms: 1.02x faster                                       |
| pycparser                  | 699 ms                                                      | 687 ms: 1.02x faster                                        |
| 2to3                       | 218 ms                                                      | 215 ms: 1.02x faster                                        |
| sympy_str                  | 175 ms                                                      | 173 ms: 1.01x faster                                        |
| dask                       | 263 ms                                                      | 259 ms: 1.01x faster                                        |
| comprehensions             | 14.1 us                                                     | 13.9 us: 1.01x faster                                       |
| scimark_sor                | 78.8 ms                                                     | 77.8 ms: 1.01x faster                                       |
| meteor_contest             | 74.6 ms                                                     | 73.7 ms: 1.01x faster                                       |
| async_tree_io_tg           | 771 ms                                                      | 762 ms: 1.01x faster                                        |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.01x faster                                       |
| async_tree_none            | 291 ms                                                      | 288 ms: 1.01x faster                                        |
| async_generators           | 239 ms                                                      | 237 ms: 1.01x faster                                        |
| pickle_dict                | 18.4 us                                                     | 18.2 us: 1.01x faster                                       |
| pickle_pure_python         | 195 us                                                      | 193 us: 1.01x faster                                        |
| deltablue                  | 2.16 ms                                                     | 2.14 ms: 1.01x faster                                       |
| regex_v8                   | 14.2 ms                                                     | 14.1 ms: 1.01x faster                                       |
| sympy_integrate            | 13.0 ms                                                     | 12.9 ms: 1.01x faster                                       |
| sqlalchemy_imperative      | 9.29 ms                                                     | 9.23 ms: 1.01x faster                                       |
| pidigits                   | 152 ms                                                      | 151 ms: 1.01x faster                                        |
| pprint_safe_repr           | 513 ms                                                      | 511 ms: 1.00x faster                                        |
| chaos                      | 43.3 ms                                                     | 43.2 ms: 1.00x faster                                       |
| mdp                        | 1.37 sec                                                    | 1.38 sec: 1.00x slower                                      |
| raytrace                   | 192 ms                                                      | 193 ms: 1.01x slower                                        |
| regex_effbot               | 1.62 ms                                                     | 1.63 ms: 1.01x slower                                       |
| pickle_list                | 2.83 us                                                     | 2.85 us: 1.01x slower                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 44.1 ms: 1.01x slower                                       |
| scimark_lu                 | 58.9 ms                                                     | 59.4 ms: 1.01x slower                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                       |
| deepcopy_reduce            | 2.09 us                                                     | 2.13 us: 1.02x slower                                       |
| chameleon                  | 4.98 ms                                                     | 5.06 ms: 1.02x slower                                       |
| logging_simple             | 6.28 us                                                     | 6.39 us: 1.02x slower                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 1.04 ms: 1.02x slower                                       |
| xml_etree_process          | 37.7 ms                                                     | 38.4 ms: 1.02x slower                                       |
| sqlglot_parse              | 804 us                                                      | 821 us: 1.02x slower                                        |
| xml_etree_generate         | 55.8 ms                                                     | 57.1 ms: 1.02x slower                                       |
| logging_format             | 6.72 us                                                     | 6.87 us: 1.02x slower                                       |
| logging_silent             | 60.5 ns                                                     | 62.1 ns: 1.03x slower                                       |
| django_template            | 22.9 ms                                                     | 23.7 ms: 1.03x slower                                       |
| unpack_sequence            | 37.5 ns                                                     | 39.9 ns: 1.06x slower                                       |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                |

Benchmark hidden because not significant (23): mypy2, async_tree_cpu_io_mixed, coroutines, unpickle, nqueens, tomli_loads, xml_etree_parse, pyflate, telco, json_dumps, unpickle_pure_python, pprint_pformat, python_startup, sympy_expand, async_tree_io, sqlglot_normalize, async_tree_memoization, deepcopy_memo, sqlite_synth, generators, bench_thread_pool, pathlib, python_startup_no_site


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown