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

| Benchmark      | bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 276 ms: 1.05x slower                                           |
| chameleon      | 6.84 ms                                                                | 6.96 ms: 1.02x slower                                          |
| docutils       | 2.59 sec                                                               | 2.66 sec: 1.03x slower                                         |
| tornado_http   | 94.5 ms                                                                | 97.4 ms: 1.03x slower                                          |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 720 ms                                                                 | 728 ms: 1.01x slower                                           |
| async_tree_io_tg           | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                         |
| async_tree_none_tg         | 446 ms                                                                 | 453 ms: 1.02x slower                                           |
| async_tree_io              | 1.17 sec                                                               | 1.19 sec: 1.02x slower                                         |
| async_tree_cpu_io_mixed    | 703 ms                                                                 | 715 ms: 1.02x slower                                           |
| async_tree_memoization     | 557 ms                                                                 | 572 ms: 1.03x slower                                           |
| async_tree_memoization_tg  | 572 ms                                                                 | 589 ms: 1.03x slower                                           |
| async_tree_none            | 433 ms                                                                 | 446 ms: 1.03x slower                                           |
| Geometric mean             | (ref)                                                                  | 1.02x slower                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 187 ms                                                                 | 188 ms: 1.00x slower                                           |
| float          | 79.9 ms                                                                | 87.1 ms: 1.09x slower                                          |
| nbody          | 89.4 ms                                                                | 104 ms: 1.16x slower                                           |
| Geometric mean | (ref)                                                                  | 1.08x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 225 ms                                                                 | 220 ms: 1.02x faster                                           |
| regex_effbot   | 3.68 ms                                                                | 3.62 ms: 1.01x faster                                          |
| regex_v8       | 24.7 ms                                                                | 25.5 ms: 1.03x slower                                          |
| regex_compile  | 129 ms                                                                 | 141 ms: 1.10x slower                                           |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_dict          | 34.4 us                                                                | 34.0 us: 1.01x faster                                          |
| json_dumps           | 10.4 ms                                                                | 10.3 ms: 1.01x faster                                          |
| xml_etree_parse      | 157 ms                                                                 | 158 ms: 1.01x slower                                           |
| xml_etree_process    | 58.6 ms                                                                | 59.4 ms: 1.01x slower                                          |
| pickle_list          | 5.15 us                                                                | 5.23 us: 1.02x slower                                          |
| tomli_loads          | 2.16 sec                                                               | 2.20 sec: 1.02x slower                                         |
| pickle               | 11.5 us                                                                | 11.7 us: 1.02x slower                                          |
| xml_etree_generate   | 85.4 ms                                                                | 87.9 ms: 1.03x slower                                          |
| unpickle             | 14.9 us                                                                | 15.5 us: 1.04x slower                                          |
| xml_etree_iterparse  | 105 ms                                                                 | 109 ms: 1.04x slower                                           |
| unpickle_pure_python | 212 us                                                                 | 229 us: 1.08x slower                                           |
| Geometric mean       | (ref)                                                                  | 1.02x slower                                                   |

Benchmark hidden because not significant (3): pickle_pure_python, json_loads, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                          |
| python_startup_no_site | 8.71 ms                                                                | 8.82 ms: 1.01x slower                                          |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 10.9 ms                                                                | 12.7 ms: 1.16x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20240126-linux-x86_64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-linux-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| gc_traversal               | 3.99 ms                                                                | 3.77 ms: 1.06x faster                                          |
| richards_super             | 54.4 ms                                                                | 51.9 ms: 1.05x faster                                          |
| richards                   | 48.2 ms                                                                | 46.0 ms: 1.05x faster                                          |
| mdp                        | 2.69 sec                                                               | 2.64 sec: 1.02x faster                                         |
| regex_dna                  | 225 ms                                                                 | 220 ms: 1.02x faster                                           |
| regex_effbot               | 3.68 ms                                                                | 3.62 ms: 1.01x faster                                          |
| pickle_dict                | 34.4 us                                                                | 34.0 us: 1.01x faster                                          |
| coverage                   | 95.1 ms                                                                | 94.1 ms: 1.01x faster                                          |
| sqlite_synth               | 2.86 us                                                                | 2.84 us: 1.01x faster                                          |
| json_dumps                 | 10.4 ms                                                                | 10.3 ms: 1.01x faster                                          |
| generators                 | 29.5 ms                                                                | 29.2 ms: 1.01x faster                                          |
| deepcopy_reduce            | 3.11 us                                                                | 3.09 us: 1.01x faster                                          |
| pidigits                   | 187 ms                                                                 | 188 ms: 1.00x slower                                           |
| xml_etree_parse            | 157 ms                                                                 | 158 ms: 1.01x slower                                           |
| asyncio_tcp_ssl            | 1.78 sec                                                               | 1.79 sec: 1.01x slower                                         |
| python_startup             | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                          |
| async_tree_cpu_io_mixed_tg | 720 ms                                                                 | 728 ms: 1.01x slower                                           |
| python_startup_no_site     | 8.71 ms                                                                | 8.82 ms: 1.01x slower                                          |
| xml_etree_process          | 58.6 ms                                                                | 59.4 ms: 1.01x slower                                          |
| async_tree_io_tg           | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                         |
| async_tree_none_tg         | 446 ms                                                                 | 453 ms: 1.02x slower                                           |
| dask                       | 361 ms                                                                 | 366 ms: 1.02x slower                                           |
| pickle_list                | 5.15 us                                                                | 5.23 us: 1.02x slower                                          |
| asyncio_tcp                | 482 ms                                                                 | 490 ms: 1.02x slower                                           |
| async_tree_io              | 1.17 sec                                                               | 1.19 sec: 1.02x slower                                         |
| chameleon                  | 6.84 ms                                                                | 6.96 ms: 1.02x slower                                          |
| async_tree_cpu_io_mixed    | 703 ms                                                                 | 715 ms: 1.02x slower                                           |
| deepcopy                   | 344 us                                                                 | 350 us: 1.02x slower                                           |
| coroutines                 | 22.1 ms                                                                | 22.5 ms: 1.02x slower                                          |
| tomli_loads                | 2.16 sec                                                               | 2.20 sec: 1.02x slower                                         |
| unpack_sequence            | 48.7 ns                                                                | 49.7 ns: 1.02x slower                                          |
| pickle                     | 11.5 us                                                                | 11.7 us: 1.02x slower                                          |
| telco                      | 8.34 ms                                                                | 8.54 ms: 1.02x slower                                          |
| bench_thread_pool          | 817 us                                                                 | 837 us: 1.02x slower                                           |
| docutils                   | 2.59 sec                                                               | 2.66 sec: 1.03x slower                                         |
| create_gc_cycles           | 1.46 ms                                                                | 1.50 ms: 1.03x slower                                          |
| typing_runtime_protocols   | 109 us                                                                 | 111 us: 1.03x slower                                           |
| meteor_contest             | 108 ms                                                                 | 111 ms: 1.03x slower                                           |
| sympy_str                  | 278 ms                                                                 | 285 ms: 1.03x slower                                           |
| scimark_sor                | 120 ms                                                                 | 123 ms: 1.03x slower                                           |
| async_tree_memoization     | 557 ms                                                                 | 572 ms: 1.03x slower                                           |
| xml_etree_generate         | 85.4 ms                                                                | 87.9 ms: 1.03x slower                                          |
| sqlglot_parse              | 1.25 ms                                                                | 1.28 ms: 1.03x slower                                          |
| async_tree_memoization_tg  | 572 ms                                                                 | 589 ms: 1.03x slower                                           |
| sqlglot_normalize          | 107 ms                                                                 | 110 ms: 1.03x slower                                           |
| tornado_http               | 94.5 ms                                                                | 97.4 ms: 1.03x slower                                          |
| logging_format             | 6.18 us                                                                | 6.37 us: 1.03x slower                                          |
| async_tree_none            | 433 ms                                                                 | 446 ms: 1.03x slower                                           |
| sympy_expand               | 465 ms                                                                 | 479 ms: 1.03x slower                                           |
| regex_v8                   | 24.7 ms                                                                | 25.5 ms: 1.03x slower                                          |
| sqlglot_transpile          | 1.57 ms                                                                | 1.62 ms: 1.03x slower                                          |
| logging_simple             | 5.62 us                                                                | 5.81 us: 1.03x slower                                          |
| unpickle                   | 14.9 us                                                                | 15.5 us: 1.04x slower                                          |
| dulwich_log                | 65.1 ms                                                                | 67.9 ms: 1.04x slower                                          |
| xml_etree_iterparse        | 105 ms                                                                 | 109 ms: 1.04x slower                                           |
| logging_silent             | 102 ns                                                                 | 106 ns: 1.04x slower                                           |
| deepcopy_memo              | 37.5 us                                                                | 39.2 us: 1.05x slower                                          |
| 2to3                       | 263 ms                                                                 | 276 ms: 1.05x slower                                           |
| pycparser                  | 1.15 sec                                                               | 1.20 sec: 1.05x slower                                         |
| sqlglot_optimize           | 53.9 ms                                                                | 56.5 ms: 1.05x slower                                          |
| scimark_fft                | 361 ms                                                                 | 382 ms: 1.06x slower                                           |
| fannkuch                   | 407 ms                                                                 | 433 ms: 1.06x slower                                           |
| sympy_integrate            | 19.5 ms                                                                | 20.9 ms: 1.07x slower                                          |
| sympy_sum                  | 149 ms                                                                 | 160 ms: 1.08x slower                                           |
| unpickle_pure_python       | 212 us                                                                 | 229 us: 1.08x slower                                           |
| go                         | 137 ms                                                                 | 149 ms: 1.09x slower                                           |
| float                      | 79.9 ms                                                                | 87.1 ms: 1.09x slower                                          |
| raytrace                   | 259 ms                                                                 | 282 ms: 1.09x slower                                           |
| crypto_pyaes               | 72.6 ms                                                                | 79.3 ms: 1.09x slower                                          |
| pyflate                    | 469 ms                                                                 | 513 ms: 1.09x slower                                           |
| regex_compile              | 129 ms                                                                 | 141 ms: 1.10x slower                                           |
| scimark_monte_carlo        | 67.3 ms                                                                | 74.6 ms: 1.11x slower                                          |
| scimark_sparse_mat_mult    | 4.94 ms                                                                | 5.55 ms: 1.12x slower                                          |
| pprint_safe_repr           | 731 ms                                                                 | 827 ms: 1.13x slower                                           |
| pprint_pformat             | 1.50 sec                                                               | 1.70 sec: 1.14x slower                                         |
| nqueens                    | 79.0 ms                                                                | 89.9 ms: 1.14x slower                                          |
| nbody                      | 89.4 ms                                                                | 104 ms: 1.16x slower                                           |
| mako                       | 10.9 ms                                                                | 12.7 ms: 1.16x slower                                          |
| comprehensions             | 16.3 us                                                                | 19.6 us: 1.20x slower                                          |
| chaos                      | 58.4 ms                                                                | 70.8 ms: 1.21x slower                                          |
| spectral_norm              | 112 ms                                                                 | 141 ms: 1.27x slower                                           |
| deltablue                  | 3.19 ms                                                                | 4.05 ms: 1.27x slower                                          |
| hexiom                     | 6.06 ms                                                                | 7.98 ms: 1.32x slower                                          |
| Geometric mean             | (ref)                                                                  | 1.04x slower                                                   |

Benchmark hidden because not significant (10): json, async_generators, bench_mp_pool, pathlib, asyncio_websockets, scimark_lu, pickle_pure_python, json_loads, unpickle_list, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.04x