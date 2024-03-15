# Results vs. 3.12.0

- fork: python
- ref: fdb2d90a274158aee23b
- machine: linux-x86_64
- commit hash: fdb2d90
- commit date: 2024-03-08
- overall geometric mean: 1.14x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x slower
- Memory change: 0.89x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 322 ms: 1.13x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.57 ms: 1.05x slower                                                        |
| docutils       | 2.87 sec                                                     | 3.07 sec: 1.07x slower                                                       |
| tornado_http   | 121 ms                                                       | 129 ms: 1.06x slower                                                         |
| Geometric mean | (ref)                                                        | 1.08x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 446 ms: 1.01x faster                                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 712 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 713 ms: 1.02x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 559 ms: 1.03x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 443 ms: 1.03x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 560 ms: 1.04x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.10 sec: 1.04x slower                                                       |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                                       |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 105 ms: 1.37x slower                                                         |
| nbody          | 88.0 ms                                                      | 132 ms: 1.50x slower                                                         |
| Geometric mean | (ref)                                                        | 1.27x slower                                                                 |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 249 ms: 1.04x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 26.4 ms: 1.12x slower                                                        |
| regex_compile  | 144 ms                                                       | 203 ms: 1.41x slower                                                         |
| Geometric mean | (ref)                                                        | 1.13x slower                                                                 |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| unpickle_list        | 4.66 us                                                      | 4.59 us: 1.01x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 315 us: 1.01x faster                                                         |
| pickle_dict          | 32.5 us                                                      | 32.8 us: 1.01x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 145 ms: 1.01x slower                                                         |
| json_loads           | 24.4 us                                                      | 24.8 us: 1.02x slower                                                        |
| unpickle             | 14.8 us                                                      | 15.0 us: 1.02x slower                                                        |
| pickle               | 10.5 us                                                      | 10.8 us: 1.02x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.5 ms: 1.03x slower                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 90.6 ms: 1.05x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 62.1 ms: 1.06x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 113 ms: 1.10x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.99 sec: 1.39x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 309 us: 1.48x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.07x slower                                                                 |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.8 ms: 1.10x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.2 ms: 1.30x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.19x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|-----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 39.6 ms: 1.04x slower                                                        |
| mako            | 10.0 ms                                                      | 14.1 ms: 1.41x slower                                                        |
| Geometric mean  | (ref)                                                        | 1.21x slower                                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 123 us: 1.23x faster                                                         |
| generators                 | 37.4 ms                                                      | 34.1 ms: 1.10x faster                                                        |
| coroutines                 | 23.0 ms                                                      | 22.6 ms: 1.02x faster                                                        |
| unpickle_list              | 4.66 us                                                      | 4.59 us: 1.01x faster                                                        |
| async_tree_none            | 452 ms                                                       | 446 ms: 1.01x faster                                                         |
| pickle_pure_python         | 318 us                                                       | 315 us: 1.01x faster                                                         |
| asyncio_tcp                | 378 ms                                                       | 375 ms: 1.01x faster                                                         |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.59 sec: 1.00x slower                                                       |
| async_generators           | 390 ms                                                       | 393 ms: 1.01x slower                                                         |
| pickle_dict                | 32.5 us                                                      | 32.8 us: 1.01x slower                                                        |
| xml_etree_parse            | 144 ms                                                       | 145 ms: 1.01x slower                                                         |
| deepcopy_reduce            | 3.37 us                                                      | 3.42 us: 1.01x slower                                                        |
| json_loads                 | 24.4 us                                                      | 24.8 us: 1.02x slower                                                        |
| unpickle                   | 14.8 us                                                      | 15.0 us: 1.02x slower                                                        |
| pickle                     | 10.5 us                                                      | 10.8 us: 1.02x slower                                                        |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 712 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 713 ms: 1.02x slower                                                         |
| logging_simple             | 6.71 us                                                      | 6.87 us: 1.02x slower                                                        |
| sqlite_synth               | 2.77 us                                                      | 2.84 us: 1.03x slower                                                        |
| async_tree_memoization     | 544 ms                                                       | 559 ms: 1.03x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 443 ms: 1.03x slower                                                         |
| json_dumps                 | 10.2 ms                                                      | 10.5 ms: 1.03x slower                                                        |
| async_tree_memoization_tg  | 540 ms                                                       | 560 ms: 1.04x slower                                                         |
| django_template            | 38.2 ms                                                      | 39.6 ms: 1.04x slower                                                        |
| gc_traversal               | 3.48 ms                                                      | 3.61 ms: 1.04x slower                                                        |
| async_tree_io_tg           | 1.05 sec                                                     | 1.10 sec: 1.04x slower                                                       |
| deepcopy                   | 368 us                                                       | 383 us: 1.04x slower                                                         |
| mdp                        | 2.57 sec                                                     | 2.68 sec: 1.04x slower                                                       |
| regex_dna                  | 239 ms                                                       | 249 ms: 1.04x slower                                                         |
| chameleon                  | 7.23 ms                                                      | 7.57 ms: 1.05x slower                                                        |
| xml_etree_generate         | 86.1 ms                                                      | 90.6 ms: 1.05x slower                                                        |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                                       |
| bench_thread_pool          | 950 us                                                       | 1.00 ms: 1.05x slower                                                        |
| sqlglot_normalize          | 116 ms                                                       | 122 ms: 1.05x slower                                                         |
| sympy_integrate            | 23.9 ms                                                      | 25.3 ms: 1.06x slower                                                        |
| json                       | 5.12 ms                                                      | 5.41 ms: 1.06x slower                                                        |
| tornado_http               | 121 ms                                                       | 129 ms: 1.06x slower                                                         |
| xml_etree_process          | 58.4 ms                                                      | 62.1 ms: 1.06x slower                                                        |
| docutils                   | 2.87 sec                                                     | 3.07 sec: 1.07x slower                                                       |
| pathlib                    | 18.9 ms                                                      | 20.2 ms: 1.07x slower                                                        |
| logging_silent             | 94.4 ns                                                      | 101 ns: 1.07x slower                                                         |
| sympy_sum                  | 162 ms                                                       | 174 ms: 1.07x slower                                                         |
| gunicorn                   | 1.00 ms                                                      | 1.09 ms: 1.08x slower                                                        |
| aiohttp                    | 1.02 ms                                                      | 1.11 ms: 1.09x slower                                                        |
| python_startup             | 11.6 ms                                                      | 12.8 ms: 1.10x slower                                                        |
| crypto_pyaes               | 80.3 ms                                                      | 88.4 ms: 1.10x slower                                                        |
| xml_etree_iterparse        | 103 ms                                                       | 113 ms: 1.10x slower                                                         |
| sympy_str                  | 302 ms                                                       | 337 ms: 1.12x slower                                                         |
| meteor_contest             | 128 ms                                                       | 143 ms: 1.12x slower                                                         |
| regex_v8                   | 23.6 ms                                                      | 26.4 ms: 1.12x slower                                                        |
| sqlglot_transpile          | 1.78 ms                                                      | 1.99 ms: 1.12x slower                                                        |
| mypy2                      | 830 ms                                                       | 934 ms: 1.12x slower                                                         |
| sqlglot_parse              | 1.38 ms                                                      | 1.55 ms: 1.13x slower                                                        |
| 2to3                       | 285 ms                                                       | 322 ms: 1.13x slower                                                         |
| comprehensions             | 21.9 us                                                      | 25.2 us: 1.15x slower                                                        |
| deepcopy_memo              | 36.8 us                                                      | 42.3 us: 1.15x slower                                                        |
| dulwich_log                | 65.4 ms                                                      | 75.6 ms: 1.16x slower                                                        |
| sqlglot_optimize           | 57.5 ms                                                      | 66.5 ms: 1.16x slower                                                        |
| pycparser                  | 1.23 sec                                                     | 1.45 sec: 1.17x slower                                                       |
| sympy_expand               | 484 ms                                                       | 573 ms: 1.18x slower                                                         |
| telco                      | 6.96 ms                                                      | 8.28 ms: 1.19x slower                                                        |
| raytrace                   | 298 ms                                                       | 357 ms: 1.20x slower                                                         |
| chaos                      | 64.0 ms                                                      | 77.6 ms: 1.21x slower                                                        |
| pprint_safe_repr           | 807 ms                                                       | 982 ms: 1.22x slower                                                         |
| pprint_pformat             | 1.65 sec                                                     | 2.02 sec: 1.22x slower                                                       |
| coverage                   | 66.7 ms                                                      | 82.4 ms: 1.24x slower                                                        |
| unpack_sequence            | 53.2 ns                                                      | 65.7 ns: 1.24x slower                                                        |
| richards_super             | 51.3 ms                                                      | 64.6 ms: 1.26x slower                                                        |
| deltablue                  | 3.24 ms                                                      | 4.10 ms: 1.27x slower                                                        |
| richards                   | 45.7 ms                                                      | 58.4 ms: 1.28x slower                                                        |
| python_startup_no_site     | 8.64 ms                                                      | 11.2 ms: 1.30x slower                                                        |
| nqueens                    | 89.9 ms                                                      | 117 ms: 1.30x slower                                                         |
| go                         | 150 ms                                                       | 200 ms: 1.33x slower                                                         |
| float                      | 76.6 ms                                                      | 105 ms: 1.37x slower                                                         |
| tomli_loads                | 2.16 sec                                                     | 2.99 sec: 1.39x slower                                                       |
| mako                       | 10.0 ms                                                      | 14.1 ms: 1.41x slower                                                        |
| regex_compile              | 144 ms                                                       | 203 ms: 1.41x slower                                                         |
| scimark_lu                 | 98.8 ms                                                      | 140 ms: 1.42x slower                                                         |
| scimark_fft                | 301 ms                                                       | 430 ms: 1.43x slower                                                         |
| unpickle_pure_python       | 210 us                                                       | 309 us: 1.48x slower                                                         |
| scimark_sor                | 109 ms                                                       | 162 ms: 1.48x slower                                                         |
| nbody                      | 88.0 ms                                                      | 132 ms: 1.50x slower                                                         |
| dask                       | 392 ms                                                       | 591 ms: 1.51x slower                                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 105 ms: 1.52x slower                                                         |
| fannkuch                   | 350 ms                                                       | 543 ms: 1.55x slower                                                         |
| pyflate                    | 439 ms                                                       | 695 ms: 1.58x slower                                                         |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.71 ms: 1.60x slower                                                        |
| spectral_norm              | 91.6 ms                                                      | 152 ms: 1.66x slower                                                         |
| hexiom                     | 5.96 ms                                                      | 10.7 ms: 1.79x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.14x slower                                                                 |

Benchmark hidden because not significant (7): asyncio_websockets, pidigits, regex_effbot, logging_format, pickle_list, bench_mp_pool, create_gc_cycles
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240308-3.13.0a4+-fdb2d90-PYTHON_UOPS/bm-20240308-pythonperf2-x86_64-python-fdb2d90a274158aee23b-3.13.0a4+-fdb2d90.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.07x
- 95% likely to have a slowdown of 1.07x
- 99% likely to have a slowdown of 1.06x


# Memory

- memory change: 0.89x