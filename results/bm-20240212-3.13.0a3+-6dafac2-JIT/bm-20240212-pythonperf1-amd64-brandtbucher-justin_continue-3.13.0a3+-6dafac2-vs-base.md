# Results vs. base

- fork: brandtbucher
- ref: justin_continue
- machine: windows-amd64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 216 ms                                                                      | 214 ms: 1.01x faster                                                         |
| chameleon      | 4.78 ms                                                                     | 4.71 ms: 1.02x faster                                                        |
| docutils       | 1.57 sec                                                                    | 1.56 sec: 1.01x faster                                                       |
| tornado_http   | 84.9 ms                                                                     | 83.9 ms: 1.01x faster                                                        |
| Geometric mean | (ref)                                                                       | 1.01x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_none_tg, async_tree_io, async_tree_memoization, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 61.7 ms                                                                     | 58.4 ms: 1.06x faster                                                        |
| float          | 50.0 ms                                                                     | 49.5 ms: 1.01x faster                                                        |
| pidigits       | 152 ms                                                                      | 151 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                                       | 1.03x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 79.9 ms                                                                     | 76.9 ms: 1.04x faster                                                        |
| regex_effbot   | 1.59 ms                                                                     | 1.58 ms: 1.01x faster                                                        |
| regex_v8       | 15.2 ms                                                                     | 15.1 ms: 1.00x faster                                                        |
| Geometric mean | (ref)                                                                       | 1.01x faster                                                                 |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| tomli_loads          | 1.27 sec                                                                    | 1.19 sec: 1.07x faster                                                       |
| xml_etree_parse      | 93.9 ms                                                                     | 92.7 ms: 1.01x faster                                                        |
| unpickle_pure_python | 125 us                                                                      | 123 us: 1.01x faster                                                         |
| xml_etree_iterparse  | 63.4 ms                                                                     | 62.7 ms: 1.01x faster                                                        |
| pickle_dict          | 17.6 us                                                                     | 17.5 us: 1.01x faster                                                        |
| pickle               | 7.16 us                                                                     | 7.10 us: 1.01x faster                                                        |
| xml_etree_generate   | 52.6 ms                                                                     | 52.2 ms: 1.01x faster                                                        |
| json_loads           | 13.7 us                                                                     | 13.6 us: 1.01x faster                                                        |
| xml_etree_process    | 36.3 ms                                                                     | 36.1 ms: 1.01x faster                                                        |
| pickle_pure_python   | 173 us                                                                      | 174 us: 1.01x slower                                                         |
| Geometric mean       | (ref)                                                                       | 1.01x faster                                                                 |

Benchmark hidden because not significant (4): unpickle, json_dumps, pickle_list, unpickle_list

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup, python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 6.44 ms                                                                     | 5.98 ms: 1.08x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|--------------------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| spectral_norm            | 65.7 ms                                                                     | 54.4 ms: 1.21x faster                                                        |
| scimark_monte_carlo      | 56.7 ms                                                                     | 47.6 ms: 1.19x faster                                                        |
| hexiom                   | 5.22 ms                                                                     | 4.44 ms: 1.18x faster                                                        |
| scimark_sparse_mat_mult  | 2.67 ms                                                                     | 2.33 ms: 1.15x faster                                                        |
| fannkuch                 | 243 ms                                                                      | 218 ms: 1.11x faster                                                         |
| scimark_fft              | 196 ms                                                                      | 176 ms: 1.11x faster                                                         |
| pyflate                  | 310 ms                                                                      | 284 ms: 1.09x faster                                                         |
| asyncio_tcp_ssl          | 1.84 sec                                                                    | 1.69 sec: 1.09x faster                                                       |
| go                       | 97.1 ms                                                                     | 90.0 ms: 1.08x faster                                                        |
| mako                     | 6.44 ms                                                                     | 5.98 ms: 1.08x faster                                                        |
| tomli_loads              | 1.27 sec                                                                    | 1.19 sec: 1.07x faster                                                       |
| comprehensions           | 11.3 us                                                                     | 10.6 us: 1.07x faster                                                        |
| nbody                    | 61.7 ms                                                                     | 58.4 ms: 1.06x faster                                                        |
| unpack_sequence          | 40.8 ns                                                                     | 38.8 ns: 1.05x faster                                                        |
| chaos                    | 42.5 ms                                                                     | 40.6 ms: 1.05x faster                                                        |
| crypto_pyaes             | 45.5 ms                                                                     | 43.5 ms: 1.05x faster                                                        |
| pprint_pformat           | 991 ms                                                                      | 950 ms: 1.04x faster                                                         |
| meteor_contest           | 75.5 ms                                                                     | 72.4 ms: 1.04x faster                                                        |
| telco                    | 4.71 ms                                                                     | 4.53 ms: 1.04x faster                                                        |
| regex_compile            | 79.9 ms                                                                     | 76.9 ms: 1.04x faster                                                        |
| sqlglot_optimize         | 34.5 ms                                                                     | 33.3 ms: 1.04x faster                                                        |
| deepcopy_memo            | 21.5 us                                                                     | 20.7 us: 1.03x faster                                                        |
| sqlglot_normalize        | 180 ms                                                                      | 174 ms: 1.03x faster                                                         |
| sympy_str                | 167 ms                                                                      | 161 ms: 1.03x faster                                                         |
| pprint_safe_repr         | 480 ms                                                                      | 465 ms: 1.03x faster                                                         |
| bench_thread_pool        | 826 us                                                                      | 803 us: 1.03x faster                                                         |
| scimark_lu               | 55.9 ms                                                                     | 54.4 ms: 1.03x faster                                                        |
| raytrace                 | 172 ms                                                                      | 167 ms: 1.03x faster                                                         |
| sympy_expand             | 282 ms                                                                      | 275 ms: 1.03x faster                                                         |
| sympy_integrate          | 13.2 ms                                                                     | 12.8 ms: 1.02x faster                                                        |
| sympy_sum                | 88.1 ms                                                                     | 86.5 ms: 1.02x faster                                                        |
| sqlglot_transpile        | 979 us                                                                      | 963 us: 1.02x faster                                                         |
| dulwich_log              | 40.2 ms                                                                     | 39.6 ms: 1.02x faster                                                        |
| chameleon                | 4.78 ms                                                                     | 4.71 ms: 1.02x faster                                                        |
| deepcopy                 | 217 us                                                                      | 214 us: 1.02x faster                                                         |
| coverage                 | 47.7 ms                                                                     | 47.0 ms: 1.01x faster                                                        |
| scimark_sor              | 77.2 ms                                                                     | 76.1 ms: 1.01x faster                                                        |
| richards_super           | 28.2 ms                                                                     | 27.9 ms: 1.01x faster                                                        |
| mypy2                    | 425 ms                                                                      | 420 ms: 1.01x faster                                                         |
| xml_etree_parse          | 93.9 ms                                                                     | 92.7 ms: 1.01x faster                                                        |
| coroutines               | 12.9 ms                                                                     | 12.8 ms: 1.01x faster                                                        |
| tornado_http             | 84.9 ms                                                                     | 83.9 ms: 1.01x faster                                                        |
| float                    | 50.0 ms                                                                     | 49.5 ms: 1.01x faster                                                        |
| unpickle_pure_python     | 125 us                                                                      | 123 us: 1.01x faster                                                         |
| async_generators         | 237 ms                                                                      | 235 ms: 1.01x faster                                                         |
| nqueens                  | 58.8 ms                                                                     | 58.2 ms: 1.01x faster                                                        |
| deltablue                | 1.96 ms                                                                     | 1.94 ms: 1.01x faster                                                        |
| xml_etree_iterparse      | 63.4 ms                                                                     | 62.7 ms: 1.01x faster                                                        |
| pickle_dict              | 17.6 us                                                                     | 17.5 us: 1.01x faster                                                        |
| pickle                   | 7.16 us                                                                     | 7.10 us: 1.01x faster                                                        |
| sqlglot_parse            | 754 us                                                                      | 747 us: 1.01x faster                                                         |
| pidigits                 | 152 ms                                                                      | 151 ms: 1.01x faster                                                         |
| regex_effbot             | 1.59 ms                                                                     | 1.58 ms: 1.01x faster                                                        |
| 2to3                     | 216 ms                                                                      | 214 ms: 1.01x faster                                                         |
| docutils                 | 1.57 sec                                                                    | 1.56 sec: 1.01x faster                                                       |
| richards                 | 25.0 ms                                                                     | 24.8 ms: 1.01x faster                                                        |
| bench_mp_pool            | 66.1 ms                                                                     | 65.6 ms: 1.01x faster                                                        |
| xml_etree_generate       | 52.6 ms                                                                     | 52.2 ms: 1.01x faster                                                        |
| json_loads               | 13.7 us                                                                     | 13.6 us: 1.01x faster                                                        |
| xml_etree_process        | 36.3 ms                                                                     | 36.1 ms: 1.01x faster                                                        |
| regex_v8                 | 15.2 ms                                                                     | 15.1 ms: 1.00x faster                                                        |
| logging_silent           | 52.2 ns                                                                     | 52.0 ns: 1.00x faster                                                        |
| mdp                      | 1.54 sec                                                                    | 1.54 sec: 1.00x faster                                                       |
| pickle_pure_python       | 173 us                                                                      | 174 us: 1.01x slower                                                         |
| pathlib                  | 74.5 ms                                                                     | 75.2 ms: 1.01x slower                                                        |
| logging_format           | 6.28 us                                                                     | 6.35 us: 1.01x slower                                                        |
| deepcopy_reduce          | 1.89 us                                                                     | 1.91 us: 1.01x slower                                                        |
| typing_runtime_protocols | 69.1 us                                                                     | 70.5 us: 1.02x slower                                                        |
| Geometric mean           | (ref)                                                                       | 1.03x faster                                                                 |

Benchmark hidden because not significant (24): json, async_tree_none, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, python_startup, unpickle, async_tree_memoization_tg, async_tree_none_tg, json_dumps, async_tree_io, dask, python_startup_no_site, generators, sqlite_synth, async_tree_memoization, pycparser, logging_simple, async_tree_io_tg, regex_dna, gc_traversal, pickle_list, unpickle_list, create_gc_cycles, asyncio_tcp


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown