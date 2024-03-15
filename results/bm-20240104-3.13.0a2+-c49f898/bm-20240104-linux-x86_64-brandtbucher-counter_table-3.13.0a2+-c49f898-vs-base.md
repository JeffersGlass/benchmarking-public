# Results vs. base

- fork: brandtbucher
- ref: counter_table
- machine: linux-x86_64
- commit hash: c49f898
- commit date: 2024-01-04
- overall geometric mean: 1.01x slower
- HPT reliability: 99.96%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 263 ms                                                                 | 266 ms: 1.01x slower                                                  |
| docutils       | 2.61 sec                                                               | 2.62 sec: 1.00x slower                                                |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                          |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_io, async_tree_io_tg, async_tree_cpu_io_mixed_tg, async_tree_none_tg, async_tree_cpu_io_mixed, async_tree_none, async_tree_memoization, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 195 ms                                                                 | 187 ms: 1.04x faster                                                  |
| float          | 79.4 ms                                                                | 80.2 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                          |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 3.77 ms                                                                | 3.60 ms: 1.04x faster                                                 |
| regex_dna      | 224 ms                                                                 | 217 ms: 1.03x faster                                                  |
| regex_v8       | 25.3 ms                                                                | 25.4 ms: 1.01x slower                                                 |
| regex_compile  | 129 ms                                                                 | 131 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|----------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle               | 11.5 us                                                                | 11.3 us: 1.02x faster                                                 |
| pickle_pure_python   | 300 us                                                                 | 295 us: 1.01x faster                                                  |
| pickle_list          | 4.92 us                                                                | 4.87 us: 1.01x faster                                                 |
| xml_etree_parse      | 156 ms                                                                 | 157 ms: 1.01x slower                                                  |
| tomli_loads          | 2.11 sec                                                               | 2.13 sec: 1.01x slower                                                |
| xml_etree_iterparse  | 104 ms                                                                 | 106 ms: 1.02x slower                                                  |
| unpickle_pure_python | 213 us                                                                 | 218 us: 1.02x slower                                                  |
| xml_etree_generate   | 84.9 ms                                                                | 87.2 ms: 1.03x slower                                                 |
| xml_etree_process    | 58.5 ms                                                                | 60.1 ms: 1.03x slower                                                 |
| unpickle_list        | 5.13 us                                                                | 5.29 us: 1.03x slower                                                 |
| pickle_dict          | 33.4 us                                                                | 34.9 us: 1.05x slower                                                 |
| unpickle             | 15.0 us                                                                | 15.8 us: 1.05x slower                                                 |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                          |

Benchmark hidden because not significant (2): json_loads, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                 |
| python_startup_no_site | 8.70 ms                                                                | 8.82 ms: 1.01x slower                                                 |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|-----------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako      | 11.1 ms                                                                | 10.9 ms: 1.02x faster                                                 |

All benchmarks:
===============

| Benchmark               | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240104-linux-x86_64-brandtbucher-counter_table-3.13.0a2+-c49f898 |
|-------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------:|
| scimark_sor             | 129 ms                                                                 | 121 ms: 1.07x faster                                                  |
| regex_effbot            | 3.77 ms                                                                | 3.60 ms: 1.04x faster                                                 |
| pidigits                | 195 ms                                                                 | 187 ms: 1.04x faster                                                  |
| spectral_norm           | 114 ms                                                                 | 110 ms: 1.04x faster                                                  |
| gc_traversal            | 3.72 ms                                                                | 3.60 ms: 1.03x faster                                                 |
| regex_dna               | 224 ms                                                                 | 217 ms: 1.03x faster                                                  |
| fannkuch                | 400 ms                                                                 | 392 ms: 1.02x faster                                                  |
| scimark_monte_carlo     | 68.3 ms                                                                | 66.9 ms: 1.02x faster                                                 |
| pickle                  | 11.5 us                                                                | 11.3 us: 1.02x faster                                                 |
| mako                    | 11.1 ms                                                                | 10.9 ms: 1.02x faster                                                 |
| pickle_pure_python      | 300 us                                                                 | 295 us: 1.01x faster                                                  |
| telco                   | 8.32 ms                                                                | 8.21 ms: 1.01x faster                                                 |
| pickle_list             | 4.92 us                                                                | 4.87 us: 1.01x faster                                                 |
| nqueens                 | 83.9 ms                                                                | 83.1 ms: 1.01x faster                                                 |
| coverage                | 96.2 ms                                                                | 95.4 ms: 1.01x faster                                                 |
| pycparser               | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                |
| chaos                   | 59.2 ms                                                                | 58.8 ms: 1.01x faster                                                 |
| create_gc_cycles        | 1.47 ms                                                                | 1.47 ms: 1.01x faster                                                 |
| asyncio_tcp_ssl         | 1.78 sec                                                               | 1.79 sec: 1.00x slower                                                |
| docutils                | 2.61 sec                                                               | 2.62 sec: 1.00x slower                                                |
| crypto_pyaes            | 71.3 ms                                                                | 71.5 ms: 1.00x slower                                                 |
| raytrace                | 260 ms                                                                 | 261 ms: 1.00x slower                                                  |
| regex_v8                | 25.3 ms                                                                | 25.4 ms: 1.01x slower                                                 |
| sqlglot_transpile       | 1.57 ms                                                                | 1.58 ms: 1.01x slower                                                 |
| sqlglot_normalize       | 106 ms                                                                 | 107 ms: 1.01x slower                                                  |
| pprint_pformat          | 1.49 sec                                                               | 1.50 sec: 1.01x slower                                                |
| logging_simple          | 5.60 us                                                                | 5.64 us: 1.01x slower                                                 |
| asyncio_tcp             | 484 ms                                                                 | 488 ms: 1.01x slower                                                  |
| xml_etree_parse         | 156 ms                                                                 | 157 ms: 1.01x slower                                                  |
| logging_format          | 6.18 us                                                                | 6.24 us: 1.01x slower                                                 |
| tomli_loads             | 2.11 sec                                                               | 2.13 sec: 1.01x slower                                                |
| 2to3                    | 263 ms                                                                 | 266 ms: 1.01x slower                                                  |
| float                   | 79.4 ms                                                                | 80.2 ms: 1.01x slower                                                 |
| sqlite_synth            | 2.82 us                                                                | 2.85 us: 1.01x slower                                                 |
| deepcopy_reduce         | 3.05 us                                                                | 3.09 us: 1.01x slower                                                 |
| python_startup          | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                 |
| dulwich_log             | 65.4 ms                                                                | 66.2 ms: 1.01x slower                                                 |
| hexiom                  | 6.20 ms                                                                | 6.27 ms: 1.01x slower                                                 |
| bench_thread_pool       | 828 us                                                                 | 838 us: 1.01x slower                                                  |
| regex_compile           | 129 ms                                                                 | 131 ms: 1.01x slower                                                  |
| sqlglot_optimize        | 53.4 ms                                                                | 54.1 ms: 1.01x slower                                                 |
| python_startup_no_site  | 8.70 ms                                                                | 8.82 ms: 1.01x slower                                                 |
| scimark_fft             | 352 ms                                                                 | 357 ms: 1.01x slower                                                  |
| sqlglot_parse           | 1.24 ms                                                                | 1.25 ms: 1.02x slower                                                 |
| pprint_safe_repr        | 728 ms                                                                 | 739 ms: 1.02x slower                                                  |
| deepcopy                | 345 us                                                                 | 350 us: 1.02x slower                                                  |
| sympy_integrate         | 19.5 ms                                                                | 19.8 ms: 1.02x slower                                                 |
| xml_etree_iterparse     | 104 ms                                                                 | 106 ms: 1.02x slower                                                  |
| deepcopy_memo           | 37.9 us                                                                | 38.6 us: 1.02x slower                                                 |
| unpickle_pure_python    | 213 us                                                                 | 218 us: 1.02x slower                                                  |
| meteor_contest          | 107 ms                                                                 | 110 ms: 1.02x slower                                                  |
| richards_super          | 53.8 ms                                                                | 55.1 ms: 1.03x slower                                                 |
| xml_etree_generate      | 84.9 ms                                                                | 87.2 ms: 1.03x slower                                                 |
| async_generators        | 438 ms                                                                 | 450 ms: 1.03x slower                                                  |
| logging_silent          | 101 ns                                                                 | 104 ns: 1.03x slower                                                  |
| xml_etree_process       | 58.5 ms                                                                | 60.1 ms: 1.03x slower                                                 |
| scimark_sparse_mat_mult | 4.93 ms                                                                | 5.07 ms: 1.03x slower                                                 |
| unpickle_list           | 5.13 us                                                                | 5.29 us: 1.03x slower                                                 |
| comprehensions          | 16.0 us                                                                | 16.6 us: 1.03x slower                                                 |
| richards                | 47.4 ms                                                                | 49.1 ms: 1.04x slower                                                 |
| scimark_lu              | 111 ms                                                                 | 116 ms: 1.04x slower                                                  |
| pickle_dict             | 33.4 us                                                                | 34.9 us: 1.05x slower                                                 |
| unpickle                | 15.0 us                                                                | 15.8 us: 1.05x slower                                                 |
| mdp                     | 2.53 sec                                                               | 2.73 sec: 1.08x slower                                                |
| unpack_sequence         | 40.5 ns                                                                | 49.7 ns: 1.23x slower                                                 |
| Geometric mean          | (ref)                                                                  | 1.01x slower                                                          |

Benchmark hidden because not significant (28): coroutines, pathlib, go, async_tree_io, pyflate, sympy_expand, chameleon, typing_runtime_protocols, nbody, bench_mp_pool, async_tree_io_tg, async_tree_cpu_io_mixed_tg, asyncio_websockets, sympy_str, generators, sympy_sum, deltablue, json, mypy2, async_tree_none_tg, tornado_http, async_tree_cpu_io_mixed, json_loads, json_dumps, async_tree_none, async_tree_memoization, dask, async_tree_memoization_tg


# HPT report

- Reliability score: 99.96% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x