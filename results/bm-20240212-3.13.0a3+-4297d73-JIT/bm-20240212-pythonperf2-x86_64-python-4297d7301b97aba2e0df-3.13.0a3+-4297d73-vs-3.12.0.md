
# Results vs. 3.12.0

- fork: python
- ref: 4297d7301b97aba2e0df
- machine: linux-x86_64
- commit hash: 4297d73
- commit date: 2024-02-12
- overall geometric mean: 1.04x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 298 ms: 1.05x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.54 ms: 1.04x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                                       |
| tornado_http   | 121 ms                                                       | 124 ms: 1.02x slower                                                         |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|---------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none           | 452 ms                                                       | 431 ms: 1.05x faster                                                         |
| async_tree_memoization_tg | 540 ms                                                       | 545 ms: 1.01x slower                                                         |
| async_tree_none_tg        | 431 ms                                                       | 435 ms: 1.01x slower                                                         |
| async_tree_io_tg          | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                       |
| async_tree_io             | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| Geometric mean            | (ref)                                                        | 1.00x slower                                                                 |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 263 ms: 1.01x faster                                                         |
| float          | 76.6 ms                                                      | 81.7 ms: 1.07x slower                                                        |
| nbody          | 88.0 ms                                                      | 107 ms: 1.21x slower                                                         |
| Geometric mean | (ref)                                                        | 1.09x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 240 ms: 1.01x slower                                                         |
| regex_compile  | 144 ms                                                       | 146 ms: 1.02x slower                                                         |
| regex_effbot   | 3.57 ms                                                      | 3.69 ms: 1.03x slower                                                        |
| regex_v8       | 23.6 ms                                                      | 26.3 ms: 1.11x slower                                                        |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 318 us                                                       | 301 us: 1.06x faster                                                         |
| xml_etree_generate   | 86.1 ms                                                      | 84.5 ms: 1.02x faster                                                        |
| pickle               | 10.5 us                                                      | 10.5 us: 1.01x faster                                                        |
| pickle_dict          | 32.5 us                                                      | 32.7 us: 1.00x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.5 ms: 1.02x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| json_loads           | 24.4 us                                                      | 25.2 us: 1.04x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 107 ms: 1.04x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.31 sec: 1.07x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 228 us: 1.09x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (4): xml_etree_process, unpickle_list, pickle_list, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 11.8 ms: 1.18x slower                                                        |

All benchmarks:
===============

| Benchmark                 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|---------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols  | 152 us                                                       | 119 us: 1.27x faster                                                         |
| unpack_sequence           | 53.2 ns                                                      | 45.1 ns: 1.18x faster                                                        |
| generators                | 37.4 ms                                                      | 33.6 ms: 1.11x faster                                                        |
| raytrace                  | 298 ms                                                       | 275 ms: 1.08x faster                                                         |
| comprehensions            | 21.9 us                                                      | 20.7 us: 1.06x faster                                                        |
| pickle_pure_python        | 318 us                                                       | 301 us: 1.06x faster                                                         |
| async_generators          | 390 ms                                                       | 370 ms: 1.05x faster                                                         |
| async_tree_none           | 452 ms                                                       | 431 ms: 1.05x faster                                                         |
| create_gc_cycles          | 1.59 ms                                                      | 1.53 ms: 1.04x faster                                                        |
| asyncio_tcp               | 378 ms                                                       | 369 ms: 1.03x faster                                                         |
| coroutines                | 23.0 ms                                                      | 22.4 ms: 1.03x faster                                                        |
| logging_format            | 7.48 us                                                      | 7.33 us: 1.02x faster                                                        |
| xml_etree_generate        | 86.1 ms                                                      | 84.5 ms: 1.02x faster                                                        |
| sympy_sum                 | 162 ms                                                       | 159 ms: 1.02x faster                                                         |
| logging_simple            | 6.71 us                                                      | 6.60 us: 1.02x faster                                                        |
| scimark_lu                | 98.8 ms                                                      | 97.6 ms: 1.01x faster                                                        |
| sqlite_synth              | 2.77 us                                                      | 2.74 us: 1.01x faster                                                        |
| deepcopy_reduce           | 3.37 us                                                      | 3.34 us: 1.01x faster                                                        |
| sympy_str                 | 302 ms                                                       | 299 ms: 1.01x faster                                                         |
| asyncio_tcp_ssl           | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                                       |
| pidigits                  | 265 ms                                                       | 263 ms: 1.01x faster                                                         |
| pickle                    | 10.5 us                                                      | 10.5 us: 1.01x faster                                                        |
| mdp                       | 2.57 sec                                                     | 2.56 sec: 1.01x faster                                                       |
| sqlglot_parse             | 1.38 ms                                                      | 1.37 ms: 1.00x faster                                                        |
| docutils                  | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                                       |
| pickle_dict               | 32.5 us                                                      | 32.7 us: 1.00x slower                                                        |
| pathlib                   | 18.9 ms                                                      | 19.0 ms: 1.01x slower                                                        |
| deepcopy_memo             | 36.8 us                                                      | 37.0 us: 1.01x slower                                                        |
| logging_silent            | 94.4 ns                                                      | 95.1 ns: 1.01x slower                                                        |
| regex_dna                 | 239 ms                                                       | 240 ms: 1.01x slower                                                         |
| async_tree_memoization_tg | 540 ms                                                       | 545 ms: 1.01x slower                                                         |
| async_tree_none_tg        | 431 ms                                                       | 435 ms: 1.01x slower                                                         |
| sqlglot_transpile         | 1.78 ms                                                      | 1.80 ms: 1.01x slower                                                        |
| meteor_contest            | 128 ms                                                       | 130 ms: 1.01x slower                                                         |
| sympy_integrate           | 23.9 ms                                                      | 24.3 ms: 1.01x slower                                                        |
| regex_compile             | 144 ms                                                       | 146 ms: 1.02x slower                                                         |
| async_tree_io_tg          | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                       |
| json_dumps                | 10.2 ms                                                      | 10.5 ms: 1.02x slower                                                        |
| tornado_http              | 121 ms                                                       | 124 ms: 1.02x slower                                                         |
| sqlglot_normalize         | 116 ms                                                       | 119 ms: 1.03x slower                                                         |
| async_tree_io             | 1.04 sec                                                     | 1.07 sec: 1.03x slower                                                       |
| dask                      | 392 ms                                                       | 403 ms: 1.03x slower                                                         |
| xml_etree_parse           | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| regex_effbot              | 3.57 ms                                                      | 3.69 ms: 1.03x slower                                                        |
| sympy_expand              | 484 ms                                                       | 501 ms: 1.04x slower                                                         |
| json_loads                | 24.4 us                                                      | 25.2 us: 1.04x slower                                                        |
| xml_etree_iterparse       | 103 ms                                                       | 107 ms: 1.04x slower                                                         |
| pprint_pformat            | 1.65 sec                                                     | 1.72 sec: 1.04x slower                                                       |
| json                      | 5.12 ms                                                      | 5.33 ms: 1.04x slower                                                        |
| chameleon                 | 7.23 ms                                                      | 7.54 ms: 1.04x slower                                                        |
| 2to3                      | 285 ms                                                       | 298 ms: 1.05x slower                                                         |
| gc_traversal              | 3.48 ms                                                      | 3.64 ms: 1.05x slower                                                        |
| pprint_safe_repr          | 807 ms                                                       | 847 ms: 1.05x slower                                                         |
| dulwich_log               | 65.4 ms                                                      | 69.3 ms: 1.06x slower                                                        |
| pycparser                 | 1.23 sec                                                     | 1.31 sec: 1.06x slower                                                       |
| sqlglot_optimize          | 57.5 ms                                                      | 61.1 ms: 1.06x slower                                                        |
| float                     | 76.6 ms                                                      | 81.7 ms: 1.07x slower                                                        |
| tomli_loads               | 2.16 sec                                                     | 2.31 sec: 1.07x slower                                                       |
| nqueens                   | 89.9 ms                                                      | 97.4 ms: 1.08x slower                                                        |
| python_startup            | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| unpickle_pure_python      | 210 us                                                       | 228 us: 1.09x slower                                                         |
| chaos                     | 64.0 ms                                                      | 70.3 ms: 1.10x slower                                                        |
| richards_super            | 51.3 ms                                                      | 56.9 ms: 1.11x slower                                                        |
| regex_v8                  | 23.6 ms                                                      | 26.3 ms: 1.11x slower                                                        |
| richards                  | 45.7 ms                                                      | 51.0 ms: 1.12x slower                                                        |
| go                        | 150 ms                                                       | 169 ms: 1.13x slower                                                         |
| scimark_monte_carlo       | 69.0 ms                                                      | 78.5 ms: 1.14x slower                                                        |
| deltablue                 | 3.24 ms                                                      | 3.68 ms: 1.14x slower                                                        |
| fannkuch                  | 350 ms                                                       | 406 ms: 1.16x slower                                                         |
| telco                     | 6.96 ms                                                      | 8.15 ms: 1.17x slower                                                        |
| mako                      | 10.0 ms                                                      | 11.8 ms: 1.18x slower                                                        |
| pyflate                   | 439 ms                                                       | 521 ms: 1.19x slower                                                         |
| scimark_sparse_mat_mult   | 4.21 ms                                                      | 5.01 ms: 1.19x slower                                                        |
| scimark_fft               | 301 ms                                                       | 360 ms: 1.20x slower                                                         |
| nbody                     | 88.0 ms                                                      | 107 ms: 1.21x slower                                                         |
| coverage                  | 66.7 ms                                                      | 81.8 ms: 1.23x slower                                                        |
| python_startup_no_site    | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                        |
| spectral_norm             | 91.6 ms                                                      | 118 ms: 1.29x slower                                                         |
| hexiom                    | 5.96 ms                                                      | 7.70 ms: 1.29x slower                                                        |
| scimark_sor               | 109 ms                                                       | 142 ms: 1.30x slower                                                         |
| Geometric mean            | (ref)                                                        | 1.04x slower                                                                 |

Benchmark hidden because not significant (13): xml_etree_process, bench_mp_pool, deepcopy, unpickle_list, pickle_list, unpickle, asyncio_websockets, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization, crypto_pyaes, bench_thread_pool, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.91x