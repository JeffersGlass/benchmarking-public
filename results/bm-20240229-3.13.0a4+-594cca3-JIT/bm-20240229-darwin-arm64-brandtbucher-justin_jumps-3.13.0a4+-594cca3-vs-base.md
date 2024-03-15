# Results vs. base

- fork: brandtbucher
- ref: justin_jumps
- machine: darwin-arm64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.00x slower
- HPT reliability: 86.73%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| chameleon      | 4.84 ms                                                                | 4.85 ms: 1.00x slower                                                |
| docutils       | 1.51 sec                                                               | 1.53 sec: 1.01x slower                                               |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (2): 2to3, tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_none, async_tree_memoization, async_tree_io_tg, async_tree_io, async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_none_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 282 ms                                                                 | 282 ms: 1.00x slower                                                 |
| nbody          | 70.0 ms                                                                | 70.6 ms: 1.01x slower                                                |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 87.1 ms                                                                | 86.7 ms: 1.01x faster                                                |
| regex_v8       | 17.1 ms                                                                | 17.2 ms: 1.01x slower                                                |
| regex_effbot   | 2.58 ms                                                                | 2.63 ms: 1.02x slower                                                |
| regex_dna      | 145 ms                                                                 | 152 ms: 1.05x slower                                                 |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark         | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| xml_etree_process | 40.0 ms                                                                | 39.0 ms: 1.02x faster                                                |
| unpickle          | 9.19 us                                                                | 9.15 us: 1.00x faster                                                |
| json_dumps        | 6.56 ms                                                                | 6.54 ms: 1.00x faster                                                |
| pickle_dict       | 18.1 us                                                                | 18.3 us: 1.01x slower                                                |
| pickle_list       | 2.91 us                                                                | 2.96 us: 1.02x slower                                                |
| Geometric mean    | (ref)                                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (9): xml_etree_iterparse, tomli_loads, pickle, unpickle_pure_python, json_loads, pickle_pure_python, unpickle_list, xml_etree_parse, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 16.4 ms                                                                | 15.9 ms: 1.03x faster                                                |
| python_startup         | 17.7 ms                                                                | 17.3 ms: 1.02x faster                                                |
| Geometric mean         | (ref)                                                                  | 1.03x faster                                                         |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark              | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 16.4 ms                                                                | 15.9 ms: 1.03x faster                                                |
| fannkuch               | 325 ms                                                                 | 316 ms: 1.03x faster                                                 |
| xml_etree_process      | 40.0 ms                                                                | 39.0 ms: 1.02x faster                                                |
| python_startup         | 17.7 ms                                                                | 17.3 ms: 1.02x faster                                                |
| richards               | 40.4 ms                                                                | 39.8 ms: 1.02x faster                                                |
| deepcopy               | 231 us                                                                 | 228 us: 1.01x faster                                                 |
| sqlite_synth           | 1.61 us                                                                | 1.59 us: 1.01x faster                                                |
| bench_thread_pool      | 514 us                                                                 | 510 us: 1.01x faster                                                 |
| async_generators       | 311 ms                                                                 | 309 ms: 1.01x faster                                                 |
| coroutines             | 18.7 ms                                                                | 18.6 ms: 1.01x faster                                                |
| regex_compile          | 87.1 ms                                                                | 86.7 ms: 1.01x faster                                                |
| unpickle               | 9.19 us                                                                | 9.15 us: 1.00x faster                                                |
| deltablue              | 2.55 ms                                                                | 2.54 ms: 1.00x faster                                                |
| pprint_pformat         | 1.06 sec                                                               | 1.06 sec: 1.00x faster                                               |
| json_dumps             | 6.56 ms                                                                | 6.54 ms: 1.00x faster                                                |
| scimark_monte_carlo    | 46.1 ms                                                                | 46.0 ms: 1.00x faster                                                |
| sympy_expand           | 248 ms                                                                 | 247 ms: 1.00x faster                                                 |
| generators             | 28.5 ms                                                                | 28.4 ms: 1.00x faster                                                |
| pidigits               | 282 ms                                                                 | 282 ms: 1.00x slower                                                 |
| logging_silent         | 72.5 ns                                                                | 72.6 ns: 1.00x slower                                                |
| asyncio_websockets     | 408 ms                                                                 | 409 ms: 1.00x slower                                                 |
| go                     | 116 ms                                                                 | 116 ms: 1.00x slower                                                 |
| deepcopy_reduce        | 2.00 us                                                                | 2.00 us: 1.00x slower                                                |
| mdp                    | 1.63 sec                                                               | 1.64 sec: 1.00x slower                                               |
| chameleon              | 4.84 ms                                                                | 4.85 ms: 1.00x slower                                                |
| sympy_integrate        | 11.5 ms                                                                | 11.5 ms: 1.00x slower                                                |
| chaos                  | 40.3 ms                                                                | 40.4 ms: 1.00x slower                                                |
| logging_format         | 3.77 us                                                                | 3.79 us: 1.00x slower                                                |
| meteor_contest         | 74.1 ms                                                                | 74.5 ms: 1.01x slower                                                |
| regex_v8               | 17.1 ms                                                                | 17.2 ms: 1.01x slower                                                |
| comprehensions         | 12.9 us                                                                | 13.0 us: 1.01x slower                                                |
| scimark_fft            | 199 ms                                                                 | 201 ms: 1.01x slower                                                 |
| docutils               | 1.51 sec                                                               | 1.53 sec: 1.01x slower                                               |
| dulwich_log            | 30.9 ms                                                                | 31.1 ms: 1.01x slower                                                |
| nbody                  | 70.0 ms                                                                | 70.6 ms: 1.01x slower                                                |
| richards_super         | 43.4 ms                                                                | 43.8 ms: 1.01x slower                                                |
| pickle_dict            | 18.1 us                                                                | 18.3 us: 1.01x slower                                                |
| scimark_sor            | 115 ms                                                                 | 116 ms: 1.01x slower                                                 |
| pickle_list            | 2.91 us                                                                | 2.96 us: 1.02x slower                                                |
| coverage               | 47.7 ms                                                                | 48.5 ms: 1.02x slower                                                |
| regex_effbot           | 2.58 ms                                                                | 2.63 ms: 1.02x slower                                                |
| nqueens                | 63.7 ms                                                                | 65.0 ms: 1.02x slower                                                |
| regex_dna              | 145 ms                                                                 | 152 ms: 1.05x slower                                                 |
| Geometric mean         | (ref)                                                                  | 1.00x slower                                                         |

Benchmark hidden because not significant (49): spectral_norm, pathlib, bench_mp_pool, async_tree_none, json, pycparser, xml_etree_iterparse, tomli_loads, pickle, async_tree_memoization, hexiom, create_gc_cycles, async_tree_io_tg, asyncio_tcp_ssl, unpack_sequence, telco, deepcopy_memo, pprint_safe_repr, gc_traversal, sqlglot_normalize, async_tree_io, unpickle_pure_python, json_loads, pyflate, scimark_lu, scimark_sparse_mat_mult, pickle_pure_python, async_tree_memoization_tg, unpickle_list, sqlglot_transpile, async_tree_cpu_io_mixed, 2to3, async_tree_none_tg, crypto_pyaes, logging_simple, float, mako, sqlglot_parse, sympy_str, sympy_sum, sqlglot_optimize, async_tree_cpu_io_mixed_tg, xml_etree_parse, typing_runtime_protocols, tornado_http, raytrace, xml_etree_generate, asyncio_tcp, mypy2


# HPT report

- Reliability score: 86.73% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x