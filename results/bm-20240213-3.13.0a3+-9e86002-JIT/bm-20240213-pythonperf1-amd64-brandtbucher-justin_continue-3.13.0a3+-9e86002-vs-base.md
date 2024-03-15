# Results vs. base

- fork: brandtbucher
- ref: justin_continue
- machine: windows-amd64
- commit hash: 9e86002
- commit date: 2024-02-13
- overall geometric mean: 1.01x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 216 ms                                                                      | 214 ms: 1.01x faster                                                         |
| docutils       | 1.57 sec                                                                    | 1.56 sec: 1.01x faster                                                       |
| Geometric mean | (ref)                                                                       | 1.00x faster                                                                 |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-------------------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 451 ms                                                                      | 445 ms: 1.01x faster                                                         |
| Geometric mean          | (ref)                                                                       | 1.00x faster                                                                 |

Benchmark hidden because not significant (7): async_tree_none_tg, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_none, async_tree_memoization_tg, async_tree_memoization, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 61.7 ms                                                                     | 59.5 ms: 1.04x faster                                                        |
| pidigits       | 152 ms                                                                      | 151 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                                       | 1.01x faster                                                                 |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 79.9 ms                                                                     | 78.1 ms: 1.02x faster                                                        |
| regex_v8       | 15.2 ms                                                                     | 14.8 ms: 1.02x faster                                                        |
| regex_dna      | 119 ms                                                                      | 120 ms: 1.01x slower                                                         |
| Geometric mean | (ref)                                                                       | 1.01x faster                                                                 |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| xml_etree_process    | 36.3 ms                                                                     | 36.0 ms: 1.01x faster                                                        |
| pickle_dict          | 17.6 us                                                                     | 17.5 us: 1.01x faster                                                        |
| pickle_pure_python   | 173 us                                                                      | 174 us: 1.01x slower                                                         |
| unpickle_list        | 2.76 us                                                                     | 2.79 us: 1.01x slower                                                        |
| unpickle_pure_python | 125 us                                                                      | 126 us: 1.01x slower                                                         |
| json_dumps           | 5.55 ms                                                                     | 5.61 ms: 1.01x slower                                                        |
| pickle               | 7.16 us                                                                     | 7.43 us: 1.04x slower                                                        |
| Geometric mean       | (ref)                                                                       | 1.00x slower                                                                 |

Benchmark hidden because not significant (7): tomli_loads, pickle_list, xml_etree_iterparse, xml_etree_generate, json_loads, unpickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup, python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-----------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 6.44 ms                                                                     | 6.15 ms: 1.05x faster                                                        |

All benchmarks:
===============

| Benchmark               | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-------------------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| scimark_monte_carlo     | 56.7 ms                                                                     | 49.2 ms: 1.15x faster                                                        |
| json                    | 3.58 ms                                                                     | 3.26 ms: 1.10x faster                                                        |
| spectral_norm           | 65.7 ms                                                                     | 59.9 ms: 1.10x faster                                                        |
| hexiom                  | 5.22 ms                                                                     | 4.82 ms: 1.08x faster                                                        |
| asyncio_tcp_ssl         | 1.84 sec                                                                    | 1.72 sec: 1.07x faster                                                       |
| scimark_sparse_mat_mult | 2.67 ms                                                                     | 2.51 ms: 1.07x faster                                                        |
| pyflate                 | 310 ms                                                                      | 291 ms: 1.06x faster                                                         |
| fannkuch                | 243 ms                                                                      | 230 ms: 1.06x faster                                                         |
| unpack_sequence         | 40.8 ns                                                                     | 38.8 ns: 1.05x faster                                                        |
| mako                    | 6.44 ms                                                                     | 6.15 ms: 1.05x faster                                                        |
| scimark_lu              | 55.9 ms                                                                     | 53.4 ms: 1.05x faster                                                        |
| coverage                | 47.7 ms                                                                     | 45.6 ms: 1.05x faster                                                        |
| sqlglot_normalize       | 180 ms                                                                      | 172 ms: 1.04x faster                                                         |
| scimark_fft             | 196 ms                                                                      | 188 ms: 1.04x faster                                                         |
| nbody                   | 61.7 ms                                                                     | 59.5 ms: 1.04x faster                                                        |
| scimark_sor             | 77.2 ms                                                                     | 74.6 ms: 1.04x faster                                                        |
| sqlglot_optimize        | 34.5 ms                                                                     | 33.3 ms: 1.03x faster                                                        |
| go                      | 97.1 ms                                                                     | 94.3 ms: 1.03x faster                                                        |
| telco                   | 4.71 ms                                                                     | 4.58 ms: 1.03x faster                                                        |
| pprint_pformat          | 991 ms                                                                      | 967 ms: 1.03x faster                                                         |
| raytrace                | 172 ms                                                                      | 167 ms: 1.02x faster                                                         |
| sympy_str               | 167 ms                                                                      | 163 ms: 1.02x faster                                                         |
| regex_compile           | 79.9 ms                                                                     | 78.1 ms: 1.02x faster                                                        |
| bench_thread_pool       | 826 us                                                                      | 808 us: 1.02x faster                                                         |
| meteor_contest          | 75.5 ms                                                                     | 73.8 ms: 1.02x faster                                                        |
| regex_v8                | 15.2 ms                                                                     | 14.8 ms: 1.02x faster                                                        |
| chaos                   | 42.5 ms                                                                     | 41.6 ms: 1.02x faster                                                        |
| pycparser               | 685 ms                                                                      | 671 ms: 1.02x faster                                                         |
| sympy_sum               | 88.1 ms                                                                     | 86.4 ms: 1.02x faster                                                        |
| sympy_expand            | 282 ms                                                                      | 276 ms: 1.02x faster                                                         |
| sympy_integrate         | 13.2 ms                                                                     | 12.9 ms: 1.02x faster                                                        |
| comprehensions          | 11.3 us                                                                     | 11.1 us: 1.02x faster                                                        |
| pprint_safe_repr        | 480 ms                                                                      | 473 ms: 1.02x faster                                                         |
| crypto_pyaes            | 45.5 ms                                                                     | 44.9 ms: 1.01x faster                                                        |
| sqlglot_transpile       | 979 us                                                                      | 965 us: 1.01x faster                                                         |
| async_tree_cpu_io_mixed | 451 ms                                                                      | 445 ms: 1.01x faster                                                         |
| deepcopy_memo           | 21.5 us                                                                     | 21.2 us: 1.01x faster                                                        |
| mypy2                   | 425 ms                                                                      | 421 ms: 1.01x faster                                                         |
| 2to3                    | 216 ms                                                                      | 214 ms: 1.01x faster                                                         |
| pidigits                | 152 ms                                                                      | 151 ms: 1.01x faster                                                         |
| xml_etree_process       | 36.3 ms                                                                     | 36.0 ms: 1.01x faster                                                        |
| gc_traversal            | 1.50 ms                                                                     | 1.49 ms: 1.01x faster                                                        |
| deepcopy                | 217 us                                                                      | 216 us: 1.01x faster                                                         |
| pickle_dict             | 17.6 us                                                                     | 17.5 us: 1.01x faster                                                        |
| docutils                | 1.57 sec                                                                    | 1.56 sec: 1.01x faster                                                       |
| pickle_pure_python      | 173 us                                                                      | 174 us: 1.01x slower                                                         |
| coroutines              | 12.9 ms                                                                     | 13.0 ms: 1.01x slower                                                        |
| dulwich_log             | 40.2 ms                                                                     | 40.5 ms: 1.01x slower                                                        |
| sqlite_synth            | 1.51 us                                                                     | 1.52 us: 1.01x slower                                                        |
| mdp                     | 1.54 sec                                                                    | 1.56 sec: 1.01x slower                                                       |
| unpickle_list           | 2.76 us                                                                     | 2.79 us: 1.01x slower                                                        |
| regex_dna               | 119 ms                                                                      | 120 ms: 1.01x slower                                                         |
| unpickle_pure_python    | 125 us                                                                      | 126 us: 1.01x slower                                                         |
| json_dumps              | 5.55 ms                                                                     | 5.61 ms: 1.01x slower                                                        |
| logging_silent          | 52.2 ns                                                                     | 53.0 ns: 1.02x slower                                                        |
| logging_format          | 6.28 us                                                                     | 6.42 us: 1.02x slower                                                        |
| logging_simple          | 5.83 us                                                                     | 6.00 us: 1.03x slower                                                        |
| pathlib                 | 74.5 ms                                                                     | 76.9 ms: 1.03x slower                                                        |
| deepcopy_reduce         | 1.89 us                                                                     | 1.95 us: 1.03x slower                                                        |
| pickle                  | 7.16 us                                                                     | 7.43 us: 1.04x slower                                                        |
| Geometric mean          | (ref)                                                                       | 1.01x faster                                                                 |

Benchmark hidden because not significant (32): tomli_loads, async_tree_none_tg, pickle_list, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_none, typing_runtime_protocols, generators, nqueens, async_tree_memoization_tg, richards_super, tornado_http, xml_etree_iterparse, dask, create_gc_cycles, deltablue, sqlglot_parse, python_startup, bench_mp_pool, async_generators, richards, float, async_tree_memoization, xml_etree_generate, python_startup_no_site, json_loads, regex_effbot, async_tree_io, unpickle, chameleon, asyncio_tcp, xml_etree_parse


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown