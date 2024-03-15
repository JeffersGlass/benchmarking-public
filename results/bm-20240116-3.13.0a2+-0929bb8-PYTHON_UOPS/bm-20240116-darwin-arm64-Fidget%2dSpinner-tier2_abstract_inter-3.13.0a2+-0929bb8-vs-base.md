# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: darwin-arm64
- commit hash: 0929bb8
- commit date: 2024-01-16
- overall geometric mean: 1.01x slower
- HPT reliability: 98.63%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.27x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2+-77b45fa | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 173 ms                                                                 | 176 ms: 1.01x slower                                                             |
| chameleon      | 5.05 ms                                                                | 5.16 ms: 1.02x slower                                                            |
| docutils       | 1.51 sec                                                               | 1.51 sec: 1.00x slower                                                           |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2+-77b45fa | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none_tg | 268 ms                                                                 | 266 ms: 1.01x faster                                                             |
| async_tree_io_tg   | 683 ms                                                                 | 687 ms: 1.01x slower                                                             |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (6): async_tree_none, async_tree_io, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2+-77b45fa | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 68.8 ms                                                                | 68.1 ms: 1.01x faster                                                            |
| nbody          | 87.1 ms                                                                | 118 ms: 1.35x slower                                                             |
| Geometric mean | (ref)                                                                  | 1.10x slower                                                                     |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2+-77b45fa | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_v8       | 18.2 ms                                                                | 17.9 ms: 1.02x faster                                                            |
| regex_effbot   | 2.79 ms                                                                | 2.75 ms: 1.02x faster                                                            |
| regex_dna      | 157 ms                                                                 | 156 ms: 1.01x faster                                                             |
| regex_compile  | 82.2 ms                                                                | 82.0 ms: 1.00x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2+-77b45fa | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| unpickle_list        | 3.06 us                                                                | 3.00 us: 1.02x faster                                                            |
| tomli_loads          | 1.65 sec                                                               | 1.64 sec: 1.01x faster                                                           |
| json_dumps           | 6.59 ms                                                                | 6.58 ms: 1.00x faster                                                            |
| xml_etree_iterparse  | 80.1 ms                                                                | 80.4 ms: 1.00x slower                                                            |
| unpickle_pure_python | 163 us                                                                 | 164 us: 1.01x slower                                                             |
| pickle_pure_python   | 196 us                                                                 | 197 us: 1.01x slower                                                             |
| pickle               | 7.41 us                                                                | 7.48 us: 1.01x slower                                                            |
| pickle_dict          | 18.0 us                                                                | 18.2 us: 1.01x slower                                                            |
| xml_etree_generate   | 58.6 ms                                                                | 59.4 ms: 1.01x slower                                                            |
| unpickle             | 9.05 us                                                                | 9.17 us: 1.01x slower                                                            |
| Geometric mean       | (ref)                                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (4): json_loads, xml_etree_process, pickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2+-77b45fa | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup | 12.5 ms                                                                | 12.3 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                                     |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2+-77b45fa | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 9.69 ms                                                                | 9.66 ms: 1.00x faster                                                            |

All benchmarks:
===============

| Benchmark               | bm-20240113-darwin-arm64-python-77b45fa6d0b8c0c14657-3.13.0a2+-77b45fa | bm-20240116-darwin-arm64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a2+-0929bb8 |
|-------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| asyncio_tcp             | 432 ms                                                                 | 374 ms: 1.15x faster                                                             |
| spectral_norm           | 105 ms                                                                 | 101 ms: 1.04x faster                                                             |
| json                    | 3.02 ms                                                                | 2.94 ms: 1.03x faster                                                            |
| scimark_sparse_mat_mult | 4.14 ms                                                                | 4.06 ms: 1.02x faster                                                            |
| unpickle_list           | 3.06 us                                                                | 3.00 us: 1.02x faster                                                            |
| regex_v8                | 18.2 ms                                                                | 17.9 ms: 1.02x faster                                                            |
| fannkuch                | 322 ms                                                                 | 316 ms: 1.02x faster                                                             |
| regex_effbot            | 2.79 ms                                                                | 2.75 ms: 1.02x faster                                                            |
| python_startup          | 12.5 ms                                                                | 12.3 ms: 1.01x faster                                                            |
| regex_dna               | 157 ms                                                                 | 156 ms: 1.01x faster                                                             |
| float                   | 68.8 ms                                                                | 68.1 ms: 1.01x faster                                                            |
| async_tree_none_tg      | 268 ms                                                                 | 266 ms: 1.01x faster                                                             |
| logging_format          | 3.88 us                                                                | 3.85 us: 1.01x faster                                                            |
| sympy_expand            | 248 ms                                                                 | 246 ms: 1.01x faster                                                             |
| nqueens                 | 68.2 ms                                                                | 67.7 ms: 1.01x faster                                                            |
| deepcopy                | 228 us                                                                 | 226 us: 1.01x faster                                                             |
| deepcopy_reduce         | 2.00 us                                                                | 1.99 us: 1.01x faster                                                            |
| tomli_loads             | 1.65 sec                                                               | 1.64 sec: 1.01x faster                                                           |
| telco                   | 4.70 ms                                                                | 4.68 ms: 1.00x faster                                                            |
| meteor_contest          | 77.0 ms                                                                | 76.7 ms: 1.00x faster                                                            |
| deepcopy_memo           | 26.9 us                                                                | 26.7 us: 1.00x faster                                                            |
| regex_compile           | 82.2 ms                                                                | 82.0 ms: 1.00x faster                                                            |
| mako                    | 9.69 ms                                                                | 9.66 ms: 1.00x faster                                                            |
| richards                | 32.7 ms                                                                | 32.6 ms: 1.00x faster                                                            |
| sqlite_synth            | 1.64 us                                                                | 1.64 us: 1.00x faster                                                            |
| json_dumps              | 6.59 ms                                                                | 6.58 ms: 1.00x faster                                                            |
| pyflate                 | 367 ms                                                                 | 366 ms: 1.00x faster                                                             |
| docutils                | 1.51 sec                                                               | 1.51 sec: 1.00x slower                                                           |
| async_generators        | 298 ms                                                                 | 299 ms: 1.00x slower                                                             |
| logging_simple          | 3.56 us                                                                | 3.57 us: 1.00x slower                                                            |
| generators              | 28.8 ms                                                                | 28.9 ms: 1.00x slower                                                            |
| raytrace                | 185 ms                                                                 | 186 ms: 1.00x slower                                                             |
| sqlglot_normalize       | 190 ms                                                                 | 190 ms: 1.00x slower                                                             |
| xml_etree_iterparse     | 80.1 ms                                                                | 80.4 ms: 1.00x slower                                                            |
| create_gc_cycles        | 701 us                                                                 | 704 us: 1.00x slower                                                             |
| dulwich_log             | 29.9 ms                                                                | 30.1 ms: 1.00x slower                                                            |
| async_tree_io_tg        | 683 ms                                                                 | 687 ms: 1.01x slower                                                             |
| logging_silent          | 71.7 ns                                                                | 72.1 ns: 1.01x slower                                                            |
| bench_thread_pool       | 514 us                                                                 | 517 us: 1.01x slower                                                             |
| sqlglot_parse           | 808 us                                                                 | 813 us: 1.01x slower                                                             |
| mdp                     | 1.61 sec                                                               | 1.62 sec: 1.01x slower                                                           |
| unpickle_pure_python    | 163 us                                                                 | 164 us: 1.01x slower                                                             |
| sqlglot_transpile       | 987 us                                                                 | 994 us: 1.01x slower                                                             |
| pickle_pure_python      | 196 us                                                                 | 197 us: 1.01x slower                                                             |
| sympy_sum               | 79.9 ms                                                                | 80.6 ms: 1.01x slower                                                            |
| hexiom                  | 5.92 ms                                                                | 5.97 ms: 1.01x slower                                                            |
| sqlglot_optimize        | 35.7 ms                                                                | 36.0 ms: 1.01x slower                                                            |
| pickle                  | 7.41 us                                                                | 7.48 us: 1.01x slower                                                            |
| pickle_dict             | 18.0 us                                                                | 18.2 us: 1.01x slower                                                            |
| scimark_sor             | 106 ms                                                                 | 107 ms: 1.01x slower                                                             |
| sympy_str               | 148 ms                                                                 | 149 ms: 1.01x slower                                                             |
| xml_etree_generate      | 58.6 ms                                                                | 59.4 ms: 1.01x slower                                                            |
| unpickle                | 9.05 us                                                                | 9.17 us: 1.01x slower                                                            |
| 2to3                    | 173 ms                                                                 | 176 ms: 1.01x slower                                                             |
| bench_mp_pool           | 44.7 ms                                                                | 45.4 ms: 1.02x slower                                                            |
| pathlib                 | 25.1 ms                                                                | 25.6 ms: 1.02x slower                                                            |
| richards_super          | 36.2 ms                                                                | 36.9 ms: 1.02x slower                                                            |
| comprehensions          | 15.4 us                                                                | 15.7 us: 1.02x slower                                                            |
| scimark_fft             | 250 ms                                                                 | 255 ms: 1.02x slower                                                             |
| sympy_integrate         | 11.5 ms                                                                | 11.8 ms: 1.02x slower                                                            |
| chameleon               | 5.05 ms                                                                | 5.16 ms: 1.02x slower                                                            |
| pprint_pformat          | 1.17 sec                                                               | 1.21 sec: 1.03x slower                                                           |
| pprint_safe_repr        | 570 ms                                                                 | 590 ms: 1.04x slower                                                             |
| chaos                   | 46.4 ms                                                                | 48.4 ms: 1.04x slower                                                            |
| coroutines              | 18.9 ms                                                                | 19.8 ms: 1.04x slower                                                            |
| unpack_sequence         | 28.0 ns                                                                | 29.9 ns: 1.07x slower                                                            |
| nbody                   | 87.1 ms                                                                | 118 ms: 1.35x slower                                                             |
| Geometric mean          | (ref)                                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (26): python_startup_no_site, dask, coverage, go, asyncio_websockets, async_tree_none, json_loads, async_tree_io, async_tree_cpu_io_mixed, scimark_monte_carlo, async_tree_cpu_io_mixed_tg, async_tree_memoization, crypto_pyaes, xml_etree_process, pidigits, gc_traversal, deltablue, async_tree_memoization_tg, pickle_list, mypy2, scimark_lu, pycparser, xml_etree_parse, asyncio_tcp_ssl, typing_runtime_protocols, tornado_http


# HPT report

- Reliability score: 98.63% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.27x