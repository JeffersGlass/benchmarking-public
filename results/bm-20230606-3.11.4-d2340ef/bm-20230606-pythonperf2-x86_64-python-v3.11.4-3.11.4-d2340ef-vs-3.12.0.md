
# Results vs. 3.12.0

- fork: python
- ref: v3.11.4
- machine: linux-x86_64
- commit hash: d2340ef
- commit date: 2023-06-06
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| chameleon      | 7.23 ms                                                      | 7.63 ms: 1.06x slower                                        |
| docutils       | 2.87 sec                                                     | 2.83 sec: 1.01x faster                                       |
| Geometric mean | (ref)                                                        | 1.01x slower                                                 |

Benchmark hidden because not significant (2): 2to3, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 758 ms: 1.09x slower                                         |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.13x slower                                       |
| async_tree_none         | 452 ms                                                       | 522 ms: 1.16x slower                                         |
| async_tree_memoization  | 544 ms                                                       | 630 ms: 1.16x slower                                         |
| Geometric mean          | (ref)                                                        | 1.13x slower                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 252 ms: 1.05x faster                                         |
| float          | 76.6 ms                                                      | 73.8 ms: 1.04x faster                                        |
| nbody          | 88.0 ms                                                      | 95.6 ms: 1.09x slower                                        |
| Geometric mean | (ref)                                                        | 1.00x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 231 ms: 1.03x faster                                         |
| regex_effbot   | 3.57 ms                                                      | 3.46 ms: 1.03x faster                                        |
| regex_v8       | 23.6 ms                                                      | 24.5 ms: 1.04x slower                                        |
| regex_compile  | 144 ms                                                       | 155 ms: 1.08x slower                                         |
| Geometric mean | (ref)                                                        | 1.01x slower                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.70 us: 1.20x faster                                        |
| unpickle             | 14.8 us                                                      | 13.0 us: 1.14x faster                                        |
| pickle_dict          | 32.5 us                                                      | 29.7 us: 1.10x faster                                        |
| xml_etree_generate   | 86.1 ms                                                      | 81.0 ms: 1.06x faster                                        |
| pickle               | 10.5 us                                                      | 9.96 us: 1.06x faster                                        |
| xml_etree_process    | 58.4 ms                                                      | 56.3 ms: 1.04x faster                                        |
| unpickle_list        | 4.66 us                                                      | 4.69 us: 1.01x slower                                        |
| pickle_pure_python   | 318 us                                                       | 321 us: 1.01x slower                                         |
| xml_etree_iterparse  | 103 ms                                                       | 105 ms: 1.02x slower                                         |
| tomli_loads          | 2.16 sec                                                     | 2.27 sec: 1.05x slower                                       |
| xml_etree_parse      | 144 ms                                                       | 159 ms: 1.11x slower                                         |
| unpickle_pure_python | 210 us                                                       | 243 us: 1.16x slower                                         |
| json_loads           | 24.4 us                                                      | 28.4 us: 1.17x slower                                        |
| json_dumps           | 10.2 ms                                                      | 13.4 ms: 1.31x slower                                        |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.72 ms: 1.12x faster                                        |
| python_startup         | 11.6 ms                                                      | 10.7 ms: 1.09x faster                                        |
| Geometric mean         | (ref)                                                        | 1.10x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 39.7 ms: 1.04x slower                                        |
| mako            | 10.0 ms                                                      | 10.8 ms: 1.08x slower                                        |
| Geometric mean  | (ref)                                                        | 1.06x slower                                                 |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_generators         | 390 ms                                                       | 322 ms: 1.21x faster                                         |
| pickle_list              | 4.43 us                                                      | 3.70 us: 1.20x faster                                        |
| unpack_sequence          | 53.2 ns                                                      | 45.6 ns: 1.17x faster                                        |
| unpickle                 | 14.8 us                                                      | 13.0 us: 1.14x faster                                        |
| python_startup_no_site   | 8.64 ms                                                      | 7.72 ms: 1.12x faster                                        |
| sqlite_synth             | 2.77 us                                                      | 2.48 us: 1.12x faster                                        |
| pickle_dict              | 32.5 us                                                      | 29.7 us: 1.10x faster                                        |
| python_startup           | 11.6 ms                                                      | 10.7 ms: 1.09x faster                                        |
| scimark_fft              | 301 ms                                                       | 281 ms: 1.07x faster                                         |
| xml_etree_generate       | 86.1 ms                                                      | 81.0 ms: 1.06x faster                                        |
| pickle                   | 10.5 us                                                      | 9.96 us: 1.06x faster                                        |
| pidigits                 | 265 ms                                                       | 252 ms: 1.05x faster                                         |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.01 ms: 1.05x faster                                        |
| bench_mp_pool            | 4.76 ms                                                      | 4.58 ms: 1.04x faster                                        |
| aiohttp                  | 1.02 ms                                                      | 980 us: 1.04x faster                                         |
| float                    | 76.6 ms                                                      | 73.8 ms: 1.04x faster                                        |
| xml_etree_process        | 58.4 ms                                                      | 56.3 ms: 1.04x faster                                        |
| regex_dna                | 239 ms                                                       | 231 ms: 1.03x faster                                         |
| telco                    | 6.96 ms                                                      | 6.75 ms: 1.03x faster                                        |
| sqlalchemy_declarative   | 159 ms                                                       | 154 ms: 1.03x faster                                         |
| regex_effbot             | 3.57 ms                                                      | 3.46 ms: 1.03x faster                                        |
| pprint_safe_repr         | 807 ms                                                       | 784 ms: 1.03x faster                                         |
| pprint_pformat           | 1.65 sec                                                     | 1.62 sec: 1.02x faster                                       |
| gunicorn                 | 1.00 ms                                                      | 981 us: 1.02x faster                                         |
| docutils                 | 2.87 sec                                                     | 2.83 sec: 1.01x faster                                       |
| deepcopy_reduce          | 3.37 us                                                      | 3.39 us: 1.01x slower                                        |
| unpickle_list            | 4.66 us                                                      | 4.69 us: 1.01x slower                                        |
| pickle_pure_python       | 318 us                                                       | 321 us: 1.01x slower                                         |
| scimark_monte_carlo      | 69.0 ms                                                      | 69.5 ms: 1.01x slower                                        |
| logging_format           | 7.48 us                                                      | 7.58 us: 1.01x slower                                        |
| meteor_contest           | 128 ms                                                       | 130 ms: 1.01x slower                                         |
| xml_etree_iterparse      | 103 ms                                                       | 105 ms: 1.02x slower                                         |
| create_gc_cycles         | 1.59 ms                                                      | 1.63 ms: 1.02x slower                                        |
| sqlglot_optimize         | 57.5 ms                                                      | 58.7 ms: 1.02x slower                                        |
| dask                     | 392 ms                                                       | 402 ms: 1.03x slower                                         |
| spectral_norm            | 91.6 ms                                                      | 94.1 ms: 1.03x slower                                        |
| dulwich_log              | 65.4 ms                                                      | 67.6 ms: 1.03x slower                                        |
| deepcopy_memo            | 36.8 us                                                      | 38.1 us: 1.03x slower                                        |
| crypto_pyaes             | 80.3 ms                                                      | 83.1 ms: 1.03x slower                                        |
| regex_v8                 | 23.6 ms                                                      | 24.5 ms: 1.04x slower                                        |
| pycparser                | 1.23 sec                                                     | 1.28 sec: 1.04x slower                                       |
| django_template          | 38.2 ms                                                      | 39.7 ms: 1.04x slower                                        |
| pyflate                  | 439 ms                                                       | 458 ms: 1.04x slower                                         |
| raytrace                 | 298 ms                                                       | 311 ms: 1.04x slower                                         |
| sqlalchemy_imperative    | 18.7 ms                                                      | 19.6 ms: 1.05x slower                                        |
| bench_thread_pool        | 950 us                                                       | 995 us: 1.05x slower                                         |
| sqlglot_normalize        | 116 ms                                                       | 122 ms: 1.05x slower                                         |
| deepcopy                 | 368 us                                                       | 387 us: 1.05x slower                                         |
| logging_simple           | 6.71 us                                                      | 7.05 us: 1.05x slower                                        |
| tomli_loads              | 2.16 sec                                                     | 2.27 sec: 1.05x slower                                       |
| scimark_sor              | 109 ms                                                       | 115 ms: 1.05x slower                                         |
| chameleon                | 7.23 ms                                                      | 7.63 ms: 1.06x slower                                        |
| gc_traversal             | 3.48 ms                                                      | 3.70 ms: 1.06x slower                                        |
| logging_silent           | 94.4 ns                                                      | 101 ns: 1.07x slower                                         |
| sympy_integrate          | 23.9 ms                                                      | 25.6 ms: 1.07x slower                                        |
| json                     | 5.12 ms                                                      | 5.48 ms: 1.07x slower                                        |
| regex_compile            | 144 ms                                                       | 155 ms: 1.08x slower                                         |
| sqlglot_transpile        | 1.78 ms                                                      | 1.91 ms: 1.08x slower                                        |
| mako                     | 10.0 ms                                                      | 10.8 ms: 1.08x slower                                        |
| nbody                    | 88.0 ms                                                      | 95.6 ms: 1.09x slower                                        |
| async_tree_cpu_io_mixed  | 696 ms                                                       | 758 ms: 1.09x slower                                         |
| nqueens                  | 89.9 ms                                                      | 98.5 ms: 1.10x slower                                        |
| sympy_str                | 302 ms                                                       | 334 ms: 1.10x slower                                         |
| xml_etree_parse          | 144 ms                                                       | 159 ms: 1.11x slower                                         |
| mdp                      | 2.57 sec                                                     | 2.86 sec: 1.11x slower                                       |
| sqlglot_parse            | 1.38 ms                                                      | 1.55 ms: 1.12x slower                                        |
| async_tree_io            | 1.04 sec                                                     | 1.17 sec: 1.13x slower                                       |
| sympy_sum                | 162 ms                                                       | 183 ms: 1.13x slower                                         |
| go                       | 150 ms                                                       | 170 ms: 1.14x slower                                         |
| sympy_expand             | 484 ms                                                       | 550 ms: 1.14x slower                                         |
| comprehensions           | 21.9 us                                                      | 24.9 us: 1.14x slower                                        |
| richards                 | 45.7 ms                                                      | 52.2 ms: 1.14x slower                                        |
| scimark_lu               | 98.8 ms                                                      | 113 ms: 1.15x slower                                         |
| async_tree_none          | 452 ms                                                       | 522 ms: 1.16x slower                                         |
| async_tree_memoization   | 544 ms                                                       | 630 ms: 1.16x slower                                         |
| unpickle_pure_python     | 210 us                                                       | 243 us: 1.16x slower                                         |
| json_loads               | 24.4 us                                                      | 28.4 us: 1.17x slower                                        |
| chaos                    | 64.0 ms                                                      | 75.0 ms: 1.17x slower                                        |
| hexiom                   | 5.96 ms                                                      | 7.06 ms: 1.19x slower                                        |
| coroutines               | 23.0 ms                                                      | 27.8 ms: 1.21x slower                                        |
| deltablue                | 3.24 ms                                                      | 4.06 ms: 1.25x slower                                        |
| fannkuch                 | 350 ms                                                       | 441 ms: 1.26x slower                                         |
| richards_super           | 51.3 ms                                                      | 65.2 ms: 1.27x slower                                        |
| json_dumps               | 10.2 ms                                                      | 13.4 ms: 1.31x slower                                        |
| generators               | 37.4 ms                                                      | 54.7 ms: 1.46x slower                                        |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 3.07 sec: 1.93x slower                                       |
| asyncio_tcp              | 378 ms                                                       | 751 ms: 1.99x slower                                         |
| typing_runtime_protocols | 152 us                                                       | 525 us: 3.46x slower                                         |
| Geometric mean           | (ref)                                                        | 1.07x slower                                                 |

Benchmark hidden because not significant (3): tornado_http, 2to3, pathlib
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2
Ignored benchmarks (6) of results/bm-20230606-3.11.4-d2340ef/bm-20230606-pythonperf2-x86_64-python-v3.11.4-3.11.4-d2340ef.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 0.91x