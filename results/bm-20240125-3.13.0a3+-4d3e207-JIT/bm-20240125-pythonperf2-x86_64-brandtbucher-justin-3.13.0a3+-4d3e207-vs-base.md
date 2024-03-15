# Results vs. base

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 292 ms                                                                       | 299 ms: 1.02x slower                                                 |
| chameleon      | 7.10 ms                                                                      | 7.53 ms: 1.06x slower                                                |
| docutils       | 2.84 sec                                                                     | 2.88 sec: 1.01x slower                                               |
| tornado_http   | 122 ms                                                                       | 124 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                                        | 1.03x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|--------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none_tg | 430 ms                                                                       | 435 ms: 1.01x slower                                                 |
| Geometric mean     | (ref)                                                                        | 1.00x slower                                                         |

Benchmark hidden because not significant (7): async_tree_io, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_io_tg, async_tree_cpu_io_mixed_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 265 ms                                                                       | 263 ms: 1.01x faster                                                 |
| float          | 78.7 ms                                                                      | 82.4 ms: 1.05x slower                                                |
| nbody          | 85.4 ms                                                                      | 107 ms: 1.25x slower                                                 |
| Geometric mean | (ref)                                                                        | 1.09x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_v8       | 26.7 ms                                                                      | 26.7 ms: 1.00x slower                                                |
| regex_effbot   | 3.49 ms                                                                      | 3.57 ms: 1.02x slower                                                |
| regex_dna      | 236 ms                                                                       | 246 ms: 1.04x slower                                                 |
| regex_compile  | 141 ms                                                                       | 147 ms: 1.05x slower                                                 |
| Geometric mean | (ref)                                                                        | 1.03x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| xml_etree_iterparse  | 108 ms                                                                       | 105 ms: 1.02x faster                                                 |
| xml_etree_parse      | 147 ms                                                                       | 144 ms: 1.02x faster                                                 |
| pickle_pure_python   | 313 us                                                                       | 310 us: 1.01x faster                                                 |
| json_loads           | 24.9 us                                                                      | 24.8 us: 1.01x faster                                                |
| json_dumps           | 10.8 ms                                                                      | 10.7 ms: 1.00x faster                                                |
| xml_etree_generate   | 84.7 ms                                                                      | 84.9 ms: 1.00x slower                                                |
| pickle_dict          | 31.2 us                                                                      | 31.4 us: 1.01x slower                                                |
| tomli_loads          | 2.26 sec                                                                     | 2.30 sec: 1.02x slower                                               |
| pickle               | 10.3 us                                                                      | 10.6 us: 1.03x slower                                                |
| unpickle_list        | 4.87 us                                                                      | 5.09 us: 1.05x slower                                                |
| unpickle             | 14.7 us                                                                      | 15.5 us: 1.05x slower                                                |
| unpickle_pure_python | 221 us                                                                       | 235 us: 1.07x slower                                                 |
| Geometric mean       | (ref)                                                                        | 1.01x slower                                                         |

Benchmark hidden because not significant (2): pickle_list, xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 12.6 ms                                                                      | 12.6 ms: 1.00x faster                                                |
| python_startup_no_site | 11.1 ms                                                                      | 11.0 ms: 1.00x faster                                                |
| Geometric mean         | (ref)                                                                        | 1.00x faster                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 10.3 ms                                                                      | 11.9 ms: 1.16x slower                                                |

All benchmarks:
===============

| Benchmark                | bm-20240126-pythonperf2-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|--------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| unpack_sequence          | 52.2 ns                                                                      | 42.9 ns: 1.22x faster                                                |
| create_gc_cycles         | 1.63 ms                                                                      | 1.53 ms: 1.07x faster                                                |
| richards                 | 54.3 ms                                                                      | 50.9 ms: 1.07x faster                                                |
| gc_traversal             | 3.56 ms                                                                      | 3.43 ms: 1.04x faster                                                |
| xml_etree_iterparse      | 108 ms                                                                       | 105 ms: 1.02x faster                                                 |
| xml_etree_parse          | 147 ms                                                                       | 144 ms: 1.02x faster                                                 |
| generators               | 34.4 ms                                                                      | 33.7 ms: 1.02x faster                                                |
| richards_super           | 59.5 ms                                                                      | 58.4 ms: 1.02x faster                                                |
| scimark_sor              | 145 ms                                                                       | 142 ms: 1.02x faster                                                 |
| dulwich_log              | 68.6 ms                                                                      | 67.9 ms: 1.01x faster                                                |
| pickle_pure_python       | 313 us                                                                       | 310 us: 1.01x faster                                                 |
| sqlglot_parse            | 1.39 ms                                                                      | 1.38 ms: 1.01x faster                                                |
| asyncio_tcp              | 369 ms                                                                       | 367 ms: 1.01x faster                                                 |
| pidigits                 | 265 ms                                                                       | 263 ms: 1.01x faster                                                 |
| json_loads               | 24.9 us                                                                      | 24.8 us: 1.01x faster                                                |
| json_dumps               | 10.8 ms                                                                      | 10.7 ms: 1.00x faster                                                |
| python_startup           | 12.6 ms                                                                      | 12.6 ms: 1.00x faster                                                |
| python_startup_no_site   | 11.1 ms                                                                      | 11.0 ms: 1.00x faster                                                |
| regex_v8                 | 26.7 ms                                                                      | 26.7 ms: 1.00x slower                                                |
| xml_etree_generate       | 84.7 ms                                                                      | 84.9 ms: 1.00x slower                                                |
| json                     | 5.22 ms                                                                      | 5.24 ms: 1.00x slower                                                |
| logging_silent           | 96.2 ns                                                                      | 96.7 ns: 1.01x slower                                                |
| sqlite_synth             | 2.74 us                                                                      | 2.75 us: 1.01x slower                                                |
| pickle_dict              | 31.2 us                                                                      | 31.4 us: 1.01x slower                                                |
| deepcopy                 | 364 us                                                                       | 368 us: 1.01x slower                                                 |
| pathlib                  | 18.6 ms                                                                      | 18.8 ms: 1.01x slower                                                |
| async_tree_none_tg       | 430 ms                                                                       | 435 ms: 1.01x slower                                                 |
| tornado_http             | 122 ms                                                                       | 124 ms: 1.01x slower                                                 |
| docutils                 | 2.84 sec                                                                     | 2.88 sec: 1.01x slower                                               |
| deepcopy_memo            | 37.3 us                                                                      | 37.8 us: 1.02x slower                                                |
| asyncio_tcp_ssl          | 1.57 sec                                                                     | 1.60 sec: 1.02x slower                                               |
| dask                     | 397 ms                                                                       | 403 ms: 1.02x slower                                                 |
| tomli_loads              | 2.26 sec                                                                     | 2.30 sec: 1.02x slower                                               |
| sympy_expand             | 491 ms                                                                       | 501 ms: 1.02x slower                                                 |
| scimark_lu               | 99.4 ms                                                                      | 102 ms: 1.02x slower                                                 |
| regex_effbot             | 3.49 ms                                                                      | 3.57 ms: 1.02x slower                                                |
| 2to3                     | 292 ms                                                                       | 299 ms: 1.02x slower                                                 |
| meteor_contest           | 129 ms                                                                       | 133 ms: 1.03x slower                                                 |
| sqlglot_normalize        | 115 ms                                                                       | 118 ms: 1.03x slower                                                 |
| pickle                   | 10.3 us                                                                      | 10.6 us: 1.03x slower                                                |
| sympy_str                | 290 ms                                                                       | 298 ms: 1.03x slower                                                 |
| coroutines               | 22.2 ms                                                                      | 23.0 ms: 1.03x slower                                                |
| bench_thread_pool        | 948 us                                                                       | 982 us: 1.04x slower                                                 |
| pyflate                  | 522 ms                                                                       | 542 ms: 1.04x slower                                                 |
| go                       | 171 ms                                                                       | 178 ms: 1.04x slower                                                 |
| typing_runtime_protocols | 115 us                                                                       | 119 us: 1.04x slower                                                 |
| telco                    | 8.06 ms                                                                      | 8.37 ms: 1.04x slower                                                |
| mdp                      | 2.46 sec                                                                     | 2.56 sec: 1.04x slower                                               |
| regex_dna                | 236 ms                                                                       | 246 ms: 1.04x slower                                                 |
| float                    | 78.7 ms                                                                      | 82.4 ms: 1.05x slower                                                |
| unpickle_list            | 4.87 us                                                                      | 5.09 us: 1.05x slower                                                |
| regex_compile            | 141 ms                                                                       | 147 ms: 1.05x slower                                                 |
| sqlglot_optimize         | 58.3 ms                                                                      | 61.0 ms: 1.05x slower                                                |
| sympy_integrate          | 23.1 ms                                                                      | 24.3 ms: 1.05x slower                                                |
| unpickle                 | 14.7 us                                                                      | 15.5 us: 1.05x slower                                                |
| sympy_sum                | 151 ms                                                                       | 159 ms: 1.06x slower                                                 |
| chameleon                | 7.10 ms                                                                      | 7.53 ms: 1.06x slower                                                |
| unpickle_pure_python     | 221 us                                                                       | 235 us: 1.07x slower                                                 |
| pprint_safe_repr         | 806 ms                                                                       | 864 ms: 1.07x slower                                                 |
| fannkuch                 | 390 ms                                                                       | 418 ms: 1.07x slower                                                 |
| raytrace                 | 259 ms                                                                       | 278 ms: 1.08x slower                                                 |
| coverage                 | 81.5 ms                                                                      | 88.0 ms: 1.08x slower                                                |
| pprint_pformat           | 1.65 sec                                                                     | 1.80 sec: 1.09x slower                                               |
| bench_mp_pool            | 4.64 ms                                                                      | 5.07 ms: 1.09x slower                                                |
| nqueens                  | 88.0 ms                                                                      | 98.5 ms: 1.12x slower                                                |
| deltablue                | 3.53 ms                                                                      | 3.99 ms: 1.13x slower                                                |
| mako                     | 10.3 ms                                                                      | 11.9 ms: 1.16x slower                                                |
| crypto_pyaes             | 70.8 ms                                                                      | 82.9 ms: 1.17x slower                                                |
| chaos                    | 60.0 ms                                                                      | 70.7 ms: 1.18x slower                                                |
| scimark_monte_carlo      | 66.5 ms                                                                      | 79.3 ms: 1.19x slower                                                |
| scimark_fft              | 306 ms                                                                       | 368 ms: 1.20x slower                                                 |
| hexiom                   | 6.43 ms                                                                      | 7.91 ms: 1.23x slower                                                |
| scimark_sparse_mat_mult  | 4.21 ms                                                                      | 5.24 ms: 1.24x slower                                                |
| nbody                    | 85.4 ms                                                                      | 107 ms: 1.25x slower                                                 |
| comprehensions           | 16.6 us                                                                      | 20.8 us: 1.25x slower                                                |
| spectral_norm            | 90.7 ms                                                                      | 116 ms: 1.28x slower                                                 |
| Geometric mean           | (ref)                                                                        | 1.04x slower                                                         |

Benchmark hidden because not significant (17): async_tree_io, asyncio_websockets, pickle_list, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_memoization_tg, xml_etree_process, logging_format, logging_simple, deepcopy_reduce, sqlglot_transpile, async_tree_io_tg, async_generators, pycparser, async_tree_cpu_io_mixed_tg, async_tree_none, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.04x