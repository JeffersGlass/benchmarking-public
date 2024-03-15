
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: 8efbb6f
- commit date: 2024-02-14
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.95%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 300 ms: 1.05x slower                                                       |
| chameleon      | 7.23 ms                                                      | 7.20 ms: 1.00x faster                                                      |
| docutils       | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                                     |
| tornado_http   | 121 ms                                                       | 123 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                        | 1.02x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 434 ms: 1.04x faster                                                       |
| async_tree_none_tg         | 431 ms                                                       | 434 ms: 1.01x slower                                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 548 ms: 1.01x slower                                                       |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                     |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 709 ms: 1.02x slower                                                       |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 712 ms: 1.02x slower                                                       |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                                     |
| Geometric mean             | (ref)                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 261 ms: 1.01x faster                                                       |
| float          | 76.6 ms                                                      | 78.3 ms: 1.02x slower                                                      |
| nbody          | 88.0 ms                                                      | 102 ms: 1.16x slower                                                       |
| Geometric mean | (ref)                                                        | 1.05x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 241 ms: 1.01x slower                                                       |
| regex_compile  | 144 ms                                                       | 146 ms: 1.01x slower                                                       |
| regex_effbot   | 3.57 ms                                                      | 3.69 ms: 1.03x slower                                                      |
| regex_v8       | 23.6 ms                                                      | 25.7 ms: 1.09x slower                                                      |
| Geometric mean | (ref)                                                        | 1.04x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 318 us                                                       | 306 us: 1.04x faster                                                       |
| pickle               | 10.5 us                                                      | 10.4 us: 1.02x faster                                                      |
| xml_etree_generate   | 86.1 ms                                                      | 85.0 ms: 1.01x faster                                                      |
| xml_etree_process    | 58.4 ms                                                      | 58.1 ms: 1.00x faster                                                      |
| unpickle             | 14.8 us                                                      | 14.9 us: 1.01x slower                                                      |
| pickle_dict          | 32.5 us                                                      | 33.0 us: 1.01x slower                                                      |
| xml_etree_parse      | 144 ms                                                       | 146 ms: 1.01x slower                                                       |
| xml_etree_iterparse  | 103 ms                                                       | 105 ms: 1.02x slower                                                       |
| json_dumps           | 10.2 ms                                                      | 10.5 ms: 1.02x slower                                                      |
| tomli_loads          | 2.16 sec                                                     | 2.22 sec: 1.03x slower                                                     |
| json_loads           | 24.4 us                                                      | 25.2 us: 1.03x slower                                                      |
| unpickle_pure_python | 210 us                                                       | 218 us: 1.04x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (2): pickle_list, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                      |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.29x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.2 ms: 1.02x slower                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 116 us: 1.31x faster                                                       |
| comprehensions             | 21.9 us                                                      | 19.1 us: 1.15x faster                                                      |
| generators                 | 37.4 ms                                                      | 34.0 ms: 1.10x faster                                                      |
| raytrace                   | 298 ms                                                       | 278 ms: 1.07x faster                                                       |
| async_generators           | 390 ms                                                       | 365 ms: 1.07x faster                                                       |
| unpack_sequence            | 53.2 ns                                                      | 50.7 ns: 1.05x faster                                                      |
| logging_format             | 7.48 us                                                      | 7.14 us: 1.05x faster                                                      |
| crypto_pyaes               | 80.3 ms                                                      | 77.0 ms: 1.04x faster                                                      |
| logging_simple             | 6.71 us                                                      | 6.44 us: 1.04x faster                                                      |
| pickle_pure_python         | 318 us                                                       | 306 us: 1.04x faster                                                       |
| async_tree_none            | 452 ms                                                       | 434 ms: 1.04x faster                                                       |
| coroutines                 | 23.0 ms                                                      | 22.3 ms: 1.03x faster                                                      |
| sympy_sum                  | 162 ms                                                       | 157 ms: 1.03x faster                                                       |
| deepcopy_reduce            | 3.37 us                                                      | 3.30 us: 1.02x faster                                                      |
| asyncio_tcp                | 378 ms                                                       | 370 ms: 1.02x faster                                                       |
| chaos                      | 64.0 ms                                                      | 62.8 ms: 1.02x faster                                                      |
| pickle                     | 10.5 us                                                      | 10.4 us: 1.02x faster                                                      |
| create_gc_cycles           | 1.59 ms                                                      | 1.57 ms: 1.02x faster                                                      |
| pidigits                   | 265 ms                                                       | 261 ms: 1.01x faster                                                       |
| xml_etree_generate         | 86.1 ms                                                      | 85.0 ms: 1.01x faster                                                      |
| mdp                        | 2.57 sec                                                     | 2.54 sec: 1.01x faster                                                     |
| sympy_str                  | 302 ms                                                       | 298 ms: 1.01x faster                                                       |
| pprint_pformat             | 1.65 sec                                                     | 1.63 sec: 1.01x faster                                                     |
| scimark_lu                 | 98.8 ms                                                      | 97.6 ms: 1.01x faster                                                      |
| deepcopy_memo              | 36.8 us                                                      | 36.4 us: 1.01x faster                                                      |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                                     |
| pprint_safe_repr           | 807 ms                                                       | 801 ms: 1.01x faster                                                       |
| xml_etree_process          | 58.4 ms                                                      | 58.1 ms: 1.00x faster                                                      |
| sqlite_synth               | 2.77 us                                                      | 2.76 us: 1.00x faster                                                      |
| chameleon                  | 7.23 ms                                                      | 7.20 ms: 1.00x faster                                                      |
| sympy_integrate            | 23.9 ms                                                      | 24.0 ms: 1.00x slower                                                      |
| docutils                   | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                                     |
| meteor_contest             | 128 ms                                                       | 129 ms: 1.01x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 434 ms: 1.01x slower                                                       |
| unpickle                   | 14.8 us                                                      | 14.9 us: 1.01x slower                                                      |
| regex_dna                  | 239 ms                                                       | 241 ms: 1.01x slower                                                       |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                      |
| regex_compile              | 144 ms                                                       | 146 ms: 1.01x slower                                                       |
| sqlglot_parse              | 1.38 ms                                                      | 1.39 ms: 1.01x slower                                                      |
| pickle_dict                | 32.5 us                                                      | 33.0 us: 1.01x slower                                                      |
| async_tree_memoization_tg  | 540 ms                                                       | 548 ms: 1.01x slower                                                       |
| xml_etree_parse            | 144 ms                                                       | 146 ms: 1.01x slower                                                       |
| tornado_http               | 121 ms                                                       | 123 ms: 1.02x slower                                                       |
| async_tree_io_tg           | 1.05 sec                                                     | 1.07 sec: 1.02x slower                                                     |
| xml_etree_iterparse        | 103 ms                                                       | 105 ms: 1.02x slower                                                       |
| mako                       | 10.0 ms                                                      | 10.2 ms: 1.02x slower                                                      |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 709 ms: 1.02x slower                                                       |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 712 ms: 1.02x slower                                                       |
| json_dumps                 | 10.2 ms                                                      | 10.5 ms: 1.02x slower                                                      |
| float                      | 76.6 ms                                                      | 78.3 ms: 1.02x slower                                                      |
| bench_thread_pool          | 950 us                                                       | 972 us: 1.02x slower                                                       |
| sqlglot_transpile          | 1.78 ms                                                      | 1.82 ms: 1.02x slower                                                      |
| tomli_loads                | 2.16 sec                                                     | 2.22 sec: 1.03x slower                                                     |
| dask                       | 392 ms                                                       | 404 ms: 1.03x slower                                                       |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.34 ms: 1.03x slower                                                      |
| scimark_monte_carlo        | 69.0 ms                                                      | 71.1 ms: 1.03x slower                                                      |
| regex_effbot               | 3.57 ms                                                      | 3.69 ms: 1.03x slower                                                      |
| json_loads                 | 24.4 us                                                      | 25.2 us: 1.03x slower                                                      |
| bench_mp_pool              | 4.76 ms                                                      | 4.92 ms: 1.03x slower                                                      |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.03x slower                                                     |
| sqlglot_optimize           | 57.5 ms                                                      | 59.7 ms: 1.04x slower                                                      |
| unpickle_pure_python       | 210 us                                                       | 218 us: 1.04x slower                                                       |
| sympy_expand               | 484 ms                                                       | 503 ms: 1.04x slower                                                       |
| spectral_norm              | 91.6 ms                                                      | 95.3 ms: 1.04x slower                                                      |
| nqueens                    | 89.9 ms                                                      | 93.6 ms: 1.04x slower                                                      |
| json                       | 5.12 ms                                                      | 5.36 ms: 1.05x slower                                                      |
| 2to3                       | 285 ms                                                       | 300 ms: 1.05x slower                                                       |
| dulwich_log                | 65.4 ms                                                      | 69.1 ms: 1.06x slower                                                      |
| pycparser                  | 1.23 sec                                                     | 1.31 sec: 1.06x slower                                                     |
| regex_v8                   | 23.6 ms                                                      | 25.7 ms: 1.09x slower                                                      |
| python_startup             | 11.6 ms                                                      | 12.7 ms: 1.09x slower                                                      |
| scimark_fft                | 301 ms                                                       | 335 ms: 1.11x slower                                                       |
| go                         | 150 ms                                                       | 167 ms: 1.11x slower                                                       |
| deltablue                  | 3.24 ms                                                      | 3.63 ms: 1.12x slower                                                      |
| gc_traversal               | 3.48 ms                                                      | 3.94 ms: 1.13x slower                                                      |
| fannkuch                   | 350 ms                                                       | 401 ms: 1.15x slower                                                       |
| telco                      | 6.96 ms                                                      | 8.03 ms: 1.15x slower                                                      |
| pyflate                    | 439 ms                                                       | 508 ms: 1.16x slower                                                       |
| nbody                      | 88.0 ms                                                      | 102 ms: 1.16x slower                                                       |
| richards_super             | 51.3 ms                                                      | 59.6 ms: 1.16x slower                                                      |
| hexiom                     | 5.96 ms                                                      | 6.93 ms: 1.16x slower                                                      |
| richards                   | 45.7 ms                                                      | 53.6 ms: 1.17x slower                                                      |
| coverage                   | 66.7 ms                                                      | 84.2 ms: 1.26x slower                                                      |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.29x slower                                                      |
| scimark_sor                | 109 ms                                                       | 143 ms: 1.31x slower                                                       |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                               |

Benchmark hidden because not significant (8): pickle_list, deepcopy, asyncio_websockets, logging_silent, sqlglot_normalize, unpickle_list, async_tree_memoization, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.95% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.93x