# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.00x faster
- HPT reliability: 54.03%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 223 ms                                                                      | 224 ms: 1.01x slower                                                                  |
| chameleon      | 5.12 ms                                                                     | 5.01 ms: 1.02x faster                                                                 |
| docutils       | 1.62 sec                                                                    | 1.61 sec: 1.01x faster                                                                |
| tornado_http   | 88.3 ms                                                                     | 85.8 ms: 1.03x faster                                                                 |
| Geometric mean | (ref)                                                                       | 1.01x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 472 ms                                                                      | 464 ms: 1.02x faster                                                                  |
| Geometric mean          | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (7): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_none_tg, async_tree_memoization, async_tree_io, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| nbody          | 78.4 ms                                                                     | 78.8 ms: 1.01x slower                                                                 |
| pidigits       | 147 ms                                                                      | 150 ms: 1.02x slower                                                                  |
| float          | 56.3 ms                                                                     | 58.1 ms: 1.03x slower                                                                 |
| Geometric mean | (ref)                                                                       | 1.02x slower                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 84.4 ms                                                                     | 85.8 ms: 1.02x slower                                                                 |
| regex_effbot   | 1.56 ms                                                                     | 1.60 ms: 1.03x slower                                                                 |
| regex_dna      | 118 ms                                                                      | 122 ms: 1.04x slower                                                                  |
| regex_v8       | 14.7 ms                                                                     | 15.2 ms: 1.04x slower                                                                 |
| Geometric mean | (ref)                                                                       | 1.03x slower                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|---------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| json_dumps          | 5.70 ms                                                                     | 5.51 ms: 1.03x faster                                                                 |
| pickle              | 7.30 us                                                                     | 7.11 us: 1.03x faster                                                                 |
| pickle_pure_python  | 183 us                                                                      | 179 us: 1.02x faster                                                                  |
| xml_etree_generate  | 56.0 ms                                                                     | 55.6 ms: 1.01x faster                                                                 |
| xml_etree_process   | 38.2 ms                                                                     | 38.0 ms: 1.01x faster                                                                 |
| json_loads          | 13.8 us                                                                     | 13.7 us: 1.01x faster                                                                 |
| pickle_dict         | 18.7 us                                                                     | 18.6 us: 1.00x faster                                                                 |
| pickle_list         | 2.89 us                                                                     | 2.91 us: 1.01x slower                                                                 |
| unpickle            | 8.35 us                                                                     | 8.45 us: 1.01x slower                                                                 |
| xml_etree_iterparse | 68.2 ms                                                                     | 69.1 ms: 1.01x slower                                                                 |
| xml_etree_parse     | 95.2 ms                                                                     | 96.9 ms: 1.02x slower                                                                 |
| tomli_loads         | 1.42 sec                                                                    | 1.46 sec: 1.02x slower                                                                |
| unpickle_list       | 2.65 us                                                                     | 2.81 us: 1.06x slower                                                                 |
| Geometric mean      | (ref)                                                                       | 1.00x slower                                                                          |

Benchmark hidden because not significant (1): unpickle_pure_python

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup, python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 7.24 ms                                                                     | 7.99 ms: 1.10x slower                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|--------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| asyncio_tcp_ssl          | 1.90 sec                                                                    | 1.49 sec: 1.28x faster                                                                |
| scimark_sor              | 84.4 ms                                                                     | 77.7 ms: 1.09x faster                                                                 |
| generators               | 22.6 ms                                                                     | 20.9 ms: 1.08x faster                                                                 |
| pycparser                | 721 ms                                                                      | 678 ms: 1.06x faster                                                                  |
| coverage                 | 47.7 ms                                                                     | 45.0 ms: 1.06x faster                                                                 |
| scimark_lu               | 59.2 ms                                                                     | 55.9 ms: 1.06x faster                                                                 |
| richards                 | 27.6 ms                                                                     | 26.6 ms: 1.04x faster                                                                 |
| sqlglot_parse            | 810 us                                                                      | 782 us: 1.04x faster                                                                  |
| deepcopy_reduce          | 2.01 us                                                                     | 1.94 us: 1.03x faster                                                                 |
| json_dumps               | 5.70 ms                                                                     | 5.51 ms: 1.03x faster                                                                 |
| unpack_sequence          | 39.9 ns                                                                     | 38.7 ns: 1.03x faster                                                                 |
| tornado_http             | 88.3 ms                                                                     | 85.8 ms: 1.03x faster                                                                 |
| typing_runtime_protocols | 75.7 us                                                                     | 73.7 us: 1.03x faster                                                                 |
| richards_super           | 31.0 ms                                                                     | 30.2 ms: 1.03x faster                                                                 |
| crypto_pyaes             | 48.6 ms                                                                     | 47.3 ms: 1.03x faster                                                                 |
| pickle                   | 7.30 us                                                                     | 7.11 us: 1.03x faster                                                                 |
| chameleon                | 5.12 ms                                                                     | 5.01 ms: 1.02x faster                                                                 |
| deepcopy                 | 228 us                                                                      | 223 us: 1.02x faster                                                                  |
| nqueens                  | 64.9 ms                                                                     | 63.5 ms: 1.02x faster                                                                 |
| sympy_expand             | 285 ms                                                                      | 280 ms: 1.02x faster                                                                  |
| pickle_pure_python       | 183 us                                                                      | 179 us: 1.02x faster                                                                  |
| logging_silent           | 56.1 ns                                                                     | 55.0 ns: 1.02x faster                                                                 |
| async_tree_cpu_io_mixed  | 472 ms                                                                      | 464 ms: 1.02x faster                                                                  |
| bench_thread_pool        | 871 us                                                                      | 857 us: 1.02x faster                                                                  |
| sqlglot_optimize         | 35.6 ms                                                                     | 35.1 ms: 1.01x faster                                                                 |
| sqlglot_transpile        | 1.02 ms                                                                     | 1.01 ms: 1.01x faster                                                                 |
| gc_traversal             | 1.54 ms                                                                     | 1.52 ms: 1.01x faster                                                                 |
| dulwich_log              | 43.5 ms                                                                     | 43.1 ms: 1.01x faster                                                                 |
| spectral_norm            | 81.0 ms                                                                     | 80.3 ms: 1.01x faster                                                                 |
| docutils                 | 1.62 sec                                                                    | 1.61 sec: 1.01x faster                                                                |
| pathlib                  | 80.5 ms                                                                     | 79.8 ms: 1.01x faster                                                                 |
| async_generators         | 232 ms                                                                      | 230 ms: 1.01x faster                                                                  |
| mypy2                    | 434 ms                                                                      | 431 ms: 1.01x faster                                                                  |
| xml_etree_generate       | 56.0 ms                                                                     | 55.6 ms: 1.01x faster                                                                 |
| xml_etree_process        | 38.2 ms                                                                     | 38.0 ms: 1.01x faster                                                                 |
| json_loads               | 13.8 us                                                                     | 13.7 us: 1.01x faster                                                                 |
| pickle_dict              | 18.7 us                                                                     | 18.6 us: 1.00x faster                                                                 |
| nbody                    | 78.4 ms                                                                     | 78.8 ms: 1.01x slower                                                                 |
| scimark_monte_carlo      | 47.8 ms                                                                     | 48.2 ms: 1.01x slower                                                                 |
| pickle_list              | 2.89 us                                                                     | 2.91 us: 1.01x slower                                                                 |
| bench_mp_pool            | 68.2 ms                                                                     | 68.7 ms: 1.01x slower                                                                 |
| logging_simple           | 6.18 us                                                                     | 6.23 us: 1.01x slower                                                                 |
| 2to3                     | 223 ms                                                                      | 224 ms: 1.01x slower                                                                  |
| scimark_fft              | 207 ms                                                                      | 209 ms: 1.01x slower                                                                  |
| pyflate                  | 326 ms                                                                      | 329 ms: 1.01x slower                                                                  |
| sympy_str                | 167 ms                                                                      | 169 ms: 1.01x slower                                                                  |
| unpickle                 | 8.35 us                                                                     | 8.45 us: 1.01x slower                                                                 |
| pprint_pformat           | 1.08 sec                                                                    | 1.09 sec: 1.01x slower                                                                |
| sqlglot_normalize        | 183 ms                                                                      | 186 ms: 1.01x slower                                                                  |
| telco                    | 4.67 ms                                                                     | 4.74 ms: 1.01x slower                                                                 |
| xml_etree_iterparse      | 68.2 ms                                                                     | 69.1 ms: 1.01x slower                                                                 |
| fannkuch                 | 264 ms                                                                      | 268 ms: 1.02x slower                                                                  |
| pidigits                 | 147 ms                                                                      | 150 ms: 1.02x slower                                                                  |
| regex_compile            | 84.4 ms                                                                     | 85.8 ms: 1.02x slower                                                                 |
| xml_etree_parse          | 95.2 ms                                                                     | 96.9 ms: 1.02x slower                                                                 |
| raytrace                 | 174 ms                                                                      | 178 ms: 1.02x slower                                                                  |
| deltablue                | 2.68 ms                                                                     | 2.74 ms: 1.02x slower                                                                 |
| tomli_loads              | 1.42 sec                                                                    | 1.46 sec: 1.02x slower                                                                |
| regex_effbot             | 1.56 ms                                                                     | 1.60 ms: 1.03x slower                                                                 |
| float                    | 56.3 ms                                                                     | 58.1 ms: 1.03x slower                                                                 |
| hexiom                   | 4.85 ms                                                                     | 5.01 ms: 1.03x slower                                                                 |
| regex_dna                | 118 ms                                                                      | 122 ms: 1.04x slower                                                                  |
| regex_v8                 | 14.7 ms                                                                     | 15.2 ms: 1.04x slower                                                                 |
| meteor_contest           | 75.3 ms                                                                     | 78.7 ms: 1.04x slower                                                                 |
| scimark_sparse_mat_mult  | 3.05 ms                                                                     | 3.19 ms: 1.05x slower                                                                 |
| coroutines               | 13.2 ms                                                                     | 13.9 ms: 1.05x slower                                                                 |
| sqlite_synth             | 1.58 us                                                                     | 1.66 us: 1.05x slower                                                                 |
| unpickle_list            | 2.65 us                                                                     | 2.81 us: 1.06x slower                                                                 |
| mako                     | 7.24 ms                                                                     | 7.99 ms: 1.10x slower                                                                 |
| Geometric mean           | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (23): async_tree_memoization_tg, sympy_sum, dask, deepcopy_memo, logging_format, async_tree_cpu_io_mixed_tg, asyncio_tcp, sympy_integrate, go, async_tree_io_tg, chaos, mdp, unpickle_pure_python, comprehensions, async_tree_none_tg, create_gc_cycles, pprint_safe_repr, async_tree_memoization, async_tree_io, python_startup, python_startup_no_site, async_tree_none, json


# HPT report

- Reliability score: 54.03% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown