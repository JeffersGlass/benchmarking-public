# Results vs. base

- fork: python
- ref: e2a3e4b7488aff6fdc70
- machine: linux-x86_64
- commit hash: e2a3e4b
- commit date: 2024-02-28
- overall geometric mean: 1.00x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 261 ms: 1.01x faster                                                   |
| chameleon      | 6.91 ms                                                | 6.82 ms: 1.01x faster                                                  |
| docutils       | 2.59 sec                                               | 2.56 sec: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|--------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_io      | 1.17 sec                                               | 1.16 sec: 1.01x faster                                                 |
| async_tree_none_tg | 445 ms                                                 | 442 ms: 1.01x faster                                                   |
| async_tree_io_tg   | 1.19 sec                                               | 1.19 sec: 1.00x faster                                                 |
| Geometric mean     | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (5): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, async_tree_none, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| float          | 80.4 ms                                                | 79.0 ms: 1.02x faster                                                  |
| nbody          | 88.0 ms                                                | 86.5 ms: 1.02x faster                                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x slower                                                   |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 132 ms                                                 | 131 ms: 1.01x faster                                                   |
| regex_v8       | 24.6 ms                                                | 24.8 ms: 1.01x slower                                                  |
| regex_dna      | 216 ms                                                 | 219 ms: 1.01x slower                                                   |
| regex_effbot   | 3.56 ms                                                | 3.73 ms: 1.05x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_loads           | 27.6 us                                                | 27.1 us: 1.02x faster                                                  |
| xml_etree_iterparse  | 106 ms                                                 | 104 ms: 1.02x faster                                                   |
| xml_etree_parse      | 157 ms                                                 | 156 ms: 1.01x faster                                                   |
| xml_etree_process    | 58.3 ms                                                | 57.8 ms: 1.01x faster                                                  |
| unpickle_pure_python | 214 us                                                 | 212 us: 1.01x faster                                                   |
| pickle_pure_python   | 295 us                                                 | 292 us: 1.01x faster                                                   |
| unpickle_list        | 4.95 us                                                | 4.92 us: 1.01x faster                                                  |
| xml_etree_generate   | 85.0 ms                                                | 84.7 ms: 1.00x faster                                                  |
| pickle               | 11.4 us                                                | 11.7 us: 1.03x slower                                                  |
| pickle_dict          | 33.1 us                                                | 35.1 us: 1.06x slower                                                  |
| pickle_list          | 4.91 us                                                | 5.29 us: 1.08x slower                                                  |
| unpickle             | 14.5 us                                                | 15.6 us: 1.08x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (2): json_dumps, tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                | 10.2 ms: 1.01x slower                                                  |
| python_startup_no_site | 8.75 ms                                                | 8.81 ms: 1.01x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.4 ms                                                | 11.0 ms: 1.04x faster                                                  |

All benchmarks:
===============

| Benchmark               | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| unpack_sequence         | 47.4 ns                                                | 42.5 ns: 1.12x faster                                                  |
| logging_silent          | 102 ns                                                 | 95.1 ns: 1.08x faster                                                  |
| pyflate                 | 466 ms                                                 | 442 ms: 1.05x faster                                                   |
| pycparser               | 1.21 sec                                               | 1.15 sec: 1.05x faster                                                 |
| mako                    | 11.4 ms                                                | 11.0 ms: 1.04x faster                                                  |
| scimark_sor             | 124 ms                                                 | 120 ms: 1.04x faster                                                   |
| fannkuch                | 388 ms                                                 | 376 ms: 1.03x faster                                                   |
| go                      | 138 ms                                                 | 135 ms: 1.02x faster                                                   |
| scimark_sparse_mat_mult | 4.69 ms                                                | 4.60 ms: 1.02x faster                                                  |
| scimark_fft             | 360 ms                                                 | 353 ms: 1.02x faster                                                   |
| meteor_contest          | 107 ms                                                 | 105 ms: 1.02x faster                                                   |
| hexiom                  | 5.97 ms                                                | 5.86 ms: 1.02x faster                                                  |
| sqlite_synth            | 2.88 us                                                | 2.83 us: 1.02x faster                                                  |
| float                   | 80.4 ms                                                | 79.0 ms: 1.02x faster                                                  |
| json                    | 5.05 ms                                                | 4.96 ms: 1.02x faster                                                  |
| nbody                   | 88.0 ms                                                | 86.5 ms: 1.02x faster                                                  |
| nqueens                 | 78.9 ms                                                | 77.5 ms: 1.02x faster                                                  |
| json_loads              | 27.6 us                                                | 27.1 us: 1.02x faster                                                  |
| xml_etree_iterparse     | 106 ms                                                 | 104 ms: 1.02x faster                                                   |
| chameleon               | 6.91 ms                                                | 6.82 ms: 1.01x faster                                                  |
| pprint_safe_repr        | 724 ms                                                 | 715 ms: 1.01x faster                                                   |
| raytrace                | 263 ms                                                 | 260 ms: 1.01x faster                                                   |
| regex_compile           | 132 ms                                                 | 131 ms: 1.01x faster                                                   |
| sqlglot_normalize       | 105 ms                                                 | 104 ms: 1.01x faster                                                   |
| sqlglot_optimize        | 53.4 ms                                                | 52.8 ms: 1.01x faster                                                  |
| pathlib                 | 18.0 ms                                                | 17.9 ms: 1.01x faster                                                  |
| pprint_pformat          | 1.49 sec                                               | 1.47 sec: 1.01x faster                                                 |
| docutils                | 2.59 sec                                               | 2.56 sec: 1.01x faster                                                 |
| xml_etree_parse         | 157 ms                                                 | 156 ms: 1.01x faster                                                   |
| xml_etree_process       | 58.3 ms                                                | 57.8 ms: 1.01x faster                                                  |
| unpickle_pure_python    | 214 us                                                 | 212 us: 1.01x faster                                                   |
| 2to3                    | 264 ms                                                 | 261 ms: 1.01x faster                                                   |
| dulwich_log             | 65.6 ms                                                | 65.0 ms: 1.01x faster                                                  |
| create_gc_cycles        | 1.50 ms                                                | 1.48 ms: 1.01x faster                                                  |
| sqlglot_transpile       | 1.57 ms                                                | 1.56 ms: 1.01x faster                                                  |
| sympy_sum               | 148 ms                                                 | 147 ms: 1.01x faster                                                   |
| pickle_pure_python      | 295 us                                                 | 292 us: 1.01x faster                                                   |
| sqlglot_parse           | 1.25 ms                                                | 1.24 ms: 1.01x faster                                                  |
| unpickle_list           | 4.95 us                                                | 4.92 us: 1.01x faster                                                  |
| sympy_integrate         | 19.6 ms                                                | 19.4 ms: 1.01x faster                                                  |
| async_generators        | 448 ms                                                 | 445 ms: 1.01x faster                                                   |
| async_tree_io           | 1.17 sec                                               | 1.16 sec: 1.01x faster                                                 |
| async_tree_none_tg      | 445 ms                                                 | 442 ms: 1.01x faster                                                   |
| deltablue               | 3.16 ms                                                | 3.15 ms: 1.00x faster                                                  |
| xml_etree_generate      | 85.0 ms                                                | 84.7 ms: 1.00x faster                                                  |
| async_tree_io_tg        | 1.19 sec                                               | 1.19 sec: 1.00x faster                                                 |
| bench_thread_pool       | 816 us                                                 | 814 us: 1.00x faster                                                   |
| pidigits                | 187 ms                                                 | 187 ms: 1.00x slower                                                   |
| generators              | 29.3 ms                                                | 29.4 ms: 1.00x slower                                                  |
| comprehensions          | 16.0 us                                                | 16.1 us: 1.00x slower                                                  |
| crypto_pyaes            | 69.6 ms                                                | 69.9 ms: 1.00x slower                                                  |
| python_startup          | 10.1 ms                                                | 10.2 ms: 1.01x slower                                                  |
| logging_simple          | 5.60 us                                                | 5.64 us: 1.01x slower                                                  |
| python_startup_no_site  | 8.75 ms                                                | 8.81 ms: 1.01x slower                                                  |
| coroutines              | 22.1 ms                                                | 22.3 ms: 1.01x slower                                                  |
| regex_v8                | 24.6 ms                                                | 24.8 ms: 1.01x slower                                                  |
| deepcopy_memo           | 37.2 us                                                | 37.5 us: 1.01x slower                                                  |
| scimark_monte_carlo     | 66.9 ms                                                | 67.5 ms: 1.01x slower                                                  |
| deepcopy                | 344 us                                                 | 347 us: 1.01x slower                                                   |
| regex_dna               | 216 ms                                                 | 219 ms: 1.01x slower                                                   |
| logging_format          | 6.14 us                                                | 6.24 us: 1.02x slower                                                  |
| richards_super          | 52.9 ms                                                | 53.8 ms: 1.02x slower                                                  |
| telco                   | 8.20 ms                                                | 8.34 ms: 1.02x slower                                                  |
| coverage                | 93.0 ms                                                | 95.2 ms: 1.02x slower                                                  |
| scimark_lu              | 110 ms                                                 | 113 ms: 1.03x slower                                                   |
| pickle                  | 11.4 us                                                | 11.7 us: 1.03x slower                                                  |
| regex_effbot            | 3.56 ms                                                | 3.73 ms: 1.05x slower                                                  |
| pickle_dict             | 33.1 us                                                | 35.1 us: 1.06x slower                                                  |
| gc_traversal            | 3.75 ms                                                | 4.00 ms: 1.07x slower                                                  |
| pickle_list             | 4.91 us                                                | 5.29 us: 1.08x slower                                                  |
| unpickle                | 14.5 us                                                | 15.6 us: 1.08x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (21): spectral_norm, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, mypy2, sympy_expand, sympy_str, async_tree_none, async_tree_memoization, deepcopy_reduce, asyncio_tcp, asyncio_websockets, mdp, chaos, tornado_http, bench_mp_pool, asyncio_tcp_ssl, typing_runtime_protocols, json_dumps, richards, tomli_loads


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x