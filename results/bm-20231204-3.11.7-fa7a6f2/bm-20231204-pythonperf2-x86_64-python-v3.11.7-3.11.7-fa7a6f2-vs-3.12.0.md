
# Results vs. 3.12.0

- fork: python
- ref: v3.11.7
- machine: linux-x86_64
- commit hash: fa7a6f2
- commit date: 2023-12-04
- overall geometric mean: 1.06x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 280 ms: 1.02x faster                                         |
| chameleon      | 7.23 ms                                                      | 7.53 ms: 1.04x slower                                        |
| docutils       | 2.87 sec                                                     | 2.81 sec: 1.02x faster                                       |
| Geometric mean | (ref)                                                        | 1.00x slower                                                 |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 735 ms: 1.05x slower                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 743 ms: 1.07x slower                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.13 sec: 1.07x slower                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 581 ms: 1.07x slower                                         |
| async_tree_none_tg         | 431 ms                                                       | 466 ms: 1.08x slower                                         |
| async_tree_io              | 1.04 sec                                                     | 1.16 sec: 1.11x slower                                       |
| async_tree_none            | 452 ms                                                       | 514 ms: 1.14x slower                                         |
| async_tree_memoization     | 544 ms                                                       | 621 ms: 1.14x slower                                         |
| Geometric mean             | (ref)                                                        | 1.09x slower                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 74.6 ms: 1.03x faster                                        |
| pidigits       | 265 ms                                                       | 268 ms: 1.01x slower                                         |
| nbody          | 88.0 ms                                                      | 105 ms: 1.20x slower                                         |
| Geometric mean | (ref)                                                        | 1.06x slower                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.20 ms: 1.12x faster                                        |
| regex_dna      | 239 ms                                                       | 223 ms: 1.07x faster                                         |
| regex_v8       | 23.6 ms                                                      | 23.0 ms: 1.03x faster                                        |
| regex_compile  | 144 ms                                                       | 151 ms: 1.05x slower                                         |
| Geometric mean | (ref)                                                        | 1.04x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.80 us: 1.17x faster                                        |
| unpickle             | 14.8 us                                                      | 13.0 us: 1.14x faster                                        |
| xml_etree_generate   | 86.1 ms                                                      | 79.9 ms: 1.08x faster                                        |
| pickle               | 10.5 us                                                      | 9.84 us: 1.07x faster                                        |
| xml_etree_process    | 58.4 ms                                                      | 55.4 ms: 1.05x faster                                        |
| pickle_dict          | 32.5 us                                                      | 31.5 us: 1.03x faster                                        |
| pickle_pure_python   | 318 us                                                       | 314 us: 1.01x faster                                         |
| json_loads           | 24.4 us                                                      | 24.9 us: 1.02x slower                                        |
| xml_etree_iterparse  | 103 ms                                                       | 107 ms: 1.04x slower                                         |
| tomli_loads          | 2.16 sec                                                     | 2.28 sec: 1.06x slower                                       |
| xml_etree_parse      | 144 ms                                                       | 158 ms: 1.10x slower                                         |
| unpickle_pure_python | 210 us                                                       | 239 us: 1.14x slower                                         |
| json_dumps           | 10.2 ms                                                      | 13.2 ms: 1.29x slower                                        |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                 |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.69 ms: 1.12x faster                                        |
| python_startup         | 11.6 ms                                                      | 10.7 ms: 1.09x faster                                        |
| Geometric mean         | (ref)                                                        | 1.11x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 40.8 ms: 1.07x slower                                        |
| mako            | 10.0 ms                                                      | 11.0 ms: 1.10x slower                                        |
| Geometric mean  | (ref)                                                        | 1.08x slower                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_generators           | 390 ms                                                       | 312 ms: 1.25x faster                                         |
| unpack_sequence            | 53.2 ns                                                      | 45.2 ns: 1.18x faster                                        |
| pickle_list                | 4.43 us                                                      | 3.80 us: 1.17x faster                                        |
| unpickle                   | 14.8 us                                                      | 13.0 us: 1.14x faster                                        |
| python_startup_no_site     | 8.64 ms                                                      | 7.69 ms: 1.12x faster                                        |
| sqlite_synth               | 2.77 us                                                      | 2.47 us: 1.12x faster                                        |
| regex_effbot               | 3.57 ms                                                      | 3.20 ms: 1.12x faster                                        |
| mypy2                      | 830 ms                                                       | 751 ms: 1.11x faster                                         |
| python_startup             | 11.6 ms                                                      | 10.7 ms: 1.09x faster                                        |
| xml_etree_generate         | 86.1 ms                                                      | 79.9 ms: 1.08x faster                                        |
| scimark_fft                | 301 ms                                                       | 280 ms: 1.07x faster                                         |
| pickle                     | 10.5 us                                                      | 9.84 us: 1.07x faster                                        |
| regex_dna                  | 239 ms                                                       | 223 ms: 1.07x faster                                         |
| aiohttp                    | 1.02 ms                                                      | 954 us: 1.07x faster                                         |
| xml_etree_process          | 58.4 ms                                                      | 55.4 ms: 1.05x faster                                        |
| pprint_safe_repr           | 807 ms                                                       | 767 ms: 1.05x faster                                         |
| gunicorn                   | 1.00 ms                                                      | 951 us: 1.05x faster                                         |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.03 ms: 1.04x faster                                        |
| telco                      | 6.96 ms                                                      | 6.67 ms: 1.04x faster                                        |
| pprint_pformat             | 1.65 sec                                                     | 1.59 sec: 1.04x faster                                       |
| sqlalchemy_declarative     | 159 ms                                                       | 153 ms: 1.04x faster                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 66.3 ms: 1.04x faster                                        |
| pickle_dict                | 32.5 us                                                      | 31.5 us: 1.03x faster                                        |
| float                      | 76.6 ms                                                      | 74.6 ms: 1.03x faster                                        |
| regex_v8                   | 23.6 ms                                                      | 23.0 ms: 1.03x faster                                        |
| docutils                   | 2.87 sec                                                     | 2.81 sec: 1.02x faster                                       |
| 2to3                       | 285 ms                                                       | 280 ms: 1.02x faster                                         |
| pathlib                    | 18.9 ms                                                      | 18.6 ms: 1.02x faster                                        |
| coverage                   | 66.7 ms                                                      | 65.6 ms: 1.02x faster                                        |
| pickle_pure_python         | 318 us                                                       | 314 us: 1.01x faster                                         |
| asyncio_websockets         | 387 ms                                                       | 390 ms: 1.01x slower                                         |
| pyflate                    | 439 ms                                                       | 442 ms: 1.01x slower                                         |
| pidigits                   | 265 ms                                                       | 268 ms: 1.01x slower                                         |
| dulwich_log                | 65.4 ms                                                      | 66.3 ms: 1.01x slower                                        |
| dask                       | 392 ms                                                       | 400 ms: 1.02x slower                                         |
| scimark_sor                | 109 ms                                                       | 111 ms: 1.02x slower                                         |
| json_loads                 | 24.4 us                                                      | 24.9 us: 1.02x slower                                        |
| bench_thread_pool          | 950 us                                                       | 975 us: 1.03x slower                                         |
| meteor_contest             | 128 ms                                                       | 132 ms: 1.03x slower                                         |
| crypto_pyaes               | 80.3 ms                                                      | 82.7 ms: 1.03x slower                                        |
| sqlglot_optimize           | 57.5 ms                                                      | 59.2 ms: 1.03x slower                                        |
| json                       | 5.12 ms                                                      | 5.29 ms: 1.03x slower                                        |
| deepcopy_reduce            | 3.37 us                                                      | 3.48 us: 1.03x slower                                        |
| xml_etree_iterparse        | 103 ms                                                       | 107 ms: 1.04x slower                                         |
| sqlalchemy_imperative      | 18.7 ms                                                      | 19.5 ms: 1.04x slower                                        |
| sympy_integrate            | 23.9 ms                                                      | 24.9 ms: 1.04x slower                                        |
| logging_format             | 7.48 us                                                      | 7.78 us: 1.04x slower                                        |
| chameleon                  | 7.23 ms                                                      | 7.53 ms: 1.04x slower                                        |
| spectral_norm              | 91.6 ms                                                      | 95.9 ms: 1.05x slower                                        |
| deepcopy_memo              | 36.8 us                                                      | 38.5 us: 1.05x slower                                        |
| regex_compile              | 144 ms                                                       | 151 ms: 1.05x slower                                         |
| raytrace                   | 298 ms                                                       | 313 ms: 1.05x slower                                         |
| logging_simple             | 6.71 us                                                      | 7.06 us: 1.05x slower                                        |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 735 ms: 1.05x slower                                         |
| gc_traversal               | 3.48 ms                                                      | 3.67 ms: 1.05x slower                                        |
| pycparser                  | 1.23 sec                                                     | 1.30 sec: 1.06x slower                                       |
| tomli_loads                | 2.16 sec                                                     | 2.28 sec: 1.06x slower                                       |
| richards                   | 45.7 ms                                                      | 48.5 ms: 1.06x slower                                        |
| go                         | 150 ms                                                       | 159 ms: 1.06x slower                                         |
| sqlglot_transpile          | 1.78 ms                                                      | 1.89 ms: 1.06x slower                                        |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 743 ms: 1.07x slower                                         |
| sqlglot_normalize          | 116 ms                                                       | 124 ms: 1.07x slower                                         |
| django_template            | 38.2 ms                                                      | 40.8 ms: 1.07x slower                                        |
| async_tree_io_tg           | 1.05 sec                                                     | 1.13 sec: 1.07x slower                                       |
| logging_silent             | 94.4 ns                                                      | 101 ns: 1.07x slower                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 581 ms: 1.07x slower                                         |
| mdp                        | 2.57 sec                                                     | 2.78 sec: 1.08x slower                                       |
| async_tree_none_tg         | 431 ms                                                       | 466 ms: 1.08x slower                                         |
| deepcopy                   | 368 us                                                       | 399 us: 1.08x slower                                         |
| nqueens                    | 89.9 ms                                                      | 97.8 ms: 1.09x slower                                        |
| sympy_str                  | 302 ms                                                       | 329 ms: 1.09x slower                                         |
| comprehensions             | 21.9 us                                                      | 24.0 us: 1.09x slower                                        |
| mako                       | 10.0 ms                                                      | 11.0 ms: 1.10x slower                                        |
| xml_etree_parse            | 144 ms                                                       | 158 ms: 1.10x slower                                         |
| sympy_sum                  | 162 ms                                                       | 180 ms: 1.11x slower                                         |
| sqlglot_parse              | 1.38 ms                                                      | 1.53 ms: 1.11x slower                                        |
| async_tree_io              | 1.04 sec                                                     | 1.16 sec: 1.11x slower                                       |
| sympy_expand               | 484 ms                                                       | 545 ms: 1.13x slower                                         |
| async_tree_none            | 452 ms                                                       | 514 ms: 1.14x slower                                         |
| unpickle_pure_python       | 210 us                                                       | 239 us: 1.14x slower                                         |
| async_tree_memoization     | 544 ms                                                       | 621 ms: 1.14x slower                                         |
| scimark_lu                 | 98.8 ms                                                      | 114 ms: 1.16x slower                                         |
| hexiom                     | 5.96 ms                                                      | 7.07 ms: 1.19x slower                                        |
| richards_super             | 51.3 ms                                                      | 61.2 ms: 1.19x slower                                        |
| nbody                      | 88.0 ms                                                      | 105 ms: 1.20x slower                                         |
| coroutines                 | 23.0 ms                                                      | 27.8 ms: 1.21x slower                                        |
| deltablue                  | 3.24 ms                                                      | 3.99 ms: 1.23x slower                                        |
| fannkuch                   | 350 ms                                                       | 435 ms: 1.24x slower                                         |
| chaos                      | 64.0 ms                                                      | 82.4 ms: 1.29x slower                                        |
| json_dumps                 | 10.2 ms                                                      | 13.2 ms: 1.29x slower                                        |
| generators                 | 37.4 ms                                                      | 54.4 ms: 1.45x slower                                        |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 3.07 sec: 1.93x slower                                       |
| asyncio_tcp                | 378 ms                                                       | 742 ms: 1.96x slower                                         |
| typing_runtime_protocols   | 152 us                                                       | 526 us: 3.47x slower                                         |
| Geometric mean             | (ref)                                                        | 1.06x slower                                                 |

Benchmark hidden because not significant (4): bench_mp_pool, create_gc_cycles, unpickle_list, tornado_http
Ignored benchmarks (6) of results/bm-20231204-3.11.7-fa7a6f2/bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.90x