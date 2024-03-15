
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_ghccc
- machine: linux-x86_64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.04x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.92x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 298 ms: 1.05x slower                                                       |
| chameleon      | 7.23 ms                                                      | 7.60 ms: 1.05x slower                                                      |
| docutils       | 2.87 sec                                                     | 2.90 sec: 1.01x slower                                                     |
| tornado_http   | 121 ms                                                       | 124 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                        | 1.03x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 435 ms: 1.04x faster                                                       |
| async_tree_none_tg         | 431 ms                                                       | 436 ms: 1.01x slower                                                       |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 706 ms: 1.01x slower                                                       |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                     |
| async_tree_memoization_tg  | 540 ms                                                       | 551 ms: 1.02x slower                                                       |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                                     |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 262 ms: 1.01x faster                                                       |
| float          | 76.6 ms                                                      | 80.5 ms: 1.05x slower                                                      |
| nbody          | 88.0 ms                                                      | 94.1 ms: 1.07x slower                                                      |
| Geometric mean | (ref)                                                        | 1.04x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.61 ms: 1.01x slower                                                      |
| regex_compile  | 144 ms                                                       | 146 ms: 1.01x slower                                                       |
| regex_dna      | 239 ms                                                       | 248 ms: 1.04x slower                                                       |
| regex_v8       | 23.6 ms                                                      | 26.1 ms: 1.10x slower                                                      |
| Geometric mean | (ref)                                                        | 1.04x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 30.9 us: 1.05x faster                                                      |
| pickle_pure_python   | 318 us                                                       | 307 us: 1.04x faster                                                       |
| pickle               | 10.5 us                                                      | 10.3 us: 1.03x faster                                                      |
| xml_etree_generate   | 86.1 ms                                                      | 85.9 ms: 1.00x faster                                                      |
| pickle_list          | 4.43 us                                                      | 4.46 us: 1.01x slower                                                      |
| xml_etree_process    | 58.4 ms                                                      | 59.1 ms: 1.01x slower                                                      |
| unpickle             | 14.8 us                                                      | 15.1 us: 1.02x slower                                                      |
| xml_etree_iterparse  | 103 ms                                                       | 105 ms: 1.02x slower                                                       |
| json_loads           | 24.4 us                                                      | 25.0 us: 1.03x slower                                                      |
| xml_etree_parse      | 144 ms                                                       | 148 ms: 1.03x slower                                                       |
| json_dumps           | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                      |
| unpickle_list        | 4.66 us                                                      | 4.93 us: 1.06x slower                                                      |
| tomli_loads          | 2.16 sec                                                     | 2.31 sec: 1.07x slower                                                     |
| unpickle_pure_python | 210 us                                                       | 230 us: 1.10x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                      |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.29x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 11.6 ms: 1.16x slower                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240203-pythonperf2-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 121 us: 1.26x faster                                                       |
| unpack_sequence            | 53.2 ns                                                      | 45.8 ns: 1.16x faster                                                      |
| raytrace                   | 298 ms                                                       | 270 ms: 1.10x faster                                                       |
| generators                 | 37.4 ms                                                      | 34.4 ms: 1.09x faster                                                      |
| comprehensions             | 21.9 us                                                      | 20.3 us: 1.08x faster                                                      |
| crypto_pyaes               | 80.3 ms                                                      | 75.0 ms: 1.07x faster                                                      |
| async_generators           | 390 ms                                                       | 366 ms: 1.07x faster                                                       |
| pickle_dict                | 32.5 us                                                      | 30.9 us: 1.05x faster                                                      |
| create_gc_cycles           | 1.59 ms                                                      | 1.52 ms: 1.05x faster                                                      |
| async_tree_none            | 452 ms                                                       | 435 ms: 1.04x faster                                                       |
| pickle_pure_python         | 318 us                                                       | 307 us: 1.04x faster                                                       |
| logging_format             | 7.48 us                                                      | 7.27 us: 1.03x faster                                                      |
| pickle                     | 10.5 us                                                      | 10.3 us: 1.03x faster                                                      |
| deepcopy_reduce            | 3.37 us                                                      | 3.29 us: 1.02x faster                                                      |
| sympy_sum                  | 162 ms                                                       | 158 ms: 1.02x faster                                                       |
| asyncio_tcp                | 378 ms                                                       | 370 ms: 1.02x faster                                                       |
| logging_simple             | 6.71 us                                                      | 6.57 us: 1.02x faster                                                      |
| sympy_str                  | 302 ms                                                       | 297 ms: 1.02x faster                                                       |
| coroutines                 | 23.0 ms                                                      | 22.7 ms: 1.02x faster                                                      |
| sqlite_synth               | 2.77 us                                                      | 2.74 us: 1.01x faster                                                      |
| pidigits                   | 265 ms                                                       | 262 ms: 1.01x faster                                                       |
| pathlib                    | 18.9 ms                                                      | 18.7 ms: 1.01x faster                                                      |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                                     |
| mdp                        | 2.57 sec                                                     | 2.55 sec: 1.01x faster                                                     |
| xml_etree_generate         | 86.1 ms                                                      | 85.9 ms: 1.00x faster                                                      |
| deepcopy                   | 368 us                                                       | 371 us: 1.01x slower                                                       |
| pickle_list                | 4.43 us                                                      | 4.46 us: 1.01x slower                                                      |
| sympy_integrate            | 23.9 ms                                                      | 24.1 ms: 1.01x slower                                                      |
| sqlglot_parse              | 1.38 ms                                                      | 1.39 ms: 1.01x slower                                                      |
| docutils                   | 2.87 sec                                                     | 2.90 sec: 1.01x slower                                                     |
| regex_effbot               | 3.57 ms                                                      | 3.61 ms: 1.01x slower                                                      |
| xml_etree_process          | 58.4 ms                                                      | 59.1 ms: 1.01x slower                                                      |
| regex_compile              | 144 ms                                                       | 146 ms: 1.01x slower                                                       |
| json                       | 5.12 ms                                                      | 5.18 ms: 1.01x slower                                                      |
| async_tree_none_tg         | 431 ms                                                       | 436 ms: 1.01x slower                                                       |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 706 ms: 1.01x slower                                                       |
| logging_silent             | 94.4 ns                                                      | 95.8 ns: 1.01x slower                                                      |
| unpickle                   | 14.8 us                                                      | 15.1 us: 1.02x slower                                                      |
| sqlglot_transpile          | 1.78 ms                                                      | 1.81 ms: 1.02x slower                                                      |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                     |
| async_tree_memoization_tg  | 540 ms                                                       | 551 ms: 1.02x slower                                                       |
| xml_etree_iterparse        | 103 ms                                                       | 105 ms: 1.02x slower                                                       |
| meteor_contest             | 128 ms                                                       | 131 ms: 1.02x slower                                                       |
| json_loads                 | 24.4 us                                                      | 25.0 us: 1.03x slower                                                      |
| tornado_http               | 121 ms                                                       | 124 ms: 1.03x slower                                                       |
| dask                       | 392 ms                                                       | 404 ms: 1.03x slower                                                       |
| xml_etree_parse            | 144 ms                                                       | 148 ms: 1.03x slower                                                       |
| scimark_lu                 | 98.8 ms                                                      | 102 ms: 1.03x slower                                                       |
| deepcopy_memo              | 36.8 us                                                      | 37.9 us: 1.03x slower                                                      |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                                     |
| sympy_expand               | 484 ms                                                       | 501 ms: 1.03x slower                                                       |
| json_dumps                 | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                      |
| regex_dna                  | 239 ms                                                       | 248 ms: 1.04x slower                                                       |
| dulwich_log                | 65.4 ms                                                      | 67.9 ms: 1.04x slower                                                      |
| sqlglot_normalize          | 116 ms                                                       | 120 ms: 1.04x slower                                                       |
| pycparser                  | 1.23 sec                                                     | 1.29 sec: 1.04x slower                                                     |
| chaos                      | 64.0 ms                                                      | 66.8 ms: 1.04x slower                                                      |
| 2to3                       | 285 ms                                                       | 298 ms: 1.05x slower                                                       |
| float                      | 76.6 ms                                                      | 80.5 ms: 1.05x slower                                                      |
| chameleon                  | 7.23 ms                                                      | 7.60 ms: 1.05x slower                                                      |
| unpickle_list              | 4.66 us                                                      | 4.93 us: 1.06x slower                                                      |
| pprint_safe_repr           | 807 ms                                                       | 858 ms: 1.06x slower                                                       |
| nqueens                    | 89.9 ms                                                      | 95.8 ms: 1.07x slower                                                      |
| sqlglot_optimize           | 57.5 ms                                                      | 61.5 ms: 1.07x slower                                                      |
| nbody                      | 88.0 ms                                                      | 94.1 ms: 1.07x slower                                                      |
| tomli_loads                | 2.16 sec                                                     | 2.31 sec: 1.07x slower                                                     |
| bench_mp_pool              | 4.76 ms                                                      | 5.11 ms: 1.07x slower                                                      |
| pprint_pformat             | 1.65 sec                                                     | 1.79 sec: 1.08x slower                                                     |
| python_startup             | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                      |
| unpickle_pure_python       | 210 us                                                       | 230 us: 1.10x slower                                                       |
| richards_super             | 51.3 ms                                                      | 56.4 ms: 1.10x slower                                                      |
| scimark_monte_carlo        | 69.0 ms                                                      | 75.8 ms: 1.10x slower                                                      |
| regex_v8                   | 23.6 ms                                                      | 26.1 ms: 1.10x slower                                                      |
| richards                   | 45.7 ms                                                      | 50.6 ms: 1.11x slower                                                      |
| gc_traversal               | 3.48 ms                                                      | 3.88 ms: 1.12x slower                                                      |
| go                         | 150 ms                                                       | 168 ms: 1.13x slower                                                       |
| scimark_fft                | 301 ms                                                       | 346 ms: 1.15x slower                                                       |
| pyflate                    | 439 ms                                                       | 506 ms: 1.15x slower                                                       |
| mako                       | 10.0 ms                                                      | 11.6 ms: 1.16x slower                                                      |
| telco                      | 6.96 ms                                                      | 8.11 ms: 1.16x slower                                                      |
| fannkuch                   | 350 ms                                                       | 409 ms: 1.17x slower                                                       |
| coverage                   | 66.7 ms                                                      | 79.3 ms: 1.19x slower                                                      |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 5.03 ms: 1.20x slower                                                      |
| deltablue                  | 3.24 ms                                                      | 3.91 ms: 1.21x slower                                                      |
| spectral_norm              | 91.6 ms                                                      | 112 ms: 1.22x slower                                                       |
| hexiom                     | 5.96 ms                                                      | 7.60 ms: 1.27x slower                                                      |
| scimark_sor                | 109 ms                                                       | 140 ms: 1.29x slower                                                       |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.29x slower                                                      |
| Geometric mean             | (ref)                                                        | 1.04x slower                                                               |

Benchmark hidden because not significant (5): asyncio_websockets, async_tree_cpu_io_mixed, async_tree_memoization, bench_thread_pool, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.92x