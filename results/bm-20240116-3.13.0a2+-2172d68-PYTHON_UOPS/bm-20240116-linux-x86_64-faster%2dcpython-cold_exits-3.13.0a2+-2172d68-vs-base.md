# Results vs. base

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 2172d68
- commit date: 2024-01-16
- overall geometric mean: 1.00x faster
- HPT reliability: 95.95%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 284 ms                                                                 | 288 ms: 1.01x slower                                                   |
| chameleon      | 7.37 ms                                                                | 7.27 ms: 1.01x faster                                                  |
| docutils       | 2.72 sec                                                               | 2.75 sec: 1.01x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|---------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_memoization_tg | 588 ms                                                                 | 578 ms: 1.02x faster                                                   |
| async_tree_memoization    | 577 ms                                                                 | 570 ms: 1.01x faster                                                   |
| async_tree_none_tg        | 451 ms                                                                 | 446 ms: 1.01x faster                                                   |
| Geometric mean            | (ref)                                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (5): async_tree_io_tg, async_tree_none, async_tree_io, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 131 ms                                                                 | 115 ms: 1.13x faster                                                   |
| float          | 100 ms                                                                 | 92.1 ms: 1.09x faster                                                  |
| pidigits       | 197 ms                                                                 | 197 ms: 1.00x faster                                                   |
| Geometric mean | (ref)                                                                  | 1.07x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_v8       | 24.9 ms                                                                | 25.2 ms: 1.01x slower                                                  |
| regex_dna      | 223 ms                                                                 | 226 ms: 1.02x slower                                                   |
| regex_effbot   | 3.64 ms                                                                | 3.72 ms: 1.02x slower                                                  |
| regex_compile  | 156 ms                                                                 | 170 ms: 1.09x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.04x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_list          | 5.32 us                                                                | 4.88 us: 1.09x faster                                                  |
| unpickle_pure_python | 240 us                                                                 | 233 us: 1.03x faster                                                   |
| pickle               | 11.7 us                                                                | 11.4 us: 1.03x faster                                                  |
| unpickle_list        | 5.51 us                                                                | 5.36 us: 1.03x faster                                                  |
| pickle_dict          | 34.9 us                                                                | 34.4 us: 1.02x faster                                                  |
| xml_etree_iterparse  | 113 ms                                                                 | 112 ms: 1.01x faster                                                   |
| xml_etree_generate   | 90.4 ms                                                                | 89.9 ms: 1.01x faster                                                  |
| pickle_pure_python   | 302 us                                                                 | 300 us: 1.01x faster                                                   |
| json_loads           | 28.5 us                                                                | 28.4 us: 1.00x faster                                                  |
| tomli_loads          | 2.54 sec                                                               | 2.71 sec: 1.06x slower                                                 |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (4): xml_etree_process, json_dumps, unpickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.01x slower                                                  |
| python_startup_no_site | 8.71 ms                                                                | 8.78 ms: 1.01x slower                                                  |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 15.0 ms                                                                | 13.6 ms: 1.10x faster                                                  |

All benchmarks:
===============

| Benchmark                 | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|---------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| generators                | 36.4 ms                                                                | 29.1 ms: 1.25x faster                                                  |
| nbody                     | 131 ms                                                                 | 115 ms: 1.13x faster                                                   |
| spectral_norm             | 161 ms                                                                 | 145 ms: 1.11x faster                                                   |
| mako                      | 15.0 ms                                                                | 13.6 ms: 1.10x faster                                                  |
| pickle_list               | 5.32 us                                                                | 4.88 us: 1.09x faster                                                  |
| float                     | 100 ms                                                                 | 92.1 ms: 1.09x faster                                                  |
| comprehensions            | 22.9 us                                                                | 21.2 us: 1.08x faster                                                  |
| scimark_sparse_mat_mult   | 6.40 ms                                                                | 5.98 ms: 1.07x faster                                                  |
| scimark_fft               | 480 ms                                                                 | 449 ms: 1.07x faster                                                   |
| deltablue                 | 5.11 ms                                                                | 4.82 ms: 1.06x faster                                                  |
| chaos                     | 78.2 ms                                                                | 74.4 ms: 1.05x faster                                                  |
| crypto_pyaes              | 87.7 ms                                                                | 83.5 ms: 1.05x faster                                                  |
| pycparser                 | 1.25 sec                                                               | 1.21 sec: 1.04x faster                                                 |
| unpickle_pure_python      | 240 us                                                                 | 233 us: 1.03x faster                                                   |
| pickle                    | 11.7 us                                                                | 11.4 us: 1.03x faster                                                  |
| unpickle_list             | 5.51 us                                                                | 5.36 us: 1.03x faster                                                  |
| raytrace                  | 308 ms                                                                 | 302 ms: 1.02x faster                                                   |
| async_tree_memoization_tg | 588 ms                                                                 | 578 ms: 1.02x faster                                                   |
| deepcopy_memo             | 42.4 us                                                                | 41.7 us: 1.02x faster                                                  |
| pickle_dict               | 34.9 us                                                                | 34.4 us: 1.02x faster                                                  |
| chameleon                 | 7.37 ms                                                                | 7.27 ms: 1.01x faster                                                  |
| async_tree_memoization    | 577 ms                                                                 | 570 ms: 1.01x faster                                                   |
| meteor_contest            | 117 ms                                                                 | 116 ms: 1.01x faster                                                   |
| async_tree_none_tg        | 451 ms                                                                 | 446 ms: 1.01x faster                                                   |
| sqlite_synth              | 2.88 us                                                                | 2.85 us: 1.01x faster                                                  |
| xml_etree_iterparse       | 113 ms                                                                 | 112 ms: 1.01x faster                                                   |
| xml_etree_generate        | 90.4 ms                                                                | 89.9 ms: 1.01x faster                                                  |
| pickle_pure_python        | 302 us                                                                 | 300 us: 1.01x faster                                                   |
| asyncio_tcp               | 496 ms                                                                 | 493 ms: 1.01x faster                                                   |
| json_loads                | 28.5 us                                                                | 28.4 us: 1.00x faster                                                  |
| hexiom                    | 9.08 ms                                                                | 9.05 ms: 1.00x faster                                                  |
| asyncio_tcp_ssl           | 1.80 sec                                                               | 1.80 sec: 1.00x faster                                                 |
| pidigits                  | 197 ms                                                                 | 197 ms: 1.00x faster                                                   |
| bench_thread_pool         | 851 us                                                                 | 855 us: 1.00x slower                                                   |
| pprint_pformat            | 1.77 sec                                                               | 1.78 sec: 1.01x slower                                                 |
| python_startup            | 10.1 ms                                                                | 10.1 ms: 1.01x slower                                                  |
| docutils                  | 2.72 sec                                                               | 2.75 sec: 1.01x slower                                                 |
| deepcopy                  | 358 us                                                                 | 361 us: 1.01x slower                                                   |
| python_startup_no_site    | 8.71 ms                                                                | 8.78 ms: 1.01x slower                                                  |
| async_generators          | 454 ms                                                                 | 459 ms: 1.01x slower                                                   |
| sympy_sum                 | 162 ms                                                                 | 163 ms: 1.01x slower                                                   |
| sqlglot_normalize         | 115 ms                                                                 | 116 ms: 1.01x slower                                                   |
| regex_v8                  | 24.9 ms                                                                | 25.2 ms: 1.01x slower                                                  |
| sympy_str                 | 296 ms                                                                 | 299 ms: 1.01x slower                                                   |
| pprint_safe_repr          | 845 ms                                                                 | 856 ms: 1.01x slower                                                   |
| sympy_integrate           | 21.4 ms                                                                | 21.7 ms: 1.01x slower                                                  |
| 2to3                      | 284 ms                                                                 | 288 ms: 1.01x slower                                                   |
| sympy_expand              | 493 ms                                                                 | 500 ms: 1.01x slower                                                   |
| gc_traversal              | 3.70 ms                                                                | 3.76 ms: 1.02x slower                                                  |
| regex_dna                 | 223 ms                                                                 | 226 ms: 1.02x slower                                                   |
| fannkuch                  | 479 ms                                                                 | 487 ms: 1.02x slower                                                   |
| deepcopy_reduce           | 3.13 us                                                                | 3.19 us: 1.02x slower                                                  |
| regex_effbot              | 3.64 ms                                                                | 3.72 ms: 1.02x slower                                                  |
| sqlglot_optimize          | 58.6 ms                                                                | 59.9 ms: 1.02x slower                                                  |
| pathlib                   | 18.7 ms                                                                | 19.1 ms: 1.02x slower                                                  |
| richards                  | 48.9 ms                                                                | 50.0 ms: 1.02x slower                                                  |
| richards_super            | 55.2 ms                                                                | 56.5 ms: 1.02x slower                                                  |
| create_gc_cycles          | 1.47 ms                                                                | 1.51 ms: 1.02x slower                                                  |
| typing_runtime_protocols  | 116 us                                                                 | 119 us: 1.03x slower                                                   |
| sqlglot_transpile         | 1.66 ms                                                                | 1.71 ms: 1.03x slower                                                  |
| pyflate                   | 562 ms                                                                 | 582 ms: 1.04x slower                                                   |
| dulwich_log               | 69.2 ms                                                                | 71.8 ms: 1.04x slower                                                  |
| scimark_monte_carlo       | 86.2 ms                                                                | 89.5 ms: 1.04x slower                                                  |
| sqlglot_parse             | 1.33 ms                                                                | 1.38 ms: 1.04x slower                                                  |
| mdp                       | 2.65 sec                                                               | 2.78 sec: 1.05x slower                                                 |
| scimark_sor               | 132 ms                                                                 | 139 ms: 1.05x slower                                                   |
| logging_simple            | 6.05 us                                                                | 6.39 us: 1.06x slower                                                  |
| unpack_sequence           | 54.0 ns                                                                | 57.5 ns: 1.06x slower                                                  |
| tomli_loads               | 2.54 sec                                                               | 2.71 sec: 1.06x slower                                                 |
| logging_format            | 6.71 us                                                                | 7.24 us: 1.08x slower                                                  |
| go                        | 160 ms                                                                 | 175 ms: 1.09x slower                                                   |
| regex_compile             | 156 ms                                                                 | 170 ms: 1.09x slower                                                   |
| scimark_lu                | 119 ms                                                                 | 149 ms: 1.26x slower                                                   |
| Geometric mean            | (ref)                                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (20): json, nqueens, xml_etree_process, json_dumps, async_tree_io_tg, bench_mp_pool, telco, async_tree_none, coverage, asyncio_websockets, unpickle, tornado_http, async_tree_io, dask, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, coroutines, xml_etree_parse, logging_silent, mypy2


# HPT report

- Reliability score: 95.95% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x