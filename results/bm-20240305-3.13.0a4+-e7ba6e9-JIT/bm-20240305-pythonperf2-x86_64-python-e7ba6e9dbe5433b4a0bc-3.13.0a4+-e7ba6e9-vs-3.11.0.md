# Results vs. 3.11.0

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: linux-x86_64
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.02x faster \*
- HPT reliability: 80.66%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.25x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 306 ms: 1.07x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.45 ms: 1.06x faster                                                        |
| docutils       | 2.85 sec                                                     | 2.91 sec: 1.02x slower                                                       |
| html5lib       | 72.2 ms                                                      | 74.1 ms: 1.03x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 438 ms: 1.18x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 555 ms: 1.13x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 438 ms: 1.08x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.08x faster                                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 559 ms: 1.07x faster                                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 705 ms: 1.07x faster                                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 709 ms: 1.06x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.09x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 77.6 ms: 1.04x slower                                                        |
| pidigits       | 251 ms                                                       | 261 ms: 1.04x slower                                                         |
| nbody          | 92.9 ms                                                      | 105 ms: 1.14x slower                                                         |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 148 ms: 1.06x faster                                                         |
| regex_dna      | 227 ms                                                       | 235 ms: 1.03x slower                                                         |
| regex_effbot   | 3.34 ms                                                      | 3.46 ms: 1.03x slower                                                        |
| regex_v8       | 24.4 ms                                                      | 25.4 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                        |
| json_loads           | 28.9 us                                                      | 25.0 us: 1.16x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 144 ms: 1.08x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 30.5 us: 1.06x faster                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.13 sec: 1.06x faster                                                       |
| xml_etree_iterparse  | 107 ms                                                       | 102 ms: 1.04x faster                                                         |
| unpickle_pure_python | 238 us                                                       | 230 us: 1.03x faster                                                         |
| pickle_pure_python   | 316 us                                                       | 311 us: 1.02x faster                                                         |
| unpickle_list        | 4.60 us                                                      | 4.72 us: 1.03x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 57.6 ms: 1.03x slower                                                        |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 84.3 ms: 1.06x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.21 us: 1.07x slower                                                        |
| unpickle             | 13.3 us                                                      | 15.2 us: 1.15x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 15.5 ms: 1.44x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 14.0 ms: 1.81x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.62x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 9.93 ms: 1.11x faster                                                        |
| django_template | 39.3 ms                                                      | 38.2 ms: 1.03x faster                                                        |
| genshi_xml      | 57.1 ms                                                      | 60.1 ms: 1.05x slower                                                        |
| genshi_text     | 25.5 ms                                                      | 28.5 ms: 1.12x slower                                                        |
| Geometric mean  | (ref)                                                        | 1.01x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 119 us: 4.47x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 368 ms: 2.03x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                                       |
| generators                 | 54.6 ms                                                      | 34.0 ms: 1.61x faster                                                        |
| pylint                     | 514 ms                                                       | 359 ms: 1.43x faster                                                         |
| comprehensions             | 25.1 us                                                      | 18.8 us: 1.33x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.3 ms: 1.24x faster                                                        |
| async_tree_none            | 518 ms                                                       | 438 ms: 1.18x faster                                                         |
| sympy_sum                  | 186 ms                                                       | 159 ms: 1.17x faster                                                         |
| json_loads                 | 28.9 us                                                      | 25.0 us: 1.16x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 555 ms: 1.13x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 3.67 ms: 1.13x faster                                                        |
| richards_super             | 63.6 ms                                                      | 56.7 ms: 1.12x faster                                                        |
| sympy_str                  | 337 ms                                                       | 302 ms: 1.12x faster                                                         |
| mako                       | 11.0 ms                                                      | 9.93 ms: 1.11x faster                                                        |
| chaos                      | 74.9 ms                                                      | 68.3 ms: 1.10x faster                                                        |
| async_tree_none_tg         | 474 ms                                                       | 438 ms: 1.08x faster                                                         |
| thrift                     | 931 us                                                       | 861 us: 1.08x faster                                                         |
| logging_simple             | 7.24 us                                                      | 6.69 us: 1.08x faster                                                        |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.08x faster                                                       |
| sympy_expand               | 553 ms                                                       | 513 ms: 1.08x faster                                                         |
| xml_etree_parse            | 155 ms                                                       | 144 ms: 1.08x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 559 ms: 1.07x faster                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 77.6 ms: 1.07x faster                                                        |
| mdp                        | 2.77 sec                                                     | 2.59 sec: 1.07x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 705 ms: 1.07x faster                                                         |
| sqlglot_parse              | 1.51 ms                                                      | 1.42 ms: 1.07x faster                                                        |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                       |
| chameleon                  | 7.92 ms                                                      | 7.45 ms: 1.06x faster                                                        |
| pickle_dict                | 32.3 us                                                      | 30.5 us: 1.06x faster                                                        |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 709 ms: 1.06x faster                                                         |
| fannkuch                   | 416 ms                                                       | 394 ms: 1.06x faster                                                         |
| regex_compile              | 156 ms                                                       | 148 ms: 1.06x faster                                                         |
| tomli_loads                | 2.25 sec                                                     | 2.13 sec: 1.06x faster                                                       |
| sympy_integrate            | 25.8 ms                                                      | 24.5 ms: 1.05x faster                                                        |
| deltablue                  | 3.97 ms                                                      | 3.78 ms: 1.05x faster                                                        |
| logging_format             | 7.71 us                                                      | 7.34 us: 1.05x faster                                                        |
| xml_etree_iterparse        | 107 ms                                                       | 102 ms: 1.04x faster                                                         |
| json                       | 5.58 ms                                                      | 5.37 ms: 1.04x faster                                                        |
| deepcopy                   | 391 us                                                       | 376 us: 1.04x faster                                                         |
| unpickle_pure_python       | 238 us                                                       | 230 us: 1.03x faster                                                         |
| logging_silent             | 100 ns                                                       | 97.1 ns: 1.03x faster                                                        |
| django_template            | 39.3 ms                                                      | 38.2 ms: 1.03x faster                                                        |
| spectral_norm              | 95.1 ms                                                      | 92.4 ms: 1.03x faster                                                        |
| sqlglot_normalize          | 122 ms                                                       | 119 ms: 1.03x faster                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.86 ms: 1.03x faster                                                        |
| raytrace                   | 309 ms                                                       | 303 ms: 1.02x faster                                                         |
| create_gc_cycles           | 1.58 ms                                                      | 1.55 ms: 1.02x faster                                                        |
| deepcopy_reduce            | 3.40 us                                                      | 3.34 us: 1.02x faster                                                        |
| pickle_pure_python         | 316 us                                                       | 311 us: 1.02x faster                                                         |
| nqueens                    | 103 ms                                                       | 101 ms: 1.01x faster                                                         |
| meteor_contest             | 131 ms                                                       | 132 ms: 1.01x slower                                                         |
| richards                   | 49.7 ms                                                      | 50.1 ms: 1.01x slower                                                        |
| scimark_lu                 | 114 ms                                                       | 115 ms: 1.01x slower                                                         |
| docutils                   | 2.85 sec                                                     | 2.91 sec: 1.02x slower                                                       |
| dulwich_log                | 67.4 ms                                                      | 69.1 ms: 1.02x slower                                                        |
| html5lib                   | 72.2 ms                                                      | 74.1 ms: 1.03x slower                                                        |
| pathlib                    | 18.9 ms                                                      | 19.4 ms: 1.03x slower                                                        |
| unpickle_list              | 4.60 us                                                      | 4.72 us: 1.03x slower                                                        |
| xml_etree_process          | 55.9 ms                                                      | 57.6 ms: 1.03x slower                                                        |
| pycparser                  | 1.31 sec                                                     | 1.35 sec: 1.03x slower                                                       |
| regex_dna                  | 227 ms                                                       | 235 ms: 1.03x slower                                                         |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.20 ms: 1.03x slower                                                        |
| regex_effbot               | 3.34 ms                                                      | 3.46 ms: 1.03x slower                                                        |
| float                      | 74.9 ms                                                      | 77.6 ms: 1.04x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 25.4 ms: 1.04x slower                                                        |
| pidigits                   | 251 ms                                                       | 261 ms: 1.04x slower                                                         |
| pprint_pformat             | 1.67 sec                                                     | 1.74 sec: 1.04x slower                                                       |
| pprint_safe_repr           | 805 ms                                                       | 844 ms: 1.05x slower                                                         |
| pickle                     | 9.89 us                                                      | 10.4 us: 1.05x slower                                                        |
| genshi_xml                 | 57.1 ms                                                      | 60.1 ms: 1.05x slower                                                        |
| hexiom                     | 6.98 ms                                                      | 7.37 ms: 1.06x slower                                                        |
| xml_etree_generate         | 79.7 ms                                                      | 84.3 ms: 1.06x slower                                                        |
| sqlglot_optimize           | 59.0 ms                                                      | 62.8 ms: 1.07x slower                                                        |
| 2to3                       | 287 ms                                                       | 306 ms: 1.07x slower                                                         |
| pickle_list                | 3.94 us                                                      | 4.21 us: 1.07x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.70 us: 1.07x slower                                                        |
| go                         | 158 ms                                                       | 174 ms: 1.10x slower                                                         |
| gunicorn                   | 966 us                                                       | 1.07 ms: 1.11x slower                                                        |
| scimark_monte_carlo        | 69.8 ms                                                      | 77.5 ms: 1.11x slower                                                        |
| aiohttp                    | 986 us                                                       | 1.10 ms: 1.12x slower                                                        |
| genshi_text                | 25.5 ms                                                      | 28.5 ms: 1.12x slower                                                        |
| scimark_fft                | 281 ms                                                       | 316 ms: 1.13x slower                                                         |
| nbody                      | 92.9 ms                                                      | 105 ms: 1.14x slower                                                         |
| unpickle                   | 13.3 us                                                      | 15.2 us: 1.15x slower                                                        |
| pyflate                    | 449 ms                                                       | 518 ms: 1.15x slower                                                         |
| telco                      | 6.81 ms                                                      | 8.12 ms: 1.19x slower                                                        |
| async_generators           | 322 ms                                                       | 384 ms: 1.20x slower                                                         |
| mypy2                      | 762 ms                                                       | 917 ms: 1.20x slower                                                         |
| coverage                   | 66.1 ms                                                      | 81.9 ms: 1.24x slower                                                        |
| unpack_sequence            | 45.7 ns                                                      | 61.9 ns: 1.35x slower                                                        |
| scimark_sor                | 110 ms                                                       | 151 ms: 1.37x slower                                                         |
| dask                       | 410 ms                                                       | 589 ms: 1.44x slower                                                         |
| python_startup             | 10.7 ms                                                      | 15.5 ms: 1.44x slower                                                        |
| bench_mp_pool              | 4.70 ms                                                      | 6.88 ms: 1.47x slower                                                        |
| python_startup_no_site     | 7.73 ms                                                      | 14.0 ms: 1.81x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.02x faster                                                                 |

Benchmark hidden because not significant (4): bench_thread_pool, asyncio_websockets, deepcopy_memo, tornado_http
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 80.66% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.25x