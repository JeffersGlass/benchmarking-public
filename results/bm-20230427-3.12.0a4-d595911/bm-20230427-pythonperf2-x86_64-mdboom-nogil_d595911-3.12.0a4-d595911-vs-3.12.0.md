
# Results vs. 3.12.0

- fork: mdboom
- ref: nogil_d595911
- machine: linux-x86_64
- commit hash: d595911
- commit date: 2023-04-27
- overall geometric mean: 1.11x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x slower
- Memory change: 1.21x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 303 ms: 1.06x slower                                                 |
| chameleon      | 7.23 ms                                                      | 8.37 ms: 1.16x slower                                                |
| docutils       | 2.87 sec                                                     | 2.99 sec: 1.04x slower                                               |
| Geometric mean | (ref)                                                        | 1.09x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_io           | 1.04 sec                                                     | 595 ms: 1.75x faster                                                 |
| async_tree_memoization  | 544 ms                                                       | 361 ms: 1.51x faster                                                 |
| async_tree_none         | 452 ms                                                       | 304 ms: 1.49x faster                                                 |
| async_tree_cpu_io_mixed | 696 ms                                                       | 529 ms: 1.32x faster                                                 |
| Geometric mean          | (ref)                                                        | 1.51x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 65.5 ms: 1.17x faster                                                |
| pidigits       | 265 ms                                                       | 246 ms: 1.08x faster                                                 |
| nbody          | 88.0 ms                                                      | 102 ms: 1.16x slower                                                 |
| Geometric mean | (ref)                                                        | 1.03x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.30 ms: 1.08x faster                                                |
| regex_dna      | 239 ms                                                       | 233 ms: 1.03x faster                                                 |
| regex_v8       | 23.6 ms                                                      | 23.1 ms: 1.02x faster                                                |
| regex_compile  | 144 ms                                                       | 157 ms: 1.09x slower                                                 |
| Geometric mean | (ref)                                                        | 1.01x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle               | 10.5 us                                                      | 9.64 us: 1.09x faster                                                |
| xml_etree_parse      | 144 ms                                                       | 137 ms: 1.05x faster                                                 |
| xml_etree_generate   | 86.1 ms                                                      | 85.4 ms: 1.01x faster                                                |
| pickle_dict          | 32.5 us                                                      | 32.7 us: 1.00x slower                                                |
| pickle_list          | 4.43 us                                                      | 4.46 us: 1.01x slower                                                |
| pickle_pure_python   | 318 us                                                       | 329 us: 1.03x slower                                                 |
| unpickle             | 14.8 us                                                      | 15.8 us: 1.07x slower                                                |
| unpickle_list        | 4.66 us                                                      | 5.01 us: 1.08x slower                                                |
| xml_etree_process    | 58.4 ms                                                      | 62.8 ms: 1.08x slower                                                |
| unpickle_pure_python | 210 us                                                       | 233 us: 1.11x slower                                                 |
| json_dumps           | 10.2 ms                                                      | 11.4 ms: 1.12x slower                                                |
| tomli_loads          | 2.16 sec                                                     | 2.49 sec: 1.16x slower                                               |
| xml_etree_iterparse  | 103 ms                                                       | 126 ms: 1.23x slower                                                 |
| json_loads           | 24.4 us                                                      | 32.3 us: 1.33x slower                                                |
| Geometric mean       | (ref)                                                        | 1.07x slower                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 8.45 ms: 1.02x faster                                                |
| python_startup         | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                                |
| Geometric mean         | (ref)                                                        | 1.02x faster                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 40.6 ms: 1.06x slower                                                |
| mako            | 10.0 ms                                                      | 14.9 ms: 1.49x slower                                                |
| Geometric mean  | (ref)                                                        | 1.26x slower                                                         |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911 |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_io            | 1.04 sec                                                     | 595 ms: 1.75x faster                                                 |
| async_tree_memoization   | 544 ms                                                       | 361 ms: 1.51x faster                                                 |
| async_tree_none          | 452 ms                                                       | 304 ms: 1.49x faster                                                 |
| async_tree_cpu_io_mixed  | 696 ms                                                       | 529 ms: 1.32x faster                                                 |
| float                    | 76.6 ms                                                      | 65.5 ms: 1.17x faster                                                |
| async_generators         | 390 ms                                                       | 335 ms: 1.16x faster                                                 |
| gc_traversal             | 3.48 ms                                                      | 3.08 ms: 1.13x faster                                                |
| pickle                   | 10.5 us                                                      | 9.64 us: 1.09x faster                                                |
| regex_effbot             | 3.57 ms                                                      | 3.30 ms: 1.08x faster                                                |
| pidigits                 | 265 ms                                                       | 246 ms: 1.08x faster                                                 |
| xml_etree_parse          | 144 ms                                                       | 137 ms: 1.05x faster                                                 |
| regex_dna                | 239 ms                                                       | 233 ms: 1.03x faster                                                 |
| regex_v8                 | 23.6 ms                                                      | 23.1 ms: 1.02x faster                                                |
| python_startup_no_site   | 8.64 ms                                                      | 8.45 ms: 1.02x faster                                                |
| unpack_sequence          | 53.2 ns                                                      | 52.4 ns: 1.01x faster                                                |
| python_startup           | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                                |
| pycparser                | 1.23 sec                                                     | 1.22 sec: 1.01x faster                                               |
| xml_etree_generate       | 86.1 ms                                                      | 85.4 ms: 1.01x faster                                                |
| pickle_dict              | 32.5 us                                                      | 32.7 us: 1.00x slower                                                |
| pickle_list              | 4.43 us                                                      | 4.46 us: 1.01x slower                                                |
| dulwich_log              | 65.4 ms                                                      | 67.2 ms: 1.03x slower                                                |
| pickle_pure_python       | 318 us                                                       | 329 us: 1.03x slower                                                 |
| sqlite_synth             | 2.77 us                                                      | 2.88 us: 1.04x slower                                                |
| sqlglot_optimize         | 57.5 ms                                                      | 59.9 ms: 1.04x slower                                                |
| docutils                 | 2.87 sec                                                     | 2.99 sec: 1.04x slower                                               |
| telco                    | 6.96 ms                                                      | 7.29 ms: 1.05x slower                                                |
| logging_silent           | 94.4 ns                                                      | 99.0 ns: 1.05x slower                                                |
| pathlib                  | 18.9 ms                                                      | 19.8 ms: 1.05x slower                                                |
| asyncio_tcp              | 378 ms                                                       | 399 ms: 1.06x slower                                                 |
| django_template          | 38.2 ms                                                      | 40.6 ms: 1.06x slower                                                |
| 2to3                     | 285 ms                                                       | 303 ms: 1.06x slower                                                 |
| sqlglot_normalize        | 116 ms                                                       | 123 ms: 1.06x slower                                                 |
| unpickle                 | 14.8 us                                                      | 15.8 us: 1.07x slower                                                |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.70 sec: 1.07x slower                                               |
| scimark_sor              | 109 ms                                                       | 117 ms: 1.07x slower                                                 |
| unpickle_list            | 4.66 us                                                      | 5.01 us: 1.08x slower                                                |
| xml_etree_process        | 58.4 ms                                                      | 62.8 ms: 1.08x slower                                                |
| pprint_safe_repr         | 807 ms                                                       | 871 ms: 1.08x slower                                                 |
| scimark_fft              | 301 ms                                                       | 327 ms: 1.09x slower                                                 |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.58 ms: 1.09x slower                                                |
| regex_compile            | 144 ms                                                       | 157 ms: 1.09x slower                                                 |
| logging_format           | 7.48 us                                                      | 8.16 us: 1.09x slower                                                |
| logging_simple           | 6.71 us                                                      | 7.32 us: 1.09x slower                                                |
| pprint_pformat           | 1.65 sec                                                     | 1.81 sec: 1.09x slower                                               |
| deepcopy                 | 368 us                                                       | 403 us: 1.09x slower                                                 |
| scimark_lu               | 98.8 ms                                                      | 108 ms: 1.09x slower                                                 |
| mdp                      | 2.57 sec                                                     | 2.82 sec: 1.10x slower                                               |
| pyflate                  | 439 ms                                                       | 482 ms: 1.10x slower                                                 |
| sympy_integrate          | 23.9 ms                                                      | 26.4 ms: 1.11x slower                                                |
| crypto_pyaes             | 80.3 ms                                                      | 88.9 ms: 1.11x slower                                                |
| deepcopy_reduce          | 3.37 us                                                      | 3.74 us: 1.11x slower                                                |
| nqueens                  | 89.9 ms                                                      | 99.8 ms: 1.11x slower                                                |
| unpickle_pure_python     | 210 us                                                       | 233 us: 1.11x slower                                                 |
| deepcopy_memo            | 36.8 us                                                      | 41.0 us: 1.11x slower                                                |
| json_dumps               | 10.2 ms                                                      | 11.4 ms: 1.12x slower                                                |
| go                       | 150 ms                                                       | 169 ms: 1.13x slower                                                 |
| sympy_str                | 302 ms                                                       | 344 ms: 1.14x slower                                                 |
| spectral_norm            | 91.6 ms                                                      | 105 ms: 1.14x slower                                                 |
| tomli_loads              | 2.16 sec                                                     | 2.49 sec: 1.16x slower                                               |
| nbody                    | 88.0 ms                                                      | 102 ms: 1.16x slower                                                 |
| chameleon                | 7.23 ms                                                      | 8.37 ms: 1.16x slower                                                |
| sympy_expand             | 484 ms                                                       | 562 ms: 1.16x slower                                                 |
| richards                 | 45.7 ms                                                      | 53.5 ms: 1.17x slower                                                |
| sqlglot_transpile        | 1.78 ms                                                      | 2.08 ms: 1.17x slower                                                |
| hexiom                   | 5.96 ms                                                      | 7.01 ms: 1.18x slower                                                |
| sympy_sum                | 162 ms                                                       | 191 ms: 1.18x slower                                                 |
| meteor_contest           | 128 ms                                                       | 153 ms: 1.19x slower                                                 |
| scimark_monte_carlo      | 69.0 ms                                                      | 82.9 ms: 1.20x slower                                                |
| create_gc_cycles         | 1.59 ms                                                      | 1.93 ms: 1.21x slower                                                |
| chaos                    | 64.0 ms                                                      | 77.8 ms: 1.22x slower                                                |
| coroutines               | 23.0 ms                                                      | 28.1 ms: 1.22x slower                                                |
| xml_etree_iterparse      | 103 ms                                                       | 126 ms: 1.23x slower                                                 |
| json                     | 5.12 ms                                                      | 6.28 ms: 1.23x slower                                                |
| deltablue                | 3.24 ms                                                      | 4.00 ms: 1.24x slower                                                |
| sqlglot_parse            | 1.38 ms                                                      | 1.73 ms: 1.26x slower                                                |
| raytrace                 | 298 ms                                                       | 376 ms: 1.26x slower                                                 |
| fannkuch                 | 350 ms                                                       | 447 ms: 1.28x slower                                                 |
| richards_super           | 51.3 ms                                                      | 66.5 ms: 1.30x slower                                                |
| json_loads               | 24.4 us                                                      | 32.3 us: 1.33x slower                                                |
| comprehensions           | 21.9 us                                                      | 29.6 us: 1.35x slower                                                |
| coverage                 | 66.7 ms                                                      | 97.6 ms: 1.46x slower                                                |
| mako                     | 10.0 ms                                                      | 14.9 ms: 1.49x slower                                                |
| bench_mp_pool            | 4.76 ms                                                      | 7.77 ms: 1.63x slower                                                |
| generators               | 37.4 ms                                                      | 62.3 ms: 1.67x slower                                                |
| bench_thread_pool        | 950 us                                                       | 2.03 ms: 2.13x slower                                                |
| typing_runtime_protocols | 152 us                                                       | 575 us: 3.79x slower                                                 |
| Geometric mean           | (ref)                                                        | 1.11x slower                                                         |
Ignored benchmarks (12) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, dask, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
Ignored benchmarks (4) of results/bm-20230427-3.12.0a4-d595911/bm-20230427-pythonperf2-x86_64-mdboom-nogil_d595911-3.12.0a4-d595911.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.07x
- 95% likely to have a slowdown of 1.07x
- 99% likely to have a slowdown of 1.06x


# Memory

- memory change: 1.21x