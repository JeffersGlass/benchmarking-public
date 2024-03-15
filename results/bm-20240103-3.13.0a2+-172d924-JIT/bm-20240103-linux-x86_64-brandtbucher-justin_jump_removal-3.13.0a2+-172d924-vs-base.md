# Results vs. base

- fork: brandtbucher
- ref: justin_jump_removal
- machine: linux-x86_64
- commit hash: 172d924
- commit date: 2024-01-03
- overall geometric mean: 1.03x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                                 | 274 ms: 1.04x slower                                                        |
| chameleon      | 6.90 ms                                                                | 7.00 ms: 1.01x slower                                                       |
| docutils       | 2.59 sec                                                               | 2.65 sec: 1.02x slower                                                      |
| tornado_http   | 94.1 ms                                                                | 96.6 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 574 ms                                                                 | 582 ms: 1.01x slower                                                        |
| async_tree_cpu_io_mixed_tg | 720 ms                                                                 | 733 ms: 1.02x slower                                                        |
| async_tree_memoization     | 559 ms                                                                 | 570 ms: 1.02x slower                                                        |
| async_tree_cpu_io_mixed    | 706 ms                                                                 | 720 ms: 1.02x slower                                                        |
| async_tree_none_tg         | 438 ms                                                                 | 448 ms: 1.02x slower                                                        |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                                |

Benchmark hidden because not significant (3): async_tree_io_tg, async_tree_io, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                                 | 188 ms: 1.00x slower                                                        |
| float          | 79.7 ms                                                                | 84.3 ms: 1.06x slower                                                       |
| nbody          | 87.4 ms                                                                | 95.8 ms: 1.10x slower                                                       |
| Geometric mean | (ref)                                                                  | 1.05x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 223 ms                                                                 | 222 ms: 1.00x faster                                                        |
| regex_effbot   | 3.65 ms                                                                | 3.68 ms: 1.01x slower                                                       |
| regex_v8       | 25.0 ms                                                                | 25.3 ms: 1.01x slower                                                       |
| regex_compile  | 130 ms                                                                 | 139 ms: 1.07x slower                                                        |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_dict          | 35.5 us                                                                | 34.4 us: 1.03x faster                                                       |
| pickle_list          | 5.20 us                                                                | 5.03 us: 1.03x faster                                                       |
| pickle               | 11.7 us                                                                | 11.5 us: 1.01x faster                                                       |
| pickle_pure_python   | 302 us                                                                 | 300 us: 1.01x faster                                                        |
| xml_etree_process    | 58.6 ms                                                                | 59.1 ms: 1.01x slower                                                       |
| xml_etree_parse      | 157 ms                                                                 | 159 ms: 1.01x slower                                                        |
| json_loads           | 28.1 us                                                                | 28.6 us: 1.02x slower                                                       |
| tomli_loads          | 2.13 sec                                                               | 2.16 sec: 1.02x slower                                                      |
| xml_etree_generate   | 85.1 ms                                                                | 86.9 ms: 1.02x slower                                                       |
| unpickle             | 14.9 us                                                                | 15.3 us: 1.02x slower                                                       |
| xml_etree_iterparse  | 105 ms                                                                 | 109 ms: 1.04x slower                                                        |
| unpickle_pure_python | 216 us                                                                 | 226 us: 1.05x slower                                                        |
| unpickle_list        | 5.05 us                                                                | 5.37 us: 1.06x slower                                                       |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                                |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                       |
| python_startup_no_site | 8.71 ms                                                                | 8.86 ms: 1.02x slower                                                       |
| Geometric mean         | (ref)                                                                  | 1.02x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|-----------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 11.2 ms                                                                | 12.1 ms: 1.08x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20240104-linux-x86_64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------------------|:----------------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| richards                   | 48.3 ms                                                                | 45.6 ms: 1.06x faster                                                       |
| richards_super             | 55.0 ms                                                                | 52.0 ms: 1.06x faster                                                       |
| scimark_sor                | 128 ms                                                                 | 123 ms: 1.04x faster                                                        |
| pickle_dict                | 35.5 us                                                                | 34.4 us: 1.03x faster                                                       |
| pickle_list                | 5.20 us                                                                | 5.03 us: 1.03x faster                                                       |
| pycparser                  | 1.19 sec                                                               | 1.17 sec: 1.02x faster                                                      |
| coroutines                 | 22.4 ms                                                                | 22.0 ms: 1.02x faster                                                       |
| pickle                     | 11.7 us                                                                | 11.5 us: 1.01x faster                                                       |
| pickle_pure_python         | 302 us                                                                 | 300 us: 1.01x faster                                                        |
| regex_dna                  | 223 ms                                                                 | 222 ms: 1.00x faster                                                        |
| pidigits                   | 187 ms                                                                 | 188 ms: 1.00x slower                                                        |
| sqlglot_normalize          | 108 ms                                                                 | 108 ms: 1.01x slower                                                        |
| regex_effbot               | 3.65 ms                                                                | 3.68 ms: 1.01x slower                                                       |
| pathlib                    | 18.3 ms                                                                | 18.4 ms: 1.01x slower                                                       |
| xml_etree_process          | 58.6 ms                                                                | 59.1 ms: 1.01x slower                                                       |
| json                       | 5.18 ms                                                                | 5.23 ms: 1.01x slower                                                       |
| regex_v8                   | 25.0 ms                                                                | 25.3 ms: 1.01x slower                                                       |
| xml_etree_parse            | 157 ms                                                                 | 159 ms: 1.01x slower                                                        |
| chameleon                  | 6.90 ms                                                                | 7.00 ms: 1.01x slower                                                       |
| async_tree_memoization_tg  | 574 ms                                                                 | 582 ms: 1.01x slower                                                        |
| python_startup             | 10.1 ms                                                                | 10.2 ms: 1.01x slower                                                       |
| asyncio_tcp                | 480 ms                                                                 | 487 ms: 1.01x slower                                                        |
| scimark_fft                | 362 ms                                                                 | 367 ms: 1.01x slower                                                        |
| dask                       | 359 ms                                                                 | 365 ms: 1.02x slower                                                        |
| asyncio_tcp_ssl            | 1.77 sec                                                               | 1.80 sec: 1.02x slower                                                      |
| json_loads                 | 28.1 us                                                                | 28.6 us: 1.02x slower                                                       |
| create_gc_cycles           | 1.47 ms                                                                | 1.50 ms: 1.02x slower                                                       |
| python_startup_no_site     | 8.71 ms                                                                | 8.86 ms: 1.02x slower                                                       |
| gc_traversal               | 3.69 ms                                                                | 3.76 ms: 1.02x slower                                                       |
| tomli_loads                | 2.13 sec                                                               | 2.16 sec: 1.02x slower                                                      |
| async_tree_cpu_io_mixed_tg | 720 ms                                                                 | 733 ms: 1.02x slower                                                        |
| bench_thread_pool          | 827 us                                                                 | 843 us: 1.02x slower                                                        |
| deepcopy                   | 344 us                                                                 | 351 us: 1.02x slower                                                        |
| async_tree_memoization     | 559 ms                                                                 | 570 ms: 1.02x slower                                                        |
| sympy_expand               | 465 ms                                                                 | 474 ms: 1.02x slower                                                        |
| async_tree_cpu_io_mixed    | 706 ms                                                                 | 720 ms: 1.02x slower                                                        |
| xml_etree_generate         | 85.1 ms                                                                | 86.9 ms: 1.02x slower                                                       |
| deepcopy_memo              | 38.4 us                                                                | 39.2 us: 1.02x slower                                                       |
| async_tree_none_tg         | 438 ms                                                                 | 448 ms: 1.02x slower                                                        |
| scimark_lu                 | 112 ms                                                                 | 115 ms: 1.02x slower                                                        |
| unpickle                   | 14.9 us                                                                | 15.3 us: 1.02x slower                                                       |
| docutils                   | 2.59 sec                                                               | 2.65 sec: 1.02x slower                                                      |
| dulwich_log                | 65.3 ms                                                                | 66.9 ms: 1.02x slower                                                       |
| mdp                        | 2.53 sec                                                               | 2.59 sec: 1.03x slower                                                      |
| tornado_http               | 94.1 ms                                                                | 96.6 ms: 1.03x slower                                                       |
| sqlglot_parse              | 1.25 ms                                                                | 1.28 ms: 1.03x slower                                                       |
| sympy_str                  | 276 ms                                                                 | 283 ms: 1.03x slower                                                        |
| sqlglot_optimize           | 53.9 ms                                                                | 55.4 ms: 1.03x slower                                                       |
| async_generators           | 439 ms                                                                 | 452 ms: 1.03x slower                                                        |
| sqlglot_transpile          | 1.57 ms                                                                | 1.62 ms: 1.03x slower                                                       |
| telco                      | 8.35 ms                                                                | 8.60 ms: 1.03x slower                                                       |
| deepcopy_reduce            | 3.02 us                                                                | 3.12 us: 1.03x slower                                                       |
| meteor_contest             | 108 ms                                                                 | 112 ms: 1.03x slower                                                        |
| 2to3                       | 264 ms                                                                 | 274 ms: 1.04x slower                                                        |
| logging_format             | 6.18 us                                                                | 6.42 us: 1.04x slower                                                       |
| xml_etree_iterparse        | 105 ms                                                                 | 109 ms: 1.04x slower                                                        |
| logging_silent             | 102 ns                                                                 | 106 ns: 1.05x slower                                                        |
| unpickle_pure_python       | 216 us                                                                 | 226 us: 1.05x slower                                                        |
| logging_simple             | 5.62 us                                                                | 5.92 us: 1.05x slower                                                       |
| scimark_sparse_mat_mult    | 4.87 ms                                                                | 5.14 ms: 1.06x slower                                                       |
| float                      | 79.7 ms                                                                | 84.3 ms: 1.06x slower                                                       |
| unpickle_list              | 5.05 us                                                                | 5.37 us: 1.06x slower                                                       |
| sympy_sum                  | 148 ms                                                                 | 158 ms: 1.07x slower                                                        |
| fannkuch                   | 399 ms                                                                 | 426 ms: 1.07x slower                                                        |
| raytrace                   | 262 ms                                                                 | 280 ms: 1.07x slower                                                        |
| sympy_integrate            | 19.5 ms                                                                | 20.8 ms: 1.07x slower                                                       |
| regex_compile              | 130 ms                                                                 | 139 ms: 1.07x slower                                                        |
| go                         | 139 ms                                                                 | 149 ms: 1.08x slower                                                        |
| mako                       | 11.2 ms                                                                | 12.1 ms: 1.08x slower                                                       |
| pprint_safe_repr           | 724 ms                                                                 | 788 ms: 1.09x slower                                                        |
| nbody                      | 87.4 ms                                                                | 95.8 ms: 1.10x slower                                                       |
| scimark_monte_carlo        | 67.6 ms                                                                | 74.4 ms: 1.10x slower                                                       |
| pyflate                    | 455 ms                                                                 | 502 ms: 1.10x slower                                                        |
| crypto_pyaes               | 70.0 ms                                                                | 77.6 ms: 1.11x slower                                                       |
| nqueens                    | 80.6 ms                                                                | 89.4 ms: 1.11x slower                                                       |
| pprint_pformat             | 1.48 sec                                                               | 1.65 sec: 1.11x slower                                                      |
| unpack_sequence            | 44.4 ns                                                                | 49.7 ns: 1.12x slower                                                       |
| chaos                      | 58.9 ms                                                                | 66.8 ms: 1.13x slower                                                       |
| comprehensions             | 16.0 us                                                                | 18.3 us: 1.14x slower                                                       |
| spectral_norm              | 109 ms                                                                 | 131 ms: 1.20x slower                                                        |
| deltablue                  | 3.26 ms                                                                | 3.91 ms: 1.20x slower                                                       |
| hexiom                     | 6.07 ms                                                                | 7.58 ms: 1.25x slower                                                       |
| Geometric mean             | (ref)                                                                  | 1.03x slower                                                                |

Benchmark hidden because not significant (11): coverage, sqlite_synth, generators, json_dumps, async_tree_io_tg, async_tree_io, bench_mp_pool, asyncio_websockets, typing_runtime_protocols, async_tree_none, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.04x