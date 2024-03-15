
# Results vs. 3.12.0

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 4448793
- commit date: 2024-01-16
- overall geometric mean: 1.14x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 318 ms: 1.12x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.85 ms: 1.09x slower                                                        |
| docutils       | 2.87 sec                                                     | 3.08 sec: 1.07x slower                                                       |
| tornado_http   | 121 ms                                                       | 124 ms: 1.02x slower                                                         |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 696 ms                                                       | 712 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 715 ms: 1.03x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 444 ms: 1.03x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 562 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.03x slower                                                       |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 571 ms: 1.06x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 106 ms: 1.38x slower                                                         |
| nbody          | 88.0 ms                                                      | 131 ms: 1.49x slower                                                         |
| Geometric mean | (ref)                                                        | 1.27x slower                                                                 |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.48 ms: 1.03x faster                                                        |
| regex_dna      | 239 ms                                                       | 250 ms: 1.05x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 26.9 ms: 1.14x slower                                                        |
| regex_compile  | 144 ms                                                       | 194 ms: 1.35x slower                                                         |
| Geometric mean | (ref)                                                        | 1.12x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 30.8 us: 1.06x faster                                                        |
| pickle               | 10.5 us                                                      | 10.2 us: 1.04x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 310 us: 1.03x faster                                                         |
| unpickle             | 14.8 us                                                      | 14.7 us: 1.00x faster                                                        |
| json_loads           | 24.4 us                                                      | 24.6 us: 1.01x slower                                                        |
| pickle_list          | 4.43 us                                                      | 4.50 us: 1.02x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| unpickle_list        | 4.66 us                                                      | 4.97 us: 1.07x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 62.6 ms: 1.07x slower                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 92.5 ms: 1.07x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 11.0 ms: 1.08x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 114 ms: 1.11x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.89 sec: 1.34x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 317 us: 1.51x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.07x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 14.9 ms: 1.49x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-pythonperf2-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-4448793 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 127 us: 1.19x faster                                                         |
| generators                 | 37.4 ms                                                      | 33.6 ms: 1.11x faster                                                        |
| pickle_dict                | 32.5 us                                                      | 30.8 us: 1.06x faster                                                        |
| coroutines                 | 23.0 ms                                                      | 22.1 ms: 1.04x faster                                                        |
| pickle                     | 10.5 us                                                      | 10.2 us: 1.04x faster                                                        |
| async_generators           | 390 ms                                                       | 379 ms: 1.03x faster                                                         |
| pickle_pure_python         | 318 us                                                       | 310 us: 1.03x faster                                                         |
| regex_effbot               | 3.57 ms                                                      | 3.48 ms: 1.03x faster                                                        |
| asyncio_tcp                | 378 ms                                                       | 373 ms: 1.01x faster                                                         |
| deepcopy_reduce            | 3.37 us                                                      | 3.34 us: 1.01x faster                                                        |
| unpickle                   | 14.8 us                                                      | 14.7 us: 1.00x faster                                                        |
| json_loads                 | 24.4 us                                                      | 24.6 us: 1.01x slower                                                        |
| sqlite_synth               | 2.77 us                                                      | 2.81 us: 1.01x slower                                                        |
| logging_format             | 7.48 us                                                      | 7.57 us: 1.01x slower                                                        |
| pickle_list                | 4.43 us                                                      | 4.50 us: 1.02x slower                                                        |
| tornado_http               | 121 ms                                                       | 124 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 712 ms: 1.02x slower                                                         |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 715 ms: 1.03x slower                                                         |
| mdp                        | 2.57 sec                                                     | 2.64 sec: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 444 ms: 1.03x slower                                                         |
| json                       | 5.12 ms                                                      | 5.28 ms: 1.03x slower                                                        |
| async_tree_memoization     | 544 ms                                                       | 562 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.03x slower                                                       |
| pathlib                    | 18.9 ms                                                      | 19.5 ms: 1.03x slower                                                        |
| deepcopy                   | 368 us                                                       | 381 us: 1.04x slower                                                         |
| bench_thread_pool          | 950 us                                                       | 990 us: 1.04x slower                                                         |
| logging_simple             | 6.71 us                                                      | 7.03 us: 1.05x slower                                                        |
| regex_dna                  | 239 ms                                                       | 250 ms: 1.05x slower                                                         |
| dask                       | 392 ms                                                       | 412 ms: 1.05x slower                                                         |
| logging_silent             | 94.4 ns                                                      | 99.4 ns: 1.05x slower                                                        |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 571 ms: 1.06x slower                                                         |
| crypto_pyaes               | 80.3 ms                                                      | 85.7 ms: 1.07x slower                                                        |
| unpickle_list              | 4.66 us                                                      | 4.97 us: 1.07x slower                                                        |
| raytrace                   | 298 ms                                                       | 319 ms: 1.07x slower                                                         |
| xml_etree_process          | 58.4 ms                                                      | 62.6 ms: 1.07x slower                                                        |
| xml_etree_generate         | 86.1 ms                                                      | 92.5 ms: 1.07x slower                                                        |
| docutils                   | 2.87 sec                                                     | 3.08 sec: 1.07x slower                                                       |
| json_dumps                 | 10.2 ms                                                      | 11.0 ms: 1.08x slower                                                        |
| sympy_sum                  | 162 ms                                                       | 175 ms: 1.08x slower                                                         |
| sympy_integrate            | 23.9 ms                                                      | 26.0 ms: 1.08x slower                                                        |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.09x slower                                                        |
| chameleon                  | 7.23 ms                                                      | 7.85 ms: 1.09x slower                                                        |
| gc_traversal               | 3.48 ms                                                      | 3.81 ms: 1.10x slower                                                        |
| meteor_contest             | 128 ms                                                       | 141 ms: 1.10x slower                                                         |
| sqlglot_transpile          | 1.78 ms                                                      | 1.96 ms: 1.10x slower                                                        |
| sqlglot_normalize          | 116 ms                                                       | 128 ms: 1.10x slower                                                         |
| xml_etree_iterparse        | 103 ms                                                       | 114 ms: 1.11x slower                                                         |
| sympy_str                  | 302 ms                                                       | 336 ms: 1.11x slower                                                         |
| 2to3                       | 285 ms                                                       | 318 ms: 1.12x slower                                                         |
| sqlglot_parse              | 1.38 ms                                                      | 1.54 ms: 1.12x slower                                                        |
| mypy2                      | 830 ms                                                       | 929 ms: 1.12x slower                                                         |
| deepcopy_memo              | 36.8 us                                                      | 41.2 us: 1.12x slower                                                        |
| regex_v8                   | 23.6 ms                                                      | 26.9 ms: 1.14x slower                                                        |
| sympy_expand               | 484 ms                                                       | 556 ms: 1.15x slower                                                         |
| dulwich_log                | 65.4 ms                                                      | 75.7 ms: 1.16x slower                                                        |
| pycparser                  | 1.23 sec                                                     | 1.44 sec: 1.16x slower                                                       |
| sqlglot_optimize           | 57.5 ms                                                      | 67.3 ms: 1.17x slower                                                        |
| coverage                   | 66.7 ms                                                      | 79.1 ms: 1.19x slower                                                        |
| comprehensions             | 21.9 us                                                      | 26.2 us: 1.20x slower                                                        |
| telco                      | 6.96 ms                                                      | 8.51 ms: 1.22x slower                                                        |
| chaos                      | 64.0 ms                                                      | 78.5 ms: 1.23x slower                                                        |
| pprint_safe_repr           | 807 ms                                                       | 998 ms: 1.24x slower                                                         |
| pprint_pformat             | 1.65 sec                                                     | 2.05 sec: 1.24x slower                                                       |
| unpack_sequence            | 53.2 ns                                                      | 66.4 ns: 1.25x slower                                                        |
| python_startup_no_site     | 8.64 ms                                                      | 11.1 ms: 1.28x slower                                                        |
| nqueens                    | 89.9 ms                                                      | 116 ms: 1.29x slower                                                         |
| tomli_loads                | 2.16 sec                                                     | 2.89 sec: 1.34x slower                                                       |
| go                         | 150 ms                                                       | 202 ms: 1.35x slower                                                         |
| regex_compile              | 144 ms                                                       | 194 ms: 1.35x slower                                                         |
| float                      | 76.6 ms                                                      | 106 ms: 1.38x slower                                                         |
| scimark_lu                 | 98.8 ms                                                      | 140 ms: 1.41x slower                                                         |
| scimark_fft                | 301 ms                                                       | 426 ms: 1.41x slower                                                         |
| scimark_sor                | 109 ms                                                       | 160 ms: 1.47x slower                                                         |
| fannkuch                   | 350 ms                                                       | 516 ms: 1.47x slower                                                         |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.23 ms: 1.48x slower                                                        |
| nbody                      | 88.0 ms                                                      | 131 ms: 1.49x slower                                                         |
| mako                       | 10.0 ms                                                      | 14.9 ms: 1.49x slower                                                        |
| pyflate                    | 439 ms                                                       | 660 ms: 1.51x slower                                                         |
| unpickle_pure_python       | 210 us                                                       | 317 us: 1.51x slower                                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 105 ms: 1.53x slower                                                         |
| richards_super             | 51.3 ms                                                      | 80.0 ms: 1.56x slower                                                        |
| richards                   | 45.7 ms                                                      | 71.6 ms: 1.56x slower                                                        |
| spectral_norm              | 91.6 ms                                                      | 161 ms: 1.76x slower                                                         |
| deltablue                  | 3.24 ms                                                      | 5.76 ms: 1.78x slower                                                        |
| hexiom                     | 5.96 ms                                                      | 10.9 ms: 1.82x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.14x slower                                                                 |

Benchmark hidden because not significant (6): bench_mp_pool, async_tree_none, asyncio_websockets, pidigits, create_gc_cycles, asyncio_tcp_ssl
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.07x
- 95% likely to have a slowdown of 1.07x
- 99% likely to have a slowdown of 1.06x


# Memory

- memory change: 0.88x