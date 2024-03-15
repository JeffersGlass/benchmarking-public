# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_superinstructi
- machine: linux-x86_64
- commit hash: c04ea6c
- commit date: 2024-03-01
- overall geometric mean: 1.01x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4+-75c6c05 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| chameleon      | 6.86 ms                                                                | 6.99 ms: 1.02x slower                                                            |
| docutils       | 2.76 sec                                                               | 2.74 sec: 1.01x faster                                                           |
| tornado_http   | 97.1 ms                                                                | 96.3 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4+-75c6c05 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|-------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 716 ms                                                                 | 708 ms: 1.01x faster                                                             |
| async_tree_none_tg      | 456 ms                                                                 | 452 ms: 1.01x faster                                                             |
| async_tree_io           | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| async_tree_io_tg        | 1.20 sec                                                               | 1.21 sec: 1.00x slower                                                           |
| Geometric mean          | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (4): async_tree_none, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4+-75c6c05 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 98.1 ms                                                                | 96.2 ms: 1.02x faster                                                            |
| pidigits       | 187 ms                                                                 | 187 ms: 1.00x faster                                                             |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4+-75c6c05 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.66 ms                                                                | 3.61 ms: 1.01x faster                                                            |
| regex_compile  | 155 ms                                                                 | 153 ms: 1.01x faster                                                             |
| regex_v8       | 25.4 ms                                                                | 25.2 ms: 1.01x faster                                                            |
| regex_dna      | 226 ms                                                                 | 232 ms: 1.03x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4+-75c6c05 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_list          | 5.46 us                                                                | 4.97 us: 1.10x faster                                                            |
| pickle_dict          | 36.4 us                                                                | 34.1 us: 1.07x faster                                                            |
| json_loads           | 28.1 us                                                                | 27.3 us: 1.03x faster                                                            |
| unpickle_pure_python | 248 us                                                                 | 245 us: 1.01x faster                                                             |
| unpickle_list        | 4.98 us                                                                | 4.93 us: 1.01x faster                                                            |
| json_dumps           | 10.4 ms                                                                | 10.3 ms: 1.01x faster                                                            |
| xml_etree_process    | 59.3 ms                                                                | 58.7 ms: 1.01x faster                                                            |
| xml_etree_parse      | 157 ms                                                                 | 156 ms: 1.01x faster                                                             |
| tomli_loads          | 2.18 sec                                                               | 2.16 sec: 1.01x faster                                                           |
| pickle               | 11.7 us                                                                | 11.7 us: 1.00x faster                                                            |
| pickle_pure_python   | 297 us                                                                 | 299 us: 1.00x slower                                                             |
| xml_etree_generate   | 86.3 ms                                                                | 86.8 ms: 1.01x slower                                                            |
| unpickle             | 15.0 us                                                                | 16.2 us: 1.08x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4+-75c6c05 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup_no_site | 10.9 ms                                                                | 10.9 ms: 1.00x slower                                                            |
| python_startup         | 12.2 ms                                                                | 12.3 ms: 1.00x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4+-75c6c05 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.6 ms                                                                | 11.9 ms: 1.02x slower                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240228-linux-x86_64-python-75c6c05fea212330f4b0-3.13.0a4+-75c6c05 | bm-20240301-linux-x86_64-Fidget%2dSpinner-tier2_superinstructi-3.13.0a4+-c04ea6c |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_list              | 5.46 us                                                                | 4.97 us: 1.10x faster                                                            |
| raytrace                 | 300 ms                                                                 | 276 ms: 1.09x faster                                                             |
| pickle_dict              | 36.4 us                                                                | 34.1 us: 1.07x faster                                                            |
| spectral_norm            | 126 ms                                                                 | 120 ms: 1.05x faster                                                             |
| gc_traversal             | 3.87 ms                                                                | 3.72 ms: 1.04x faster                                                            |
| typing_runtime_protocols | 113 us                                                                 | 110 us: 1.03x faster                                                             |
| deepcopy                 | 357 us                                                                 | 347 us: 1.03x faster                                                             |
| json_loads               | 28.1 us                                                                | 27.3 us: 1.03x faster                                                            |
| nqueens                  | 93.9 ms                                                                | 91.4 ms: 1.03x faster                                                            |
| deepcopy_memo            | 40.1 us                                                                | 39.0 us: 1.03x faster                                                            |
| scimark_sparse_mat_mult  | 5.21 ms                                                                | 5.08 ms: 1.03x faster                                                            |
| scimark_lu               | 134 ms                                                                 | 131 ms: 1.02x faster                                                             |
| mdp                      | 2.72 sec                                                               | 2.66 sec: 1.02x faster                                                           |
| nbody                    | 98.1 ms                                                                | 96.2 ms: 1.02x faster                                                            |
| scimark_fft              | 360 ms                                                                 | 354 ms: 1.02x faster                                                             |
| sqlglot_transpile        | 1.67 ms                                                                | 1.65 ms: 1.02x faster                                                            |
| sqlglot_parse            | 1.34 ms                                                                | 1.31 ms: 1.02x faster                                                            |
| chaos                    | 65.9 ms                                                                | 64.8 ms: 1.02x faster                                                            |
| sqlglot_normalize        | 111 ms                                                                 | 109 ms: 1.02x faster                                                             |
| meteor_contest           | 110 ms                                                                 | 108 ms: 1.02x faster                                                             |
| regex_effbot             | 3.66 ms                                                                | 3.61 ms: 1.01x faster                                                            |
| unpickle_pure_python     | 248 us                                                                 | 245 us: 1.01x faster                                                             |
| coverage                 | 97.5 ms                                                                | 96.3 ms: 1.01x faster                                                            |
| regex_compile            | 155 ms                                                                 | 153 ms: 1.01x faster                                                             |
| sympy_str                | 290 ms                                                                 | 286 ms: 1.01x faster                                                             |
| async_tree_cpu_io_mixed  | 716 ms                                                                 | 708 ms: 1.01x faster                                                             |
| unpickle_list            | 4.98 us                                                                | 4.93 us: 1.01x faster                                                            |
| sympy_integrate          | 21.7 ms                                                                | 21.5 ms: 1.01x faster                                                            |
| sympy_sum                | 163 ms                                                                 | 161 ms: 1.01x faster                                                             |
| sympy_expand             | 490 ms                                                                 | 485 ms: 1.01x faster                                                             |
| coroutines               | 22.3 ms                                                                | 22.1 ms: 1.01x faster                                                            |
| sqlglot_optimize         | 57.3 ms                                                                | 56.7 ms: 1.01x faster                                                            |
| json_dumps               | 10.4 ms                                                                | 10.3 ms: 1.01x faster                                                            |
| xml_etree_process        | 59.3 ms                                                                | 58.7 ms: 1.01x faster                                                            |
| regex_v8                 | 25.4 ms                                                                | 25.2 ms: 1.01x faster                                                            |
| pyflate                  | 514 ms                                                                 | 509 ms: 1.01x faster                                                             |
| xml_etree_parse          | 157 ms                                                                 | 156 ms: 1.01x faster                                                             |
| async_tree_none_tg       | 456 ms                                                                 | 452 ms: 1.01x faster                                                             |
| tornado_http             | 97.1 ms                                                                | 96.3 ms: 1.01x faster                                                            |
| tomli_loads              | 2.18 sec                                                               | 2.16 sec: 1.01x faster                                                           |
| dulwich_log              | 69.9 ms                                                                | 69.3 ms: 1.01x faster                                                            |
| async_tree_io            | 1.20 sec                                                               | 1.19 sec: 1.01x faster                                                           |
| docutils                 | 2.76 sec                                                               | 2.74 sec: 1.01x faster                                                           |
| unpack_sequence          | 127 ns                                                                 | 126 ns: 1.01x faster                                                             |
| logging_silent           | 101 ns                                                                 | 101 ns: 1.01x faster                                                             |
| richards_super           | 56.3 ms                                                                | 56.0 ms: 1.01x faster                                                            |
| generators               | 29.4 ms                                                                | 29.3 ms: 1.01x faster                                                            |
| deepcopy_reduce          | 3.13 us                                                                | 3.12 us: 1.01x faster                                                            |
| pickle                   | 11.7 us                                                                | 11.7 us: 1.00x faster                                                            |
| create_gc_cycles         | 1.50 ms                                                                | 1.50 ms: 1.00x faster                                                            |
| pidigits                 | 187 ms                                                                 | 187 ms: 1.00x faster                                                             |
| asyncio_tcp_ssl          | 1.80 sec                                                               | 1.80 sec: 1.00x slower                                                           |
| python_startup_no_site   | 10.9 ms                                                                | 10.9 ms: 1.00x slower                                                            |
| python_startup           | 12.2 ms                                                                | 12.3 ms: 1.00x slower                                                            |
| asyncio_tcp              | 490 ms                                                                 | 492 ms: 1.00x slower                                                             |
| async_tree_io_tg         | 1.20 sec                                                               | 1.21 sec: 1.00x slower                                                           |
| pickle_pure_python       | 297 us                                                                 | 299 us: 1.00x slower                                                             |
| xml_etree_generate       | 86.3 ms                                                                | 86.8 ms: 1.01x slower                                                            |
| async_generators         | 459 ms                                                                 | 463 ms: 1.01x slower                                                             |
| hexiom                   | 7.64 ms                                                                | 7.74 ms: 1.01x slower                                                            |
| telco                    | 8.47 ms                                                                | 8.59 ms: 1.01x slower                                                            |
| logging_simple           | 5.77 us                                                                | 5.86 us: 1.01x slower                                                            |
| mako                     | 11.6 ms                                                                | 11.9 ms: 1.02x slower                                                            |
| chameleon                | 6.86 ms                                                                | 6.99 ms: 1.02x slower                                                            |
| regex_dna                | 226 ms                                                                 | 232 ms: 1.03x slower                                                             |
| unpickle                 | 15.0 us                                                                | 16.2 us: 1.08x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (26): async_tree_none, async_tree_memoization, async_tree_cpu_io_mixed_tg, pprint_safe_repr, scimark_sor, xml_etree_iterparse, comprehensions, bench_mp_pool, deltablue, go, richards, async_tree_memoization_tg, mypy2, pathlib, pycparser, asyncio_websockets, crypto_pyaes, bench_thread_pool, sqlite_synth, json, 2to3, fannkuch, logging_format, scimark_monte_carlo, float, pprint_pformat


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x