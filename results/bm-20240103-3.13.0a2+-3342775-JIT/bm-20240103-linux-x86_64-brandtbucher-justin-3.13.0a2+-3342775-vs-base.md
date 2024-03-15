# Results vs. base

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: 3342775
- commit date: 2024-01-03
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 264 ms                                                                 | 278 ms: 1.05x slower                                           |
| chameleon      | 6.90 ms                                                                | 7.20 ms: 1.04x slower                                          |
| docutils       | 2.59 sec                                                               | 2.68 sec: 1.03x slower                                         |
| tornado_http   | 94.1 ms                                                                | 97.3 ms: 1.03x slower                                          |
| Geometric mean | (ref)                                                                  | 1.04x slower                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|---------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_memoization    | 559 ms                                                                 | 566 ms: 1.01x slower                                           |
| async_tree_io_tg          | 1.19 sec                                                               | 1.21 sec: 1.02x slower                                         |
| async_tree_io             | 1.17 sec                                                               | 1.19 sec: 1.02x slower                                         |
| async_tree_none           | 434 ms                                                                 | 443 ms: 1.02x slower                                           |
| async_tree_memoization_tg | 574 ms                                                                 | 589 ms: 1.03x slower                                           |
| async_tree_none_tg        | 438 ms                                                                 | 451 ms: 1.03x slower                                           |
| Geometric mean            | (ref)                                                                  | 1.02x slower                                                   |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 187 ms                                                                 | 188 ms: 1.00x slower                                           |
| float          | 79.7 ms                                                                | 87.7 ms: 1.10x slower                                          |
| nbody          | 87.4 ms                                                                | 104 ms: 1.19x slower                                           |
| Geometric mean | (ref)                                                                  | 1.10x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 223 ms                                                                 | 218 ms: 1.02x faster                                           |
| regex_effbot   | 3.65 ms                                                                | 3.62 ms: 1.01x faster                                          |
| regex_v8       | 25.0 ms                                                                | 25.6 ms: 1.03x slower                                          |
| regex_compile  | 130 ms                                                                 | 145 ms: 1.12x slower                                           |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_list          | 5.20 us                                                                | 5.12 us: 1.02x faster                                          |
| pickle_dict          | 35.5 us                                                                | 35.0 us: 1.02x faster                                          |
| unpickle             | 14.9 us                                                                | 14.7 us: 1.01x faster                                          |
| xml_etree_parse      | 157 ms                                                                 | 158 ms: 1.01x slower                                           |
| json_loads           | 28.1 us                                                                | 28.3 us: 1.01x slower                                          |
| xml_etree_process    | 58.6 ms                                                                | 59.4 ms: 1.01x slower                                          |
| xml_etree_generate   | 85.1 ms                                                                | 87.4 ms: 1.03x slower                                          |
| xml_etree_iterparse  | 105 ms                                                                 | 110 ms: 1.05x slower                                           |
| unpickle_list        | 5.05 us                                                                | 5.32 us: 1.05x slower                                          |
| unpickle_pure_python | 216 us                                                                 | 228 us: 1.06x slower                                           |
| tomli_loads          | 2.13 sec                                                               | 2.26 sec: 1.06x slower                                         |
| Geometric mean       | (ref)                                                                  | 1.02x slower                                                   |

Benchmark hidden because not significant (3): pickle, json_dumps, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                          |
| python_startup_no_site | 8.71 ms                                                                | 8.88 ms: 1.02x slower                                          |
| Geometric mean         | (ref)                                                                  | 1.02x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 11.2 ms                                                                | 12.9 ms: 1.15x slower                                          |

All benchmarks:
===============

| Benchmark                 | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin-3.13.0a2+-3342775 |
|---------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| richards_super            | 55.0 ms                                                                | 52.6 ms: 1.04x faster                                          |
| richards                  | 48.3 ms                                                                | 46.4 ms: 1.04x faster                                          |
| gc_traversal              | 3.69 ms                                                                | 3.58 ms: 1.03x faster                                          |
| regex_dna                 | 223 ms                                                                 | 218 ms: 1.02x faster                                           |
| pickle_list               | 5.20 us                                                                | 5.12 us: 1.02x faster                                          |
| pickle_dict               | 35.5 us                                                                | 35.0 us: 1.02x faster                                          |
| unpickle                  | 14.9 us                                                                | 14.7 us: 1.01x faster                                          |
| regex_effbot              | 3.65 ms                                                                | 3.62 ms: 1.01x faster                                          |
| create_gc_cycles          | 1.47 ms                                                                | 1.48 ms: 1.00x slower                                          |
| pidigits                  | 187 ms                                                                 | 188 ms: 1.00x slower                                           |
| generators                | 29.4 ms                                                                | 29.6 ms: 1.01x slower                                          |
| xml_etree_parse           | 157 ms                                                                 | 158 ms: 1.01x slower                                           |
| json_loads                | 28.1 us                                                                | 28.3 us: 1.01x slower                                          |
| coverage                  | 95.0 ms                                                                | 95.9 ms: 1.01x slower                                          |
| json                      | 5.18 ms                                                                | 5.23 ms: 1.01x slower                                          |
| sqlite_synth              | 2.85 us                                                                | 2.88 us: 1.01x slower                                          |
| async_tree_memoization    | 559 ms                                                                 | 566 ms: 1.01x slower                                           |
| python_startup            | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                          |
| xml_etree_process         | 58.6 ms                                                                | 59.4 ms: 1.01x slower                                          |
| async_tree_io_tg          | 1.19 sec                                                               | 1.21 sec: 1.02x slower                                         |
| async_tree_io             | 1.17 sec                                                               | 1.19 sec: 1.02x slower                                         |
| asyncio_tcp               | 480 ms                                                                 | 488 ms: 1.02x slower                                           |
| scimark_sor               | 128 ms                                                                 | 130 ms: 1.02x slower                                           |
| pycparser                 | 1.19 sec                                                               | 1.21 sec: 1.02x slower                                         |
| asyncio_tcp_ssl           | 1.77 sec                                                               | 1.80 sec: 1.02x slower                                         |
| python_startup_no_site    | 8.71 ms                                                                | 8.88 ms: 1.02x slower                                          |
| bench_thread_pool         | 827 us                                                                 | 844 us: 1.02x slower                                           |
| telco                     | 8.35 ms                                                                | 8.52 ms: 1.02x slower                                          |
| async_tree_none           | 434 ms                                                                 | 443 ms: 1.02x slower                                           |
| dask                      | 359 ms                                                                 | 368 ms: 1.02x slower                                           |
| logging_simple            | 5.62 us                                                                | 5.75 us: 1.02x slower                                          |
| regex_v8                  | 25.0 ms                                                                | 25.6 ms: 1.03x slower                                          |
| async_tree_memoization_tg | 574 ms                                                                 | 589 ms: 1.03x slower                                           |
| xml_etree_generate        | 85.1 ms                                                                | 87.4 ms: 1.03x slower                                          |
| async_generators          | 439 ms                                                                 | 451 ms: 1.03x slower                                           |
| sqlglot_normalize         | 108 ms                                                                 | 111 ms: 1.03x slower                                           |
| deepcopy                  | 344 us                                                                 | 354 us: 1.03x slower                                           |
| async_tree_none_tg        | 438 ms                                                                 | 451 ms: 1.03x slower                                           |
| pathlib                   | 18.3 ms                                                                | 18.8 ms: 1.03x slower                                          |
| docutils                  | 2.59 sec                                                               | 2.68 sec: 1.03x slower                                         |
| tornado_http              | 94.1 ms                                                                | 97.3 ms: 1.03x slower                                          |
| typing_runtime_protocols  | 111 us                                                                 | 114 us: 1.03x slower                                           |
| scimark_lu                | 112 ms                                                                 | 116 ms: 1.03x slower                                           |
| logging_format            | 6.18 us                                                                | 6.39 us: 1.03x slower                                          |
| meteor_contest            | 108 ms                                                                 | 112 ms: 1.04x slower                                           |
| coroutines                | 22.4 ms                                                                | 23.2 ms: 1.04x slower                                          |
| deepcopy_reduce           | 3.02 us                                                                | 3.13 us: 1.04x slower                                          |
| sqlglot_parse             | 1.25 ms                                                                | 1.30 ms: 1.04x slower                                          |
| chameleon                 | 6.90 ms                                                                | 7.20 ms: 1.04x slower                                          |
| dulwich_log               | 65.3 ms                                                                | 68.3 ms: 1.05x slower                                          |
| sqlglot_transpile         | 1.57 ms                                                                | 1.64 ms: 1.05x slower                                          |
| xml_etree_iterparse       | 105 ms                                                                 | 110 ms: 1.05x slower                                           |
| sympy_expand              | 465 ms                                                                 | 489 ms: 1.05x slower                                           |
| sympy_str                 | 276 ms                                                                 | 290 ms: 1.05x slower                                           |
| 2to3                      | 264 ms                                                                 | 278 ms: 1.05x slower                                           |
| sqlglot_optimize          | 53.9 ms                                                                | 56.8 ms: 1.05x slower                                          |
| unpickle_list             | 5.05 us                                                                | 5.32 us: 1.05x slower                                          |
| unpickle_pure_python      | 216 us                                                                 | 228 us: 1.06x slower                                           |
| tomli_loads               | 2.13 sec                                                               | 2.26 sec: 1.06x slower                                         |
| deepcopy_memo             | 38.4 us                                                                | 40.8 us: 1.06x slower                                          |
| unpack_sequence           | 44.4 ns                                                                | 47.4 ns: 1.07x slower                                          |
| logging_silent            | 102 ns                                                                 | 110 ns: 1.08x slower                                           |
| raytrace                  | 262 ms                                                                 | 284 ms: 1.09x slower                                           |
| scimark_fft               | 362 ms                                                                 | 393 ms: 1.09x slower                                           |
| sympy_sum                 | 148 ms                                                                 | 161 ms: 1.09x slower                                           |
| sympy_integrate           | 19.5 ms                                                                | 21.3 ms: 1.09x slower                                          |
| float                     | 79.7 ms                                                                | 87.7 ms: 1.10x slower                                          |
| go                        | 139 ms                                                                 | 153 ms: 1.11x slower                                           |
| mdp                       | 2.53 sec                                                               | 2.82 sec: 1.12x slower                                         |
| regex_compile             | 130 ms                                                                 | 145 ms: 1.12x slower                                           |
| fannkuch                  | 399 ms                                                                 | 447 ms: 1.12x slower                                           |
| pprint_safe_repr          | 724 ms                                                                 | 811 ms: 1.12x slower                                           |
| pyflate                   | 455 ms                                                                 | 514 ms: 1.13x slower                                           |
| crypto_pyaes              | 70.0 ms                                                                | 79.8 ms: 1.14x slower                                          |
| scimark_monte_carlo       | 67.6 ms                                                                | 77.6 ms: 1.15x slower                                          |
| nqueens                   | 80.6 ms                                                                | 92.6 ms: 1.15x slower                                          |
| mako                      | 11.2 ms                                                                | 12.9 ms: 1.15x slower                                          |
| pprint_pformat            | 1.48 sec                                                               | 1.71 sec: 1.16x slower                                         |
| nbody                     | 87.4 ms                                                                | 104 ms: 1.19x slower                                           |
| scimark_sparse_mat_mult   | 4.87 ms                                                                | 5.88 ms: 1.21x slower                                          |
| chaos                     | 58.9 ms                                                                | 71.7 ms: 1.22x slower                                          |
| comprehensions            | 16.0 us                                                                | 20.0 us: 1.25x slower                                          |
| deltablue                 | 3.26 ms                                                                | 4.08 ms: 1.25x slower                                          |
| spectral_norm             | 109 ms                                                                 | 140 ms: 1.28x slower                                           |
| hexiom                    | 6.07 ms                                                                | 8.23 ms: 1.36x slower                                          |
| Geometric mean            | (ref)                                                                  | 1.05x slower                                                   |

Benchmark hidden because not significant (8): pickle, json_dumps, asyncio_websockets, bench_mp_pool, pickle_pure_python, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.04x