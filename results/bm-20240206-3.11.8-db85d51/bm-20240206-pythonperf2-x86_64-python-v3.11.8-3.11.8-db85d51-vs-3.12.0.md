
# Results vs. 3.12.0

- fork: python
- ref: v3.11.8
- machine: linux-x86_64
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 283 ms: 1.01x faster                                         |
| chameleon      | 7.23 ms                                                      | 7.43 ms: 1.03x slower                                        |
| docutils       | 2.87 sec                                                     | 2.82 sec: 1.02x faster                                       |
| tornado_http   | 121 ms                                                       | 124 ms: 1.02x slower                                         |
| Geometric mean | (ref)                                                        | 1.01x slower                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 744 ms: 1.07x slower                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 748 ms: 1.07x slower                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.15 sec: 1.09x slower                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 592 ms: 1.10x slower                                         |
| async_tree_none_tg         | 431 ms                                                       | 473 ms: 1.10x slower                                         |
| async_tree_io              | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                       |
| async_tree_none            | 452 ms                                                       | 523 ms: 1.16x slower                                         |
| async_tree_memoization     | 544 ms                                                       | 636 ms: 1.17x slower                                         |
| Geometric mean             | (ref)                                                        | 1.11x slower                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 74.9 ms: 1.02x faster                                        |
| pidigits       | 265 ms                                                       | 268 ms: 1.01x slower                                         |
| nbody          | 88.0 ms                                                      | 96.9 ms: 1.10x slower                                        |
| Geometric mean | (ref)                                                        | 1.03x slower                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.27 ms: 1.09x faster                                        |
| regex_dna      | 239 ms                                                       | 227 ms: 1.05x faster                                         |
| regex_v8       | 23.6 ms                                                      | 24.5 ms: 1.04x slower                                        |
| regex_compile  | 144 ms                                                       | 153 ms: 1.06x slower                                         |
| Geometric mean | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.90 us: 1.14x faster                                        |
| unpickle             | 14.8 us                                                      | 13.3 us: 1.11x faster                                        |
| xml_etree_generate   | 86.1 ms                                                      | 80.9 ms: 1.07x faster                                        |
| xml_etree_process    | 58.4 ms                                                      | 56.2 ms: 1.04x faster                                        |
| unpickle_list        | 4.66 us                                                      | 4.51 us: 1.03x faster                                        |
| pickle               | 10.5 us                                                      | 10.3 us: 1.03x faster                                        |
| pickle_pure_python   | 318 us                                                       | 322 us: 1.01x slower                                         |
| xml_etree_iterparse  | 103 ms                                                       | 105 ms: 1.02x slower                                         |
| json_loads           | 24.4 us                                                      | 25.1 us: 1.03x slower                                        |
| pickle_dict          | 32.5 us                                                      | 34.4 us: 1.06x slower                                        |
| tomli_loads          | 2.16 sec                                                     | 2.28 sec: 1.06x slower                                       |
| xml_etree_parse      | 144 ms                                                       | 155 ms: 1.08x slower                                         |
| unpickle_pure_python | 210 us                                                       | 240 us: 1.14x slower                                         |
| json_dumps           | 10.2 ms                                                      | 13.4 ms: 1.31x slower                                        |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.69 ms: 1.12x faster                                        |
| python_startup         | 11.6 ms                                                      | 10.7 ms: 1.09x faster                                        |
| Geometric mean         | (ref)                                                        | 1.10x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 40.3 ms: 1.06x slower                                        |
| mako            | 10.0 ms                                                      | 10.8 ms: 1.07x slower                                        |
| Geometric mean  | (ref)                                                        | 1.07x slower                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_generators           | 390 ms                                                       | 318 ms: 1.23x faster                                         |
| unpack_sequence            | 53.2 ns                                                      | 45.5 ns: 1.17x faster                                        |
| pickle_list                | 4.43 us                                                      | 3.90 us: 1.14x faster                                        |
| python_startup_no_site     | 8.64 ms                                                      | 7.69 ms: 1.12x faster                                        |
| unpickle                   | 14.8 us                                                      | 13.3 us: 1.11x faster                                        |
| mypy2                      | 830 ms                                                       | 751 ms: 1.11x faster                                         |
| sqlite_synth               | 2.77 us                                                      | 2.52 us: 1.10x faster                                        |
| scimark_fft                | 301 ms                                                       | 274 ms: 1.10x faster                                         |
| regex_effbot               | 3.57 ms                                                      | 3.27 ms: 1.09x faster                                        |
| python_startup             | 11.6 ms                                                      | 10.7 ms: 1.09x faster                                        |
| xml_etree_generate         | 86.1 ms                                                      | 80.9 ms: 1.07x faster                                        |
| regex_dna                  | 239 ms                                                       | 227 ms: 1.05x faster                                         |
| telco                      | 6.96 ms                                                      | 6.62 ms: 1.05x faster                                        |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.01 ms: 1.05x faster                                        |
| aiohttp                    | 1.02 ms                                                      | 974 us: 1.05x faster                                         |
| xml_etree_process          | 58.4 ms                                                      | 56.2 ms: 1.04x faster                                        |
| sqlalchemy_declarative     | 159 ms                                                       | 154 ms: 1.04x faster                                         |
| unpickle_list              | 4.66 us                                                      | 4.51 us: 1.03x faster                                        |
| pprint_safe_repr           | 807 ms                                                       | 785 ms: 1.03x faster                                         |
| pickle                     | 10.5 us                                                      | 10.3 us: 1.03x faster                                        |
| gunicorn                   | 1.00 ms                                                      | 976 us: 1.03x faster                                         |
| float                      | 76.6 ms                                                      | 74.9 ms: 1.02x faster                                        |
| scimark_monte_carlo        | 69.0 ms                                                      | 67.5 ms: 1.02x faster                                        |
| docutils                   | 2.87 sec                                                     | 2.82 sec: 1.02x faster                                       |
| pprint_pformat             | 1.65 sec                                                     | 1.63 sec: 1.02x faster                                       |
| coverage                   | 66.7 ms                                                      | 66.0 ms: 1.01x faster                                        |
| 2to3                       | 285 ms                                                       | 283 ms: 1.01x faster                                         |
| meteor_contest             | 128 ms                                                       | 129 ms: 1.01x slower                                         |
| pickle_pure_python         | 318 us                                                       | 322 us: 1.01x slower                                         |
| deepcopy_reduce            | 3.37 us                                                      | 3.41 us: 1.01x slower                                        |
| pidigits                   | 265 ms                                                       | 268 ms: 1.01x slower                                         |
| tornado_http               | 121 ms                                                       | 124 ms: 1.02x slower                                         |
| xml_etree_iterparse        | 103 ms                                                       | 105 ms: 1.02x slower                                         |
| sqlglot_optimize           | 57.5 ms                                                      | 58.8 ms: 1.02x slower                                        |
| deepcopy_memo              | 36.8 us                                                      | 37.7 us: 1.03x slower                                        |
| dulwich_log                | 65.4 ms                                                      | 67.1 ms: 1.03x slower                                        |
| json                       | 5.12 ms                                                      | 5.26 ms: 1.03x slower                                        |
| chameleon                  | 7.23 ms                                                      | 7.43 ms: 1.03x slower                                        |
| logging_format             | 7.48 us                                                      | 7.71 us: 1.03x slower                                        |
| json_loads                 | 24.4 us                                                      | 25.1 us: 1.03x slower                                        |
| scimark_sor                | 109 ms                                                       | 113 ms: 1.03x slower                                         |
| regex_v8                   | 23.6 ms                                                      | 24.5 ms: 1.04x slower                                        |
| dask                       | 392 ms                                                       | 407 ms: 1.04x slower                                         |
| raytrace                   | 298 ms                                                       | 311 ms: 1.04x slower                                         |
| deepcopy                   | 368 us                                                       | 384 us: 1.04x slower                                         |
| crypto_pyaes               | 80.3 ms                                                      | 84.3 ms: 1.05x slower                                        |
| bench_thread_pool          | 950 us                                                       | 996 us: 1.05x slower                                         |
| pickle_dict                | 32.5 us                                                      | 34.4 us: 1.06x slower                                        |
| logging_simple             | 6.71 us                                                      | 7.08 us: 1.06x slower                                        |
| tomli_loads                | 2.16 sec                                                     | 2.28 sec: 1.06x slower                                       |
| django_template            | 38.2 ms                                                      | 40.3 ms: 1.06x slower                                        |
| sqlglot_normalize          | 116 ms                                                       | 122 ms: 1.06x slower                                         |
| sympy_integrate            | 23.9 ms                                                      | 25.4 ms: 1.06x slower                                        |
| regex_compile              | 144 ms                                                       | 153 ms: 1.06x slower                                         |
| spectral_norm              | 91.6 ms                                                      | 97.5 ms: 1.06x slower                                        |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 744 ms: 1.07x slower                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 748 ms: 1.07x slower                                         |
| mako                       | 10.0 ms                                                      | 10.8 ms: 1.07x slower                                        |
| pycparser                  | 1.23 sec                                                     | 1.33 sec: 1.08x slower                                       |
| xml_etree_parse            | 144 ms                                                       | 155 ms: 1.08x slower                                         |
| logging_silent             | 94.4 ns                                                      | 102 ns: 1.08x slower                                         |
| sqlalchemy_imperative      | 18.7 ms                                                      | 20.3 ms: 1.08x slower                                        |
| richards                   | 45.7 ms                                                      | 49.5 ms: 1.08x slower                                        |
| sqlglot_transpile          | 1.78 ms                                                      | 1.93 ms: 1.09x slower                                        |
| async_tree_io_tg           | 1.05 sec                                                     | 1.15 sec: 1.09x slower                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 592 ms: 1.10x slower                                         |
| async_tree_none_tg         | 431 ms                                                       | 473 ms: 1.10x slower                                         |
| nbody                      | 88.0 ms                                                      | 96.9 ms: 1.10x slower                                        |
| sympy_str                  | 302 ms                                                       | 333 ms: 1.10x slower                                         |
| comprehensions             | 21.9 us                                                      | 24.4 us: 1.11x slower                                        |
| go                         | 150 ms                                                       | 167 ms: 1.11x slower                                         |
| async_tree_io              | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                       |
| sympy_sum                  | 162 ms                                                       | 182 ms: 1.13x slower                                         |
| sqlglot_parse              | 1.38 ms                                                      | 1.55 ms: 1.13x slower                                        |
| mdp                        | 2.57 sec                                                     | 2.92 sec: 1.13x slower                                       |
| sympy_expand               | 484 ms                                                       | 553 ms: 1.14x slower                                         |
| unpickle_pure_python       | 210 us                                                       | 240 us: 1.14x slower                                         |
| nqueens                    | 89.9 ms                                                      | 104 ms: 1.16x slower                                         |
| scimark_lu                 | 98.8 ms                                                      | 114 ms: 1.16x slower                                         |
| async_tree_none            | 452 ms                                                       | 523 ms: 1.16x slower                                         |
| async_tree_memoization     | 544 ms                                                       | 636 ms: 1.17x slower                                         |
| hexiom                     | 5.96 ms                                                      | 7.08 ms: 1.19x slower                                        |
| coroutines                 | 23.0 ms                                                      | 27.6 ms: 1.20x slower                                        |
| richards_super             | 51.3 ms                                                      | 61.9 ms: 1.21x slower                                        |
| chaos                      | 64.0 ms                                                      | 79.0 ms: 1.23x slower                                        |
| deltablue                  | 3.24 ms                                                      | 4.06 ms: 1.25x slower                                        |
| fannkuch                   | 350 ms                                                       | 442 ms: 1.26x slower                                         |
| json_dumps                 | 10.2 ms                                                      | 13.4 ms: 1.31x slower                                        |
| generators                 | 37.4 ms                                                      | 54.6 ms: 1.46x slower                                        |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 3.04 sec: 1.92x slower                                       |
| asyncio_tcp                | 378 ms                                                       | 735 ms: 1.95x slower                                         |
| typing_runtime_protocols   | 152 us                                                       | 522 us: 3.44x slower                                         |
| Geometric mean             | (ref)                                                        | 1.07x slower                                                 |

Benchmark hidden because not significant (6): bench_mp_pool, gc_traversal, create_gc_cycles, pathlib, pyflate, asyncio_websockets
Ignored benchmarks (6) of results/bm-20240206-3.11.8-db85d51/bm-20240206-pythonperf2-x86_64-python-v3.11.8-3.11.8-db85d51.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.90x