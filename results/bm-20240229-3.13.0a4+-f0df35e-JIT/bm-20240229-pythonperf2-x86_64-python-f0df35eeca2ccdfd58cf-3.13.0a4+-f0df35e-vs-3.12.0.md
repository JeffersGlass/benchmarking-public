# Results vs. 3.12.0

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: linux-x86_64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 310 ms: 1.09x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.45 ms: 1.03x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.96 sec: 1.03x slower                                                       |
| tornado_http   | 121 ms                                                       | 127 ms: 1.05x slower                                                         |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 444 ms: 1.02x faster                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 712 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 715 ms: 1.03x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 560 ms: 1.03x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 444 ms: 1.03x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 563 ms: 1.04x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.10 sec: 1.04x slower                                                       |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.06x slower                                                       |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 262 ms: 1.01x faster                                                         |
| float          | 76.6 ms                                                      | 78.8 ms: 1.03x slower                                                        |
| nbody          | 88.0 ms                                                      | 102 ms: 1.16x slower                                                         |
| Geometric mean | (ref)                                                        | 1.06x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.50 ms: 1.02x faster                                                        |
| regex_compile  | 144 ms                                                       | 154 ms: 1.07x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 25.3 ms: 1.07x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 30.4 us: 1.07x faster                                                        |
| pickle               | 10.5 us                                                      | 10.2 us: 1.03x faster                                                        |
| unpickle_list        | 4.66 us                                                      | 4.60 us: 1.01x faster                                                        |
| unpickle             | 14.8 us                                                      | 14.6 us: 1.01x faster                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 86.8 ms: 1.01x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 59.5 ms: 1.02x slower                                                        |
| pickle_list          | 4.43 us                                                      | 4.51 us: 1.02x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.4 ms: 1.02x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 106 ms: 1.03x slower                                                         |
| json_loads           | 24.4 us                                                      | 25.0 us: 1.03x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 151 ms: 1.05x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.39 sec: 1.11x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 243 us: 1.16x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                                 |

Benchmark hidden because not significant (1): pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 15.7 ms: 1.35x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 14.1 ms: 1.64x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.49x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 10.7 ms: 1.07x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 120 us: 1.26x faster                                                         |
| comprehensions             | 21.9 us                                                      | 19.2 us: 1.14x faster                                                        |
| generators                 | 37.4 ms                                                      | 33.4 ms: 1.12x faster                                                        |
| pickle_dict                | 32.5 us                                                      | 30.4 us: 1.07x faster                                                        |
| logging_format             | 7.48 us                                                      | 7.15 us: 1.05x faster                                                        |
| pickle                     | 10.5 us                                                      | 10.2 us: 1.03x faster                                                        |
| sqlite_synth               | 2.77 us                                                      | 2.70 us: 1.03x faster                                                        |
| coroutines                 | 23.0 ms                                                      | 22.4 ms: 1.03x faster                                                        |
| regex_effbot               | 3.57 ms                                                      | 3.50 ms: 1.02x faster                                                        |
| logging_simple             | 6.71 us                                                      | 6.58 us: 1.02x faster                                                        |
| create_gc_cycles           | 1.59 ms                                                      | 1.56 ms: 1.02x faster                                                        |
| async_tree_none            | 452 ms                                                       | 444 ms: 1.02x faster                                                         |
| unpickle_list              | 4.66 us                                                      | 4.60 us: 1.01x faster                                                        |
| unpickle                   | 14.8 us                                                      | 14.6 us: 1.01x faster                                                        |
| pidigits                   | 265 ms                                                       | 262 ms: 1.01x faster                                                         |
| async_generators           | 390 ms                                                       | 388 ms: 1.01x faster                                                         |
| sympy_sum                  | 162 ms                                                       | 163 ms: 1.01x slower                                                         |
| crypto_pyaes               | 80.3 ms                                                      | 80.9 ms: 1.01x slower                                                        |
| xml_etree_generate         | 86.1 ms                                                      | 86.8 ms: 1.01x slower                                                        |
| sympy_str                  | 302 ms                                                       | 306 ms: 1.01x slower                                                         |
| mdp                        | 2.57 sec                                                     | 2.61 sec: 1.01x slower                                                       |
| xml_etree_process          | 58.4 ms                                                      | 59.5 ms: 1.02x slower                                                        |
| pickle_list                | 4.43 us                                                      | 4.51 us: 1.02x slower                                                        |
| json_dumps                 | 10.2 ms                                                      | 10.4 ms: 1.02x slower                                                        |
| raytrace                   | 298 ms                                                       | 304 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 712 ms: 1.02x slower                                                         |
| xml_etree_iterparse        | 103 ms                                                       | 106 ms: 1.03x slower                                                         |
| json_loads                 | 24.4 us                                                      | 25.0 us: 1.03x slower                                                        |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 715 ms: 1.03x slower                                                         |
| meteor_contest             | 128 ms                                                       | 132 ms: 1.03x slower                                                         |
| float                      | 76.6 ms                                                      | 78.8 ms: 1.03x slower                                                        |
| async_tree_memoization     | 544 ms                                                       | 560 ms: 1.03x slower                                                         |
| chameleon                  | 7.23 ms                                                      | 7.45 ms: 1.03x slower                                                        |
| async_tree_none_tg         | 431 ms                                                       | 444 ms: 1.03x slower                                                         |
| deepcopy_reduce            | 3.37 us                                                      | 3.48 us: 1.03x slower                                                        |
| docutils                   | 2.87 sec                                                     | 2.96 sec: 1.03x slower                                                       |
| pathlib                    | 18.9 ms                                                      | 19.5 ms: 1.03x slower                                                        |
| sqlglot_normalize          | 116 ms                                                       | 120 ms: 1.04x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 563 ms: 1.04x slower                                                         |
| json                       | 5.12 ms                                                      | 5.33 ms: 1.04x slower                                                        |
| async_tree_io_tg           | 1.05 sec                                                     | 1.10 sec: 1.04x slower                                                       |
| tornado_http               | 121 ms                                                       | 127 ms: 1.05x slower                                                         |
| sympy_integrate            | 23.9 ms                                                      | 25.1 ms: 1.05x slower                                                        |
| xml_etree_parse            | 144 ms                                                       | 151 ms: 1.05x slower                                                         |
| bench_thread_pool          | 950 us                                                       | 998 us: 1.05x slower                                                         |
| sqlglot_parse              | 1.38 ms                                                      | 1.45 ms: 1.05x slower                                                        |
| deepcopy                   | 368 us                                                       | 388 us: 1.05x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.06x slower                                                       |
| sqlglot_transpile          | 1.78 ms                                                      | 1.88 ms: 1.06x slower                                                        |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.45 ms: 1.06x slower                                                        |
| logging_silent             | 94.4 ns                                                      | 100 ns: 1.06x slower                                                         |
| regex_compile              | 144 ms                                                       | 154 ms: 1.07x slower                                                         |
| regex_v8                   | 23.6 ms                                                      | 25.3 ms: 1.07x slower                                                        |
| mako                       | 10.0 ms                                                      | 10.7 ms: 1.07x slower                                                        |
| pycparser                  | 1.23 sec                                                     | 1.33 sec: 1.08x slower                                                       |
| chaos                      | 64.0 ms                                                      | 69.2 ms: 1.08x slower                                                        |
| sympy_expand               | 484 ms                                                       | 523 ms: 1.08x slower                                                         |
| deepcopy_memo              | 36.8 us                                                      | 39.8 us: 1.08x slower                                                        |
| spectral_norm              | 91.6 ms                                                      | 99.6 ms: 1.09x slower                                                        |
| dulwich_log                | 65.4 ms                                                      | 71.1 ms: 1.09x slower                                                        |
| 2to3                       | 285 ms                                                       | 310 ms: 1.09x slower                                                         |
| pprint_safe_repr           | 807 ms                                                       | 886 ms: 1.10x slower                                                         |
| pprint_pformat             | 1.65 sec                                                     | 1.83 sec: 1.10x slower                                                       |
| tomli_loads                | 2.16 sec                                                     | 2.39 sec: 1.11x slower                                                       |
| mypy2                      | 830 ms                                                       | 925 ms: 1.11x slower                                                         |
| sqlglot_optimize           | 57.5 ms                                                      | 64.3 ms: 1.12x slower                                                        |
| gc_traversal               | 3.48 ms                                                      | 3.89 ms: 1.12x slower                                                        |
| scimark_fft                | 301 ms                                                       | 341 ms: 1.13x slower                                                         |
| richards                   | 45.7 ms                                                      | 52.2 ms: 1.14x slower                                                        |
| richards_super             | 51.3 ms                                                      | 58.6 ms: 1.14x slower                                                        |
| nqueens                    | 89.9 ms                                                      | 104 ms: 1.15x slower                                                         |
| unpickle_pure_python       | 210 us                                                       | 243 us: 1.16x slower                                                         |
| nbody                      | 88.0 ms                                                      | 102 ms: 1.16x slower                                                         |
| deltablue                  | 3.24 ms                                                      | 3.80 ms: 1.17x slower                                                        |
| go                         | 150 ms                                                       | 176 ms: 1.18x slower                                                         |
| telco                      | 6.96 ms                                                      | 8.32 ms: 1.20x slower                                                        |
| scimark_monte_carlo        | 69.0 ms                                                      | 84.3 ms: 1.22x slower                                                        |
| scimark_lu                 | 98.8 ms                                                      | 121 ms: 1.22x slower                                                         |
| pyflate                    | 439 ms                                                       | 544 ms: 1.24x slower                                                         |
| fannkuch                   | 350 ms                                                       | 440 ms: 1.26x slower                                                         |
| coverage                   | 66.7 ms                                                      | 84.7 ms: 1.27x slower                                                        |
| hexiom                     | 5.96 ms                                                      | 7.69 ms: 1.29x slower                                                        |
| python_startup             | 11.6 ms                                                      | 15.7 ms: 1.35x slower                                                        |
| scimark_sor                | 109 ms                                                       | 156 ms: 1.43x slower                                                         |
| bench_mp_pool              | 4.76 ms                                                      | 6.93 ms: 1.45x slower                                                        |
| unpack_sequence            | 53.2 ns                                                      | 81.5 ns: 1.53x slower                                                        |
| python_startup_no_site     | 8.64 ms                                                      | 14.1 ms: 1.64x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.07x slower                                                                 |

Benchmark hidden because not significant (5): asyncio_websockets, asyncio_tcp_ssl, asyncio_tcp, regex_dna, pickle_pure_python
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.11x