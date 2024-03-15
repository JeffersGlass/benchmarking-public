# Results vs. base

- fork: mdboom
- ref: rare_event_stats
- machine: linux-x86_64
- commit hash: 937bd66
- commit date: 2024-01-22
- overall geometric mean: 1.00x faster
- HPT reliability: 54.04%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 262 ms                                                                 | 264 ms: 1.00x slower                                               |
| chameleon      | 6.95 ms                                                                | 7.06 ms: 1.02x slower                                              |
| docutils       | 2.61 sec                                                               | 2.60 sec: 1.01x faster                                             |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                       |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_io_tg | 1.19 sec                                                               | 1.19 sec: 1.00x slower                                             |
| Geometric mean   | (ref)                                                                  | 1.00x slower                                                       |

Benchmark hidden because not significant (7): async_tree_io, async_tree_cpu_io_mixed, async_tree_none, async_tree_memoization_tg, async_tree_none_tg, async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 89.4 ms                                                                | 86.1 ms: 1.04x faster                                              |
| pidigits       | 188 ms                                                                 | 187 ms: 1.00x faster                                               |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                       |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_effbot   | 3.74 ms                                                                | 3.54 ms: 1.06x faster                                              |
| regex_v8       | 25.8 ms                                                                | 25.5 ms: 1.01x faster                                              |
| regex_dna      | 223 ms                                                                 | 222 ms: 1.00x faster                                               |
| regex_compile  | 129 ms                                                                 | 130 ms: 1.01x slower                                               |
| Geometric mean | (ref)                                                                  | 1.02x faster                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| unpickle_pure_python | 214 us                                                                 | 212 us: 1.01x faster                                               |
| json_dumps           | 10.5 ms                                                                | 10.4 ms: 1.01x faster                                              |
| pickle               | 11.8 us                                                                | 11.7 us: 1.01x faster                                              |
| xml_etree_process    | 58.4 ms                                                                | 58.6 ms: 1.00x slower                                              |
| tomli_loads          | 2.11 sec                                                               | 2.12 sec: 1.01x slower                                             |
| pickle_dict          | 34.5 us                                                                | 34.8 us: 1.01x slower                                              |
| unpickle_list        | 5.25 us                                                                | 5.41 us: 1.03x slower                                              |
| pickle_list          | 4.94 us                                                                | 5.27 us: 1.07x slower                                              |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                       |

Benchmark hidden because not significant (6): json_loads, pickle_pure_python, xml_etree_iterparse, xml_etree_generate, unpickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup_no_site | 8.71 ms                                                                | 8.68 ms: 1.00x faster                                              |
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                              |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|-----------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 11.1 ms                                                                | 11.1 ms: 1.01x faster                                              |

All benchmarks:
===============

| Benchmark               | bm-20240119-linux-x86_64-python-05e47202a34e6ae05e69-3.13.0a3+-05e4720 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|-------------------------|:----------------------------------------------------------------------:|:------------------------------------------------------------------:|
| unpack_sequence         | 48.1 ns                                                                | 45.2 ns: 1.06x faster                                              |
| regex_effbot            | 3.74 ms                                                                | 3.54 ms: 1.06x faster                                              |
| gc_traversal            | 4.16 ms                                                                | 3.94 ms: 1.05x faster                                              |
| scimark_sor             | 127 ms                                                                 | 121 ms: 1.05x faster                                               |
| nbody                   | 89.4 ms                                                                | 86.1 ms: 1.04x faster                                              |
| hexiom                  | 6.11 ms                                                                | 5.89 ms: 1.04x faster                                              |
| pycparser               | 1.19 sec                                                               | 1.15 sec: 1.03x faster                                             |
| scimark_monte_carlo     | 68.5 ms                                                                | 66.4 ms: 1.03x faster                                              |
| telco                   | 8.48 ms                                                                | 8.24 ms: 1.03x faster                                              |
| raytrace                | 264 ms                                                                 | 257 ms: 1.03x faster                                               |
| scimark_fft             | 359 ms                                                                 | 350 ms: 1.02x faster                                               |
| spectral_norm           | 110 ms                                                                 | 108 ms: 1.02x faster                                               |
| richards                | 48.1 ms                                                                | 47.4 ms: 1.02x faster                                              |
| go                      | 139 ms                                                                 | 137 ms: 1.01x faster                                               |
| regex_v8                | 25.8 ms                                                                | 25.5 ms: 1.01x faster                                              |
| richards_super          | 54.0 ms                                                                | 53.3 ms: 1.01x faster                                              |
| crypto_pyaes            | 71.7 ms                                                                | 70.9 ms: 1.01x faster                                              |
| pyflate                 | 465 ms                                                                 | 460 ms: 1.01x faster                                               |
| unpickle_pure_python    | 214 us                                                                 | 212 us: 1.01x faster                                               |
| fannkuch                | 407 ms                                                                 | 403 ms: 1.01x faster                                               |
| nqueens                 | 80.9 ms                                                                | 80.1 ms: 1.01x faster                                              |
| logging_format          | 6.32 us                                                                | 6.26 us: 1.01x faster                                              |
| json_dumps              | 10.5 ms                                                                | 10.4 ms: 1.01x faster                                              |
| comprehensions          | 16.2 us                                                                | 16.1 us: 1.01x faster                                              |
| sqlite_synth            | 2.84 us                                                                | 2.81 us: 1.01x faster                                              |
| deltablue               | 3.17 ms                                                                | 3.15 ms: 1.01x faster                                              |
| pickle                  | 11.8 us                                                                | 11.7 us: 1.01x faster                                              |
| mako                    | 11.1 ms                                                                | 11.1 ms: 1.01x faster                                              |
| chaos                   | 59.9 ms                                                                | 59.5 ms: 1.01x faster                                              |
| dulwich_log             | 65.7 ms                                                                | 65.3 ms: 1.01x faster                                              |
| docutils                | 2.61 sec                                                               | 2.60 sec: 1.01x faster                                             |
| regex_dna               | 223 ms                                                                 | 222 ms: 1.00x faster                                               |
| pidigits                | 188 ms                                                                 | 187 ms: 1.00x faster                                               |
| python_startup_no_site  | 8.71 ms                                                                | 8.68 ms: 1.00x faster                                              |
| python_startup          | 10.1 ms                                                                | 10.1 ms: 1.00x faster                                              |
| asyncio_tcp_ssl         | 1.78 sec                                                               | 1.78 sec: 1.00x faster                                             |
| meteor_contest          | 108 ms                                                                 | 108 ms: 1.00x slower                                               |
| asyncio_tcp             | 479 ms                                                                 | 480 ms: 1.00x slower                                               |
| sqlglot_normalize       | 107 ms                                                                 | 107 ms: 1.00x slower                                               |
| async_tree_io_tg        | 1.19 sec                                                               | 1.19 sec: 1.00x slower                                             |
| sympy_sum               | 148 ms                                                                 | 149 ms: 1.00x slower                                               |
| xml_etree_process       | 58.4 ms                                                                | 58.6 ms: 1.00x slower                                              |
| 2to3                    | 262 ms                                                                 | 264 ms: 1.00x slower                                               |
| regex_compile           | 129 ms                                                                 | 130 ms: 1.01x slower                                               |
| sqlglot_optimize        | 53.9 ms                                                                | 54.2 ms: 1.01x slower                                              |
| sqlglot_transpile       | 1.57 ms                                                                | 1.58 ms: 1.01x slower                                              |
| tomli_loads             | 2.11 sec                                                               | 2.12 sec: 1.01x slower                                             |
| generators              | 29.0 ms                                                                | 29.3 ms: 1.01x slower                                              |
| logging_simple          | 5.71 us                                                                | 5.76 us: 1.01x slower                                              |
| sqlglot_parse           | 1.24 ms                                                                | 1.25 ms: 1.01x slower                                              |
| mdp                     | 2.70 sec                                                               | 2.73 sec: 1.01x slower                                             |
| pickle_dict             | 34.5 us                                                                | 34.8 us: 1.01x slower                                              |
| sympy_expand            | 459 ms                                                                 | 464 ms: 1.01x slower                                               |
| chameleon               | 6.95 ms                                                                | 7.06 ms: 1.02x slower                                              |
| pathlib                 | 18.0 ms                                                                | 18.3 ms: 1.02x slower                                              |
| deepcopy_reduce         | 3.03 us                                                                | 3.07 us: 1.02x slower                                              |
| logging_silent          | 103 ns                                                                 | 106 ns: 1.03x slower                                               |
| unpickle_list           | 5.25 us                                                                | 5.41 us: 1.03x slower                                              |
| sympy_str               | 270 ms                                                                 | 279 ms: 1.03x slower                                               |
| pickle_list             | 4.94 us                                                                | 5.27 us: 1.07x slower                                              |
| scimark_sparse_mat_mult | 4.60 ms                                                                | 5.05 ms: 1.10x slower                                              |
| Geometric mean          | (ref)                                                                  | 1.00x faster                                                       |

Benchmark hidden because not significant (32): json_loads, coverage, json, dask, async_generators, bench_mp_pool, async_tree_io, pickle_pure_python, xml_etree_iterparse, tornado_http, async_tree_cpu_io_mixed, bench_thread_pool, async_tree_none, coroutines, asyncio_websockets, sympy_integrate, deepcopy_memo, create_gc_cycles, async_tree_memoization_tg, async_tree_none_tg, scimark_lu, mypy2, pprint_pformat, typing_runtime_protocols, float, xml_etree_generate, deepcopy, pprint_safe_repr, async_tree_memoization, unpickle, async_tree_cpu_io_mixed_tg, xml_etree_parse


# HPT report

- Reliability score: 54.04% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x