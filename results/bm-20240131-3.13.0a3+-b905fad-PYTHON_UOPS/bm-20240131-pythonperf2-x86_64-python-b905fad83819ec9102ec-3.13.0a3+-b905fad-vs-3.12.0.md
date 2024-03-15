
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: linux-x86_64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.10x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 308 ms: 1.08x slower                                                         |
| chameleon      | 7.23 ms                                                      | 8.14 ms: 1.13x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.95 sec: 1.03x slower                                                       |
| tornado_http   | 121 ms                                                       | 126 ms: 1.04x slower                                                         |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 443 ms: 1.02x faster                                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 708 ms: 1.02x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 555 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 714 ms: 1.02x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 445 ms: 1.03x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.04x slower                                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 567 ms: 1.05x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 266 ms: 1.00x slower                                                         |
| float          | 76.6 ms                                                      | 104 ms: 1.36x slower                                                         |
| nbody          | 88.0 ms                                                      | 129 ms: 1.47x slower                                                         |
| Geometric mean | (ref)                                                        | 1.26x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.49 ms: 1.02x faster                                                        |
| regex_dna      | 239 ms                                                       | 243 ms: 1.02x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 25.7 ms: 1.09x slower                                                        |
| regex_compile  | 144 ms                                                       | 169 ms: 1.18x slower                                                         |
| Geometric mean | (ref)                                                        | 1.06x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 31.1 us: 1.05x faster                                                        |
| pickle               | 10.5 us                                                      | 10.2 us: 1.03x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 312 us: 1.02x faster                                                         |
| pickle_list          | 4.43 us                                                      | 4.40 us: 1.01x faster                                                        |
| unpickle             | 14.8 us                                                      | 14.9 us: 1.01x slower                                                        |
| json_loads           | 24.4 us                                                      | 24.9 us: 1.02x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| unpickle_list        | 4.66 us                                                      | 4.80 us: 1.03x slower                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 89.9 ms: 1.04x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.8 ms: 1.05x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 62.2 ms: 1.07x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 116 ms: 1.13x slower                                                         |
| unpickle_pure_python | 210 us                                                       | 242 us: 1.16x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.81 sec: 1.30x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.05x slower                                                                 |

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
| mako      | 10.0 ms                                                      | 15.0 ms: 1.50x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpack_sequence            | 53.2 ns                                                      | 43.3 ns: 1.23x faster                                                        |
| typing_runtime_protocols   | 152 us                                                       | 128 us: 1.19x faster                                                         |
| generators                 | 37.4 ms                                                      | 34.1 ms: 1.10x faster                                                        |
| async_generators           | 390 ms                                                       | 372 ms: 1.05x faster                                                         |
| pickle_dict                | 32.5 us                                                      | 31.1 us: 1.05x faster                                                        |
| pickle                     | 10.5 us                                                      | 10.2 us: 1.03x faster                                                        |
| coroutines                 | 23.0 ms                                                      | 22.4 ms: 1.03x faster                                                        |
| regex_effbot               | 3.57 ms                                                      | 3.49 ms: 1.02x faster                                                        |
| async_tree_none            | 452 ms                                                       | 443 ms: 1.02x faster                                                         |
| pickle_pure_python         | 318 us                                                       | 312 us: 1.02x faster                                                         |
| asyncio_tcp                | 378 ms                                                       | 374 ms: 1.01x faster                                                         |
| pickle_list                | 4.43 us                                                      | 4.40 us: 1.01x faster                                                        |
| pidigits                   | 265 ms                                                       | 266 ms: 1.00x slower                                                         |
| logging_format             | 7.48 us                                                      | 7.54 us: 1.01x slower                                                        |
| unpickle                   | 14.8 us                                                      | 14.9 us: 1.01x slower                                                        |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.60 sec: 1.01x slower                                                       |
| deepcopy_reduce            | 3.37 us                                                      | 3.42 us: 1.01x slower                                                        |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 708 ms: 1.02x slower                                                         |
| regex_dna                  | 239 ms                                                       | 243 ms: 1.02x slower                                                         |
| mdp                        | 2.57 sec                                                     | 2.62 sec: 1.02x slower                                                       |
| async_tree_memoization     | 544 ms                                                       | 555 ms: 1.02x slower                                                         |
| logging_simple             | 6.71 us                                                      | 6.85 us: 1.02x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                        |
| json_loads                 | 24.4 us                                                      | 24.9 us: 1.02x slower                                                        |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 714 ms: 1.02x slower                                                         |
| json                       | 5.12 ms                                                      | 5.25 ms: 1.03x slower                                                        |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                       |
| logging_silent             | 94.4 ns                                                      | 97.0 ns: 1.03x slower                                                        |
| docutils                   | 2.87 sec                                                     | 2.95 sec: 1.03x slower                                                       |
| unpickle_list              | 4.66 us                                                      | 4.80 us: 1.03x slower                                                        |
| deepcopy                   | 368 us                                                       | 380 us: 1.03x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 445 ms: 1.03x slower                                                         |
| bench_thread_pool          | 950 us                                                       | 984 us: 1.04x slower                                                         |
| sympy_integrate            | 23.9 ms                                                      | 24.8 ms: 1.04x slower                                                        |
| sympy_sum                  | 162 ms                                                       | 168 ms: 1.04x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.04x slower                                                       |
| sqlglot_parse              | 1.38 ms                                                      | 1.43 ms: 1.04x slower                                                        |
| tornado_http               | 121 ms                                                       | 126 ms: 1.04x slower                                                         |
| xml_etree_generate         | 86.1 ms                                                      | 89.9 ms: 1.04x slower                                                        |
| dask                       | 392 ms                                                       | 411 ms: 1.05x slower                                                         |
| scimark_lu                 | 98.8 ms                                                      | 104 ms: 1.05x slower                                                         |
| sqlglot_transpile          | 1.78 ms                                                      | 1.86 ms: 1.05x slower                                                        |
| async_tree_memoization_tg  | 540 ms                                                       | 567 ms: 1.05x slower                                                         |
| json_dumps                 | 10.2 ms                                                      | 10.8 ms: 1.05x slower                                                        |
| sqlglot_normalize          | 116 ms                                                       | 123 ms: 1.06x slower                                                         |
| sympy_str                  | 302 ms                                                       | 322 ms: 1.06x slower                                                         |
| xml_etree_process          | 58.4 ms                                                      | 62.2 ms: 1.07x slower                                                        |
| crypto_pyaes               | 80.3 ms                                                      | 86.0 ms: 1.07x slower                                                        |
| meteor_contest             | 128 ms                                                       | 137 ms: 1.07x slower                                                         |
| gc_traversal               | 3.48 ms                                                      | 3.73 ms: 1.07x slower                                                        |
| pycparser                  | 1.23 sec                                                     | 1.33 sec: 1.07x slower                                                       |
| 2to3                       | 285 ms                                                       | 308 ms: 1.08x slower                                                         |
| regex_v8                   | 23.6 ms                                                      | 25.7 ms: 1.09x slower                                                        |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| sympy_expand               | 484 ms                                                       | 532 ms: 1.10x slower                                                         |
| sqlglot_optimize           | 57.5 ms                                                      | 63.3 ms: 1.10x slower                                                        |
| dulwich_log                | 65.4 ms                                                      | 72.5 ms: 1.11x slower                                                        |
| deepcopy_memo              | 36.8 us                                                      | 41.2 us: 1.12x slower                                                        |
| chameleon                  | 7.23 ms                                                      | 8.14 ms: 1.13x slower                                                        |
| xml_etree_iterparse        | 103 ms                                                       | 116 ms: 1.13x slower                                                         |
| comprehensions             | 21.9 us                                                      | 25.1 us: 1.15x slower                                                        |
| pprint_safe_repr           | 807 ms                                                       | 931 ms: 1.15x slower                                                         |
| unpickle_pure_python       | 210 us                                                       | 242 us: 1.16x slower                                                         |
| pprint_pformat             | 1.65 sec                                                     | 1.93 sec: 1.16x slower                                                       |
| richards_super             | 51.3 ms                                                      | 60.1 ms: 1.17x slower                                                        |
| regex_compile              | 144 ms                                                       | 169 ms: 1.18x slower                                                         |
| coverage                   | 66.7 ms                                                      | 78.8 ms: 1.18x slower                                                        |
| richards                   | 45.7 ms                                                      | 54.1 ms: 1.18x slower                                                        |
| telco                      | 6.96 ms                                                      | 8.24 ms: 1.18x slower                                                        |
| go                         | 150 ms                                                       | 180 ms: 1.20x slower                                                         |
| nqueens                    | 89.9 ms                                                      | 109 ms: 1.21x slower                                                         |
| chaos                      | 64.0 ms                                                      | 78.0 ms: 1.22x slower                                                        |
| scimark_monte_carlo        | 69.0 ms                                                      | 87.5 ms: 1.27x slower                                                        |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                        |
| tomli_loads                | 2.16 sec                                                     | 2.81 sec: 1.30x slower                                                       |
| pyflate                    | 439 ms                                                       | 586 ms: 1.34x slower                                                         |
| scimark_sor                | 109 ms                                                       | 147 ms: 1.35x slower                                                         |
| fannkuch                   | 350 ms                                                       | 474 ms: 1.35x slower                                                         |
| float                      | 76.6 ms                                                      | 104 ms: 1.36x slower                                                         |
| scimark_fft                | 301 ms                                                       | 434 ms: 1.44x slower                                                         |
| nbody                      | 88.0 ms                                                      | 129 ms: 1.47x slower                                                         |
| mako                       | 10.0 ms                                                      | 15.0 ms: 1.50x slower                                                        |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.71 ms: 1.60x slower                                                        |
| hexiom                     | 5.96 ms                                                      | 9.82 ms: 1.65x slower                                                        |
| deltablue                  | 3.24 ms                                                      | 5.43 ms: 1.68x slower                                                        |
| spectral_norm              | 91.6 ms                                                      | 162 ms: 1.77x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.10x slower                                                                 |

Benchmark hidden because not significant (6): bench_mp_pool, asyncio_websockets, raytrace, sqlite_synth, create_gc_cycles, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.88x