# Results vs. base

- fork: brandtbucher
- ref: justin_jumps
- machine: windows-x86
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.03x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 255 ms                                                                          | 264 ms: 1.04x slower                                                          |
| chameleon      | 5.77 ms                                                                         | 5.90 ms: 1.02x slower                                                         |
| docutils       | 1.82 sec                                                                        | 1.89 sec: 1.04x slower                                                        |
| tornado_http   | 95.2 ms                                                                         | 99.4 ms: 1.04x slower                                                         |
| Geometric mean | (ref)                                                                           | 1.04x slower                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_io_tg           | 597 ms                                                                          | 618 ms: 1.04x slower                                                          |
| async_tree_io              | 612 ms                                                                          | 637 ms: 1.04x slower                                                          |
| async_tree_none_tg         | 241 ms                                                                          | 251 ms: 1.04x slower                                                          |
| async_tree_none            | 257 ms                                                                          | 268 ms: 1.04x slower                                                          |
| async_tree_memoization     | 318 ms                                                                          | 332 ms: 1.04x slower                                                          |
| async_tree_memoization_tg  | 302 ms                                                                          | 315 ms: 1.04x slower                                                          |
| async_tree_cpu_io_mixed    | 523 ms                                                                          | 556 ms: 1.06x slower                                                          |
| async_tree_cpu_io_mixed_tg | 507 ms                                                                          | 541 ms: 1.07x slower                                                          |
| Geometric mean             | (ref)                                                                           | 1.05x slower                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pidigits       | 201 ms                                                                          | 200 ms: 1.01x faster                                                          |
| float          | 54.7 ms                                                                         | 55.2 ms: 1.01x slower                                                         |
| nbody          | 93.7 ms                                                                         | 97.7 ms: 1.04x slower                                                         |
| Geometric mean | (ref)                                                                           | 1.02x slower                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_dna      | 130 ms                                                                          | 119 ms: 1.09x faster                                                          |
| regex_effbot   | 1.97 ms                                                                         | 1.89 ms: 1.04x faster                                                         |
| regex_compile  | 111 ms                                                                          | 114 ms: 1.02x slower                                                          |
| Geometric mean | (ref)                                                                           | 1.03x faster                                                                  |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pickle               | 8.02 us                                                                         | 7.91 us: 1.01x faster                                                         |
| pickle_dict          | 20.3 us                                                                         | 20.1 us: 1.01x faster                                                         |
| xml_etree_iterparse  | 66.6 ms                                                                         | 66.9 ms: 1.00x slower                                                         |
| xml_etree_parse      | 107 ms                                                                          | 108 ms: 1.01x slower                                                          |
| pickle_list          | 3.25 us                                                                         | 3.29 us: 1.01x slower                                                         |
| unpickle             | 9.86 us                                                                         | 10.0 us: 1.01x slower                                                         |
| unpickle_pure_python | 167 us                                                                          | 174 us: 1.05x slower                                                          |
| tomli_loads          | 1.66 sec                                                                        | 1.75 sec: 1.05x slower                                                        |
| unpickle_list        | 2.65 us                                                                         | 2.79 us: 1.05x slower                                                         |
| json_dumps           | 6.80 ms                                                                         | 7.16 ms: 1.05x slower                                                         |
| xml_etree_generate   | 60.4 ms                                                                         | 63.8 ms: 1.06x slower                                                         |
| xml_etree_process    | 41.9 ms                                                                         | 44.3 ms: 1.06x slower                                                         |
| pickle_pure_python   | 214 us                                                                          | 227 us: 1.06x slower                                                          |
| Geometric mean       | (ref)                                                                           | 1.03x slower                                                                  |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup_no_site | 23.6 ms                                                                         | 23.7 ms: 1.01x slower                                                         |
| Geometric mean         | (ref)                                                                           | 1.00x slower                                                                  |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20240229-pythonperf1_win32-x86-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:-------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| unpack_sequence            | 61.0 ns                                                                         | 43.7 ns: 1.40x faster                                                         |
| regex_dna                  | 130 ms                                                                          | 119 ms: 1.09x faster                                                          |
| regex_effbot               | 1.97 ms                                                                         | 1.89 ms: 1.04x faster                                                         |
| json                       | 4.25 ms                                                                         | 4.13 ms: 1.03x faster                                                         |
| scimark_lu                 | 89.2 ms                                                                         | 87.2 ms: 1.02x faster                                                         |
| sqlite_synth               | 1.90 us                                                                         | 1.86 us: 1.02x faster                                                         |
| scimark_sparse_mat_mult    | 3.16 ms                                                                         | 3.11 ms: 1.01x faster                                                         |
| pickle                     | 8.02 us                                                                         | 7.91 us: 1.01x faster                                                         |
| telco                      | 6.26 ms                                                                         | 6.18 ms: 1.01x faster                                                         |
| pickle_dict                | 20.3 us                                                                         | 20.1 us: 1.01x faster                                                         |
| pidigits                   | 201 ms                                                                          | 200 ms: 1.01x faster                                                          |
| hexiom                     | 6.35 ms                                                                         | 6.32 ms: 1.00x faster                                                         |
| xml_etree_iterparse        | 66.6 ms                                                                         | 66.9 ms: 1.00x slower                                                         |
| scimark_monte_carlo        | 65.4 ms                                                                         | 65.7 ms: 1.00x slower                                                         |
| python_startup_no_site     | 23.6 ms                                                                         | 23.7 ms: 1.01x slower                                                         |
| float                      | 54.7 ms                                                                         | 55.2 ms: 1.01x slower                                                         |
| scimark_fft                | 236 ms                                                                          | 239 ms: 1.01x slower                                                          |
| bench_mp_pool              | 73.7 ms                                                                         | 74.5 ms: 1.01x slower                                                         |
| logging_simple             | 8.23 us                                                                         | 8.33 us: 1.01x slower                                                         |
| xml_etree_parse            | 107 ms                                                                          | 108 ms: 1.01x slower                                                          |
| logging_format             | 8.76 us                                                                         | 8.87 us: 1.01x slower                                                         |
| pickle_list                | 3.25 us                                                                         | 3.29 us: 1.01x slower                                                         |
| unpickle                   | 9.86 us                                                                         | 10.0 us: 1.01x slower                                                         |
| sympy_sum                  | 107 ms                                                                          | 109 ms: 1.02x slower                                                          |
| fannkuch                   | 325 ms                                                                          | 332 ms: 1.02x slower                                                          |
| chameleon                  | 5.77 ms                                                                         | 5.90 ms: 1.02x slower                                                         |
| sympy_str                  | 208 ms                                                                          | 213 ms: 1.02x slower                                                          |
| regex_compile              | 111 ms                                                                          | 114 ms: 1.02x slower                                                          |
| sympy_expand               | 362 ms                                                                          | 372 ms: 1.03x slower                                                          |
| nqueens                    | 89.2 ms                                                                         | 91.7 ms: 1.03x slower                                                         |
| typing_runtime_protocols   | 94.5 us                                                                         | 97.1 us: 1.03x slower                                                         |
| spectral_norm              | 71.1 ms                                                                         | 73.3 ms: 1.03x slower                                                         |
| pycparser                  | 850 ms                                                                          | 878 ms: 1.03x slower                                                          |
| pyflate                    | 376 ms                                                                          | 388 ms: 1.03x slower                                                          |
| bench_thread_pool          | 1.03 ms                                                                         | 1.06 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 597 ms                                                                          | 618 ms: 1.04x slower                                                          |
| richards                   | 35.8 ms                                                                         | 37.1 ms: 1.04x slower                                                         |
| docutils                   | 1.82 sec                                                                        | 1.89 sec: 1.04x slower                                                        |
| 2to3                       | 255 ms                                                                          | 264 ms: 1.04x slower                                                          |
| sympy_integrate            | 15.3 ms                                                                         | 15.9 ms: 1.04x slower                                                         |
| async_tree_io              | 612 ms                                                                          | 637 ms: 1.04x slower                                                          |
| async_tree_none_tg         | 241 ms                                                                          | 251 ms: 1.04x slower                                                          |
| async_tree_none            | 257 ms                                                                          | 268 ms: 1.04x slower                                                          |
| nbody                      | 93.7 ms                                                                         | 97.7 ms: 1.04x slower                                                         |
| tornado_http               | 95.2 ms                                                                         | 99.4 ms: 1.04x slower                                                         |
| async_tree_memoization     | 318 ms                                                                          | 332 ms: 1.04x slower                                                          |
| async_tree_memoization_tg  | 302 ms                                                                          | 315 ms: 1.04x slower                                                          |
| crypto_pyaes               | 58.5 ms                                                                         | 61.1 ms: 1.04x slower                                                         |
| unpickle_pure_python       | 167 us                                                                          | 174 us: 1.05x slower                                                          |
| meteor_contest             | 79.7 ms                                                                         | 83.5 ms: 1.05x slower                                                         |
| tomli_loads                | 1.66 sec                                                                        | 1.75 sec: 1.05x slower                                                        |
| unpickle_list              | 2.65 us                                                                         | 2.79 us: 1.05x slower                                                         |
| json_dumps                 | 6.80 ms                                                                         | 7.16 ms: 1.05x slower                                                         |
| xml_etree_generate         | 60.4 ms                                                                         | 63.8 ms: 1.06x slower                                                         |
| mdp                        | 1.70 sec                                                                        | 1.80 sec: 1.06x slower                                                        |
| xml_etree_process          | 41.9 ms                                                                         | 44.3 ms: 1.06x slower                                                         |
| pickle_pure_python         | 214 us                                                                          | 227 us: 1.06x slower                                                          |
| sqlglot_optimize           | 44.6 ms                                                                         | 47.4 ms: 1.06x slower                                                         |
| raytrace                   | 261 ms                                                                          | 277 ms: 1.06x slower                                                          |
| async_tree_cpu_io_mixed    | 523 ms                                                                          | 556 ms: 1.06x slower                                                          |
| async_tree_cpu_io_mixed_tg | 507 ms                                                                          | 541 ms: 1.07x slower                                                          |
| coroutines                 | 14.1 ms                                                                         | 15.1 ms: 1.07x slower                                                         |
| go                         | 119 ms                                                                          | 128 ms: 1.07x slower                                                          |
| sqlglot_normalize          | 218 ms                                                                          | 235 ms: 1.08x slower                                                          |
| comprehensions             | 14.1 us                                                                         | 15.3 us: 1.09x slower                                                         |
| deepcopy_reduce            | 2.40 us                                                                         | 2.61 us: 1.09x slower                                                         |
| sqlglot_parse              | 958 us                                                                          | 1.04 ms: 1.09x slower                                                         |
| sqlglot_transpile          | 1.20 ms                                                                         | 1.31 ms: 1.09x slower                                                         |
| coverage                   | 301 ms                                                                          | 330 ms: 1.09x slower                                                          |
| deltablue                  | 2.51 ms                                                                         | 2.74 ms: 1.09x slower                                                         |
| deepcopy                   | 268 us                                                                          | 294 us: 1.10x slower                                                          |
| scimark_sor                | 98.4 ms                                                                         | 108 ms: 1.10x slower                                                          |
| async_generators           | 278 ms                                                                          | 316 ms: 1.13x slower                                                          |
| deepcopy_memo              | 24.2 us                                                                         | 27.9 us: 1.15x slower                                                         |
| generators                 | 21.6 ms                                                                         | 25.0 ms: 1.16x slower                                                         |
| logging_silent             | 60.2 ns                                                                         | 70.3 ns: 1.17x slower                                                         |
| Geometric mean             | (ref)                                                                           | 1.03x slower                                                                  |

Benchmark hidden because not significant (13): asyncio_tcp, python_startup, create_gc_cycles, pprint_pformat, json_loads, pathlib, richards_super, pprint_safe_repr, regex_v8, mako, asyncio_tcp_ssl, gc_traversal, chaos


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: unknown