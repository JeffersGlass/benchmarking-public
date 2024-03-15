# Results vs. base

- fork: faster-cpython
- ref: better_set_ip_check_
- machine: linux-x86_64
- commit hash: 4d59a84
- commit date: 2024-02-09
- overall geometric mean: 1.02x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                                 | 282 ms: 1.01x faster                                                             |
| chameleon      | 7.27 ms                                                                | 7.34 ms: 1.01x slower                                                            |
| docutils       | 2.72 sec                                                               | 2.70 sec: 1.01x faster                                                           |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_memoization | 583 ms                                                                 | 576 ms: 1.01x faster                                                             |
| async_tree_none_tg     | 458 ms                                                                 | 454 ms: 1.01x faster                                                             |
| async_tree_io_tg       | 1.23 sec                                                               | 1.22 sec: 1.00x faster                                                           |
| async_tree_io          | 1.21 sec                                                               | 1.21 sec: 1.00x faster                                                           |
| Geometric mean         | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (4): async_tree_none, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 126 ms                                                                 | 114 ms: 1.11x faster                                                             |
| float          | 94.0 ms                                                                | 91.8 ms: 1.02x faster                                                            |
| pidigits       | 190 ms                                                                 | 188 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                                  | 1.05x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                                 | 151 ms: 1.03x faster                                                             |
| regex_dna      | 227 ms                                                                 | 227 ms: 1.00x slower                                                             |
| regex_effbot   | 3.63 ms                                                                | 3.66 ms: 1.01x slower                                                            |
| regex_v8       | 24.6 ms                                                                | 25.2 ms: 1.02x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tomli_loads          | 2.53 sec                                                               | 2.37 sec: 1.07x faster                                                           |
| unpickle_list        | 5.39 us                                                                | 5.17 us: 1.04x faster                                                            |
| xml_etree_iterparse  | 113 ms                                                                 | 110 ms: 1.03x faster                                                             |
| unpickle_pure_python | 239 us                                                                 | 233 us: 1.02x faster                                                             |
| xml_etree_process    | 62.0 ms                                                                | 60.5 ms: 1.02x faster                                                            |
| xml_etree_generate   | 90.9 ms                                                                | 88.8 ms: 1.02x faster                                                            |
| pickle               | 11.6 us                                                                | 11.4 us: 1.01x faster                                                            |
| xml_etree_parse      | 157 ms                                                                 | 158 ms: 1.01x slower                                                             |
| json_dumps           | 10.6 ms                                                                | 10.6 ms: 1.01x slower                                                            |
| pickle_dict          | 35.1 us                                                                | 35.8 us: 1.02x slower                                                            |
| pickle_list          | 5.13 us                                                                | 5.26 us: 1.02x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (3): pickle_pure_python, json_loads, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup_no_site | 8.77 ms                                                                | 8.74 ms: 1.00x faster                                                            |
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                                | 13.6 ms: 1.08x faster                                                            |

All benchmarks:
===============

| Benchmark               | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240209-linux-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-4d59a84 |
|-------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody                   | 126 ms                                                                 | 114 ms: 1.11x faster                                                             |
| spectral_norm           | 157 ms                                                                 | 143 ms: 1.10x faster                                                             |
| hexiom                  | 9.02 ms                                                                | 8.24 ms: 1.10x faster                                                            |
| comprehensions          | 22.5 us                                                                | 20.6 us: 1.09x faster                                                            |
| fannkuch                | 477 ms                                                                 | 437 ms: 1.09x faster                                                             |
| pyflate                 | 554 ms                                                                 | 508 ms: 1.09x faster                                                             |
| scimark_sparse_mat_mult | 6.30 ms                                                                | 5.84 ms: 1.08x faster                                                            |
| mako                    | 14.7 ms                                                                | 13.6 ms: 1.08x faster                                                            |
| deltablue               | 4.87 ms                                                                | 4.53 ms: 1.07x faster                                                            |
| scimark_fft             | 472 ms                                                                 | 441 ms: 1.07x faster                                                             |
| tomli_loads             | 2.53 sec                                                               | 2.37 sec: 1.07x faster                                                           |
| nqueens                 | 101 ms                                                                 | 95.0 ms: 1.06x faster                                                            |
| scimark_monte_carlo     | 84.8 ms                                                                | 79.9 ms: 1.06x faster                                                            |
| chaos                   | 76.0 ms                                                                | 72.2 ms: 1.05x faster                                                            |
| meteor_contest          | 119 ms                                                                 | 113 ms: 1.05x faster                                                             |
| crypto_pyaes            | 87.4 ms                                                                | 83.2 ms: 1.05x faster                                                            |
| scimark_sor             | 132 ms                                                                 | 126 ms: 1.05x faster                                                             |
| unpickle_list           | 5.39 us                                                                | 5.17 us: 1.04x faster                                                            |
| deepcopy_memo           | 41.9 us                                                                | 40.3 us: 1.04x faster                                                            |
| telco                   | 8.88 ms                                                                | 8.57 ms: 1.04x faster                                                            |
| gc_traversal            | 3.83 ms                                                                | 3.70 ms: 1.04x faster                                                            |
| sympy_expand            | 505 ms                                                                 | 490 ms: 1.03x faster                                                             |
| pprint_safe_repr        | 836 ms                                                                 | 811 ms: 1.03x faster                                                             |
| xml_etree_iterparse     | 113 ms                                                                 | 110 ms: 1.03x faster                                                             |
| pprint_pformat          | 1.74 sec                                                               | 1.69 sec: 1.03x faster                                                           |
| regex_compile           | 156 ms                                                                 | 151 ms: 1.03x faster                                                             |
| go                      | 161 ms                                                                 | 156 ms: 1.03x faster                                                             |
| unpickle_pure_python    | 239 us                                                                 | 233 us: 1.02x faster                                                             |
| xml_etree_process       | 62.0 ms                                                                | 60.5 ms: 1.02x faster                                                            |
| xml_etree_generate      | 90.9 ms                                                                | 88.8 ms: 1.02x faster                                                            |
| sympy_sum               | 163 ms                                                                 | 160 ms: 1.02x faster                                                             |
| float                   | 94.0 ms                                                                | 91.8 ms: 1.02x faster                                                            |
| sympy_str               | 298 ms                                                                 | 292 ms: 1.02x faster                                                             |
| raytrace                | 304 ms                                                                 | 297 ms: 1.02x faster                                                             |
| pathlib                 | 18.9 ms                                                                | 18.5 ms: 1.02x faster                                                            |
| sympy_integrate         | 21.6 ms                                                                | 21.2 ms: 1.02x faster                                                            |
| sqlglot_optimize        | 58.9 ms                                                                | 57.7 ms: 1.02x faster                                                            |
| sqlglot_normalize       | 116 ms                                                                 | 114 ms: 1.02x faster                                                             |
| richards                | 49.7 ms                                                                | 48.9 ms: 1.02x faster                                                            |
| async_tree_memoization  | 583 ms                                                                 | 576 ms: 1.01x faster                                                             |
| logging_simple          | 6.08 us                                                                | 6.02 us: 1.01x faster                                                            |
| deepcopy                | 360 us                                                                 | 357 us: 1.01x faster                                                             |
| 2to3                    | 285 ms                                                                 | 282 ms: 1.01x faster                                                             |
| pickle                  | 11.6 us                                                                | 11.4 us: 1.01x faster                                                            |
| async_tree_none_tg      | 458 ms                                                                 | 454 ms: 1.01x faster                                                             |
| docutils                | 2.72 sec                                                               | 2.70 sec: 1.01x faster                                                           |
| sqlglot_transpile       | 1.68 ms                                                                | 1.66 ms: 1.01x faster                                                            |
| pidigits                | 190 ms                                                                 | 188 ms: 1.01x faster                                                             |
| richards_super          | 56.0 ms                                                                | 55.7 ms: 1.01x faster                                                            |
| sqlglot_parse           | 1.34 ms                                                                | 1.33 ms: 1.01x faster                                                            |
| async_generators        | 453 ms                                                                 | 450 ms: 1.01x faster                                                             |
| asyncio_tcp_ssl         | 1.81 sec                                                               | 1.80 sec: 1.00x faster                                                           |
| bench_thread_pool       | 854 us                                                                 | 850 us: 1.00x faster                                                             |
| python_startup_no_site  | 8.77 ms                                                                | 8.74 ms: 1.00x faster                                                            |
| async_tree_io_tg        | 1.23 sec                                                               | 1.22 sec: 1.00x faster                                                           |
| python_startup          | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                                            |
| async_tree_io           | 1.21 sec                                                               | 1.21 sec: 1.00x faster                                                           |
| regex_dna               | 227 ms                                                                 | 227 ms: 1.00x slower                                                             |
| xml_etree_parse         | 157 ms                                                                 | 158 ms: 1.01x slower                                                             |
| json_dumps              | 10.6 ms                                                                | 10.6 ms: 1.01x slower                                                            |
| coverage                | 94.7 ms                                                                | 95.4 ms: 1.01x slower                                                            |
| chameleon               | 7.27 ms                                                                | 7.34 ms: 1.01x slower                                                            |
| regex_effbot            | 3.63 ms                                                                | 3.66 ms: 1.01x slower                                                            |
| generators              | 29.1 ms                                                                | 29.4 ms: 1.01x slower                                                            |
| pickle_dict             | 35.1 us                                                                | 35.8 us: 1.02x slower                                                            |
| unpack_sequence         | 41.7 ns                                                                | 42.7 ns: 1.02x slower                                                            |
| pickle_list             | 5.13 us                                                                | 5.26 us: 1.02x slower                                                            |
| regex_v8                | 24.6 ms                                                                | 25.2 ms: 1.02x slower                                                            |
| Geometric mean          | (ref)                                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (25): async_tree_none, async_tree_memoization_tg, deepcopy_reduce, coroutines, sqlite_synth, logging_silent, scimark_lu, pickle_pure_python, logging_format, json_loads, bench_mp_pool, create_gc_cycles, unpickle, asyncio_tcp, dulwich_log, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, asyncio_websockets, json, mdp, mypy2, typing_runtime_protocols, dask, tornado_http, pycparser


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x