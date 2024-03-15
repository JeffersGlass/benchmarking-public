# Results vs. base

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.00x faster
- HPT reliability: 93.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 309 ms                                                                       | 310 ms: 1.01x slower                                                       |
| chameleon      | 7.43 ms                                                                      | 7.65 ms: 1.03x slower                                                      |
| Geometric mean | (ref)                                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none_tg      | 436 ms                                                                       | 440 ms: 1.01x slower                                                       |
| async_tree_cpu_io_mixed | 701 ms                                                                       | 707 ms: 1.01x slower                                                       |
| async_tree_memoization  | 548 ms                                                                       | 555 ms: 1.01x slower                                                       |
| async_tree_io_tg        | 1.08 sec                                                                     | 1.09 sec: 1.01x slower                                                     |
| async_tree_io           | 1.08 sec                                                                     | 1.09 sec: 1.01x slower                                                     |
| async_tree_none         | 435 ms                                                                       | 443 ms: 1.02x slower                                                       |
| Geometric mean          | (ref)                                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 83.9 ms                                                                      | 80.2 ms: 1.05x faster                                                      |
| nbody          | 103 ms                                                                       | 102 ms: 1.01x faster                                                       |
| pidigits       | 262 ms                                                                       | 262 ms: 1.00x faster                                                       |
| Geometric mean | (ref)                                                                        | 1.02x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_v8       | 25.7 ms                                                                      | 25.5 ms: 1.01x faster                                                      |
| regex_effbot   | 3.52 ms                                                                      | 3.50 ms: 1.01x faster                                                      |
| regex_compile  | 153 ms                                                                       | 152 ms: 1.00x faster                                                       |
| Geometric mean | (ref)                                                                        | 1.00x faster                                                               |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpickle_pure_python | 260 us                                                                       | 240 us: 1.08x faster                                                       |
| json_loads           | 25.1 us                                                                      | 24.7 us: 1.01x faster                                                      |
| unpickle             | 15.0 us                                                                      | 14.8 us: 1.01x faster                                                      |
| pickle_list          | 4.30 us                                                                      | 4.27 us: 1.01x faster                                                      |
| unpickle_list        | 4.66 us                                                                      | 4.68 us: 1.00x slower                                                      |
| xml_etree_process    | 59.0 ms                                                                      | 59.4 ms: 1.01x slower                                                      |
| tomli_loads          | 2.35 sec                                                                     | 2.37 sec: 1.01x slower                                                     |
| pickle               | 10.3 us                                                                      | 10.3 us: 1.01x slower                                                      |
| pickle_pure_python   | 310 us                                                                       | 315 us: 1.01x slower                                                       |
| xml_etree_parse      | 144 ms                                                                       | 151 ms: 1.05x slower                                                       |
| pickle_dict          | 30.5 us                                                                      | 32.2 us: 1.06x slower                                                      |
| Geometric mean       | (ref)                                                                        | 1.00x slower                                                               |

Benchmark hidden because not significant (3): xml_etree_generate, json_dumps, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 14.8 ms                                                                      | 15.6 ms: 1.05x slower                                                      |
| python_startup_no_site | 13.2 ms                                                                      | 14.1 ms: 1.06x slower                                                      |
| Geometric mean         | (ref)                                                                        | 1.06x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 11.6 ms                                                                      | 10.7 ms: 1.09x faster                                                      |

All benchmarks:
===============

| Benchmark               | bm-20240221-pythonperf2-x86_64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| scimark_sparse_mat_mult | 5.14 ms                                                                      | 4.36 ms: 1.18x faster                                                      |
| unpack_sequence         | 92.0 ns                                                                      | 79.7 ns: 1.15x faster                                                      |
| spectral_norm           | 110 ms                                                                       | 96.2 ms: 1.15x faster                                                      |
| mako                    | 11.6 ms                                                                      | 10.7 ms: 1.09x faster                                                      |
| unpickle_pure_python    | 260 us                                                                       | 240 us: 1.08x faster                                                       |
| hexiom                  | 8.33 ms                                                                      | 7.90 ms: 1.05x faster                                                      |
| comprehensions          | 20.1 us                                                                      | 19.1 us: 1.05x faster                                                      |
| pyflate                 | 573 ms                                                                       | 547 ms: 1.05x faster                                                       |
| scimark_fft             | 355 ms                                                                       | 339 ms: 1.05x faster                                                       |
| float                   | 83.9 ms                                                                      | 80.2 ms: 1.05x faster                                                      |
| fannkuch                | 442 ms                                                                       | 431 ms: 1.02x faster                                                       |
| nqueens                 | 107 ms                                                                       | 104 ms: 1.02x faster                                                       |
| richards                | 55.4 ms                                                                      | 54.4 ms: 1.02x faster                                                      |
| json_loads              | 25.1 us                                                                      | 24.7 us: 1.01x faster                                                      |
| unpickle                | 15.0 us                                                                      | 14.8 us: 1.01x faster                                                      |
| richards_super          | 61.2 ms                                                                      | 60.5 ms: 1.01x faster                                                      |
| meteor_contest          | 134 ms                                                                       | 133 ms: 1.01x faster                                                       |
| deltablue               | 3.79 ms                                                                      | 3.75 ms: 1.01x faster                                                      |
| regex_v8                | 25.7 ms                                                                      | 25.5 ms: 1.01x faster                                                      |
| chaos                   | 69.8 ms                                                                      | 69.3 ms: 1.01x faster                                                      |
| nbody                   | 103 ms                                                                       | 102 ms: 1.01x faster                                                       |
| pickle_list             | 4.30 us                                                                      | 4.27 us: 1.01x faster                                                      |
| regex_effbot            | 3.52 ms                                                                      | 3.50 ms: 1.01x faster                                                      |
| raytrace                | 311 ms                                                                       | 310 ms: 1.01x faster                                                       |
| mdp                     | 2.64 sec                                                                     | 2.62 sec: 1.01x faster                                                     |
| json                    | 5.32 ms                                                                      | 5.30 ms: 1.00x faster                                                      |
| regex_compile           | 153 ms                                                                       | 152 ms: 1.00x faster                                                       |
| coroutines              | 22.5 ms                                                                      | 22.4 ms: 1.00x faster                                                      |
| crypto_pyaes            | 80.0 ms                                                                      | 79.7 ms: 1.00x faster                                                      |
| sqlite_synth            | 2.76 us                                                                      | 2.76 us: 1.00x faster                                                      |
| scimark_monte_carlo     | 83.8 ms                                                                      | 83.6 ms: 1.00x faster                                                      |
| pidigits                | 262 ms                                                                       | 262 ms: 1.00x faster                                                       |
| unpickle_list           | 4.66 us                                                                      | 4.68 us: 1.00x slower                                                      |
| 2to3                    | 309 ms                                                                       | 310 ms: 1.01x slower                                                       |
| xml_etree_process       | 59.0 ms                                                                      | 59.4 ms: 1.01x slower                                                      |
| tomli_loads             | 2.35 sec                                                                     | 2.37 sec: 1.01x slower                                                     |
| pathlib                 | 19.1 ms                                                                      | 19.2 ms: 1.01x slower                                                      |
| sympy_integrate         | 24.7 ms                                                                      | 24.9 ms: 1.01x slower                                                      |
| create_gc_cycles        | 1.57 ms                                                                      | 1.59 ms: 1.01x slower                                                      |
| sympy_str               | 301 ms                                                                       | 303 ms: 1.01x slower                                                       |
| async_tree_none_tg      | 436 ms                                                                       | 440 ms: 1.01x slower                                                       |
| pickle                  | 10.3 us                                                                      | 10.3 us: 1.01x slower                                                      |
| logging_simple          | 6.69 us                                                                      | 6.75 us: 1.01x slower                                                      |
| async_tree_cpu_io_mixed | 701 ms                                                                       | 707 ms: 1.01x slower                                                       |
| scimark_sor             | 153 ms                                                                       | 155 ms: 1.01x slower                                                       |
| sympy_sum               | 160 ms                                                                       | 161 ms: 1.01x slower                                                       |
| async_generators        | 386 ms                                                                       | 390 ms: 1.01x slower                                                       |
| sympy_expand            | 510 ms                                                                       | 516 ms: 1.01x slower                                                       |
| async_tree_memoization  | 548 ms                                                                       | 555 ms: 1.01x slower                                                       |
| sqlglot_transpile       | 1.85 ms                                                                      | 1.87 ms: 1.01x slower                                                      |
| async_tree_io_tg        | 1.08 sec                                                                     | 1.09 sec: 1.01x slower                                                     |
| pickle_pure_python      | 310 us                                                                       | 315 us: 1.01x slower                                                       |
| async_tree_io           | 1.08 sec                                                                     | 1.09 sec: 1.01x slower                                                     |
| logging_format          | 7.37 us                                                                      | 7.48 us: 1.02x slower                                                      |
| async_tree_none         | 435 ms                                                                       | 443 ms: 1.02x slower                                                       |
| sqlglot_parse           | 1.42 ms                                                                      | 1.44 ms: 1.02x slower                                                      |
| deepcopy_memo           | 37.7 us                                                                      | 38.4 us: 1.02x slower                                                      |
| logging_silent          | 98.5 ns                                                                      | 100 ns: 1.02x slower                                                       |
| sqlglot_optimize        | 62.7 ms                                                                      | 64.0 ms: 1.02x slower                                                      |
| sqlglot_normalize       | 118 ms                                                                       | 121 ms: 1.02x slower                                                       |
| deepcopy                | 377 us                                                                       | 386 us: 1.02x slower                                                       |
| deepcopy_reduce         | 3.32 us                                                                      | 3.41 us: 1.03x slower                                                      |
| chameleon               | 7.43 ms                                                                      | 7.65 ms: 1.03x slower                                                      |
| go                      | 176 ms                                                                       | 182 ms: 1.03x slower                                                       |
| xml_etree_parse         | 144 ms                                                                       | 151 ms: 1.05x slower                                                       |
| scimark_lu              | 124 ms                                                                       | 131 ms: 1.05x slower                                                       |
| python_startup          | 14.8 ms                                                                      | 15.6 ms: 1.05x slower                                                      |
| coverage                | 79.5 ms                                                                      | 83.7 ms: 1.05x slower                                                      |
| pickle_dict             | 30.5 us                                                                      | 32.2 us: 1.06x slower                                                      |
| python_startup_no_site  | 13.2 ms                                                                      | 14.1 ms: 1.06x slower                                                      |
| gc_traversal            | 3.49 ms                                                                      | 3.95 ms: 1.13x slower                                                      |
| Geometric mean          | (ref)                                                                        | 1.00x faster                                                               |

Benchmark hidden because not significant (21): bench_thread_pool, tornado_http, typing_runtime_protocols, asyncio_tcp_ssl, docutils, xml_etree_generate, bench_mp_pool, pycparser, pprint_pformat, dulwich_log, telco, json_dumps, asyncio_tcp, regex_dna, asyncio_websockets, pprint_safe_repr, xml_etree_iterparse, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, generators, mypy2


# HPT report

- Reliability score: 93.99% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.09x