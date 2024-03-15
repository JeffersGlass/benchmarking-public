# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_jumps
- machine: windows-amd64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 222 ms: 1.02x slower                                                      |
| chameleon      | 4.98 ms                                                     | 4.77 ms: 1.05x faster                                                     |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                    |
| tornado_http   | 89.5 ms                                                     | 84.6 ms: 1.06x faster                                                     |
| Geometric mean | (ref)                                                       | 1.03x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 263 ms: 1.11x faster                                                      |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 451 ms: 1.08x faster                                                      |
| async_tree_memoization_tg  | 367 ms                                                      | 349 ms: 1.05x faster                                                      |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                      |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 480 ms: 1.05x faster                                                      |
| async_tree_io_tg           | 771 ms                                                      | 760 ms: 1.02x faster                                                      |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                              |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 60.2 ms: 1.19x faster                                                     |
| float          | 56.8 ms                                                     | 48.7 ms: 1.17x faster                                                     |
| pidigits       | 152 ms                                                      | 151 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                       | 1.12x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 120 ms: 1.05x faster                                                      |
| regex_compile  | 87.5 ms                                                     | 83.6 ms: 1.05x faster                                                     |
| regex_effbot   | 1.62 ms                                                     | 1.58 ms: 1.03x faster                                                     |
| regex_v8       | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                     |
| Geometric mean | (ref)                                                       | 1.02x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| tomli_loads          | 1.37 sec                                                    | 1.17 sec: 1.17x faster                                                    |
| pickle_pure_python   | 195 us                                                      | 178 us: 1.10x faster                                                      |
| json_dumps           | 5.70 ms                                                     | 5.43 ms: 1.05x faster                                                     |
| xml_etree_iterparse  | 65.2 ms                                                     | 62.3 ms: 1.05x faster                                                     |
| xml_etree_generate   | 55.8 ms                                                     | 53.4 ms: 1.05x faster                                                     |
| pickle_dict          | 18.4 us                                                     | 17.7 us: 1.04x faster                                                     |
| xml_etree_process    | 37.7 ms                                                     | 36.4 ms: 1.04x faster                                                     |
| unpickle_pure_python | 133 us                                                      | 130 us: 1.02x faster                                                      |
| xml_etree_parse      | 93.0 ms                                                     | 92.2 ms: 1.01x faster                                                     |
| json_loads           | 13.9 us                                                     | 13.8 us: 1.01x faster                                                     |
| pickle               | 7.43 us                                                     | 7.60 us: 1.02x slower                                                     |
| unpickle_list        | 2.75 us                                                     | 2.83 us: 1.03x slower                                                     |
| unpickle             | 8.18 us                                                     | 8.69 us: 1.06x slower                                                     |
| pickle_list          | 2.83 us                                                     | 3.12 us: 1.11x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 23.8 ms: 1.22x slower                                                     |
| python_startup_no_site | 16.2 ms                                                     | 21.7 ms: 1.33x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.28x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 5.63 ms: 1.26x faster                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| comprehensions             | 14.1 us                                                     | 10.3 us: 1.38x faster                                                     |
| typing_runtime_protocols   | 95.1 us                                                     | 69.9 us: 1.36x faster                                                     |
| spectral_norm              | 66.9 ms                                                     | 51.1 ms: 1.31x faster                                                     |
| mako                       | 7.09 ms                                                     | 5.63 ms: 1.26x faster                                                     |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.69 sec: 1.24x faster                                                    |
| nbody                      | 71.9 ms                                                     | 60.2 ms: 1.19x faster                                                     |
| mypy2                      | 509 ms                                                      | 436 ms: 1.17x faster                                                      |
| float                      | 56.8 ms                                                     | 48.7 ms: 1.17x faster                                                     |
| tomli_loads                | 1.37 sec                                                    | 1.17 sec: 1.17x faster                                                    |
| fannkuch                   | 247 ms                                                      | 221 ms: 1.12x faster                                                      |
| generators                 | 22.5 ms                                                     | 20.2 ms: 1.12x faster                                                     |
| crypto_pyaes               | 48.5 ms                                                     | 43.5 ms: 1.12x faster                                                     |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.29 ms: 1.11x faster                                                     |
| sqlite_synth               | 1.76 us                                                     | 1.58 us: 1.11x faster                                                     |
| async_tree_none            | 291 ms                                                      | 263 ms: 1.11x faster                                                      |
| logging_silent             | 60.5 ns                                                     | 54.7 ns: 1.11x faster                                                     |
| chaos                      | 43.3 ms                                                     | 39.3 ms: 1.10x faster                                                     |
| pickle_pure_python         | 195 us                                                      | 178 us: 1.10x faster                                                      |
| scimark_fft                | 184 ms                                                      | 169 ms: 1.09x faster                                                      |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 451 ms: 1.08x faster                                                      |
| logging_simple             | 6.28 us                                                     | 5.80 us: 1.08x faster                                                     |
| coroutines                 | 14.3 ms                                                     | 13.2 ms: 1.08x faster                                                     |
| pprint_safe_repr           | 513 ms                                                      | 475 ms: 1.08x faster                                                      |
| pprint_pformat             | 1.05 sec                                                    | 969 ms: 1.08x faster                                                      |
| logging_format             | 6.72 us                                                     | 6.24 us: 1.08x faster                                                     |
| raytrace                   | 192 ms                                                      | 179 ms: 1.08x faster                                                      |
| deepcopy_reduce            | 2.09 us                                                     | 1.95 us: 1.08x faster                                                     |
| deepcopy_memo              | 23.7 us                                                     | 22.1 us: 1.08x faster                                                     |
| sympy_str                  | 175 ms                                                      | 163 ms: 1.07x faster                                                      |
| dulwich_log                | 44.3 ms                                                     | 41.3 ms: 1.07x faster                                                     |
| deepcopy                   | 238 us                                                      | 224 us: 1.06x faster                                                      |
| pathlib                    | 80.5 ms                                                     | 76.0 ms: 1.06x faster                                                     |
| tornado_http               | 89.5 ms                                                     | 84.6 ms: 1.06x faster                                                     |
| sympy_sum                  | 91.5 ms                                                     | 86.6 ms: 1.06x faster                                                     |
| sqlglot_normalize          | 187 ms                                                      | 177 ms: 1.06x faster                                                      |
| scimark_monte_carlo        | 43.7 ms                                                     | 41.5 ms: 1.05x faster                                                     |
| deltablue                  | 2.16 ms                                                     | 2.05 ms: 1.05x faster                                                     |
| regex_dna                  | 126 ms                                                      | 120 ms: 1.05x faster                                                      |
| asyncio_tcp                | 487 ms                                                      | 464 ms: 1.05x faster                                                      |
| async_tree_memoization_tg  | 367 ms                                                      | 349 ms: 1.05x faster                                                      |
| json_dumps                 | 5.70 ms                                                     | 5.43 ms: 1.05x faster                                                     |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                      |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 480 ms: 1.05x faster                                                      |
| regex_compile              | 87.5 ms                                                     | 83.6 ms: 1.05x faster                                                     |
| xml_etree_iterparse        | 65.2 ms                                                     | 62.3 ms: 1.05x faster                                                     |
| xml_etree_generate         | 55.8 ms                                                     | 53.4 ms: 1.05x faster                                                     |
| chameleon                  | 4.98 ms                                                     | 4.77 ms: 1.05x faster                                                     |
| pickle_dict                | 18.4 us                                                     | 17.7 us: 1.04x faster                                                     |
| docutils                   | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                    |
| xml_etree_process          | 37.7 ms                                                     | 36.4 ms: 1.04x faster                                                     |
| meteor_contest             | 74.6 ms                                                     | 72.2 ms: 1.03x faster                                                     |
| sqlglot_parse              | 804 us                                                      | 778 us: 1.03x faster                                                      |
| pyflate                    | 295 ms                                                      | 287 ms: 1.03x faster                                                      |
| regex_effbot               | 1.62 ms                                                     | 1.58 ms: 1.03x faster                                                     |
| nqueens                    | 62.8 ms                                                     | 61.3 ms: 1.03x faster                                                     |
| unpickle_pure_python       | 133 us                                                      | 130 us: 1.02x faster                                                      |
| create_gc_cycles           | 752 us                                                      | 738 us: 1.02x faster                                                      |
| sqlglot_transpile          | 1.02 ms                                                     | 1.01 ms: 1.02x faster                                                     |
| async_tree_io_tg           | 771 ms                                                      | 760 ms: 1.02x faster                                                      |
| sympy_expand               | 284 ms                                                      | 280 ms: 1.02x faster                                                      |
| pidigits                   | 152 ms                                                      | 151 ms: 1.01x faster                                                      |
| richards_super             | 32.1 ms                                                     | 31.8 ms: 1.01x faster                                                     |
| xml_etree_parse            | 93.0 ms                                                     | 92.2 ms: 1.01x faster                                                     |
| json_loads                 | 13.9 us                                                     | 13.8 us: 1.01x faster                                                     |
| sympy_integrate            | 13.0 ms                                                     | 13.0 ms: 1.01x slower                                                     |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                                     |
| bench_mp_pool              | 69.2 ms                                                     | 69.8 ms: 1.01x slower                                                     |
| 2to3                       | 218 ms                                                      | 222 ms: 1.02x slower                                                      |
| pickle                     | 7.43 us                                                     | 7.60 us: 1.02x slower                                                     |
| unpickle_list              | 2.75 us                                                     | 2.83 us: 1.03x slower                                                     |
| regex_v8                   | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                     |
| go                         | 91.6 ms                                                     | 96.8 ms: 1.06x slower                                                     |
| unpickle                   | 8.18 us                                                     | 8.69 us: 1.06x slower                                                     |
| hexiom                     | 4.10 ms                                                     | 4.39 ms: 1.07x slower                                                     |
| scimark_sor                | 78.8 ms                                                     | 84.6 ms: 1.07x slower                                                     |
| mdp                        | 1.37 sec                                                    | 1.52 sec: 1.11x slower                                                    |
| pickle_list                | 2.83 us                                                     | 3.12 us: 1.11x slower                                                     |
| telco                      | 4.13 ms                                                     | 4.57 ms: 1.11x slower                                                     |
| coverage                   | 40.8 ms                                                     | 45.7 ms: 1.12x slower                                                     |
| unpack_sequence            | 37.5 ns                                                     | 45.2 ns: 1.21x slower                                                     |
| python_startup             | 19.5 ms                                                     | 23.8 ms: 1.22x slower                                                     |
| scimark_lu                 | 58.9 ms                                                     | 73.0 ms: 1.24x slower                                                     |
| python_startup_no_site     | 16.2 ms                                                     | 21.7 ms: 1.33x slower                                                     |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                              |

Benchmark hidden because not significant (8): bench_thread_pool, async_tree_io, json, gc_traversal, async_tree_memoization, pycparser, async_generators, richards
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown