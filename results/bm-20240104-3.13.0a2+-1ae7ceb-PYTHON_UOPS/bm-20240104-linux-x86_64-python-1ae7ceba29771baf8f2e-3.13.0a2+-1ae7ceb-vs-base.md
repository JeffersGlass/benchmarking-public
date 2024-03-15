# Results vs. base

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: linux-x86_64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.01x slower \*
- HPT reliability: 99.91%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 285 ms                                                                 | 286 ms: 1.01x slower                                                   |
| chameleon      | 7.27 ms                                                                | 7.38 ms: 1.01x slower                                                  |
| docutils       | 2.72 sec                                                               | 2.73 sec: 1.00x slower                                                 |
| tornado_http   | 98.2 ms                                                                | 99.4 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_io_tg | 1.23 sec                                                               | 1.22 sec: 1.00x faster                                                 |
| async_tree_io    | 1.21 sec                                                               | 1.21 sec: 1.00x faster                                                 |
| Geometric mean   | (ref)                                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (6): async_tree_cpu_io_mixed_tg, async_tree_none_tg, async_tree_none, async_tree_memoization, async_tree_memoization_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 190 ms                                                                 | 189 ms: 1.00x faster                                                   |
| nbody          | 126 ms                                                                 | 127 ms: 1.01x slower                                                   |
| float          | 94.0 ms                                                                | 99.6 ms: 1.06x slower                                                  |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.63 ms                                                                | 3.61 ms: 1.01x faster                                                  |
| regex_dna      | 227 ms                                                                 | 226 ms: 1.00x faster                                                   |
| regex_compile  | 156 ms                                                                 | 157 ms: 1.01x slower                                                   |
| regex_v8       | 24.6 ms                                                                | 24.8 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpickle_list        | 5.39 us                                                                | 5.27 us: 1.02x faster                                                  |
| pickle               | 11.6 us                                                                | 11.3 us: 1.02x faster                                                  |
| pickle_dict          | 35.1 us                                                                | 34.4 us: 1.02x faster                                                  |
| xml_etree_process    | 62.0 ms                                                                | 61.6 ms: 1.01x faster                                                  |
| xml_etree_iterparse  | 113 ms                                                                 | 114 ms: 1.01x slower                                                   |
| unpickle_pure_python | 239 us                                                                 | 240 us: 1.01x slower                                                   |
| xml_etree_parse      | 157 ms                                                                 | 159 ms: 1.01x slower                                                   |
| json_dumps           | 10.6 ms                                                                | 10.8 ms: 1.02x slower                                                  |
| json_loads           | 28.2 us                                                                | 28.8 us: 1.02x slower                                                  |
| unpickle             | 14.7 us                                                                | 15.0 us: 1.03x slower                                                  |
| Geometric mean       | (ref)                                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (4): pickle_list, xml_etree_generate, tomli_loads, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup_no_site | 8.77 ms                                                                | 8.77 ms: 1.00x slower                                                  |
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                  |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 14.7 ms                                                                | 14.9 ms: 1.02x slower                                                  |

All benchmarks:
===============

| Benchmark                | bm-20240104-linux-x86_64-python-35ef8cb25917bfd6cbbd-3.13.0a2+-35ef8cb | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|--------------------------|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| gc_traversal             | 3.83 ms                                                                | 3.50 ms: 1.09x faster                                                  |
| pyflate                  | 554 ms                                                                 | 528 ms: 1.05x faster                                                   |
| logging_silent           | 108 ns                                                                 | 105 ns: 1.02x faster                                                   |
| unpickle_list            | 5.39 us                                                                | 5.27 us: 1.02x faster                                                  |
| pickle                   | 11.6 us                                                                | 11.3 us: 1.02x faster                                                  |
| fannkuch                 | 477 ms                                                                 | 468 ms: 1.02x faster                                                   |
| pickle_dict              | 35.1 us                                                                | 34.4 us: 1.02x faster                                                  |
| nqueens                  | 101 ms                                                                 | 99.0 ms: 1.02x faster                                                  |
| coroutines               | 22.5 ms                                                                | 22.3 ms: 1.01x faster                                                  |
| meteor_contest           | 119 ms                                                                 | 118 ms: 1.01x faster                                                   |
| asyncio_tcp              | 494 ms                                                                 | 490 ms: 1.01x faster                                                   |
| pathlib                  | 18.9 ms                                                                | 18.8 ms: 1.01x faster                                                  |
| xml_etree_process        | 62.0 ms                                                                | 61.6 ms: 1.01x faster                                                  |
| regex_effbot             | 3.63 ms                                                                | 3.61 ms: 1.01x faster                                                  |
| asyncio_tcp_ssl          | 1.81 sec                                                               | 1.80 sec: 1.01x faster                                                 |
| async_tree_io_tg         | 1.23 sec                                                               | 1.22 sec: 1.00x faster                                                 |
| async_tree_io            | 1.21 sec                                                               | 1.21 sec: 1.00x faster                                                 |
| bench_thread_pool        | 854 us                                                                 | 851 us: 1.00x faster                                                   |
| pidigits                 | 190 ms                                                                 | 189 ms: 1.00x faster                                                   |
| regex_dna                | 227 ms                                                                 | 226 ms: 1.00x faster                                                   |
| python_startup_no_site   | 8.77 ms                                                                | 8.77 ms: 1.00x slower                                                  |
| python_startup           | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                  |
| docutils                 | 2.72 sec                                                               | 2.73 sec: 1.00x slower                                                 |
| deepcopy                 | 360 us                                                                 | 362 us: 1.00x slower                                                   |
| crypto_pyaes             | 87.4 ms                                                                | 87.7 ms: 1.00x slower                                                  |
| sqlglot_transpile        | 1.68 ms                                                                | 1.69 ms: 1.01x slower                                                  |
| nbody                    | 126 ms                                                                 | 127 ms: 1.01x slower                                                   |
| sympy_integrate          | 21.6 ms                                                                | 21.7 ms: 1.01x slower                                                  |
| scimark_fft              | 472 ms                                                                 | 474 ms: 1.01x slower                                                   |
| xml_etree_iterparse      | 113 ms                                                                 | 114 ms: 1.01x slower                                                   |
| pprint_safe_repr         | 836 ms                                                                 | 841 ms: 1.01x slower                                                   |
| generators               | 29.1 ms                                                                | 29.3 ms: 1.01x slower                                                  |
| go                       | 161 ms                                                                 | 162 ms: 1.01x slower                                                   |
| 2to3                     | 285 ms                                                                 | 286 ms: 1.01x slower                                                   |
| unpickle_pure_python     | 239 us                                                                 | 240 us: 1.01x slower                                                   |
| sympy_sum                | 163 ms                                                                 | 165 ms: 1.01x slower                                                   |
| regex_compile            | 156 ms                                                                 | 157 ms: 1.01x slower                                                   |
| sqlglot_normalize        | 116 ms                                                                 | 117 ms: 1.01x slower                                                   |
| regex_v8                 | 24.6 ms                                                                | 24.8 ms: 1.01x slower                                                  |
| sqlglot_parse            | 1.34 ms                                                                | 1.35 ms: 1.01x slower                                                  |
| sqlglot_optimize         | 58.9 ms                                                                | 59.5 ms: 1.01x slower                                                  |
| pycparser                | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                                 |
| typing_runtime_protocols | 117 us                                                                 | 118 us: 1.01x slower                                                   |
| create_gc_cycles         | 1.47 ms                                                                | 1.48 ms: 1.01x slower                                                  |
| async_generators         | 453 ms                                                                 | 457 ms: 1.01x slower                                                   |
| pprint_pformat           | 1.74 sec                                                               | 1.75 sec: 1.01x slower                                                 |
| logging_format           | 6.80 us                                                                | 6.87 us: 1.01x slower                                                  |
| tornado_http             | 98.2 ms                                                                | 99.4 ms: 1.01x slower                                                  |
| richards_super           | 56.0 ms                                                                | 56.8 ms: 1.01x slower                                                  |
| scimark_monte_carlo      | 84.8 ms                                                                | 86.0 ms: 1.01x slower                                                  |
| richards                 | 49.7 ms                                                                | 50.4 ms: 1.01x slower                                                  |
| chameleon                | 7.27 ms                                                                | 7.38 ms: 1.01x slower                                                  |
| scimark_lu               | 119 ms                                                                 | 121 ms: 1.01x slower                                                   |
| comprehensions           | 22.5 us                                                                | 22.8 us: 1.01x slower                                                  |
| xml_etree_parse          | 157 ms                                                                 | 159 ms: 1.01x slower                                                   |
| chaos                    | 76.0 ms                                                                | 77.1 ms: 1.01x slower                                                  |
| deepcopy_reduce          | 3.16 us                                                                | 3.21 us: 1.02x slower                                                  |
| coverage                 | 94.7 ms                                                                | 96.3 ms: 1.02x slower                                                  |
| json_dumps               | 10.6 ms                                                                | 10.8 ms: 1.02x slower                                                  |
| deepcopy_memo            | 41.9 us                                                                | 42.6 us: 1.02x slower                                                  |
| spectral_norm            | 157 ms                                                                 | 159 ms: 1.02x slower                                                   |
| mako                     | 14.7 ms                                                                | 14.9 ms: 1.02x slower                                                  |
| hexiom                   | 9.02 ms                                                                | 9.21 ms: 1.02x slower                                                  |
| json_loads               | 28.2 us                                                                | 28.8 us: 1.02x slower                                                  |
| scimark_sor              | 132 ms                                                                 | 135 ms: 1.02x slower                                                   |
| raytrace                 | 304 ms                                                                 | 311 ms: 1.02x slower                                                   |
| unpickle                 | 14.7 us                                                                | 15.0 us: 1.03x slower                                                  |
| mdp                      | 2.66 sec                                                               | 2.78 sec: 1.04x slower                                                 |
| scimark_sparse_mat_mult  | 6.30 ms                                                                | 6.61 ms: 1.05x slower                                                  |
| deltablue                | 4.87 ms                                                                | 5.14 ms: 1.06x slower                                                  |
| float                    | 94.0 ms                                                                | 99.6 ms: 1.06x slower                                                  |
| unpack_sequence          | 41.7 ns                                                                | 52.1 ns: 1.25x slower                                                  |
| Geometric mean           | (ref)                                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (21): telco, sympy_expand, async_tree_cpu_io_mixed_tg, pickle_list, async_tree_none_tg, async_tree_none, asyncio_websockets, xml_etree_generate, bench_mp_pool, dask, tomli_loads, async_tree_memoization, async_tree_memoization_tg, dulwich_log, async_tree_cpu_io_mixed, pickle_pure_python, mypy2, logging_simple, json, sqlite_synth, sympy_str


# HPT report

- Reliability score: 99.91% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x