
# Results vs. 3.12.0

- fork: python
- ref: v3.11.0
- machine: linux-x86_64
- commit hash: deaf509
- commit date: 2022-10-24
- overall geometric mean: 1.07x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 287 ms: 1.01x slower                                         |
| chameleon      | 7.23 ms                                                      | 7.92 ms: 1.10x slower                                        |
| docutils       | 2.87 sec                                                     | 2.85 sec: 1.01x faster                                       |
| tornado_http   | 121 ms                                                       | 124 ms: 1.03x slower                                         |
| Geometric mean | (ref)                                                        | 1.03x slower                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 750 ms: 1.08x slower                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 753 ms: 1.08x slower                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.15 sec: 1.10x slower                                       |
| async_tree_none_tg         | 431 ms                                                       | 474 ms: 1.10x slower                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 600 ms: 1.11x slower                                         |
| async_tree_io              | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                       |
| async_tree_none            | 452 ms                                                       | 518 ms: 1.15x slower                                         |
| async_tree_memoization     | 544 ms                                                       | 629 ms: 1.16x slower                                         |
| Geometric mean             | (ref)                                                        | 1.11x slower                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 251 ms: 1.05x faster                                         |
| float          | 76.6 ms                                                      | 74.9 ms: 1.02x faster                                        |
| nbody          | 88.0 ms                                                      | 92.9 ms: 1.06x slower                                        |
| Geometric mean | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.34 ms: 1.07x faster                                        |
| regex_dna      | 239 ms                                                       | 227 ms: 1.05x faster                                         |
| regex_v8       | 23.6 ms                                                      | 24.4 ms: 1.03x slower                                        |
| regex_compile  | 144 ms                                                       | 156 ms: 1.08x slower                                         |
| Geometric mean | (ref)                                                        | 1.00x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.94 us: 1.12x faster                                        |
| unpickle             | 14.8 us                                                      | 13.3 us: 1.12x faster                                        |
| xml_etree_generate   | 86.1 ms                                                      | 79.7 ms: 1.08x faster                                        |
| pickle               | 10.5 us                                                      | 9.89 us: 1.06x faster                                        |
| xml_etree_process    | 58.4 ms                                                      | 55.9 ms: 1.05x faster                                        |
| unpickle_list        | 4.66 us                                                      | 4.60 us: 1.01x faster                                        |
| pickle_pure_python   | 318 us                                                       | 316 us: 1.01x faster                                         |
| pickle_dict          | 32.5 us                                                      | 32.3 us: 1.01x faster                                        |
| xml_etree_iterparse  | 103 ms                                                       | 107 ms: 1.04x slower                                         |
| tomli_loads          | 2.16 sec                                                     | 2.25 sec: 1.04x slower                                       |
| xml_etree_parse      | 144 ms                                                       | 155 ms: 1.08x slower                                         |
| unpickle_pure_python | 210 us                                                       | 238 us: 1.14x slower                                         |
| json_loads           | 24.4 us                                                      | 28.9 us: 1.19x slower                                        |
| json_dumps           | 10.2 ms                                                      | 13.3 ms: 1.30x slower                                        |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.73 ms: 1.12x faster                                        |
| python_startup         | 11.6 ms                                                      | 10.7 ms: 1.08x faster                                        |
| Geometric mean         | (ref)                                                        | 1.10x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 39.3 ms: 1.03x slower                                        |
| mako            | 10.0 ms                                                      | 11.0 ms: 1.10x slower                                        |
| Geometric mean  | (ref)                                                        | 1.06x slower                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_generators           | 390 ms                                                       | 322 ms: 1.21x faster                                         |
| unpack_sequence            | 53.2 ns                                                      | 45.7 ns: 1.16x faster                                        |
| pickle_list                | 4.43 us                                                      | 3.94 us: 1.12x faster                                        |
| python_startup_no_site     | 8.64 ms                                                      | 7.73 ms: 1.12x faster                                        |
| unpickle                   | 14.8 us                                                      | 13.3 us: 1.12x faster                                        |
| sqlite_synth               | 2.77 us                                                      | 2.52 us: 1.10x faster                                        |
| mypy2                      | 830 ms                                                       | 762 ms: 1.09x faster                                         |
| python_startup             | 11.6 ms                                                      | 10.7 ms: 1.08x faster                                        |
| xml_etree_generate         | 86.1 ms                                                      | 79.7 ms: 1.08x faster                                        |
| scimark_fft                | 301 ms                                                       | 281 ms: 1.07x faster                                         |
| regex_effbot               | 3.57 ms                                                      | 3.34 ms: 1.07x faster                                        |
| pickle                     | 10.5 us                                                      | 9.89 us: 1.06x faster                                        |
| pidigits                   | 265 ms                                                       | 251 ms: 1.05x faster                                         |
| regex_dna                  | 239 ms                                                       | 227 ms: 1.05x faster                                         |
| xml_etree_process          | 58.4 ms                                                      | 55.9 ms: 1.05x faster                                        |
| gunicorn                   | 1.00 ms                                                      | 966 us: 1.04x faster                                         |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.06 ms: 1.04x faster                                        |
| aiohttp                    | 1.02 ms                                                      | 986 us: 1.03x faster                                         |
| sqlalchemy_declarative     | 159 ms                                                       | 154 ms: 1.03x faster                                         |
| telco                      | 6.96 ms                                                      | 6.81 ms: 1.02x faster                                        |
| float                      | 76.6 ms                                                      | 74.9 ms: 1.02x faster                                        |
| unpickle_list              | 4.66 us                                                      | 4.60 us: 1.01x faster                                        |
| coverage                   | 66.7 ms                                                      | 66.1 ms: 1.01x faster                                        |
| docutils                   | 2.87 sec                                                     | 2.85 sec: 1.01x faster                                       |
| pickle_pure_python         | 318 us                                                       | 316 us: 1.01x faster                                         |
| pickle_dict                | 32.5 us                                                      | 32.3 us: 1.01x faster                                        |
| 2to3                       | 285 ms                                                       | 287 ms: 1.01x slower                                         |
| scimark_sor                | 109 ms                                                       | 110 ms: 1.01x slower                                         |
| pprint_pformat             | 1.65 sec                                                     | 1.67 sec: 1.01x slower                                       |
| deepcopy_reduce            | 3.37 us                                                      | 3.40 us: 1.01x slower                                        |
| scimark_monte_carlo        | 69.0 ms                                                      | 69.8 ms: 1.01x slower                                        |
| meteor_contest             | 128 ms                                                       | 131 ms: 1.02x slower                                         |
| deepcopy_memo              | 36.8 us                                                      | 37.5 us: 1.02x slower                                        |
| pyflate                    | 439 ms                                                       | 449 ms: 1.02x slower                                         |
| sqlglot_optimize           | 57.5 ms                                                      | 59.0 ms: 1.03x slower                                        |
| tornado_http               | 121 ms                                                       | 124 ms: 1.03x slower                                         |
| django_template            | 38.2 ms                                                      | 39.3 ms: 1.03x slower                                        |
| logging_format             | 7.48 us                                                      | 7.71 us: 1.03x slower                                        |
| dulwich_log                | 65.4 ms                                                      | 67.4 ms: 1.03x slower                                        |
| regex_v8                   | 23.6 ms                                                      | 24.4 ms: 1.03x slower                                        |
| crypto_pyaes               | 80.3 ms                                                      | 83.3 ms: 1.04x slower                                        |
| spectral_norm              | 91.6 ms                                                      | 95.1 ms: 1.04x slower                                        |
| raytrace                   | 298 ms                                                       | 309 ms: 1.04x slower                                         |
| xml_etree_iterparse        | 103 ms                                                       | 107 ms: 1.04x slower                                         |
| tomli_loads                | 2.16 sec                                                     | 2.25 sec: 1.04x slower                                       |
| dask                       | 392 ms                                                       | 410 ms: 1.05x slower                                         |
| sqlglot_normalize          | 116 ms                                                       | 122 ms: 1.05x slower                                         |
| bench_thread_pool          | 950 us                                                       | 1.00 ms: 1.05x slower                                        |
| go                         | 150 ms                                                       | 158 ms: 1.05x slower                                         |
| sqlalchemy_imperative      | 18.7 ms                                                      | 19.8 ms: 1.05x slower                                        |
| nbody                      | 88.0 ms                                                      | 92.9 ms: 1.06x slower                                        |
| pycparser                  | 1.23 sec                                                     | 1.31 sec: 1.06x slower                                       |
| deepcopy                   | 368 us                                                       | 391 us: 1.06x slower                                         |
| logging_silent             | 94.4 ns                                                      | 100 ns: 1.06x slower                                         |
| xml_etree_parse            | 144 ms                                                       | 155 ms: 1.08x slower                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 750 ms: 1.08x slower                                         |
| sqlglot_transpile          | 1.78 ms                                                      | 1.91 ms: 1.08x slower                                        |
| sympy_integrate            | 23.9 ms                                                      | 25.8 ms: 1.08x slower                                        |
| mdp                        | 2.57 sec                                                     | 2.77 sec: 1.08x slower                                       |
| logging_simple             | 6.71 us                                                      | 7.24 us: 1.08x slower                                        |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 753 ms: 1.08x slower                                         |
| regex_compile              | 144 ms                                                       | 156 ms: 1.08x slower                                         |
| richards                   | 45.7 ms                                                      | 49.7 ms: 1.09x slower                                        |
| json                       | 5.12 ms                                                      | 5.58 ms: 1.09x slower                                        |
| async_tree_io_tg           | 1.05 sec                                                     | 1.15 sec: 1.10x slower                                       |
| chameleon                  | 7.23 ms                                                      | 7.92 ms: 1.10x slower                                        |
| sqlglot_parse              | 1.38 ms                                                      | 1.51 ms: 1.10x slower                                        |
| mako                       | 10.0 ms                                                      | 11.0 ms: 1.10x slower                                        |
| async_tree_none_tg         | 431 ms                                                       | 474 ms: 1.10x slower                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 600 ms: 1.11x slower                                         |
| sympy_str                  | 302 ms                                                       | 337 ms: 1.11x slower                                         |
| async_tree_io              | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                       |
| unpickle_pure_python       | 210 us                                                       | 238 us: 1.14x slower                                         |
| nqueens                    | 89.9 ms                                                      | 103 ms: 1.14x slower                                         |
| sympy_expand               | 484 ms                                                       | 553 ms: 1.14x slower                                         |
| comprehensions             | 21.9 us                                                      | 25.1 us: 1.14x slower                                        |
| sympy_sum                  | 162 ms                                                       | 186 ms: 1.15x slower                                         |
| async_tree_none            | 452 ms                                                       | 518 ms: 1.15x slower                                         |
| scimark_lu                 | 98.8 ms                                                      | 114 ms: 1.15x slower                                         |
| async_tree_memoization     | 544 ms                                                       | 629 ms: 1.16x slower                                         |
| hexiom                     | 5.96 ms                                                      | 6.98 ms: 1.17x slower                                        |
| chaos                      | 64.0 ms                                                      | 74.9 ms: 1.17x slower                                        |
| json_loads                 | 24.4 us                                                      | 28.9 us: 1.19x slower                                        |
| fannkuch                   | 350 ms                                                       | 416 ms: 1.19x slower                                         |
| gc_traversal               | 3.48 ms                                                      | 4.15 ms: 1.19x slower                                        |
| coroutines                 | 23.0 ms                                                      | 27.8 ms: 1.21x slower                                        |
| deltablue                  | 3.24 ms                                                      | 3.97 ms: 1.23x slower                                        |
| richards_super             | 51.3 ms                                                      | 63.6 ms: 1.24x slower                                        |
| json_dumps                 | 10.2 ms                                                      | 13.3 ms: 1.30x slower                                        |
| generators                 | 37.4 ms                                                      | 54.6 ms: 1.46x slower                                        |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 3.07 sec: 1.93x slower                                       |
| asyncio_tcp                | 378 ms                                                       | 747 ms: 1.98x slower                                         |
| typing_runtime_protocols   | 152 us                                                       | 532 us: 3.51x slower                                         |
| Geometric mean             | (ref)                                                        | 1.07x slower                                                 |

Benchmark hidden because not significant (5): bench_mp_pool, create_gc_cycles, pprint_safe_repr, pathlib, asyncio_websockets
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.90x