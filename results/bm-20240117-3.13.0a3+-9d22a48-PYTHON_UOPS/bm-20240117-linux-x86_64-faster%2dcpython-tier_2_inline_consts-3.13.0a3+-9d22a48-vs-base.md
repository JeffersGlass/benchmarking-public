# Results vs. base

- fork: faster-cpython
- ref: tier_2_inline_consts
- machine: linux-x86_64
- commit hash: 9d22a48
- commit date: 2024-01-17
- overall geometric mean: 1.00x faster
- HPT reliability: 90.27%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 281 ms                                                                 | 281 ms: 1.00x faster                                                             |
| chameleon      | 7.38 ms                                                                | 7.35 ms: 1.00x faster                                                            |
| docutils       | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| tornado_http   | 98.2 ms                                                                | 99.7 ms: 1.02x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark        | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_io_tg | 1.20 sec                                                               | 1.21 sec: 1.00x slower                                                           |
| async_tree_io    | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                                           |
| Geometric mean   | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (6): async_tree_none_tg, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_cpu_io_mixed, async_tree_memoization, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 116 ms                                                                 | 114 ms: 1.02x faster                                                             |
| float          | 91.2 ms                                                                | 89.9 ms: 1.01x faster                                                            |
| pidigits       | 189 ms                                                                 | 189 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 150 ms                                                                 | 149 ms: 1.01x faster                                                             |
| regex_dna      | 218 ms                                                                 | 226 ms: 1.04x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (2): regex_v8, regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list        | 5.27 us                                                                | 5.13 us: 1.03x faster                                                            |
| tomli_loads          | 2.39 sec                                                               | 2.34 sec: 1.02x faster                                                           |
| json_loads           | 28.5 us                                                                | 28.1 us: 1.01x faster                                                            |
| pickle               | 11.7 us                                                                | 11.5 us: 1.01x faster                                                            |
| xml_etree_process    | 60.8 ms                                                                | 60.5 ms: 1.00x faster                                                            |
| pickle_pure_python   | 302 us                                                                 | 301 us: 1.00x faster                                                             |
| unpickle_pure_python | 235 us                                                                 | 234 us: 1.00x faster                                                             |
| xml_etree_iterparse  | 109 ms                                                                 | 110 ms: 1.01x slower                                                             |
| json_dumps           | 10.5 ms                                                                | 10.6 ms: 1.01x slower                                                            |
| pickle_dict          | 33.2 us                                                                | 34.1 us: 1.03x slower                                                            |
| pickle_list          | 4.91 us                                                                | 5.14 us: 1.05x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (3): xml_etree_parse, xml_etree_generate, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup_no_site | 8.74 ms                                                                | 8.75 ms: 1.00x slower                                                            |
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 13.6 ms                                                                | 13.3 ms: 1.02x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20240122-linux-x86_64-python-d1b031cc58516e1aba82-3.13.0a3+-d1b031c | bm-20240117-linux-x86_64-faster%2dcpython-tier_2_inline_consts-3.13.0a3+-9d22a48 |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pycparser                | 1.24 sec                                                               | 1.19 sec: 1.05x faster                                                           |
| nqueens                  | 94.6 ms                                                                | 91.0 ms: 1.04x faster                                                            |
| sympy_str                | 303 ms                                                                 | 291 ms: 1.04x faster                                                             |
| pyflate                  | 528 ms                                                                 | 509 ms: 1.04x faster                                                             |
| sympy_expand             | 502 ms                                                                 | 487 ms: 1.03x faster                                                             |
| unpickle_list            | 5.27 us                                                                | 5.13 us: 1.03x faster                                                            |
| generators               | 29.7 ms                                                                | 29.1 ms: 1.02x faster                                                            |
| logging_simple           | 6.23 us                                                                | 6.09 us: 1.02x faster                                                            |
| sqlite_synth             | 2.93 us                                                                | 2.86 us: 1.02x faster                                                            |
| richards                 | 48.9 ms                                                                | 47.9 ms: 1.02x faster                                                            |
| richards_super           | 55.3 ms                                                                | 54.2 ms: 1.02x faster                                                            |
| scimark_monte_carlo      | 80.5 ms                                                                | 78.9 ms: 1.02x faster                                                            |
| tomli_loads              | 2.39 sec                                                               | 2.34 sec: 1.02x faster                                                           |
| mako                     | 13.6 ms                                                                | 13.3 ms: 1.02x faster                                                            |
| nbody                    | 116 ms                                                                 | 114 ms: 1.02x faster                                                             |
| sqlglot_normalize        | 116 ms                                                                 | 114 ms: 1.02x faster                                                             |
| scimark_sor              | 134 ms                                                                 | 132 ms: 1.02x faster                                                             |
| scimark_lu               | 118 ms                                                                 | 117 ms: 1.01x faster                                                             |
| hexiom                   | 8.15 ms                                                                | 8.04 ms: 1.01x faster                                                            |
| json_loads               | 28.5 us                                                                | 28.1 us: 1.01x faster                                                            |
| float                    | 91.2 ms                                                                | 89.9 ms: 1.01x faster                                                            |
| sqlglot_optimize         | 58.4 ms                                                                | 57.6 ms: 1.01x faster                                                            |
| pickle                   | 11.7 us                                                                | 11.5 us: 1.01x faster                                                            |
| comprehensions           | 20.6 us                                                                | 20.4 us: 1.01x faster                                                            |
| typing_runtime_protocols | 117 us                                                                 | 116 us: 1.01x faster                                                             |
| logging_silent           | 107 ns                                                                 | 106 ns: 1.01x faster                                                             |
| regex_compile            | 150 ms                                                                 | 149 ms: 1.01x faster                                                             |
| raytrace                 | 298 ms                                                                 | 296 ms: 1.01x faster                                                             |
| spectral_norm            | 140 ms                                                                 | 139 ms: 1.01x faster                                                             |
| sqlglot_parse            | 1.33 ms                                                                | 1.32 ms: 1.01x faster                                                            |
| deepcopy_memo            | 41.5 us                                                                | 41.2 us: 1.01x faster                                                            |
| meteor_contest           | 114 ms                                                                 | 113 ms: 1.01x faster                                                             |
| xml_etree_process        | 60.8 ms                                                                | 60.5 ms: 1.00x faster                                                            |
| chameleon                | 7.38 ms                                                                | 7.35 ms: 1.00x faster                                                            |
| pickle_pure_python       | 302 us                                                                 | 301 us: 1.00x faster                                                             |
| gc_traversal             | 3.72 ms                                                                | 3.70 ms: 1.00x faster                                                            |
| docutils                 | 2.71 sec                                                               | 2.70 sec: 1.00x faster                                                           |
| unpickle_pure_python     | 235 us                                                                 | 234 us: 1.00x faster                                                             |
| 2to3                     | 281 ms                                                                 | 281 ms: 1.00x faster                                                             |
| asyncio_tcp_ssl          | 1.80 sec                                                               | 1.80 sec: 1.00x slower                                                           |
| pidigits                 | 189 ms                                                                 | 189 ms: 1.00x slower                                                             |
| python_startup_no_site   | 8.74 ms                                                                | 8.75 ms: 1.00x slower                                                            |
| python_startup           | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                            |
| crypto_pyaes             | 81.2 ms                                                                | 81.5 ms: 1.00x slower                                                            |
| async_generators         | 452 ms                                                                 | 454 ms: 1.00x slower                                                             |
| async_tree_io_tg         | 1.20 sec                                                               | 1.21 sec: 1.00x slower                                                           |
| sympy_integrate          | 21.1 ms                                                                | 21.2 ms: 1.00x slower                                                            |
| dulwich_log              | 69.2 ms                                                                | 69.5 ms: 1.01x slower                                                            |
| coroutines               | 22.1 ms                                                                | 22.2 ms: 1.01x slower                                                            |
| async_tree_io            | 1.19 sec                                                               | 1.20 sec: 1.01x slower                                                           |
| xml_etree_iterparse      | 109 ms                                                                 | 110 ms: 1.01x slower                                                             |
| pprint_pformat           | 1.69 sec                                                               | 1.71 sec: 1.01x slower                                                           |
| create_gc_cycles         | 1.48 ms                                                                | 1.50 ms: 1.01x slower                                                            |
| pprint_safe_repr         | 816 ms                                                                 | 824 ms: 1.01x slower                                                             |
| json_dumps               | 10.5 ms                                                                | 10.6 ms: 1.01x slower                                                            |
| tornado_http             | 98.2 ms                                                                | 99.7 ms: 1.02x slower                                                            |
| sympy_sum                | 160 ms                                                                 | 163 ms: 1.02x slower                                                             |
| mdp                      | 2.63 sec                                                               | 2.68 sec: 1.02x slower                                                           |
| deepcopy_reduce          | 3.14 us                                                                | 3.20 us: 1.02x slower                                                            |
| deepcopy                 | 357 us                                                                 | 364 us: 1.02x slower                                                             |
| asyncio_tcp              | 486 ms                                                                 | 497 ms: 1.02x slower                                                             |
| pickle_dict              | 33.2 us                                                                | 34.1 us: 1.03x slower                                                            |
| regex_dna                | 218 ms                                                                 | 226 ms: 1.04x slower                                                             |
| unpack_sequence          | 38.0 ns                                                                | 39.7 ns: 1.05x slower                                                            |
| pickle_list              | 4.91 us                                                                | 5.14 us: 1.05x slower                                                            |
| Geometric mean           | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (28): regex_v8, logging_format, xml_etree_parse, sqlglot_transpile, coverage, mypy2, deltablue, xml_etree_generate, scimark_fft, regex_effbot, json, go, chaos, bench_mp_pool, telco, async_tree_none_tg, dask, fannkuch, async_tree_cpu_io_mixed_tg, asyncio_websockets, async_tree_none, pathlib, bench_thread_pool, scimark_sparse_mat_mult, async_tree_cpu_io_mixed, unpickle, async_tree_memoization, async_tree_memoization_tg


# HPT report

- Reliability score: 90.27% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.03x