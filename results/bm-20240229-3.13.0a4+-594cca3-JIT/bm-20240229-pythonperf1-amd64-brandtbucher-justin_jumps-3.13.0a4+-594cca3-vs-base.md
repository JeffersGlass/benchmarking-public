# Results vs. base

- fork: brandtbucher
- ref: justin_jumps
- machine: windows-amd64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.02x faster
- HPT reliability: 99.90%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| chameleon      | 4.80 ms                                                                     | 4.77 ms: 1.01x faster                                                     |
| Geometric mean | (ref)                                                                       | 1.00x faster                                                              |

Benchmark hidden because not significant (3): 2to3, docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 465 ms                                                                      | 480 ms: 1.03x slower                                                      |
| Geometric mean             | (ref)                                                                       | 1.01x slower                                                              |

Benchmark hidden because not significant (7): async_tree_none, async_tree_memoization, async_tree_none_tg, async_tree_io_tg, async_tree_io, async_tree_cpu_io_mixed, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

Benchmark hidden because not significant (3): float, pidigits, nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 90.9 ms                                                                     | 83.6 ms: 1.09x faster                                                     |
| regex_effbot   | 1.56 ms                                                                     | 1.58 ms: 1.01x slower                                                     |
| regex_v8       | 14.5 ms                                                                     | 14.8 ms: 1.02x slower                                                     |
| regex_dna      | 114 ms                                                                      | 120 ms: 1.05x slower                                                      |
| Geometric mean | (ref)                                                                       | 1.00x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| tomli_loads          | 1.29 sec                                                                    | 1.17 sec: 1.10x faster                                                    |
| unpickle_pure_python | 138 us                                                                      | 130 us: 1.06x faster                                                      |
| pickle_pure_python   | 180 us                                                                      | 178 us: 1.01x faster                                                      |
| json_dumps           | 5.49 ms                                                                     | 5.43 ms: 1.01x faster                                                     |
| json_loads           | 13.7 us                                                                     | 13.8 us: 1.00x slower                                                     |
| xml_etree_process    | 36.2 ms                                                                     | 36.4 ms: 1.01x slower                                                     |
| xml_etree_generate   | 53.1 ms                                                                     | 53.4 ms: 1.01x slower                                                     |
| pickle_dict          | 17.5 us                                                                     | 17.7 us: 1.01x slower                                                     |
| unpickle_list        | 2.78 us                                                                     | 2.83 us: 1.02x slower                                                     |
| unpickle             | 8.50 us                                                                     | 8.69 us: 1.02x slower                                                     |
| pickle               | 7.19 us                                                                     | 7.60 us: 1.06x slower                                                     |
| pickle_list          | 2.88 us                                                                     | 3.12 us: 1.09x slower                                                     |
| Geometric mean       | (ref)                                                                       | 1.00x slower                                                              |

Benchmark hidden because not significant (2): xml_etree_iterparse, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup | 24.0 ms                                                                     | 23.8 ms: 1.01x faster                                                     |
| Geometric mean | (ref)                                                                       | 1.00x faster                                                              |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 5.90 ms                                                                     | 5.63 ms: 1.05x faster                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpack_sequence            | 58.3 ns                                                                     | 45.2 ns: 1.29x faster                                                     |
| fannkuch                   | 261 ms                                                                      | 221 ms: 1.19x faster                                                      |
| hexiom                     | 5.01 ms                                                                     | 4.39 ms: 1.14x faster                                                     |
| scimark_monte_carlo        | 46.3 ms                                                                     | 41.5 ms: 1.12x faster                                                     |
| richards                   | 31.6 ms                                                                     | 28.5 ms: 1.11x faster                                                     |
| richards_super             | 35.0 ms                                                                     | 31.8 ms: 1.10x faster                                                     |
| spectral_norm              | 56.3 ms                                                                     | 51.1 ms: 1.10x faster                                                     |
| tomli_loads                | 1.29 sec                                                                    | 1.17 sec: 1.10x faster                                                    |
| pprint_pformat             | 1.06 sec                                                                    | 969 ms: 1.09x faster                                                      |
| regex_compile              | 90.9 ms                                                                     | 83.6 ms: 1.09x faster                                                     |
| comprehensions             | 11.1 us                                                                     | 10.3 us: 1.08x faster                                                     |
| pprint_safe_repr           | 510 ms                                                                      | 475 ms: 1.07x faster                                                      |
| unpickle_pure_python       | 138 us                                                                      | 130 us: 1.06x faster                                                      |
| pycparser                  | 740 ms                                                                      | 696 ms: 1.06x faster                                                      |
| scimark_fft                | 179 ms                                                                      | 169 ms: 1.06x faster                                                      |
| chaos                      | 41.2 ms                                                                     | 39.3 ms: 1.05x faster                                                     |
| mako                       | 5.90 ms                                                                     | 5.63 ms: 1.05x faster                                                     |
| pyflate                    | 298 ms                                                                      | 287 ms: 1.04x faster                                                      |
| go                         | 99.8 ms                                                                     | 96.8 ms: 1.03x faster                                                     |
| sympy_expand               | 288 ms                                                                      | 280 ms: 1.03x faster                                                      |
| scimark_sor                | 87.1 ms                                                                     | 84.6 ms: 1.03x faster                                                     |
| deepcopy_memo              | 22.7 us                                                                     | 22.1 us: 1.03x faster                                                     |
| logging_simple             | 5.96 us                                                                     | 5.80 us: 1.03x faster                                                     |
| sympy_str                  | 167 ms                                                                      | 163 ms: 1.02x faster                                                      |
| logging_silent             | 56.0 ns                                                                     | 54.7 ns: 1.02x faster                                                     |
| logging_format             | 6.38 us                                                                     | 6.24 us: 1.02x faster                                                     |
| deepcopy_reduce            | 1.99 us                                                                     | 1.95 us: 1.02x faster                                                     |
| raytrace                   | 183 ms                                                                      | 179 ms: 1.02x faster                                                      |
| telco                      | 4.65 ms                                                                     | 4.57 ms: 1.02x faster                                                     |
| sympy_sum                  | 88.2 ms                                                                     | 86.6 ms: 1.02x faster                                                     |
| sqlglot_parse              | 792 us                                                                      | 778 us: 1.02x faster                                                      |
| crypto_pyaes               | 44.2 ms                                                                     | 43.5 ms: 1.02x faster                                                     |
| deltablue                  | 2.09 ms                                                                     | 2.05 ms: 1.02x faster                                                     |
| sympy_integrate            | 13.3 ms                                                                     | 13.0 ms: 1.02x faster                                                     |
| meteor_contest             | 73.3 ms                                                                     | 72.2 ms: 1.02x faster                                                     |
| dulwich_log                | 41.8 ms                                                                     | 41.3 ms: 1.01x faster                                                     |
| pickle_pure_python         | 180 us                                                                      | 178 us: 1.01x faster                                                      |
| sqlglot_transpile          | 1.02 ms                                                                     | 1.01 ms: 1.01x faster                                                     |
| json_dumps                 | 5.49 ms                                                                     | 5.43 ms: 1.01x faster                                                     |
| chameleon                  | 4.80 ms                                                                     | 4.77 ms: 1.01x faster                                                     |
| python_startup             | 24.0 ms                                                                     | 23.8 ms: 1.01x faster                                                     |
| async_generators           | 242 ms                                                                      | 240 ms: 1.01x faster                                                      |
| mypy2                      | 438 ms                                                                      | 436 ms: 1.00x faster                                                      |
| scimark_sparse_mat_mult    | 2.29 ms                                                                     | 2.29 ms: 1.00x slower                                                     |
| sqlglot_normalize          | 176 ms                                                                      | 177 ms: 1.00x slower                                                      |
| json_loads                 | 13.7 us                                                                     | 13.8 us: 1.00x slower                                                     |
| generators                 | 20.1 ms                                                                     | 20.2 ms: 1.00x slower                                                     |
| xml_etree_process          | 36.2 ms                                                                     | 36.4 ms: 1.01x slower                                                     |
| xml_etree_generate         | 53.1 ms                                                                     | 53.4 ms: 1.01x slower                                                     |
| gc_traversal               | 1.50 ms                                                                     | 1.51 ms: 1.01x slower                                                     |
| regex_effbot               | 1.56 ms                                                                     | 1.58 ms: 1.01x slower                                                     |
| pickle_dict                | 17.5 us                                                                     | 17.7 us: 1.01x slower                                                     |
| coroutines                 | 13.1 ms                                                                     | 13.2 ms: 1.01x slower                                                     |
| scimark_lu                 | 72.0 ms                                                                     | 73.0 ms: 1.01x slower                                                     |
| unpickle_list              | 2.78 us                                                                     | 2.83 us: 1.02x slower                                                     |
| regex_v8                   | 14.5 ms                                                                     | 14.8 ms: 1.02x slower                                                     |
| unpickle                   | 8.50 us                                                                     | 8.69 us: 1.02x slower                                                     |
| async_tree_cpu_io_mixed_tg | 465 ms                                                                      | 480 ms: 1.03x slower                                                      |
| regex_dna                  | 114 ms                                                                      | 120 ms: 1.05x slower                                                      |
| pickle                     | 7.19 us                                                                     | 7.60 us: 1.06x slower                                                     |
| mdp                        | 1.43 sec                                                                    | 1.52 sec: 1.06x slower                                                    |
| pickle_list                | 2.88 us                                                                     | 3.12 us: 1.09x slower                                                     |
| Geometric mean             | (ref)                                                                       | 1.02x faster                                                              |

Benchmark hidden because not significant (29): asyncio_tcp_ssl, asyncio_tcp, create_gc_cycles, 2to3, xml_etree_iterparse, coverage, float, async_tree_none, pathlib, tornado_http, sqlglot_optimize, nqueens, async_tree_memoization, async_tree_none_tg, python_startup_no_site, bench_mp_pool, docutils, typing_runtime_protocols, sqlite_synth, deepcopy, pidigits, async_tree_io_tg, xml_etree_parse, nbody, async_tree_io, json, bench_thread_pool, async_tree_cpu_io_mixed, async_tree_memoization_tg


# HPT report

- Reliability score: 99.90% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown