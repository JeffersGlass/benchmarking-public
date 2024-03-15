
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_ghccc
- machine: windows-amd64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.24%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| chameleon      | 4.98 ms                                                     | 4.81 ms: 1.04x faster                                                     |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                    |
| tornado_http   | 89.5 ms                                                     | 87.4 ms: 1.02x faster                                                     |
| Geometric mean | (ref)                                                       | 1.02x faster                                                              |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 489 ms                                                      | 461 ms: 1.06x faster                                                      |
| async_tree_none            | 291 ms                                                      | 279 ms: 1.04x faster                                                      |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 482 ms: 1.04x faster                                                      |
| async_tree_memoization_tg  | 367 ms                                                      | 354 ms: 1.04x faster                                                      |
| async_tree_io              | 731 ms                                                      | 750 ms: 1.03x slower                                                      |
| async_tree_memoization     | 339 ms                                                      | 354 ms: 1.04x slower                                                      |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                              |

Benchmark hidden because not significant (2): async_tree_none_tg, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 55.3 ms: 1.30x faster                                                     |
| float          | 56.8 ms                                                     | 50.6 ms: 1.12x faster                                                     |
| pidigits       | 152 ms                                                      | 153 ms: 1.01x slower                                                      |
| Geometric mean | (ref)                                                       | 1.13x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 81.6 ms: 1.07x faster                                                     |
| regex_dna      | 126 ms                                                      | 118 ms: 1.07x faster                                                      |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                     |
| regex_v8       | 14.2 ms                                                     | 16.4 ms: 1.15x slower                                                     |
| Geometric mean | (ref)                                                       | 1.01x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 177 us: 1.10x faster                                                      |
| xml_etree_generate   | 55.8 ms                                                     | 53.1 ms: 1.05x faster                                                     |
| tomli_loads          | 1.37 sec                                                    | 1.30 sec: 1.05x faster                                                    |
| xml_etree_process    | 37.7 ms                                                     | 36.0 ms: 1.05x faster                                                     |
| pickle_dict          | 18.4 us                                                     | 17.7 us: 1.04x faster                                                     |
| json_dumps           | 5.70 ms                                                     | 5.54 ms: 1.03x faster                                                     |
| unpickle_pure_python | 133 us                                                      | 130 us: 1.02x faster                                                      |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.02x faster                                                     |
| pickle               | 7.43 us                                                     | 7.41 us: 1.00x faster                                                     |
| xml_etree_parse      | 93.0 ms                                                     | 94.3 ms: 1.01x slower                                                     |
| unpickle_list        | 2.75 us                                                     | 2.84 us: 1.03x slower                                                     |
| unpickle             | 8.18 us                                                     | 8.73 us: 1.07x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                              |

Benchmark hidden because not significant (2): xml_etree_iterparse, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 21.1 ms: 1.09x slower                                                     |
| python_startup_no_site | 16.2 ms                                                     | 19.0 ms: 1.17x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.13x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.63 ms: 1.07x faster                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 70.1 us: 1.36x faster                                                     |
| nbody                      | 71.9 ms                                                     | 55.3 ms: 1.30x faster                                                     |
| comprehensions             | 14.1 us                                                     | 11.4 us: 1.24x faster                                                     |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.71 sec: 1.23x faster                                                    |
| mypy2                      | 509 ms                                                      | 436 ms: 1.17x faster                                                      |
| raytrace                   | 192 ms                                                      | 167 ms: 1.15x faster                                                      |
| sqlite_synth               | 1.76 us                                                     | 1.56 us: 1.13x faster                                                     |
| logging_silent             | 60.5 ns                                                     | 53.6 ns: 1.13x faster                                                     |
| generators                 | 22.5 ms                                                     | 20.0 ms: 1.13x faster                                                     |
| richards                   | 28.4 ms                                                     | 25.2 ms: 1.13x faster                                                     |
| float                      | 56.8 ms                                                     | 50.6 ms: 1.12x faster                                                     |
| richards_super             | 32.1 ms                                                     | 28.6 ms: 1.12x faster                                                     |
| crypto_pyaes               | 48.5 ms                                                     | 43.6 ms: 1.11x faster                                                     |
| coroutines                 | 14.3 ms                                                     | 12.9 ms: 1.10x faster                                                     |
| pickle_pure_python         | 195 us                                                      | 177 us: 1.10x faster                                                      |
| deepcopy_reduce            | 2.09 us                                                     | 1.93 us: 1.09x faster                                                     |
| deepcopy                   | 238 us                                                      | 220 us: 1.08x faster                                                      |
| regex_compile              | 87.5 ms                                                     | 81.6 ms: 1.07x faster                                                     |
| spectral_norm              | 66.9 ms                                                     | 62.5 ms: 1.07x faster                                                     |
| regex_dna                  | 126 ms                                                      | 118 ms: 1.07x faster                                                      |
| mako                       | 7.09 ms                                                     | 6.63 ms: 1.07x faster                                                     |
| deepcopy_memo              | 23.7 us                                                     | 22.2 us: 1.07x faster                                                     |
| scimark_lu                 | 58.9 ms                                                     | 55.3 ms: 1.06x faster                                                     |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 461 ms: 1.06x faster                                                      |
| dulwich_log                | 44.3 ms                                                     | 41.8 ms: 1.06x faster                                                     |
| xml_etree_generate         | 55.8 ms                                                     | 53.1 ms: 1.05x faster                                                     |
| tomli_loads                | 1.37 sec                                                    | 1.30 sec: 1.05x faster                                                    |
| logging_simple             | 6.28 us                                                     | 5.98 us: 1.05x faster                                                     |
| xml_etree_process          | 37.7 ms                                                     | 36.0 ms: 1.05x faster                                                     |
| chaos                      | 43.3 ms                                                     | 41.3 ms: 1.05x faster                                                     |
| sqlglot_parse              | 804 us                                                      | 768 us: 1.05x faster                                                      |
| logging_format             | 6.72 us                                                     | 6.41 us: 1.05x faster                                                     |
| async_tree_none            | 291 ms                                                      | 279 ms: 1.04x faster                                                      |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 482 ms: 1.04x faster                                                      |
| pprint_safe_repr           | 513 ms                                                      | 493 ms: 1.04x faster                                                      |
| deltablue                  | 2.16 ms                                                     | 2.08 ms: 1.04x faster                                                     |
| pickle_dict                | 18.4 us                                                     | 17.7 us: 1.04x faster                                                     |
| docutils                   | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                    |
| sqlglot_normalize          | 187 ms                                                      | 180 ms: 1.04x faster                                                      |
| chameleon                  | 4.98 ms                                                     | 4.81 ms: 1.04x faster                                                     |
| fannkuch                   | 247 ms                                                      | 238 ms: 1.04x faster                                                      |
| async_tree_memoization_tg  | 367 ms                                                      | 354 ms: 1.04x faster                                                      |
| sqlglot_transpile          | 1.02 ms                                                     | 988 us: 1.03x faster                                                      |
| scimark_sor                | 78.8 ms                                                     | 76.3 ms: 1.03x faster                                                     |
| regex_effbot               | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                     |
| nqueens                    | 62.8 ms                                                     | 61.0 ms: 1.03x faster                                                     |
| json_dumps                 | 5.70 ms                                                     | 5.54 ms: 1.03x faster                                                     |
| tornado_http               | 89.5 ms                                                     | 87.4 ms: 1.02x faster                                                     |
| unpickle_pure_python       | 133 us                                                      | 130 us: 1.02x faster                                                      |
| sympy_str                  | 175 ms                                                      | 172 ms: 1.02x faster                                                      |
| pprint_pformat             | 1.05 sec                                                    | 1.03 sec: 1.02x faster                                                    |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.02x faster                                                     |
| pickle                     | 7.43 us                                                     | 7.41 us: 1.00x faster                                                     |
| sqlglot_optimize           | 34.5 ms                                                     | 34.7 ms: 1.01x slower                                                     |
| pidigits                   | 152 ms                                                      | 153 ms: 1.01x slower                                                      |
| xml_etree_parse            | 93.0 ms                                                     | 94.3 ms: 1.01x slower                                                     |
| sympy_expand               | 284 ms                                                      | 288 ms: 1.01x slower                                                      |
| scimark_fft                | 184 ms                                                      | 188 ms: 1.02x slower                                                      |
| bench_mp_pool              | 69.2 ms                                                     | 70.8 ms: 1.02x slower                                                     |
| async_generators           | 239 ms                                                      | 245 ms: 1.02x slower                                                      |
| async_tree_io              | 731 ms                                                      | 750 ms: 1.03x slower                                                      |
| sympy_integrate            | 13.0 ms                                                     | 13.3 ms: 1.03x slower                                                     |
| unpickle_list              | 2.75 us                                                     | 2.84 us: 1.03x slower                                                     |
| async_tree_memoization     | 339 ms                                                      | 354 ms: 1.04x slower                                                      |
| meteor_contest             | 74.6 ms                                                     | 78.3 ms: 1.05x slower                                                     |
| pyflate                    | 295 ms                                                      | 310 ms: 1.05x slower                                                      |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.72 ms: 1.07x slower                                                     |
| unpickle                   | 8.18 us                                                     | 8.73 us: 1.07x slower                                                     |
| unpack_sequence            | 37.5 ns                                                     | 40.1 ns: 1.07x slower                                                     |
| go                         | 91.6 ms                                                     | 98.6 ms: 1.08x slower                                                     |
| python_startup             | 19.5 ms                                                     | 21.1 ms: 1.09x slower                                                     |
| telco                      | 4.13 ms                                                     | 4.50 ms: 1.09x slower                                                     |
| regex_v8                   | 14.2 ms                                                     | 16.4 ms: 1.15x slower                                                     |
| mdp                        | 1.37 sec                                                    | 1.60 sec: 1.17x slower                                                    |
| python_startup_no_site     | 16.2 ms                                                     | 19.0 ms: 1.17x slower                                                     |
| coverage                   | 40.8 ms                                                     | 47.8 ms: 1.17x slower                                                     |
| scimark_monte_carlo        | 43.7 ms                                                     | 56.2 ms: 1.29x slower                                                     |
| hexiom                     | 4.10 ms                                                     | 5.29 ms: 1.29x slower                                                     |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                              |

Benchmark hidden because not significant (14): async_tree_none_tg, pathlib, asyncio_tcp, sympy_sum, xml_etree_iterparse, gc_traversal, async_tree_io_tg, json, dask, 2to3, pycparser, create_gc_cycles, pickle_list, bench_thread_pool
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.24% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown