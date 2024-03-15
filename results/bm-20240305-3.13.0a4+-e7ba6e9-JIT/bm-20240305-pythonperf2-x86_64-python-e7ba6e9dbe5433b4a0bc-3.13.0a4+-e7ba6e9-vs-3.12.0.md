# Results vs. 3.12.0

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: linux-x86_64
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.05x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.12x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 306 ms: 1.07x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.45 ms: 1.03x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.91 sec: 1.02x slower                                                       |
| tornado_http   | 121 ms                                                       | 125 ms: 1.03x slower                                                         |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 438 ms: 1.03x faster                                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 705 ms: 1.01x slower                                                         |
| async_tree_none_tg         | 431 ms                                                       | 438 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 709 ms: 1.02x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 555 ms: 1.02x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.03x slower                                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 559 ms: 1.03x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.04x slower                                                       |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 261 ms: 1.01x faster                                                         |
| float          | 76.6 ms                                                      | 77.6 ms: 1.01x slower                                                        |
| nbody          | 88.0 ms                                                      | 105 ms: 1.20x slower                                                         |
| Geometric mean | (ref)                                                        | 1.06x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.46 ms: 1.03x faster                                                        |
| regex_dna      | 239 ms                                                       | 235 ms: 1.02x faster                                                         |
| regex_compile  | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 25.4 ms: 1.07x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 30.5 us: 1.07x faster                                                        |
| pickle_list          | 4.43 us                                                      | 4.21 us: 1.05x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 311 us: 1.02x faster                                                         |
| xml_etree_generate   | 86.1 ms                                                      | 84.3 ms: 1.02x faster                                                        |
| xml_etree_process    | 58.4 ms                                                      | 57.6 ms: 1.01x faster                                                        |
| pickle               | 10.5 us                                                      | 10.4 us: 1.01x faster                                                        |
| tomli_loads          | 2.16 sec                                                     | 2.13 sec: 1.01x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.72 us: 1.01x slower                                                        |
| json_loads           | 24.4 us                                                      | 25.0 us: 1.02x slower                                                        |
| unpickle             | 14.8 us                                                      | 15.2 us: 1.03x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.6 ms: 1.03x slower                                                        |
| unpickle_pure_python | 210 us                                                       | 230 us: 1.10x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.00x faster                                                                 |

Benchmark hidden because not significant (2): xml_etree_iterparse, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 15.5 ms: 1.33x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 14.0 ms: 1.62x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.47x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako           | 10.0 ms                                                      | 9.93 ms: 1.01x faster                                                        |
| Geometric mean | (ref)                                                        | 1.00x faster                                                                 |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 119 us: 1.27x faster                                                         |
| comprehensions             | 21.9 us                                                      | 18.8 us: 1.16x faster                                                        |
| generators                 | 37.4 ms                                                      | 34.0 ms: 1.10x faster                                                        |
| pickle_dict                | 32.5 us                                                      | 30.5 us: 1.07x faster                                                        |
| pickle_list                | 4.43 us                                                      | 4.21 us: 1.05x faster                                                        |
| crypto_pyaes               | 80.3 ms                                                      | 77.6 ms: 1.03x faster                                                        |
| regex_effbot               | 3.57 ms                                                      | 3.46 ms: 1.03x faster                                                        |
| async_tree_none            | 452 ms                                                       | 438 ms: 1.03x faster                                                         |
| coroutines                 | 23.0 ms                                                      | 22.3 ms: 1.03x faster                                                        |
| sqlite_synth               | 2.77 us                                                      | 2.70 us: 1.03x faster                                                        |
| create_gc_cycles           | 1.59 ms                                                      | 1.55 ms: 1.03x faster                                                        |
| asyncio_tcp                | 378 ms                                                       | 368 ms: 1.03x faster                                                         |
| pickle_pure_python         | 318 us                                                       | 311 us: 1.02x faster                                                         |
| xml_etree_generate         | 86.1 ms                                                      | 84.3 ms: 1.02x faster                                                        |
| logging_format             | 7.48 us                                                      | 7.34 us: 1.02x faster                                                        |
| sympy_sum                  | 162 ms                                                       | 159 ms: 1.02x faster                                                         |
| regex_dna                  | 239 ms                                                       | 235 ms: 1.02x faster                                                         |
| async_generators           | 390 ms                                                       | 384 ms: 1.01x faster                                                         |
| pidigits                   | 265 ms                                                       | 261 ms: 1.01x faster                                                         |
| xml_etree_process          | 58.4 ms                                                      | 57.6 ms: 1.01x faster                                                        |
| pickle                     | 10.5 us                                                      | 10.4 us: 1.01x faster                                                        |
| tomli_loads                | 2.16 sec                                                     | 2.13 sec: 1.01x faster                                                       |
| deepcopy_reduce            | 3.37 us                                                      | 3.34 us: 1.01x faster                                                        |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.57 sec: 1.01x faster                                                       |
| mako                       | 10.0 ms                                                      | 9.93 ms: 1.01x faster                                                        |
| spectral_norm              | 91.6 ms                                                      | 92.4 ms: 1.01x slower                                                        |
| mdp                        | 2.57 sec                                                     | 2.59 sec: 1.01x slower                                                       |
| float                      | 76.6 ms                                                      | 77.6 ms: 1.01x slower                                                        |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 705 ms: 1.01x slower                                                         |
| unpickle_list              | 4.66 us                                                      | 4.72 us: 1.01x slower                                                        |
| docutils                   | 2.87 sec                                                     | 2.91 sec: 1.02x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 438 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 709 ms: 1.02x slower                                                         |
| raytrace                   | 298 ms                                                       | 303 ms: 1.02x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 555 ms: 1.02x slower                                                         |
| deepcopy_memo              | 36.8 us                                                      | 37.6 us: 1.02x slower                                                        |
| deepcopy                   | 368 us                                                       | 376 us: 1.02x slower                                                         |
| sympy_integrate            | 23.9 ms                                                      | 24.5 ms: 1.02x slower                                                        |
| json_loads                 | 24.4 us                                                      | 25.0 us: 1.02x slower                                                        |
| sqlglot_normalize          | 116 ms                                                       | 119 ms: 1.03x slower                                                         |
| regex_compile              | 144 ms                                                       | 148 ms: 1.03x slower                                                         |
| meteor_contest             | 128 ms                                                       | 132 ms: 1.03x slower                                                         |
| tornado_http               | 121 ms                                                       | 125 ms: 1.03x slower                                                         |
| pathlib                    | 18.9 ms                                                      | 19.4 ms: 1.03x slower                                                        |
| logging_silent             | 94.4 ns                                                      | 97.1 ns: 1.03x slower                                                        |
| unpickle                   | 14.8 us                                                      | 15.2 us: 1.03x slower                                                        |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.03x slower                                                       |
| chameleon                  | 7.23 ms                                                      | 7.45 ms: 1.03x slower                                                        |
| sqlglot_parse              | 1.38 ms                                                      | 1.42 ms: 1.03x slower                                                        |
| async_tree_memoization_tg  | 540 ms                                                       | 559 ms: 1.03x slower                                                         |
| json_dumps                 | 10.2 ms                                                      | 10.6 ms: 1.03x slower                                                        |
| async_tree_io              | 1.04 sec                                                     | 1.08 sec: 1.04x slower                                                       |
| pprint_safe_repr           | 807 ms                                                       | 844 ms: 1.05x slower                                                         |
| bench_thread_pool          | 950 us                                                       | 994 us: 1.05x slower                                                         |
| json                       | 5.12 ms                                                      | 5.37 ms: 1.05x slower                                                        |
| scimark_fft                | 301 ms                                                       | 316 ms: 1.05x slower                                                         |
| sqlglot_transpile          | 1.78 ms                                                      | 1.86 ms: 1.05x slower                                                        |
| pprint_pformat             | 1.65 sec                                                     | 1.74 sec: 1.05x slower                                                       |
| gc_traversal               | 3.48 ms                                                      | 3.67 ms: 1.05x slower                                                        |
| dulwich_log                | 65.4 ms                                                      | 69.1 ms: 1.06x slower                                                        |
| sympy_expand               | 484 ms                                                       | 513 ms: 1.06x slower                                                         |
| chaos                      | 64.0 ms                                                      | 68.3 ms: 1.07x slower                                                        |
| gunicorn                   | 1.00 ms                                                      | 1.07 ms: 1.07x slower                                                        |
| 2to3                       | 285 ms                                                       | 306 ms: 1.07x slower                                                         |
| regex_v8                   | 23.6 ms                                                      | 25.4 ms: 1.07x slower                                                        |
| aiohttp                    | 1.02 ms                                                      | 1.10 ms: 1.08x slower                                                        |
| sqlglot_optimize           | 57.5 ms                                                      | 62.8 ms: 1.09x slower                                                        |
| richards                   | 45.7 ms                                                      | 50.1 ms: 1.09x slower                                                        |
| pycparser                  | 1.23 sec                                                     | 1.35 sec: 1.09x slower                                                       |
| unpickle_pure_python       | 210 us                                                       | 230 us: 1.10x slower                                                         |
| richards_super             | 51.3 ms                                                      | 56.7 ms: 1.10x slower                                                        |
| mypy2                      | 830 ms                                                       | 917 ms: 1.10x slower                                                         |
| scimark_monte_carlo        | 69.0 ms                                                      | 77.5 ms: 1.12x slower                                                        |
| fannkuch                   | 350 ms                                                       | 394 ms: 1.12x slower                                                         |
| nqueens                    | 89.9 ms                                                      | 101 ms: 1.13x slower                                                         |
| go                         | 150 ms                                                       | 174 ms: 1.16x slower                                                         |
| unpack_sequence            | 53.2 ns                                                      | 61.9 ns: 1.16x slower                                                        |
| telco                      | 6.96 ms                                                      | 8.12 ms: 1.17x slower                                                        |
| deltablue                  | 3.24 ms                                                      | 3.78 ms: 1.17x slower                                                        |
| scimark_lu                 | 98.8 ms                                                      | 115 ms: 1.17x slower                                                         |
| pyflate                    | 439 ms                                                       | 518 ms: 1.18x slower                                                         |
| nbody                      | 88.0 ms                                                      | 105 ms: 1.20x slower                                                         |
| coverage                   | 66.7 ms                                                      | 81.9 ms: 1.23x slower                                                        |
| hexiom                     | 5.96 ms                                                      | 7.37 ms: 1.24x slower                                                        |
| python_startup             | 11.6 ms                                                      | 15.5 ms: 1.33x slower                                                        |
| scimark_sor                | 109 ms                                                       | 151 ms: 1.38x slower                                                         |
| bench_mp_pool              | 4.76 ms                                                      | 6.88 ms: 1.45x slower                                                        |
| dask                       | 392 ms                                                       | 589 ms: 1.50x slower                                                         |
| python_startup_no_site     | 8.64 ms                                                      | 14.0 ms: 1.62x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.05x slower                                                                 |

Benchmark hidden because not significant (7): xml_etree_iterparse, logging_simple, scimark_sparse_mat_mult, xml_etree_parse, sympy_str, django_template, asyncio_websockets
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-pythonperf2-x86_64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.12x