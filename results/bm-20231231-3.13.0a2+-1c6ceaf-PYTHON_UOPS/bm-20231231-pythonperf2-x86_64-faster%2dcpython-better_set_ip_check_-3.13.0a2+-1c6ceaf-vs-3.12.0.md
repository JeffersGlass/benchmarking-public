
# Results vs. 3.12.0

- fork: faster-cpython
- ref: better_set_ip_check_
- machine: linux-x86_64
- commit hash: 1c6ceaf
- commit date: 2023-12-31
- overall geometric mean: 1.10x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 309 ms: 1.08x slower                                                                   |
| chameleon      | 7.23 ms                                                      | 8.09 ms: 1.12x slower                                                                  |
| docutils       | 2.87 sec                                                     | 2.94 sec: 1.02x slower                                                                 |
| Geometric mean | (ref)                                                        | 1.06x slower                                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 696 ms                                                       | 714 ms: 1.03x slower                                                                   |
| async_tree_memoization_tg  | 540 ms                                                       | 556 ms: 1.03x slower                                                                   |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 718 ms: 1.03x slower                                                                   |
| async_tree_memoization     | 544 ms                                                       | 562 ms: 1.03x slower                                                                   |
| async_tree_none_tg         | 431 ms                                                       | 447 ms: 1.04x slower                                                                   |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                                 |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                                 |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                           |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 263 ms: 1.01x faster                                                                   |
| float          | 76.6 ms                                                      | 103 ms: 1.34x slower                                                                   |
| nbody          | 88.0 ms                                                      | 129 ms: 1.47x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.25x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 245 ms: 1.03x slower                                                                   |
| regex_v8       | 23.6 ms                                                      | 25.5 ms: 1.08x slower                                                                  |
| regex_compile  | 144 ms                                                       | 170 ms: 1.18x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 30.7 us: 1.06x faster                                                                  |
| pickle               | 10.5 us                                                      | 10.0 us: 1.05x faster                                                                  |
| pickle_list          | 4.43 us                                                      | 4.23 us: 1.05x faster                                                                  |
| pickle_pure_python   | 318 us                                                       | 314 us: 1.01x faster                                                                   |
| unpickle_list        | 4.66 us                                                      | 4.69 us: 1.01x slower                                                                  |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                                   |
| json_loads           | 24.4 us                                                      | 25.0 us: 1.02x slower                                                                  |
| unpickle             | 14.8 us                                                      | 15.2 us: 1.02x slower                                                                  |
| xml_etree_generate   | 86.1 ms                                                      | 90.5 ms: 1.05x slower                                                                  |
| xml_etree_process    | 58.4 ms                                                      | 61.5 ms: 1.05x slower                                                                  |
| json_dumps           | 10.2 ms                                                      | 10.9 ms: 1.06x slower                                                                  |
| xml_etree_iterparse  | 103 ms                                                       | 112 ms: 1.09x slower                                                                   |
| unpickle_pure_python | 210 us                                                       | 242 us: 1.16x slower                                                                   |
| tomli_loads          | 2.16 sec                                                     | 2.75 sec: 1.27x slower                                                                 |
| Geometric mean       | (ref)                                                        | 1.04x slower                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                                  |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 14.1 ms: 1.41x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 124 us: 1.22x faster                                                                   |
| unpack_sequence            | 53.2 ns                                                      | 46.7 ns: 1.14x faster                                                                  |
| generators                 | 37.4 ms                                                      | 33.9 ms: 1.10x faster                                                                  |
| async_generators           | 390 ms                                                       | 361 ms: 1.08x faster                                                                   |
| pickle_dict                | 32.5 us                                                      | 30.7 us: 1.06x faster                                                                  |
| pickle                     | 10.5 us                                                      | 10.0 us: 1.05x faster                                                                  |
| pickle_list                | 4.43 us                                                      | 4.23 us: 1.05x faster                                                                  |
| coroutines                 | 23.0 ms                                                      | 22.0 ms: 1.04x faster                                                                  |
| pickle_pure_python         | 318 us                                                       | 314 us: 1.01x faster                                                                   |
| asyncio_tcp                | 378 ms                                                       | 373 ms: 1.01x faster                                                                   |
| pidigits                   | 265 ms                                                       | 263 ms: 1.01x faster                                                                   |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.59 sec: 1.00x slower                                                                 |
| unpickle_list              | 4.66 us                                                      | 4.69 us: 1.01x slower                                                                  |
| raytrace                   | 298 ms                                                       | 300 ms: 1.01x slower                                                                   |
| logging_simple             | 6.71 us                                                      | 6.84 us: 1.02x slower                                                                  |
| mdp                        | 2.57 sec                                                     | 2.62 sec: 1.02x slower                                                                 |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                                   |
| json                       | 5.12 ms                                                      | 5.24 ms: 1.02x slower                                                                  |
| docutils                   | 2.87 sec                                                     | 2.94 sec: 1.02x slower                                                                 |
| bench_thread_pool          | 950 us                                                       | 972 us: 1.02x slower                                                                   |
| json_loads                 | 24.4 us                                                      | 25.0 us: 1.02x slower                                                                  |
| unpickle                   | 14.8 us                                                      | 15.2 us: 1.02x slower                                                                  |
| deepcopy_reduce            | 3.37 us                                                      | 3.45 us: 1.02x slower                                                                  |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 714 ms: 1.03x slower                                                                   |
| regex_dna                  | 239 ms                                                       | 245 ms: 1.03x slower                                                                   |
| async_tree_memoization_tg  | 540 ms                                                       | 556 ms: 1.03x slower                                                                   |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 718 ms: 1.03x slower                                                                   |
| sympy_sum                  | 162 ms                                                       | 167 ms: 1.03x slower                                                                   |
| async_tree_memoization     | 544 ms                                                       | 562 ms: 1.03x slower                                                                   |
| async_tree_none_tg         | 431 ms                                                       | 447 ms: 1.04x slower                                                                   |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.04x slower                                                                 |
| sympy_integrate            | 23.9 ms                                                      | 25.0 ms: 1.04x slower                                                                  |
| pathlib                    | 18.9 ms                                                      | 19.7 ms: 1.04x slower                                                                  |
| sqlglot_parse              | 1.38 ms                                                      | 1.44 ms: 1.05x slower                                                                  |
| sqlglot_transpile          | 1.78 ms                                                      | 1.86 ms: 1.05x slower                                                                  |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.05x slower                                                                 |
| dask                       | 392 ms                                                       | 411 ms: 1.05x slower                                                                   |
| xml_etree_generate         | 86.1 ms                                                      | 90.5 ms: 1.05x slower                                                                  |
| xml_etree_process          | 58.4 ms                                                      | 61.5 ms: 1.05x slower                                                                  |
| deepcopy                   | 368 us                                                       | 388 us: 1.05x slower                                                                   |
| sqlglot_normalize          | 116 ms                                                       | 122 ms: 1.06x slower                                                                   |
| logging_silent             | 94.4 ns                                                      | 100.0 ns: 1.06x slower                                                                 |
| scimark_lu                 | 98.8 ms                                                      | 105 ms: 1.06x slower                                                                   |
| crypto_pyaes               | 80.3 ms                                                      | 85.4 ms: 1.06x slower                                                                  |
| json_dumps                 | 10.2 ms                                                      | 10.9 ms: 1.06x slower                                                                  |
| sympy_str                  | 302 ms                                                       | 323 ms: 1.07x slower                                                                   |
| meteor_contest             | 128 ms                                                       | 138 ms: 1.07x slower                                                                   |
| regex_v8                   | 23.6 ms                                                      | 25.5 ms: 1.08x slower                                                                  |
| mypy2                      | 830 ms                                                       | 897 ms: 1.08x slower                                                                   |
| 2to3                       | 285 ms                                                       | 309 ms: 1.08x slower                                                                   |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                                  |
| pycparser                  | 1.23 sec                                                     | 1.34 sec: 1.09x slower                                                                 |
| xml_etree_iterparse        | 103 ms                                                       | 112 ms: 1.09x slower                                                                   |
| deepcopy_memo              | 36.8 us                                                      | 40.3 us: 1.10x slower                                                                  |
| dulwich_log                | 65.4 ms                                                      | 71.7 ms: 1.10x slower                                                                  |
| sqlglot_optimize           | 57.5 ms                                                      | 63.4 ms: 1.10x slower                                                                  |
| sympy_expand               | 484 ms                                                       | 538 ms: 1.11x slower                                                                   |
| comprehensions             | 21.9 us                                                      | 24.5 us: 1.12x slower                                                                  |
| chameleon                  | 7.23 ms                                                      | 8.09 ms: 1.12x slower                                                                  |
| pprint_safe_repr           | 807 ms                                                       | 920 ms: 1.14x slower                                                                   |
| pprint_pformat             | 1.65 sec                                                     | 1.90 sec: 1.15x slower                                                                 |
| unpickle_pure_python       | 210 us                                                       | 242 us: 1.16x slower                                                                   |
| regex_compile              | 144 ms                                                       | 170 ms: 1.18x slower                                                                   |
| nqueens                    | 89.9 ms                                                      | 107 ms: 1.19x slower                                                                   |
| richards_super             | 51.3 ms                                                      | 61.3 ms: 1.19x slower                                                                  |
| richards                   | 45.7 ms                                                      | 54.7 ms: 1.20x slower                                                                  |
| chaos                      | 64.0 ms                                                      | 77.4 ms: 1.21x slower                                                                  |
| telco                      | 6.96 ms                                                      | 8.45 ms: 1.21x slower                                                                  |
| go                         | 150 ms                                                       | 182 ms: 1.22x slower                                                                   |
| coverage                   | 66.7 ms                                                      | 83.2 ms: 1.25x slower                                                                  |
| scimark_monte_carlo        | 69.0 ms                                                      | 86.1 ms: 1.25x slower                                                                  |
| tomli_loads                | 2.16 sec                                                     | 2.75 sec: 1.27x slower                                                                 |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                                  |
| pyflate                    | 439 ms                                                       | 567 ms: 1.29x slower                                                                   |
| scimark_sor                | 109 ms                                                       | 144 ms: 1.32x slower                                                                   |
| float                      | 76.6 ms                                                      | 103 ms: 1.34x slower                                                                   |
| fannkuch                   | 350 ms                                                       | 478 ms: 1.37x slower                                                                   |
| scimark_fft                | 301 ms                                                       | 423 ms: 1.40x slower                                                                   |
| mako                       | 10.0 ms                                                      | 14.1 ms: 1.41x slower                                                                  |
| nbody                      | 88.0 ms                                                      | 129 ms: 1.47x slower                                                                   |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.30 ms: 1.50x slower                                                                  |
| hexiom                     | 5.96 ms                                                      | 9.70 ms: 1.63x slower                                                                  |
| deltablue                  | 3.24 ms                                                      | 5.42 ms: 1.68x slower                                                                  |
| spectral_norm              | 91.6 ms                                                      | 162 ms: 1.77x slower                                                                   |
| Geometric mean             | (ref)                                                        | 1.10x slower                                                                           |

Benchmark hidden because not significant (9): bench_mp_pool, async_tree_none, logging_format, asyncio_websockets, sqlite_synth, gc_traversal, create_gc_cycles, tornado_http, regex_effbot
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.88x