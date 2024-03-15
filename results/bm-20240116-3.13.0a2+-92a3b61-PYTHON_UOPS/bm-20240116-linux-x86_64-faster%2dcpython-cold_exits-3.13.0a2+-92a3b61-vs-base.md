# Results vs. base

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 92a3b61
- commit date: 2024-01-16
- overall geometric mean: 1.01x faster
- HPT reliability: 90.27%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 284 ms                                                                 | 288 ms: 1.01x slower                                                   |
| chameleon      | 7.37 ms                                                                | 7.11 ms: 1.04x faster                                                  |
| docutils       | 2.72 sec                                                               | 2.71 sec: 1.01x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark      | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_io  | 1.21 sec                                                               | 1.20 sec: 1.00x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (7): async_tree_none, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_io_tg, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 131 ms                                                                 | 120 ms: 1.09x faster                                                   |
| float          | 100 ms                                                                 | 94.2 ms: 1.06x faster                                                  |
| pidigits       | 197 ms                                                                 | 189 ms: 1.04x faster                                                   |
| Geometric mean | (ref)                                                                  | 1.07x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_v8       | 24.9 ms                                                                | 24.7 ms: 1.01x faster                                                  |
| regex_effbot   | 3.64 ms                                                                | 3.65 ms: 1.00x slower                                                  |
| regex_compile  | 156 ms                                                                 | 164 ms: 1.06x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_list          | 5.32 us                                                                | 5.13 us: 1.04x faster                                                  |
| unpickle_list        | 5.51 us                                                                | 5.32 us: 1.04x faster                                                  |
| pickle_dict          | 34.9 us                                                                | 33.9 us: 1.03x faster                                                  |
| unpickle_pure_python | 240 us                                                                 | 233 us: 1.03x faster                                                   |
| tomli_loads          | 2.54 sec                                                               | 2.49 sec: 1.02x faster                                                 |
| xml_etree_iterparse  | 113 ms                                                                 | 111 ms: 1.02x faster                                                   |
| xml_etree_process    | 61.8 ms                                                                | 60.9 ms: 1.01x faster                                                  |
| xml_etree_generate   | 90.4 ms                                                                | 89.4 ms: 1.01x faster                                                  |
| pickle               | 11.7 us                                                                | 11.7 us: 1.01x faster                                                  |
| json_dumps           | 10.7 ms                                                                | 10.8 ms: 1.01x slower                                                  |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (4): unpickle, pickle_pure_python, xml_etree_parse, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup_no_site | 8.71 ms                                                                | 8.70 ms: 1.00x faster                                                  |
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                  |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 15.0 ms                                                                | 14.2 ms: 1.05x faster                                                  |

All benchmarks:
===============

| Benchmark               | bm-20240115-linux-x86_64-python-ac10947ba79a15bfdaa3-3.13.0a2+-ac10947 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-92a3b61 |
|-------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| generators              | 36.4 ms                                                                | 29.1 ms: 1.25x faster                                                  |
| spectral_norm           | 161 ms                                                                 | 146 ms: 1.10x faster                                                   |
| nbody                   | 131 ms                                                                 | 120 ms: 1.09x faster                                                   |
| comprehensions          | 22.9 us                                                                | 21.5 us: 1.07x faster                                                  |
| float                   | 100 ms                                                                 | 94.2 ms: 1.06x faster                                                  |
| unpack_sequence         | 54.0 ns                                                                | 50.9 ns: 1.06x faster                                                  |
| chaos                   | 78.2 ms                                                                | 74.0 ms: 1.06x faster                                                  |
| deltablue               | 5.11 ms                                                                | 4.84 ms: 1.06x faster                                                  |
| mako                    | 15.0 ms                                                                | 14.2 ms: 1.05x faster                                                  |
| deepcopy_memo           | 42.4 us                                                                | 40.4 us: 1.05x faster                                                  |
| scimark_fft             | 480 ms                                                                 | 458 ms: 1.05x faster                                                   |
| scimark_sparse_mat_mult | 6.40 ms                                                                | 6.12 ms: 1.05x faster                                                  |
| pidigits                | 197 ms                                                                 | 189 ms: 1.04x faster                                                   |
| hexiom                  | 9.08 ms                                                                | 8.74 ms: 1.04x faster                                                  |
| pickle_list             | 5.32 us                                                                | 5.13 us: 1.04x faster                                                  |
| crypto_pyaes            | 87.7 ms                                                                | 84.5 ms: 1.04x faster                                                  |
| chameleon               | 7.37 ms                                                                | 7.11 ms: 1.04x faster                                                  |
| unpickle_list           | 5.51 us                                                                | 5.32 us: 1.04x faster                                                  |
| pickle_dict             | 34.9 us                                                                | 33.9 us: 1.03x faster                                                  |
| unpickle_pure_python    | 240 us                                                                 | 233 us: 1.03x faster                                                   |
| nqueens                 | 99.2 ms                                                                | 97.0 ms: 1.02x faster                                                  |
| tomli_loads             | 2.54 sec                                                               | 2.49 sec: 1.02x faster                                                 |
| xml_etree_iterparse     | 113 ms                                                                 | 111 ms: 1.02x faster                                                   |
| xml_etree_process       | 61.8 ms                                                                | 60.9 ms: 1.01x faster                                                  |
| raytrace                | 308 ms                                                                 | 304 ms: 1.01x faster                                                   |
| richards                | 48.9 ms                                                                | 48.3 ms: 1.01x faster                                                  |
| xml_etree_generate      | 90.4 ms                                                                | 89.4 ms: 1.01x faster                                                  |
| json                    | 5.28 ms                                                                | 5.22 ms: 1.01x faster                                                  |
| scimark_sor             | 132 ms                                                                 | 131 ms: 1.01x faster                                                   |
| regex_v8                | 24.9 ms                                                                | 24.7 ms: 1.01x faster                                                  |
| async_generators        | 454 ms                                                                 | 452 ms: 1.01x faster                                                   |
| pickle                  | 11.7 us                                                                | 11.7 us: 1.01x faster                                                  |
| docutils                | 2.72 sec                                                               | 2.71 sec: 1.01x faster                                                 |
| mdp                     | 2.65 sec                                                               | 2.63 sec: 1.01x faster                                                 |
| asyncio_tcp             | 496 ms                                                                 | 493 ms: 1.00x faster                                                   |
| richards_super          | 55.2 ms                                                                | 55.0 ms: 1.00x faster                                                  |
| bench_thread_pool       | 851 us                                                                 | 848 us: 1.00x faster                                                   |
| async_tree_io           | 1.21 sec                                                               | 1.20 sec: 1.00x faster                                                 |
| python_startup_no_site  | 8.71 ms                                                                | 8.70 ms: 1.00x faster                                                  |
| python_startup          | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                  |
| regex_effbot            | 3.64 ms                                                                | 3.65 ms: 1.00x slower                                                  |
| sqlglot_normalize       | 115 ms                                                                 | 115 ms: 1.00x slower                                                   |
| dulwich_log             | 69.2 ms                                                                | 69.3 ms: 1.00x slower                                                  |
| create_gc_cycles        | 1.47 ms                                                                | 1.48 ms: 1.00x slower                                                  |
| logging_silent          | 106 ns                                                                 | 106 ns: 1.00x slower                                                   |
| sympy_sum               | 162 ms                                                                 | 163 ms: 1.01x slower                                                   |
| deepcopy_reduce         | 3.13 us                                                                | 3.15 us: 1.01x slower                                                  |
| json_dumps              | 10.7 ms                                                                | 10.8 ms: 1.01x slower                                                  |
| sqlite_synth            | 2.88 us                                                                | 2.91 us: 1.01x slower                                                  |
| sqlglot_optimize        | 58.6 ms                                                                | 59.3 ms: 1.01x slower                                                  |
| fannkuch                | 479 ms                                                                 | 485 ms: 1.01x slower                                                   |
| 2to3                    | 284 ms                                                                 | 288 ms: 1.01x slower                                                   |
| pprint_pformat          | 1.77 sec                                                               | 1.80 sec: 1.02x slower                                                 |
| coroutines              | 22.0 ms                                                                | 22.6 ms: 1.03x slower                                                  |
| pprint_safe_repr        | 845 ms                                                                 | 870 ms: 1.03x slower                                                   |
| logging_simple          | 6.05 us                                                                | 6.29 us: 1.04x slower                                                  |
| logging_format          | 6.71 us                                                                | 7.02 us: 1.05x slower                                                  |
| scimark_monte_carlo     | 86.2 ms                                                                | 90.2 ms: 1.05x slower                                                  |
| pyflate                 | 562 ms                                                                 | 589 ms: 1.05x slower                                                   |
| go                      | 160 ms                                                                 | 168 ms: 1.05x slower                                                   |
| regex_compile           | 156 ms                                                                 | 164 ms: 1.06x slower                                                   |
| gc_traversal            | 3.70 ms                                                                | 4.00 ms: 1.08x slower                                                  |
| Geometric mean          | (ref)                                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (31): async_tree_none, async_tree_memoization, async_tree_cpu_io_mixed, sympy_str, pathlib, telco, sympy_expand, unpickle, pickle_pure_python, meteor_contest, xml_etree_parse, async_tree_io_tg, async_tree_memoization_tg, asyncio_websockets, bench_mp_pool, sympy_integrate, deepcopy, dask, asyncio_tcp_ssl, regex_dna, async_tree_cpu_io_mixed_tg, pycparser, sqlglot_parse, sqlglot_transpile, json_loads, async_tree_none_tg, scimark_lu, coverage, tornado_http, typing_runtime_protocols, mypy2


# HPT report

- Reliability score: 90.27% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x