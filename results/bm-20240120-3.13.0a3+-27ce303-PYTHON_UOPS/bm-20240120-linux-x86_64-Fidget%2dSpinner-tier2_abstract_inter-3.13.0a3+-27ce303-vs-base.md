# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 27ce303
- commit date: 2024-01-20
- overall geometric mean: 1.00x faster
- HPT reliability: 69.82%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.27x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240118-linux-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 282 ms                                                                 | 287 ms: 1.02x slower                                                             |
| chameleon      | 7.13 ms                                                                | 7.39 ms: 1.04x slower                                                            |
| docutils       | 2.70 sec                                                               | 2.72 sec: 1.01x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20240118-linux-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_io          | 1.20 sec                                                               | 1.20 sec: 1.00x slower                                                           |
| async_tree_memoization | 571 ms                                                                 | 578 ms: 1.01x slower                                                             |
| async_tree_io_tg       | 1.20 sec                                                               | 1.22 sec: 1.01x slower                                                           |
| async_tree_none_tg     | 447 ms                                                                 | 460 ms: 1.03x slower                                                             |
| Geometric mean         | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (4): async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_none, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240118-linux-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 93.5 ms                                                                | 89.4 ms: 1.05x faster                                                            |
| pidigits       | 189 ms                                                                 | 188 ms: 1.00x faster                                                             |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240118-linux-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 153 ms                                                                 | 150 ms: 1.02x faster                                                             |
| regex_effbot   | 3.69 ms                                                                | 3.65 ms: 1.01x faster                                                            |
| regex_dna      | 226 ms                                                                 | 227 ms: 1.01x slower                                                             |
| regex_v8       | 25.4 ms                                                                | 25.9 ms: 1.02x slower                                                            |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240118-linux-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| tomli_loads          | 2.46 sec                                                               | 2.32 sec: 1.06x faster                                                           |
| xml_etree_iterparse  | 111 ms                                                                 | 109 ms: 1.01x faster                                                             |
| xml_etree_process    | 61.0 ms                                                                | 61.2 ms: 1.00x slower                                                            |
| pickle_pure_python   | 303 us                                                                 | 305 us: 1.01x slower                                                             |
| json_dumps           | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                                            |
| unpickle_pure_python | 236 us                                                                 | 238 us: 1.01x slower                                                             |
| pickle               | 11.3 us                                                                | 11.9 us: 1.05x slower                                                            |
| pickle_dict          | 32.9 us                                                                | 34.8 us: 1.06x slower                                                            |
| pickle_list          | 4.91 us                                                                | 5.25 us: 1.07x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (5): unpickle, xml_etree_parse, unpickle_list, json_loads, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240118-linux-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                            |
| python_startup_no_site | 8.73 ms                                                                | 8.77 ms: 1.00x slower                                                            |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240118-linux-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 14.1 ms                                                                | 13.7 ms: 1.03x faster                                                            |

All benchmarks:
===============

| Benchmark               | bm-20240118-linux-x86_64-python-68a7b78cd5185cbd9456-3.13.0a3+-68a7b78 | bm-20240120-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-27ce303 |
|-------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| spectral_norm           | 149 ms                                                                 | 138 ms: 1.08x faster                                                             |
| scimark_fft             | 454 ms                                                                 | 422 ms: 1.07x faster                                                             |
| hexiom                  | 8.66 ms                                                                | 8.15 ms: 1.06x faster                                                            |
| tomli_loads             | 2.46 sec                                                               | 2.32 sec: 1.06x faster                                                           |
| scimark_sparse_mat_mult | 6.04 ms                                                                | 5.72 ms: 1.06x faster                                                            |
| deltablue               | 4.84 ms                                                                | 4.59 ms: 1.05x faster                                                            |
| float                   | 93.5 ms                                                                | 89.4 ms: 1.05x faster                                                            |
| comprehensions          | 21.9 us                                                                | 21.1 us: 1.04x faster                                                            |
| mako                    | 14.1 ms                                                                | 13.7 ms: 1.03x faster                                                            |
| sympy_expand            | 508 ms                                                                 | 492 ms: 1.03x faster                                                             |
| sympy_str               | 301 ms                                                                 | 292 ms: 1.03x faster                                                             |
| coroutines              | 22.8 ms                                                                | 22.2 ms: 1.03x faster                                                            |
| chaos                   | 73.4 ms                                                                | 71.3 ms: 1.03x faster                                                            |
| pyflate                 | 535 ms                                                                 | 522 ms: 1.03x faster                                                             |
| pathlib                 | 18.7 ms                                                                | 18.3 ms: 1.02x faster                                                            |
| pprint_safe_repr        | 828 ms                                                                 | 810 ms: 1.02x faster                                                             |
| raytrace                | 303 ms                                                                 | 296 ms: 1.02x faster                                                             |
| regex_compile           | 153 ms                                                                 | 150 ms: 1.02x faster                                                             |
| pprint_pformat          | 1.71 sec                                                               | 1.69 sec: 1.02x faster                                                           |
| crypto_pyaes            | 85.3 ms                                                                | 84.0 ms: 1.02x faster                                                            |
| logging_simple          | 6.05 us                                                                | 5.96 us: 1.02x faster                                                            |
| sqlite_synth            | 2.90 us                                                                | 2.86 us: 1.01x faster                                                            |
| sympy_integrate         | 21.2 ms                                                                | 20.9 ms: 1.01x faster                                                            |
| xml_etree_iterparse     | 111 ms                                                                 | 109 ms: 1.01x faster                                                             |
| scimark_monte_carlo     | 80.5 ms                                                                | 79.5 ms: 1.01x faster                                                            |
| fannkuch                | 447 ms                                                                 | 442 ms: 1.01x faster                                                             |
| regex_effbot            | 3.69 ms                                                                | 3.65 ms: 1.01x faster                                                            |
| sympy_sum               | 161 ms                                                                 | 160 ms: 1.01x faster                                                             |
| nqueens                 | 94.5 ms                                                                | 93.8 ms: 1.01x faster                                                            |
| dulwich_log             | 68.9 ms                                                                | 68.6 ms: 1.00x faster                                                            |
| asyncio_websockets      | 553 ms                                                                 | 550 ms: 1.00x faster                                                             |
| sqlglot_parse           | 1.34 ms                                                                | 1.33 ms: 1.00x faster                                                            |
| generators              | 29.8 ms                                                                | 29.7 ms: 1.00x faster                                                            |
| pidigits                | 189 ms                                                                 | 188 ms: 1.00x faster                                                             |
| python_startup          | 10.1 ms                                                                | 10.1 ms: 1.00x slower                                                            |
| asyncio_tcp_ssl         | 1.80 sec                                                               | 1.80 sec: 1.00x slower                                                           |
| go                      | 157 ms                                                                 | 157 ms: 1.00x slower                                                             |
| xml_etree_process       | 61.0 ms                                                                | 61.2 ms: 1.00x slower                                                            |
| async_tree_io           | 1.20 sec                                                               | 1.20 sec: 1.00x slower                                                           |
| python_startup_no_site  | 8.73 ms                                                                | 8.77 ms: 1.00x slower                                                            |
| docutils                | 2.70 sec                                                               | 2.72 sec: 1.01x slower                                                           |
| create_gc_cycles        | 1.46 ms                                                                | 1.46 ms: 1.01x slower                                                            |
| bench_thread_pool       | 846 us                                                                 | 850 us: 1.01x slower                                                             |
| regex_dna               | 226 ms                                                                 | 227 ms: 1.01x slower                                                             |
| asyncio_tcp             | 496 ms                                                                 | 500 ms: 1.01x slower                                                             |
| pickle_pure_python      | 303 us                                                                 | 305 us: 1.01x slower                                                             |
| async_generators        | 455 ms                                                                 | 459 ms: 1.01x slower                                                             |
| json_dumps              | 10.4 ms                                                                | 10.5 ms: 1.01x slower                                                            |
| deepcopy                | 357 us                                                                 | 361 us: 1.01x slower                                                             |
| async_tree_memoization  | 571 ms                                                                 | 578 ms: 1.01x slower                                                             |
| json                    | 5.11 ms                                                                | 5.17 ms: 1.01x slower                                                            |
| async_tree_io_tg        | 1.20 sec                                                               | 1.22 sec: 1.01x slower                                                           |
| unpickle_pure_python    | 236 us                                                                 | 238 us: 1.01x slower                                                             |
| scimark_sor             | 133 ms                                                                 | 134 ms: 1.01x slower                                                             |
| coverage                | 93.8 ms                                                                | 95.2 ms: 1.01x slower                                                            |
| deepcopy_reduce         | 3.12 us                                                                | 3.17 us: 1.02x slower                                                            |
| logging_silent          | 103 ns                                                                 | 105 ns: 1.02x slower                                                             |
| regex_v8                | 25.4 ms                                                                | 25.9 ms: 1.02x slower                                                            |
| 2to3                    | 282 ms                                                                 | 287 ms: 1.02x slower                                                             |
| deepcopy_memo           | 40.5 us                                                                | 41.2 us: 1.02x slower                                                            |
| async_tree_none_tg      | 447 ms                                                                 | 460 ms: 1.03x slower                                                             |
| telco                   | 8.53 ms                                                                | 8.82 ms: 1.03x slower                                                            |
| chameleon               | 7.13 ms                                                                | 7.39 ms: 1.04x slower                                                            |
| pickle                  | 11.3 us                                                                | 11.9 us: 1.05x slower                                                            |
| pickle_dict             | 32.9 us                                                                | 34.8 us: 1.06x slower                                                            |
| pickle_list             | 4.91 us                                                                | 5.25 us: 1.07x slower                                                            |
| mdp                     | 2.64 sec                                                               | 2.83 sec: 1.07x slower                                                           |
| gc_traversal            | 3.59 ms                                                                | 3.98 ms: 1.11x slower                                                            |
| unpack_sequence         | 48.8 ns                                                                | 56.7 ns: 1.16x slower                                                            |
| Geometric mean          | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (24): unpickle, async_tree_memoization_tg, tornado_http, mypy2, sqlglot_normalize, xml_etree_parse, unpickle_list, json_loads, pycparser, meteor_contest, bench_mp_pool, scimark_lu, sqlglot_optimize, xml_etree_generate, richards_super, nbody, typing_runtime_protocols, richards, sqlglot_transpile, dask, logging_format, async_tree_cpu_io_mixed, async_tree_none, async_tree_cpu_io_mixed_tg


# HPT report

- Reliability score: 69.82% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.27x