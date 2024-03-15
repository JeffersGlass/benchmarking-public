# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_mprotect
- machine: linux-x86_64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.05x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 305 ms: 1.07x slower                                                          |
| chameleon      | 7.23 ms                                                      | 7.52 ms: 1.04x slower                                                         |
| docutils       | 2.87 sec                                                     | 2.93 sec: 1.02x slower                                                        |
| tornado_http   | 121 ms                                                       | 125 ms: 1.03x slower                                                          |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 435 ms: 1.04x faster                                                          |
| async_tree_none_tg         | 431 ms                                                       | 434 ms: 1.01x slower                                                          |
| async_tree_memoization     | 544 ms                                                       | 549 ms: 1.01x slower                                                          |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 706 ms: 1.01x slower                                                          |
| async_tree_memoization_tg  | 540 ms                                                       | 554 ms: 1.03x slower                                                          |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                        |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.04x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                                  |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 261 ms: 1.01x faster                                                          |
| float          | 76.6 ms                                                      | 78.5 ms: 1.02x slower                                                         |
| nbody          | 88.0 ms                                                      | 98.0 ms: 1.11x slower                                                         |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.63 ms: 1.02x slower                                                         |
| regex_compile  | 144 ms                                                       | 147 ms: 1.02x slower                                                          |
| regex_dna      | 239 ms                                                       | 248 ms: 1.04x slower                                                          |
| regex_v8       | 23.6 ms                                                      | 26.0 ms: 1.10x slower                                                         |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 30.6 us: 1.07x faster                                                         |
| pickle               | 10.5 us                                                      | 10.1 us: 1.04x faster                                                         |
| xml_etree_generate   | 86.1 ms                                                      | 84.4 ms: 1.02x faster                                                         |
| unpickle_list        | 4.66 us                                                      | 4.58 us: 1.02x faster                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.17 sec: 1.01x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 145 ms: 1.01x slower                                                          |
| unpickle             | 14.8 us                                                      | 14.9 us: 1.01x slower                                                         |
| json_loads           | 24.4 us                                                      | 25.2 us: 1.03x slower                                                         |
| json_dumps           | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                         |
| unpickle_pure_python | 210 us                                                       | 234 us: 1.12x slower                                                          |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                                  |

Benchmark hidden because not significant (4): xml_etree_iterparse, xml_etree_process, pickle_list, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 14.8 ms: 1.27x slower                                                         |
| python_startup_no_site | 8.64 ms                                                      | 13.3 ms: 1.54x slower                                                         |
| Geometric mean         | (ref)                                                        | 1.40x slower                                                                  |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 119 us: 1.27x faster                                                          |
| comprehensions             | 21.9 us                                                      | 19.0 us: 1.15x faster                                                         |
| generators                 | 37.4 ms                                                      | 33.8 ms: 1.11x faster                                                         |
| pickle_dict                | 32.5 us                                                      | 30.6 us: 1.07x faster                                                         |
| logging_format             | 7.48 us                                                      | 7.18 us: 1.04x faster                                                         |
| async_tree_none            | 452 ms                                                       | 435 ms: 1.04x faster                                                          |
| pickle                     | 10.5 us                                                      | 10.1 us: 1.04x faster                                                         |
| logging_simple             | 6.71 us                                                      | 6.47 us: 1.04x faster                                                         |
| crypto_pyaes               | 80.3 ms                                                      | 77.8 ms: 1.03x faster                                                         |
| sqlite_synth               | 2.77 us                                                      | 2.69 us: 1.03x faster                                                         |
| coroutines                 | 23.0 ms                                                      | 22.4 ms: 1.03x faster                                                         |
| async_generators           | 390 ms                                                       | 381 ms: 1.03x faster                                                          |
| create_gc_cycles           | 1.59 ms                                                      | 1.56 ms: 1.02x faster                                                         |
| xml_etree_generate         | 86.1 ms                                                      | 84.4 ms: 1.02x faster                                                         |
| asyncio_tcp                | 378 ms                                                       | 371 ms: 1.02x faster                                                          |
| unpickle_list              | 4.66 us                                                      | 4.58 us: 1.02x faster                                                         |
| pidigits                   | 265 ms                                                       | 261 ms: 1.01x faster                                                          |
| sympy_sum                  | 162 ms                                                       | 160 ms: 1.01x faster                                                          |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.58 sec: 1.01x faster                                                        |
| tomli_loads                | 2.16 sec                                                     | 2.17 sec: 1.01x slower                                                        |
| xml_etree_parse            | 144 ms                                                       | 145 ms: 1.01x slower                                                          |
| sympy_str                  | 302 ms                                                       | 305 ms: 1.01x slower                                                          |
| async_tree_none_tg         | 431 ms                                                       | 434 ms: 1.01x slower                                                          |
| async_tree_memoization     | 544 ms                                                       | 549 ms: 1.01x slower                                                          |
| unpickle                   | 14.8 us                                                      | 14.9 us: 1.01x slower                                                         |
| spectral_norm              | 91.6 ms                                                      | 92.7 ms: 1.01x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 706 ms: 1.01x slower                                                          |
| raytrace                   | 298 ms                                                       | 303 ms: 1.02x slower                                                          |
| regex_effbot               | 3.57 ms                                                      | 3.63 ms: 1.02x slower                                                         |
| deepcopy                   | 368 us                                                       | 374 us: 1.02x slower                                                          |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                         |
| regex_compile              | 144 ms                                                       | 147 ms: 1.02x slower                                                          |
| docutils                   | 2.87 sec                                                     | 2.93 sec: 1.02x slower                                                        |
| float                      | 76.6 ms                                                      | 78.5 ms: 1.02x slower                                                         |
| pprint_safe_repr           | 807 ms                                                       | 827 ms: 1.02x slower                                                          |
| meteor_contest             | 128 ms                                                       | 131 ms: 1.03x slower                                                          |
| async_tree_memoization_tg  | 540 ms                                                       | 554 ms: 1.03x slower                                                          |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                        |
| pprint_pformat             | 1.65 sec                                                     | 1.70 sec: 1.03x slower                                                        |
| sympy_integrate            | 23.9 ms                                                      | 24.6 ms: 1.03x slower                                                         |
| tornado_http               | 121 ms                                                       | 125 ms: 1.03x slower                                                          |
| deepcopy_memo              | 36.8 us                                                      | 38.0 us: 1.03x slower                                                         |
| sqlglot_parse              | 1.38 ms                                                      | 1.42 ms: 1.03x slower                                                         |
| json_loads                 | 24.4 us                                                      | 25.2 us: 1.03x slower                                                         |
| sqlglot_normalize          | 116 ms                                                       | 120 ms: 1.03x slower                                                          |
| logging_silent             | 94.4 ns                                                      | 97.7 ns: 1.03x slower                                                         |
| json_dumps                 | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                         |
| json                       | 5.12 ms                                                      | 5.31 ms: 1.04x slower                                                         |
| regex_dna                  | 239 ms                                                       | 248 ms: 1.04x slower                                                          |
| chameleon                  | 7.23 ms                                                      | 7.52 ms: 1.04x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.04x slower                                                        |
| bench_thread_pool          | 950 us                                                       | 991 us: 1.04x slower                                                          |
| sqlglot_transpile          | 1.78 ms                                                      | 1.86 ms: 1.05x slower                                                         |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.42 ms: 1.05x slower                                                         |
| dulwich_log                | 65.4 ms                                                      | 68.8 ms: 1.05x slower                                                         |
| pycparser                  | 1.23 sec                                                     | 1.31 sec: 1.06x slower                                                        |
| chaos                      | 64.0 ms                                                      | 67.8 ms: 1.06x slower                                                         |
| sympy_expand               | 484 ms                                                       | 515 ms: 1.06x slower                                                          |
| 2to3                       | 285 ms                                                       | 305 ms: 1.07x slower                                                          |
| scimark_fft                | 301 ms                                                       | 324 ms: 1.08x slower                                                          |
| gc_traversal               | 3.48 ms                                                      | 3.75 ms: 1.08x slower                                                         |
| richards                   | 45.7 ms                                                      | 50.4 ms: 1.10x slower                                                         |
| regex_v8                   | 23.6 ms                                                      | 26.0 ms: 1.10x slower                                                         |
| sqlglot_optimize           | 57.5 ms                                                      | 63.4 ms: 1.10x slower                                                         |
| mypy2                      | 830 ms                                                       | 916 ms: 1.10x slower                                                          |
| fannkuch                   | 350 ms                                                       | 387 ms: 1.11x slower                                                          |
| nbody                      | 88.0 ms                                                      | 98.0 ms: 1.11x slower                                                         |
| unpickle_pure_python       | 210 us                                                       | 234 us: 1.12x slower                                                          |
| richards_super             | 51.3 ms                                                      | 57.3 ms: 1.12x slower                                                         |
| nqueens                    | 89.9 ms                                                      | 102 ms: 1.13x slower                                                          |
| go                         | 150 ms                                                       | 171 ms: 1.14x slower                                                          |
| telco                      | 6.96 ms                                                      | 8.04 ms: 1.15x slower                                                         |
| unpack_sequence            | 53.2 ns                                                      | 61.4 ns: 1.16x slower                                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 80.0 ms: 1.16x slower                                                         |
| deltablue                  | 3.24 ms                                                      | 3.77 ms: 1.17x slower                                                         |
| pyflate                    | 439 ms                                                       | 517 ms: 1.18x slower                                                          |
| coverage                   | 66.7 ms                                                      | 80.4 ms: 1.21x slower                                                         |
| scimark_lu                 | 98.8 ms                                                      | 121 ms: 1.23x slower                                                          |
| hexiom                     | 5.96 ms                                                      | 7.43 ms: 1.25x slower                                                         |
| python_startup             | 11.6 ms                                                      | 14.8 ms: 1.27x slower                                                         |
| scimark_sor                | 109 ms                                                       | 153 ms: 1.40x slower                                                          |
| dask                       | 392 ms                                                       | 591 ms: 1.51x slower                                                          |
| python_startup_no_site     | 8.64 ms                                                      | 13.3 ms: 1.54x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.05x slower                                                                  |

Benchmark hidden because not significant (10): xml_etree_iterparse, mako, xml_etree_process, asyncio_websockets, pickle_list, deepcopy_reduce, mdp, bench_mp_pool, pickle_pure_python, async_tree_cpu_io_mixed
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.11x