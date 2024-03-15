# Results vs. base

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 277 ms: 1.05x slower                                           |
| chameleon      | 6.94 ms                                                                | 7.09 ms: 1.02x slower                                          |
| docutils       | 2.64 sec                                                               | 2.68 sec: 1.01x slower                                         |
| tornado_http   | 94.4 ms                                                                | 97.7 ms: 1.03x slower                                          |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_io_tg           | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                         |
| async_tree_cpu_io_mixed_tg | 718 ms                                                                 | 728 ms: 1.01x slower                                           |
| async_tree_memoization_tg  | 572 ms                                                                 | 580 ms: 1.01x slower                                           |
| async_tree_cpu_io_mixed    | 703 ms                                                                 | 717 ms: 1.02x slower                                           |
| async_tree_io              | 1.17 sec                                                               | 1.19 sec: 1.02x slower                                         |
| async_tree_none_tg         | 439 ms                                                                 | 448 ms: 1.02x slower                                           |
| async_tree_memoization     | 557 ms                                                                 | 569 ms: 1.02x slower                                           |
| async_tree_none            | 434 ms                                                                 | 446 ms: 1.03x slower                                           |
| Geometric mean             | (ref)                                                                  | 1.02x slower                                                   |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 187 ms                                                                 | 188 ms: 1.00x slower                                           |
| float          | 80.7 ms                                                                | 88.1 ms: 1.09x slower                                          |
| nbody          | 88.9 ms                                                                | 106 ms: 1.20x slower                                           |
| Geometric mean | (ref)                                                                  | 1.09x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 222 ms                                                                 | 213 ms: 1.05x faster                                           |
| regex_effbot   | 3.58 ms                                                                | 3.69 ms: 1.03x slower                                          |
| regex_compile  | 129 ms                                                                 | 142 ms: 1.10x slower                                           |
| regex_v8       | 23.5 ms                                                                | 26.1 ms: 1.11x slower                                          |
| Geometric mean | (ref)                                                                  | 1.05x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| xml_etree_generate   | 88.2 ms                                                                | 86.8 ms: 1.02x faster                                          |
| xml_etree_process    | 59.7 ms                                                                | 59.0 ms: 1.01x faster                                          |
| unpickle             | 14.7 us                                                                | 14.6 us: 1.01x faster                                          |
| pickle_pure_python   | 297 us                                                                 | 301 us: 1.01x slower                                           |
| pickle               | 11.4 us                                                                | 11.6 us: 1.01x slower                                          |
| unpickle_list        | 5.02 us                                                                | 5.13 us: 1.02x slower                                          |
| pickle_dict          | 33.9 us                                                                | 35.4 us: 1.04x slower                                          |
| xml_etree_iterparse  | 104 ms                                                                 | 109 ms: 1.04x slower                                           |
| tomli_loads          | 2.14 sec                                                               | 2.25 sec: 1.05x slower                                         |
| unpickle_pure_python | 216 us                                                                 | 228 us: 1.06x slower                                           |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (4): json_dumps, json_loads, pickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.02x slower                                          |
| python_startup_no_site | 8.72 ms                                                                | 8.87 ms: 1.02x slower                                          |
| Geometric mean         | (ref)                                                                  | 1.02x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 11.5 ms                                                                | 12.7 ms: 1.11x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231218-linux-x86_64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-linux-x86_64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna                  | 222 ms                                                                 | 213 ms: 1.05x faster                                           |
| richards                   | 47.4 ms                                                                | 46.3 ms: 1.02x faster                                          |
| deepcopy_reduce            | 3.11 us                                                                | 3.04 us: 1.02x faster                                          |
| richards_super             | 53.9 ms                                                                | 52.7 ms: 1.02x faster                                          |
| pycparser                  | 1.20 sec                                                               | 1.17 sec: 1.02x faster                                         |
| xml_etree_generate         | 88.2 ms                                                                | 86.8 ms: 1.02x faster                                          |
| coverage                   | 96.8 ms                                                                | 95.4 ms: 1.01x faster                                          |
| xml_etree_process          | 59.7 ms                                                                | 59.0 ms: 1.01x faster                                          |
| unpickle                   | 14.7 us                                                                | 14.6 us: 1.01x faster                                          |
| coroutines                 | 22.6 ms                                                                | 22.5 ms: 1.00x faster                                          |
| pidigits                   | 187 ms                                                                 | 188 ms: 1.00x slower                                           |
| deepcopy                   | 347 us                                                                 | 349 us: 1.00x slower                                           |
| create_gc_cycles           | 1.47 ms                                                                | 1.48 ms: 1.00x slower                                          |
| generators                 | 28.6 ms                                                                | 28.8 ms: 1.01x slower                                          |
| scimark_lu                 | 113 ms                                                                 | 115 ms: 1.01x slower                                           |
| async_tree_io_tg           | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                         |
| pickle_pure_python         | 297 us                                                                 | 301 us: 1.01x slower                                           |
| docutils                   | 2.64 sec                                                               | 2.68 sec: 1.01x slower                                         |
| logging_silent             | 102 ns                                                                 | 103 ns: 1.01x slower                                           |
| pickle                     | 11.4 us                                                                | 11.6 us: 1.01x slower                                          |
| async_tree_cpu_io_mixed_tg | 718 ms                                                                 | 728 ms: 1.01x slower                                           |
| async_tree_memoization_tg  | 572 ms                                                                 | 580 ms: 1.01x slower                                           |
| deepcopy_memo              | 37.6 us                                                                | 38.1 us: 1.01x slower                                          |
| python_startup             | 10.1 ms                                                                | 10.2 ms: 1.02x slower                                          |
| asyncio_tcp_ssl            | 1.78 sec                                                               | 1.81 sec: 1.02x slower                                         |
| telco                      | 8.35 ms                                                                | 8.50 ms: 1.02x slower                                          |
| pathlib                    | 18.1 ms                                                                | 18.4 ms: 1.02x slower                                          |
| dask                       | 360 ms                                                                 | 366 ms: 1.02x slower                                           |
| bench_thread_pool          | 828 us                                                                 | 843 us: 1.02x slower                                           |
| python_startup_no_site     | 8.72 ms                                                                | 8.87 ms: 1.02x slower                                          |
| async_tree_cpu_io_mixed    | 703 ms                                                                 | 717 ms: 1.02x slower                                           |
| async_tree_io              | 1.17 sec                                                               | 1.19 sec: 1.02x slower                                         |
| async_tree_none_tg         | 439 ms                                                                 | 448 ms: 1.02x slower                                           |
| meteor_contest             | 108 ms                                                                 | 110 ms: 1.02x slower                                           |
| async_tree_memoization     | 557 ms                                                                 | 569 ms: 1.02x slower                                           |
| chameleon                  | 6.94 ms                                                                | 7.09 ms: 1.02x slower                                          |
| unpickle_list              | 5.02 us                                                                | 5.13 us: 1.02x slower                                          |
| logging_simple             | 5.70 us                                                                | 5.83 us: 1.02x slower                                          |
| json                       | 5.05 ms                                                                | 5.17 ms: 1.02x slower                                          |
| gc_traversal               | 3.67 ms                                                                | 3.77 ms: 1.03x slower                                          |
| logging_format             | 6.28 us                                                                | 6.45 us: 1.03x slower                                          |
| async_tree_none            | 434 ms                                                                 | 446 ms: 1.03x slower                                           |
| typing_runtime_protocols   | 110 us                                                                 | 113 us: 1.03x slower                                           |
| asyncio_tcp                | 482 ms                                                                 | 496 ms: 1.03x slower                                           |
| sqlglot_transpile          | 1.57 ms                                                                | 1.62 ms: 1.03x slower                                          |
| regex_effbot               | 3.58 ms                                                                | 3.69 ms: 1.03x slower                                          |
| sqlglot_parse              | 1.25 ms                                                                | 1.29 ms: 1.03x slower                                          |
| mdp                        | 2.53 sec                                                               | 2.61 sec: 1.03x slower                                         |
| tornado_http               | 94.4 ms                                                                | 97.7 ms: 1.03x slower                                          |
| async_generators           | 444 ms                                                                 | 460 ms: 1.04x slower                                           |
| unpack_sequence            | 46.8 ns                                                                | 48.5 ns: 1.04x slower                                          |
| dulwich_log                | 65.5 ms                                                                | 68.0 ms: 1.04x slower                                          |
| pickle_dict                | 33.9 us                                                                | 35.4 us: 1.04x slower                                          |
| xml_etree_iterparse        | 104 ms                                                                 | 109 ms: 1.04x slower                                           |
| sqlglot_normalize          | 106 ms                                                                 | 111 ms: 1.05x slower                                           |
| sqlglot_optimize           | 53.5 ms                                                                | 56.2 ms: 1.05x slower                                          |
| tomli_loads                | 2.14 sec                                                               | 2.25 sec: 1.05x slower                                         |
| 2to3                       | 263 ms                                                                 | 277 ms: 1.05x slower                                           |
| unpickle_pure_python       | 216 us                                                                 | 228 us: 1.06x slower                                           |
| sympy_expand               | 457 ms                                                                 | 483 ms: 1.06x slower                                           |
| scimark_fft                | 367 ms                                                                 | 391 ms: 1.07x slower                                           |
| sympy_str                  | 269 ms                                                                 | 290 ms: 1.08x slower                                           |
| sympy_sum                  | 149 ms                                                                 | 162 ms: 1.08x slower                                           |
| sympy_integrate            | 19.5 ms                                                                | 21.2 ms: 1.09x slower                                          |
| raytrace                   | 259 ms                                                                 | 282 ms: 1.09x slower                                           |
| fannkuch                   | 402 ms                                                                 | 438 ms: 1.09x slower                                           |
| scimark_sor                | 120 ms                                                                 | 131 ms: 1.09x slower                                           |
| float                      | 80.7 ms                                                                | 88.1 ms: 1.09x slower                                          |
| regex_compile              | 129 ms                                                                 | 142 ms: 1.10x slower                                           |
| scimark_monte_carlo        | 68.0 ms                                                                | 75.1 ms: 1.11x slower                                          |
| pprint_safe_repr           | 729 ms                                                                 | 807 ms: 1.11x slower                                           |
| regex_v8                   | 23.5 ms                                                                | 26.1 ms: 1.11x slower                                          |
| go                         | 137 ms                                                                 | 152 ms: 1.11x slower                                           |
| mako                       | 11.5 ms                                                                | 12.7 ms: 1.11x slower                                          |
| pyflate                    | 448 ms                                                                 | 504 ms: 1.13x slower                                           |
| pprint_pformat             | 1.48 sec                                                               | 1.68 sec: 1.13x slower                                         |
| crypto_pyaes               | 71.7 ms                                                                | 81.4 ms: 1.14x slower                                          |
| nqueens                    | 79.8 ms                                                                | 91.2 ms: 1.14x slower                                          |
| scimark_sparse_mat_mult    | 4.92 ms                                                                | 5.72 ms: 1.16x slower                                          |
| chaos                      | 59.7 ms                                                                | 70.6 ms: 1.18x slower                                          |
| nbody                      | 88.9 ms                                                                | 106 ms: 1.20x slower                                           |
| comprehensions             | 16.1 us                                                                | 19.8 us: 1.23x slower                                          |
| spectral_norm              | 111 ms                                                                 | 141 ms: 1.27x slower                                           |
| deltablue                  | 3.19 ms                                                                | 4.07 ms: 1.27x slower                                          |
| hexiom                     | 6.05 ms                                                                | 8.11 ms: 1.34x slower                                          |
| Geometric mean             | (ref)                                                                  | 1.05x slower                                                   |

Benchmark hidden because not significant (8): json_dumps, json_loads, bench_mp_pool, asyncio_websockets, pickle_list, xml_etree_parse, sqlite_synth, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.04x