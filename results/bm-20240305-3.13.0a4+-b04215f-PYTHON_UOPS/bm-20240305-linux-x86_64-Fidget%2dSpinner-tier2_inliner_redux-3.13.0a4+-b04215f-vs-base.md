# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_inliner_redux
- machine: linux-x86_64
- commit hash: b04215f
- commit date: 2024-03-05
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 293 ms                                                                 | 300 ms: 1.02x slower                                                            |
| chameleon      | 6.90 ms                                                                | 7.00 ms: 1.01x slower                                                           |
| docutils       | 2.82 sec                                                               | 2.84 sec: 1.01x slower                                                          |
| tornado_http   | 99.7 ms                                                                | 102 ms: 1.02x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|-------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_none_tg      | 457 ms                                                                 | 462 ms: 1.01x slower                                                            |
| async_tree_io_tg        | 1.23 sec                                                               | 1.25 sec: 1.02x slower                                                          |
| async_tree_cpu_io_mixed | 723 ms                                                                 | 737 ms: 1.02x slower                                                            |
| async_tree_memoization  | 577 ms                                                                 | 592 ms: 1.03x slower                                                            |
| async_tree_none         | 450 ms                                                                 | 462 ms: 1.03x slower                                                            |
| async_tree_io           | 1.21 sec                                                               | 1.25 sec: 1.04x slower                                                          |
| Geometric mean          | (ref)                                                                  | 1.02x slower                                                                    |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 188 ms                                                                 | 190 ms: 1.01x slower                                                            |
| nbody          | 121 ms                                                                 | 132 ms: 1.09x slower                                                            |
| float          | 95.3 ms                                                                | 106 ms: 1.11x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.07x slower                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_dna      | 216 ms                                                                 | 213 ms: 1.01x faster                                                            |
| regex_v8       | 24.0 ms                                                                | 24.4 ms: 1.02x slower                                                           |
| regex_effbot   | 3.45 ms                                                                | 3.55 ms: 1.03x slower                                                           |
| regex_compile  | 176 ms                                                                 | 191 ms: 1.09x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.03x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|----------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 10.5 ms                                                                | 10.4 ms: 1.01x faster                                                           |
| pickle_pure_python   | 305 us                                                                 | 303 us: 1.01x faster                                                            |
| pickle               | 11.8 us                                                                | 11.9 us: 1.01x slower                                                           |
| pickle_dict          | 34.8 us                                                                | 35.1 us: 1.01x slower                                                           |
| xml_etree_parse      | 158 ms                                                                 | 159 ms: 1.01x slower                                                            |
| json_loads           | 27.5 us                                                                | 27.9 us: 1.01x slower                                                           |
| xml_etree_process    | 61.5 ms                                                                | 63.1 ms: 1.03x slower                                                           |
| pickle_list          | 5.18 us                                                                | 5.33 us: 1.03x slower                                                           |
| xml_etree_generate   | 89.8 ms                                                                | 93.3 ms: 1.04x slower                                                           |
| xml_etree_iterparse  | 111 ms                                                                 | 116 ms: 1.05x slower                                                            |
| unpickle_list        | 4.74 us                                                                | 5.12 us: 1.08x slower                                                           |
| tomli_loads          | 2.56 sec                                                               | 2.79 sec: 1.09x slower                                                          |
| unpickle_pure_python | 282 us                                                                 | 309 us: 1.09x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.03x slower                                                                    |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup_no_site | 8.81 ms                                                                | 8.84 ms: 1.00x slower                                                           |
| python_startup         | 10.2 ms                                                                | 10.2 ms: 1.01x slower                                                           |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|-----------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 13.4 ms                                                                | 15.1 ms: 1.12x slower                                                           |

All benchmarks:
===============

| Benchmark                | bm-20240304-linux-x86_64-python-ffed8d985b57a97def2e-3.13.0a4+-ffed8d9 | bm-20240305-linux-x86_64-Fidget%2dSpinner-tier2_inliner_redux-3.13.0a4+-b04215f |
|--------------------------|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| logging_simple           | 6.15 us                                                                | 6.00 us: 1.03x faster                                                           |
| logging_format           | 6.91 us                                                                | 6.79 us: 1.02x faster                                                           |
| json_dumps               | 10.5 ms                                                                | 10.4 ms: 1.01x faster                                                           |
| regex_dna                | 216 ms                                                                 | 213 ms: 1.01x faster                                                            |
| async_generators         | 466 ms                                                                 | 462 ms: 1.01x faster                                                            |
| dulwich_log              | 72.6 ms                                                                | 72.1 ms: 1.01x faster                                                           |
| pickle_pure_python       | 305 us                                                                 | 303 us: 1.01x faster                                                            |
| create_gc_cycles         | 1.51 ms                                                                | 1.50 ms: 1.00x faster                                                           |
| asyncio_tcp_ssl          | 1.80 sec                                                               | 1.80 sec: 1.00x slower                                                          |
| python_startup_no_site   | 8.81 ms                                                                | 8.84 ms: 1.00x slower                                                           |
| pickle                   | 11.8 us                                                                | 11.9 us: 1.01x slower                                                           |
| pidigits                 | 188 ms                                                                 | 190 ms: 1.01x slower                                                            |
| pickle_dict              | 34.8 us                                                                | 35.1 us: 1.01x slower                                                           |
| python_startup           | 10.2 ms                                                                | 10.2 ms: 1.01x slower                                                           |
| docutils                 | 2.82 sec                                                               | 2.84 sec: 1.01x slower                                                          |
| xml_etree_parse          | 158 ms                                                                 | 159 ms: 1.01x slower                                                            |
| pathlib                  | 19.0 ms                                                                | 19.2 ms: 1.01x slower                                                           |
| bench_thread_pool        | 858 us                                                                 | 867 us: 1.01x slower                                                            |
| sympy_sum                | 164 ms                                                                 | 166 ms: 1.01x slower                                                            |
| async_tree_none_tg       | 457 ms                                                                 | 462 ms: 1.01x slower                                                            |
| json_loads               | 27.5 us                                                                | 27.9 us: 1.01x slower                                                           |
| chameleon                | 6.90 ms                                                                | 7.00 ms: 1.01x slower                                                           |
| regex_v8                 | 24.0 ms                                                                | 24.4 ms: 1.02x slower                                                           |
| sympy_integrate          | 21.3 ms                                                                | 21.6 ms: 1.02x slower                                                           |
| sqlglot_normalize        | 112 ms                                                                 | 114 ms: 1.02x slower                                                            |
| coverage                 | 95.6 ms                                                                | 97.4 ms: 1.02x slower                                                           |
| async_tree_io_tg         | 1.23 sec                                                               | 1.25 sec: 1.02x slower                                                          |
| async_tree_cpu_io_mixed  | 723 ms                                                                 | 737 ms: 1.02x slower                                                            |
| sqlglot_transpile        | 1.78 ms                                                                | 1.82 ms: 1.02x slower                                                           |
| sqlite_synth             | 2.92 us                                                                | 2.98 us: 1.02x slower                                                           |
| pycparser                | 1.27 sec                                                               | 1.30 sec: 1.02x slower                                                          |
| sympy_expand             | 504 ms                                                                 | 514 ms: 1.02x slower                                                            |
| 2to3                     | 293 ms                                                                 | 300 ms: 1.02x slower                                                            |
| asyncio_tcp              | 478 ms                                                                 | 489 ms: 1.02x slower                                                            |
| sympy_str                | 299 ms                                                                 | 306 ms: 1.02x slower                                                            |
| telco                    | 8.64 ms                                                                | 8.84 ms: 1.02x slower                                                           |
| deepcopy                 | 357 us                                                                 | 366 us: 1.02x slower                                                            |
| tornado_http             | 99.7 ms                                                                | 102 ms: 1.02x slower                                                            |
| async_tree_memoization   | 577 ms                                                                 | 592 ms: 1.03x slower                                                            |
| scimark_sor              | 144 ms                                                                 | 148 ms: 1.03x slower                                                            |
| xml_etree_process        | 61.5 ms                                                                | 63.1 ms: 1.03x slower                                                           |
| regex_effbot             | 3.45 ms                                                                | 3.55 ms: 1.03x slower                                                           |
| async_tree_none          | 450 ms                                                                 | 462 ms: 1.03x slower                                                            |
| coroutines               | 22.1 ms                                                                | 22.7 ms: 1.03x slower                                                           |
| pickle_list              | 5.18 us                                                                | 5.33 us: 1.03x slower                                                           |
| logging_silent           | 102 ns                                                                 | 105 ns: 1.03x slower                                                            |
| sqlglot_parse            | 1.43 ms                                                                | 1.48 ms: 1.03x slower                                                           |
| meteor_contest           | 118 ms                                                                 | 122 ms: 1.04x slower                                                            |
| sqlglot_optimize         | 60.5 ms                                                                | 62.7 ms: 1.04x slower                                                           |
| typing_runtime_protocols | 115 us                                                                 | 119 us: 1.04x slower                                                            |
| async_tree_io            | 1.21 sec                                                               | 1.25 sec: 1.04x slower                                                          |
| xml_etree_generate       | 89.8 ms                                                                | 93.3 ms: 1.04x slower                                                           |
| gc_traversal             | 3.87 ms                                                                | 4.02 ms: 1.04x slower                                                           |
| scimark_lu               | 162 ms                                                                 | 169 ms: 1.04x slower                                                            |
| xml_etree_iterparse      | 111 ms                                                                 | 116 ms: 1.05x slower                                                            |
| deltablue                | 3.83 ms                                                                | 4.02 ms: 1.05x slower                                                           |
| deepcopy_memo            | 41.4 us                                                                | 43.8 us: 1.06x slower                                                           |
| mdp                      | 2.71 sec                                                               | 2.88 sec: 1.06x slower                                                          |
| pprint_pformat           | 1.83 sec                                                               | 1.96 sec: 1.07x slower                                                          |
| go                       | 177 ms                                                                 | 190 ms: 1.07x slower                                                            |
| fannkuch                 | 502 ms                                                                 | 540 ms: 1.08x slower                                                            |
| pprint_safe_repr         | 877 ms                                                                 | 945 ms: 1.08x slower                                                            |
| crypto_pyaes             | 85.5 ms                                                                | 92.2 ms: 1.08x slower                                                           |
| unpickle_list            | 4.74 us                                                                | 5.12 us: 1.08x slower                                                           |
| raytrace                 | 340 ms                                                                 | 367 ms: 1.08x slower                                                            |
| chaos                    | 74.4 ms                                                                | 80.3 ms: 1.08x slower                                                           |
| comprehensions           | 21.7 us                                                                | 23.5 us: 1.08x slower                                                           |
| regex_compile            | 176 ms                                                                 | 191 ms: 1.09x slower                                                            |
| tomli_loads              | 2.56 sec                                                               | 2.79 sec: 1.09x slower                                                          |
| richards                 | 56.2 ms                                                                | 61.2 ms: 1.09x slower                                                           |
| nbody                    | 121 ms                                                                 | 132 ms: 1.09x slower                                                            |
| richards_super           | 61.9 ms                                                                | 67.7 ms: 1.09x slower                                                           |
| unpickle_pure_python     | 282 us                                                                 | 309 us: 1.09x slower                                                            |
| scimark_fft              | 430 ms                                                                 | 473 ms: 1.10x slower                                                            |
| scimark_sparse_mat_mult  | 5.94 ms                                                                | 6.53 ms: 1.10x slower                                                           |
| nqueens                  | 102 ms                                                                 | 112 ms: 1.10x slower                                                            |
| unpack_sequence          | 55.4 ns                                                                | 61.2 ns: 1.11x slower                                                           |
| hexiom                   | 9.55 ms                                                                | 10.6 ms: 1.11x slower                                                           |
| float                    | 95.3 ms                                                                | 106 ms: 1.11x slower                                                            |
| scimark_monte_carlo      | 92.0 ms                                                                | 102 ms: 1.11x slower                                                            |
| mako                     | 13.4 ms                                                                | 15.1 ms: 1.12x slower                                                           |
| pyflate                  | 589 ms                                                                 | 660 ms: 1.12x slower                                                            |
| spectral_norm            | 140 ms                                                                 | 162 ms: 1.16x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.04x slower                                                                    |

Benchmark hidden because not significant (10): unpickle, async_tree_memoization_tg, asyncio_websockets, bench_mp_pool, json, generators, deepcopy_reduce, async_tree_cpu_io_mixed_tg, dask, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.01x