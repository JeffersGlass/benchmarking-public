# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 176 ms                                                                 | 174 ms: 1.01x faster                                                             |
| chameleon      | 5.04 ms                                                                | 5.06 ms: 1.01x slower                                                            |
| docutils       | 1.51 sec                                                               | 1.50 sec: 1.01x faster                                                           |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 532 ms                                                                 | 526 ms: 1.01x faster                                                             |
| async_tree_io           | 714 ms                                                                 | 710 ms: 1.01x faster                                                             |
| async_tree_none_tg      | 268 ms                                                                 | 267 ms: 1.01x faster                                                             |
| Geometric mean          | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (5): async_tree_none, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, async_tree_io_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 97.3 ms                                                                | 82.1 ms: 1.19x faster                                                            |
| float          | 74.6 ms                                                                | 67.0 ms: 1.11x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.10x faster                                                                     |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 84.8 ms                                                                | 81.5 ms: 1.04x faster                                                            |
| regex_v8       | 18.1 ms                                                                | 18.2 ms: 1.00x slower                                                            |
| regex_effbot   | 2.78 ms                                                                | 2.81 ms: 1.01x slower                                                            |
| regex_dna      | 157 ms                                                                 | 159 ms: 1.01x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tomli_loads          | 1.80 sec                                                               | 1.64 sec: 1.10x faster                                                           |
| xml_etree_generate   | 60.1 ms                                                                | 58.3 ms: 1.03x faster                                                            |
| unpickle_pure_python | 167 us                                                                 | 163 us: 1.02x faster                                                             |
| xml_etree_iterparse  | 83.2 ms                                                                | 81.4 ms: 1.02x faster                                                            |
| xml_etree_process    | 41.6 ms                                                                | 40.9 ms: 1.02x faster                                                            |
| pickle               | 7.29 us                                                                | 7.23 us: 1.01x faster                                                            |
| unpickle             | 9.21 us                                                                | 9.14 us: 1.01x faster                                                            |
| json_loads           | 17.2 us                                                                | 17.1 us: 1.00x faster                                                            |
| Geometric mean       | (ref)                                                                  | 1.02x faster                                                                     |

Benchmark hidden because not significant (6): unpickle_list, pickle_pure_python, json_dumps, pickle_dict, pickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 12.9 ms                                                                | 12.8 ms: 1.00x faster                                                            |
| python_startup_no_site | 11.4 ms                                                                | 11.5 ms: 1.00x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.8 ms                                                                | 9.60 ms: 1.12x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240124-darwin-arm64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d | bm-20240128-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| spectral_norm            | 119 ms                                                                 | 98.2 ms: 1.21x faster                                                            |
| nbody                    | 97.3 ms                                                                | 82.1 ms: 1.19x faster                                                            |
| scimark_fft              | 276 ms                                                                 | 233 ms: 1.18x faster                                                             |
| scimark_sparse_mat_mult  | 4.52 ms                                                                | 3.96 ms: 1.14x faster                                                            |
| mako                     | 10.8 ms                                                                | 9.60 ms: 1.12x faster                                                            |
| float                    | 74.6 ms                                                                | 67.0 ms: 1.11x faster                                                            |
| deltablue                | 3.92 ms                                                                | 3.52 ms: 1.11x faster                                                            |
| comprehensions           | 16.8 us                                                                | 15.2 us: 1.11x faster                                                            |
| tomli_loads              | 1.80 sec                                                               | 1.64 sec: 1.10x faster                                                           |
| hexiom                   | 6.47 ms                                                                | 5.88 ms: 1.10x faster                                                            |
| chaos                    | 49.9 ms                                                                | 45.6 ms: 1.09x faster                                                            |
| asyncio_tcp              | 443 ms                                                                 | 411 ms: 1.08x faster                                                             |
| scimark_monte_carlo      | 60.0 ms                                                                | 56.3 ms: 1.07x faster                                                            |
| pyflate                  | 391 ms                                                                 | 367 ms: 1.07x faster                                                             |
| nqueens                  | 71.8 ms                                                                | 67.4 ms: 1.06x faster                                                            |
| crypto_pyaes             | 58.5 ms                                                                | 55.1 ms: 1.06x faster                                                            |
| pprint_pformat           | 1.22 sec                                                               | 1.16 sec: 1.05x faster                                                           |
| pprint_safe_repr         | 591 ms                                                                 | 567 ms: 1.04x faster                                                             |
| regex_compile            | 84.8 ms                                                                | 81.5 ms: 1.04x faster                                                            |
| xml_etree_generate       | 60.1 ms                                                                | 58.3 ms: 1.03x faster                                                            |
| telco                    | 4.75 ms                                                                | 4.61 ms: 1.03x faster                                                            |
| fannkuch                 | 333 ms                                                                 | 323 ms: 1.03x faster                                                             |
| meteor_contest           | 79.3 ms                                                                | 77.1 ms: 1.03x faster                                                            |
| typing_runtime_protocols | 75.3 us                                                                | 73.3 us: 1.03x faster                                                            |
| go                       | 115 ms                                                                 | 112 ms: 1.03x faster                                                             |
| logging_simple           | 3.64 us                                                                | 3.54 us: 1.03x faster                                                            |
| raytrace                 | 189 ms                                                                 | 185 ms: 1.03x faster                                                             |
| unpickle_pure_python     | 167 us                                                                 | 163 us: 1.02x faster                                                             |
| logging_format           | 3.94 us                                                                | 3.84 us: 1.02x faster                                                            |
| sympy_str                | 151 ms                                                                 | 148 ms: 1.02x faster                                                             |
| xml_etree_iterparse      | 83.2 ms                                                                | 81.4 ms: 1.02x faster                                                            |
| sympy_sum                | 80.4 ms                                                                | 78.7 ms: 1.02x faster                                                            |
| deepcopy_memo            | 27.2 us                                                                | 26.6 us: 1.02x faster                                                            |
| asyncio_tcp_ssl          | 1.26 sec                                                               | 1.24 sec: 1.02x faster                                                           |
| sqlglot_normalize        | 193 ms                                                                 | 190 ms: 1.02x faster                                                             |
| sympy_integrate          | 11.8 ms                                                                | 11.5 ms: 1.02x faster                                                            |
| mdp                      | 1.65 sec                                                               | 1.62 sec: 1.02x faster                                                           |
| xml_etree_process        | 41.6 ms                                                                | 40.9 ms: 1.02x faster                                                            |
| sqlite_synth             | 1.66 us                                                                | 1.63 us: 1.02x faster                                                            |
| richards                 | 33.1 ms                                                                | 32.6 ms: 1.02x faster                                                            |
| sqlglot_optimize         | 36.4 ms                                                                | 35.8 ms: 1.02x faster                                                            |
| scimark_lu               | 78.0 ms                                                                | 76.9 ms: 1.01x faster                                                            |
| sqlglot_transpile        | 1.01 ms                                                                | 991 us: 1.01x faster                                                             |
| richards_super           | 36.9 ms                                                                | 36.5 ms: 1.01x faster                                                            |
| pathlib                  | 25.1 ms                                                                | 24.8 ms: 1.01x faster                                                            |
| sympy_expand             | 248 ms                                                                 | 245 ms: 1.01x faster                                                             |
| generators               | 28.9 ms                                                                | 28.6 ms: 1.01x faster                                                            |
| deepcopy                 | 229 us                                                                 | 226 us: 1.01x faster                                                             |
| async_tree_cpu_io_mixed  | 532 ms                                                                 | 526 ms: 1.01x faster                                                             |
| scimark_sor              | 107 ms                                                                 | 106 ms: 1.01x faster                                                             |
| unpack_sequence          | 28.3 ns                                                                | 28.1 ns: 1.01x faster                                                            |
| pickle                   | 7.29 us                                                                | 7.23 us: 1.01x faster                                                            |
| 2to3                     | 176 ms                                                                 | 174 ms: 1.01x faster                                                             |
| logging_silent           | 72.5 ns                                                                | 71.9 ns: 1.01x faster                                                            |
| sqlglot_parse            | 818 us                                                                 | 812 us: 1.01x faster                                                             |
| unpickle                 | 9.21 us                                                                | 9.14 us: 1.01x faster                                                            |
| json                     | 2.98 ms                                                                | 2.96 ms: 1.01x faster                                                            |
| docutils                 | 1.51 sec                                                               | 1.50 sec: 1.01x faster                                                           |
| async_tree_io            | 714 ms                                                                 | 710 ms: 1.01x faster                                                             |
| async_tree_none_tg       | 268 ms                                                                 | 267 ms: 1.01x faster                                                             |
| dulwich_log              | 30.2 ms                                                                | 30.0 ms: 1.01x faster                                                            |
| bench_thread_pool        | 514 us                                                                 | 512 us: 1.00x faster                                                             |
| json_loads               | 17.2 us                                                                | 17.1 us: 1.00x faster                                                            |
| python_startup           | 12.9 ms                                                                | 12.8 ms: 1.00x faster                                                            |
| coroutines               | 19.5 ms                                                                | 19.5 ms: 1.00x faster                                                            |
| create_gc_cycles         | 709 us                                                                 | 711 us: 1.00x slower                                                             |
| python_startup_no_site   | 11.4 ms                                                                | 11.5 ms: 1.00x slower                                                            |
| regex_v8                 | 18.1 ms                                                                | 18.2 ms: 1.00x slower                                                            |
| chameleon                | 5.04 ms                                                                | 5.06 ms: 1.01x slower                                                            |
| regex_effbot             | 2.78 ms                                                                | 2.81 ms: 1.01x slower                                                            |
| regex_dna                | 157 ms                                                                 | 159 ms: 1.01x slower                                                             |
| coverage                 | 48.1 ms                                                                | 51.0 ms: 1.06x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.03x faster                                                                     |

Benchmark hidden because not significant (21): async_tree_none, tornado_http, async_tree_memoization, pycparser, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, mypy2, async_tree_io_tg, unpickle_list, pickle_pure_python, json_dumps, pickle_dict, pidigits, deepcopy_reduce, asyncio_websockets, dask, gc_traversal, async_generators, pickle_list, bench_mp_pool, xml_etree_parse


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x