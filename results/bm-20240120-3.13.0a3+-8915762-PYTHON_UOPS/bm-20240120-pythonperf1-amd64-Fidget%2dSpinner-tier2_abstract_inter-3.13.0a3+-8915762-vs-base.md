# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: 8915762
- commit date: 2024-01-20
- overall geometric mean: 1.00x slower
- HPT reliability: 77.62%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                                      | 223 ms: 1.02x slower                                                                  |
| chameleon      | 4.90 ms                                                                     | 5.03 ms: 1.03x slower                                                                 |
| Geometric mean | (ref)                                                                       | 1.01x slower                                                                          |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_io_tg | 747 ms                                                                      | 738 ms: 1.01x faster                                                                  |
| Geometric mean   | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (7): async_tree_io, async_tree_cpu_io_mixed_tg, async_tree_none_tg, async_tree_memoization_tg, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| nbody          | 83.1 ms                                                                     | 81.4 ms: 1.02x faster                                                                 |
| Geometric mean | (ref)                                                                       | 1.01x faster                                                                          |

Benchmark hidden because not significant (2): float, pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_dna      | 121 ms                                                                      | 118 ms: 1.02x faster                                                                  |
| regex_effbot   | 1.59 ms                                                                     | 1.57 ms: 1.01x faster                                                                 |
| regex_compile  | 84.8 ms                                                                     | 84.4 ms: 1.00x faster                                                                 |
| Geometric mean | (ref)                                                                       | 1.01x faster                                                                          |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pickle_list          | 3.28 us                                                                     | 3.09 us: 1.06x faster                                                                 |
| pickle_dict          | 18.8 us                                                                     | 18.3 us: 1.02x faster                                                                 |
| xml_etree_generate   | 55.5 ms                                                                     | 54.5 ms: 1.02x faster                                                                 |
| xml_etree_process    | 37.7 ms                                                                     | 37.1 ms: 1.02x faster                                                                 |
| xml_etree_iterparse  | 67.0 ms                                                                     | 66.3 ms: 1.01x faster                                                                 |
| tomli_loads          | 1.43 sec                                                                    | 1.44 sec: 1.00x slower                                                                |
| json_loads           | 13.4 us                                                                     | 13.5 us: 1.01x slower                                                                 |
| pickle               | 7.30 us                                                                     | 7.41 us: 1.01x slower                                                                 |
| xml_etree_parse      | 92.6 ms                                                                     | 94.0 ms: 1.01x slower                                                                 |
| unpickle_list        | 2.75 us                                                                     | 2.79 us: 1.02x slower                                                                 |
| pickle_pure_python   | 176 us                                                                      | 180 us: 1.03x slower                                                                  |
| unpickle_pure_python | 133 us                                                                      | 137 us: 1.03x slower                                                                  |
| Geometric mean       | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (2): unpickle, json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup_no_site | 18.2 ms                                                                     | 18.5 ms: 1.02x slower                                                                 |
| python_startup         | 20.5 ms                                                                     | 21.0 ms: 1.02x slower                                                                 |
| Geometric mean         | (ref)                                                                       | 1.02x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|-----------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.66 ms                                                                     | 7.50 ms: 1.02x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20240118-pythonperf1-amd64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|--------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pickle_list              | 3.28 us                                                                     | 3.09 us: 1.06x faster                                                                 |
| mdp                      | 1.44 sec                                                                    | 1.36 sec: 1.06x faster                                                                |
| scimark_fft              | 215 ms                                                                      | 202 ms: 1.06x faster                                                                  |
| spectral_norm            | 85.2 ms                                                                     | 80.6 ms: 1.06x faster                                                                 |
| coverage                 | 47.1 ms                                                                     | 45.0 ms: 1.05x faster                                                                 |
| scimark_sparse_mat_mult  | 3.29 ms                                                                     | 3.19 ms: 1.03x faster                                                                 |
| regex_dna                | 121 ms                                                                      | 118 ms: 1.02x faster                                                                  |
| pickle_dict              | 18.8 us                                                                     | 18.3 us: 1.02x faster                                                                 |
| mako                     | 7.66 ms                                                                     | 7.50 ms: 1.02x faster                                                                 |
| nbody                    | 83.1 ms                                                                     | 81.4 ms: 1.02x faster                                                                 |
| fannkuch                 | 272 ms                                                                      | 267 ms: 1.02x faster                                                                  |
| typing_runtime_protocols | 74.0 us                                                                     | 72.5 us: 1.02x faster                                                                 |
| xml_etree_generate       | 55.5 ms                                                                     | 54.5 ms: 1.02x faster                                                                 |
| comprehensions           | 12.9 us                                                                     | 12.7 us: 1.02x faster                                                                 |
| crypto_pyaes             | 48.7 ms                                                                     | 47.9 ms: 1.02x faster                                                                 |
| generators               | 21.9 ms                                                                     | 21.6 ms: 1.02x faster                                                                 |
| xml_etree_process        | 37.7 ms                                                                     | 37.1 ms: 1.02x faster                                                                 |
| logging_simple           | 6.32 us                                                                     | 6.23 us: 1.01x faster                                                                 |
| dulwich_log              | 42.6 ms                                                                     | 42.1 ms: 1.01x faster                                                                 |
| async_tree_io_tg         | 747 ms                                                                      | 738 ms: 1.01x faster                                                                  |
| xml_etree_iterparse      | 67.0 ms                                                                     | 66.3 ms: 1.01x faster                                                                 |
| regex_effbot             | 1.59 ms                                                                     | 1.57 ms: 1.01x faster                                                                 |
| meteor_contest           | 76.7 ms                                                                     | 75.9 ms: 1.01x faster                                                                 |
| coroutines               | 13.4 ms                                                                     | 13.3 ms: 1.01x faster                                                                 |
| chaos                    | 44.1 ms                                                                     | 43.8 ms: 1.01x faster                                                                 |
| deepcopy                 | 224 us                                                                      | 223 us: 1.01x faster                                                                  |
| regex_compile            | 84.8 ms                                                                     | 84.4 ms: 1.00x faster                                                                 |
| pprint_pformat           | 1.07 sec                                                                    | 1.06 sec: 1.00x faster                                                                |
| hexiom                   | 4.92 ms                                                                     | 4.94 ms: 1.00x slower                                                                 |
| pprint_safe_repr         | 517 ms                                                                      | 519 ms: 1.00x slower                                                                  |
| tomli_loads              | 1.43 sec                                                                    | 1.44 sec: 1.00x slower                                                                |
| sympy_str                | 166 ms                                                                      | 167 ms: 1.01x slower                                                                  |
| deepcopy_memo            | 22.4 us                                                                     | 22.5 us: 1.01x slower                                                                 |
| mypy2                    | 421 ms                                                                      | 423 ms: 1.01x slower                                                                  |
| sqlglot_parse            | 771 us                                                                      | 776 us: 1.01x slower                                                                  |
| logging_format           | 6.69 us                                                                     | 6.74 us: 1.01x slower                                                                 |
| sympy_expand             | 278 ms                                                                      | 280 ms: 1.01x slower                                                                  |
| json_loads               | 13.4 us                                                                     | 13.5 us: 1.01x slower                                                                 |
| sqlglot_normalize        | 181 ms                                                                      | 182 ms: 1.01x slower                                                                  |
| sqlglot_transpile        | 994 us                                                                      | 1.00 ms: 1.01x slower                                                                 |
| sqlglot_optimize         | 34.6 ms                                                                     | 34.9 ms: 1.01x slower                                                                 |
| unpack_sequence          | 39.1 ns                                                                     | 39.5 ns: 1.01x slower                                                                 |
| richards_super           | 30.3 ms                                                                     | 30.7 ms: 1.01x slower                                                                 |
| deltablue                | 2.69 ms                                                                     | 2.73 ms: 1.01x slower                                                                 |
| sympy_integrate          | 13.0 ms                                                                     | 13.2 ms: 1.01x slower                                                                 |
| pickle                   | 7.30 us                                                                     | 7.41 us: 1.01x slower                                                                 |
| xml_etree_parse          | 92.6 ms                                                                     | 94.0 ms: 1.01x slower                                                                 |
| nqueens                  | 64.5 ms                                                                     | 65.5 ms: 1.02x slower                                                                 |
| async_generators         | 232 ms                                                                      | 236 ms: 1.02x slower                                                                  |
| unpickle_list            | 2.75 us                                                                     | 2.79 us: 1.02x slower                                                                 |
| python_startup_no_site   | 18.2 ms                                                                     | 18.5 ms: 1.02x slower                                                                 |
| gc_traversal             | 1.48 ms                                                                     | 1.51 ms: 1.02x slower                                                                 |
| 2to3                     | 218 ms                                                                      | 223 ms: 1.02x slower                                                                  |
| go                       | 90.4 ms                                                                     | 92.3 ms: 1.02x slower                                                                 |
| sqlite_synth             | 1.58 us                                                                     | 1.61 us: 1.02x slower                                                                 |
| python_startup           | 20.5 ms                                                                     | 21.0 ms: 1.02x slower                                                                 |
| chameleon                | 4.90 ms                                                                     | 5.03 ms: 1.03x slower                                                                 |
| pickle_pure_python       | 176 us                                                                      | 180 us: 1.03x slower                                                                  |
| unpickle_pure_python     | 133 us                                                                      | 137 us: 1.03x slower                                                                  |
| telco                    | 4.65 ms                                                                     | 4.80 ms: 1.03x slower                                                                 |
| scimark_lu               | 54.4 ms                                                                     | 56.2 ms: 1.03x slower                                                                 |
| scimark_sor              | 76.3 ms                                                                     | 79.0 ms: 1.04x slower                                                                 |
| bench_mp_pool            | 67.2 ms                                                                     | 69.7 ms: 1.04x slower                                                                 |
| asyncio_tcp_ssl          | 1.62 sec                                                                    | 1.75 sec: 1.08x slower                                                                |
| Geometric mean           | (ref)                                                                       | 1.00x slower                                                                          |

Benchmark hidden because not significant (28): asyncio_tcp, async_tree_io, unpickle, deepcopy_reduce, raytrace, pycparser, async_tree_cpu_io_mixed_tg, async_tree_none_tg, scimark_monte_carlo, json_dumps, float, logging_silent, pyflate, pidigits, regex_v8, richards, async_tree_memoization_tg, docutils, pathlib, tornado_http, async_tree_memoization, sympy_sum, async_tree_cpu_io_mixed, create_gc_cycles, dask, async_tree_none, bench_thread_pool, json


# HPT report

- Reliability score: 77.62% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown