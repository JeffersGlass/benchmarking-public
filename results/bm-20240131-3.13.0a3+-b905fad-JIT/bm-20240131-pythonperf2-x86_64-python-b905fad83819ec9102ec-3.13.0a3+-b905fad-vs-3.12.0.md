
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: linux-x86_64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.92x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 299 ms: 1.05x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.69 ms: 1.06x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.89 sec: 1.01x slower                                                       |
| tornado_http   | 121 ms                                                       | 124 ms: 1.03x slower                                                         |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 438 ms: 1.03x faster                                                         |
| async_tree_memoization     | 544 ms                                                       | 550 ms: 1.01x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 710 ms: 1.02x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 442 ms: 1.03x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 558 ms: 1.03x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.04x slower                                                       |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 262 ms: 1.01x faster                                                         |
| float          | 76.6 ms                                                      | 81.7 ms: 1.07x slower                                                        |
| nbody          | 88.0 ms                                                      | 107 ms: 1.21x slower                                                         |
| Geometric mean | (ref)                                                        | 1.09x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.46 ms: 1.03x faster                                                        |
| regex_dna      | 239 ms                                                       | 232 ms: 1.03x faster                                                         |
| regex_compile  | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 24.4 ms: 1.03x slower                                                        |
| Geometric mean | (ref)                                                        | 1.00x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 318 us                                                       | 308 us: 1.03x faster                                                         |
| xml_etree_generate   | 86.1 ms                                                      | 86.6 ms: 1.01x slower                                                        |
| pickle_dict          | 32.5 us                                                      | 32.8 us: 1.01x slower                                                        |
| pickle               | 10.5 us                                                      | 10.6 us: 1.01x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| xml_etree_process    | 58.4 ms                                                      | 59.6 ms: 1.02x slower                                                        |
| unpickle_list        | 4.66 us                                                      | 4.77 us: 1.02x slower                                                        |
| json_loads           | 24.4 us                                                      | 25.1 us: 1.03x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 106 ms: 1.03x slower                                                         |
| pickle_list          | 4.43 us                                                      | 4.62 us: 1.04x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                        |
| tomli_loads          | 2.16 sec                                                     | 2.35 sec: 1.09x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 232 us: 1.11x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 12.0 ms: 1.20x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 119 us: 1.27x faster                                                         |
| unpack_sequence            | 53.2 ns                                                      | 45.9 ns: 1.16x faster                                                        |
| raytrace                   | 298 ms                                                       | 281 ms: 1.06x faster                                                         |
| comprehensions             | 21.9 us                                                      | 20.7 us: 1.06x faster                                                        |
| generators                 | 37.4 ms                                                      | 35.6 ms: 1.05x faster                                                        |
| async_generators           | 390 ms                                                       | 374 ms: 1.04x faster                                                         |
| create_gc_cycles           | 1.59 ms                                                      | 1.54 ms: 1.04x faster                                                        |
| pickle_pure_python         | 318 us                                                       | 308 us: 1.03x faster                                                         |
| async_tree_none            | 452 ms                                                       | 438 ms: 1.03x faster                                                         |
| regex_effbot               | 3.57 ms                                                      | 3.46 ms: 1.03x faster                                                        |
| regex_dna                  | 239 ms                                                       | 232 ms: 1.03x faster                                                         |
| coroutines                 | 23.0 ms                                                      | 22.5 ms: 1.02x faster                                                        |
| sqlite_synth               | 2.77 us                                                      | 2.72 us: 1.02x faster                                                        |
| sympy_sum                  | 162 ms                                                       | 159 ms: 1.02x faster                                                         |
| asyncio_tcp                | 378 ms                                                       | 372 ms: 1.02x faster                                                         |
| deepcopy_reduce            | 3.37 us                                                      | 3.33 us: 1.01x faster                                                        |
| pidigits                   | 265 ms                                                       | 262 ms: 1.01x faster                                                         |
| sympy_str                  | 302 ms                                                       | 300 ms: 1.01x faster                                                         |
| mdp                        | 2.57 sec                                                     | 2.58 sec: 1.00x slower                                                       |
| logging_silent             | 94.4 ns                                                      | 94.9 ns: 1.01x slower                                                        |
| xml_etree_generate         | 86.1 ms                                                      | 86.6 ms: 1.01x slower                                                        |
| docutils                   | 2.87 sec                                                     | 2.89 sec: 1.01x slower                                                       |
| pickle_dict                | 32.5 us                                                      | 32.8 us: 1.01x slower                                                        |
| pickle                     | 10.5 us                                                      | 10.6 us: 1.01x slower                                                        |
| async_tree_memoization     | 544 ms                                                       | 550 ms: 1.01x slower                                                         |
| sympy_integrate            | 23.9 ms                                                      | 24.2 ms: 1.01x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                        |
| logging_format             | 7.48 us                                                      | 7.58 us: 1.01x slower                                                        |
| crypto_pyaes               | 80.3 ms                                                      | 81.5 ms: 1.01x slower                                                        |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 710 ms: 1.02x slower                                                         |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| xml_etree_process          | 58.4 ms                                                      | 59.6 ms: 1.02x slower                                                        |
| sqlglot_parse              | 1.38 ms                                                      | 1.41 ms: 1.02x slower                                                        |
| deepcopy_memo              | 36.8 us                                                      | 37.6 us: 1.02x slower                                                        |
| regex_compile              | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| json                       | 5.12 ms                                                      | 5.24 ms: 1.02x slower                                                        |
| scimark_lu                 | 98.8 ms                                                      | 101 ms: 1.02x slower                                                         |
| sqlglot_normalize          | 116 ms                                                       | 119 ms: 1.02x slower                                                         |
| unpickle_list              | 4.66 us                                                      | 4.77 us: 1.02x slower                                                        |
| deepcopy                   | 368 us                                                       | 378 us: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 442 ms: 1.03x slower                                                         |
| tornado_http               | 121 ms                                                       | 124 ms: 1.03x slower                                                         |
| json_loads                 | 24.4 us                                                      | 25.1 us: 1.03x slower                                                        |
| bench_thread_pool          | 950 us                                                       | 979 us: 1.03x slower                                                         |
| regex_v8                   | 23.6 ms                                                      | 24.4 ms: 1.03x slower                                                        |
| async_tree_memoization_tg  | 540 ms                                                       | 558 ms: 1.03x slower                                                         |
| xml_etree_iterparse        | 103 ms                                                       | 106 ms: 1.03x slower                                                         |
| dask                       | 392 ms                                                       | 406 ms: 1.03x slower                                                         |
| sqlglot_transpile          | 1.78 ms                                                      | 1.84 ms: 1.04x slower                                                        |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.04x slower                                                       |
| pycparser                  | 1.23 sec                                                     | 1.28 sec: 1.04x slower                                                       |
| pickle_list                | 4.43 us                                                      | 4.62 us: 1.04x slower                                                        |
| sympy_expand               | 484 ms                                                       | 505 ms: 1.04x slower                                                         |
| meteor_contest             | 128 ms                                                       | 134 ms: 1.05x slower                                                         |
| 2to3                       | 285 ms                                                       | 299 ms: 1.05x slower                                                         |
| gc_traversal               | 3.48 ms                                                      | 3.65 ms: 1.05x slower                                                        |
| dulwich_log                | 65.4 ms                                                      | 68.7 ms: 1.05x slower                                                        |
| bench_mp_pool              | 4.76 ms                                                      | 5.02 ms: 1.05x slower                                                        |
| json_dumps                 | 10.2 ms                                                      | 10.8 ms: 1.06x slower                                                        |
| chameleon                  | 7.23 ms                                                      | 7.69 ms: 1.06x slower                                                        |
| float                      | 76.6 ms                                                      | 81.7 ms: 1.07x slower                                                        |
| sqlglot_optimize           | 57.5 ms                                                      | 61.5 ms: 1.07x slower                                                        |
| pprint_safe_repr           | 807 ms                                                       | 865 ms: 1.07x slower                                                         |
| nqueens                    | 89.9 ms                                                      | 96.9 ms: 1.08x slower                                                        |
| pprint_pformat             | 1.65 sec                                                     | 1.79 sec: 1.08x slower                                                       |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| tomli_loads                | 2.16 sec                                                     | 2.35 sec: 1.09x slower                                                       |
| unpickle_pure_python       | 210 us                                                       | 232 us: 1.11x slower                                                         |
| richards_super             | 51.3 ms                                                      | 56.9 ms: 1.11x slower                                                        |
| richards                   | 45.7 ms                                                      | 50.8 ms: 1.11x slower                                                        |
| chaos                      | 64.0 ms                                                      | 71.6 ms: 1.12x slower                                                        |
| go                         | 150 ms                                                       | 169 ms: 1.13x slower                                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 79.0 ms: 1.14x slower                                                        |
| pyflate                    | 439 ms                                                       | 520 ms: 1.19x slower                                                         |
| fannkuch                   | 350 ms                                                       | 415 ms: 1.19x slower                                                         |
| telco                      | 6.96 ms                                                      | 8.34 ms: 1.20x slower                                                        |
| mako                       | 10.0 ms                                                      | 12.0 ms: 1.20x slower                                                        |
| scimark_fft                | 301 ms                                                       | 365 ms: 1.21x slower                                                         |
| nbody                      | 88.0 ms                                                      | 107 ms: 1.21x slower                                                         |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 5.14 ms: 1.22x slower                                                        |
| deltablue                  | 3.24 ms                                                      | 4.03 ms: 1.25x slower                                                        |
| spectral_norm              | 91.6 ms                                                      | 116 ms: 1.27x slower                                                         |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                        |
| coverage                   | 66.7 ms                                                      | 86.7 ms: 1.30x slower                                                        |
| hexiom                     | 5.96 ms                                                      | 7.86 ms: 1.32x slower                                                        |
| scimark_sor                | 109 ms                                                       | 144 ms: 1.32x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.05x slower                                                                 |

Benchmark hidden because not significant (6): logging_simple, asyncio_tcp_ssl, asyncio_websockets, unpickle, async_tree_cpu_io_mixed, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.92x