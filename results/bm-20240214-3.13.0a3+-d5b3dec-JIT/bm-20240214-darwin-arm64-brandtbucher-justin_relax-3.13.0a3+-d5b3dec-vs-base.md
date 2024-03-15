# Results vs. base

- fork: brandtbucher
- ref: justin_relax
- machine: darwin-arm64
- commit hash: d5b3dec
- commit date: 2024-02-14
- overall geometric mean: 1.00x faster
- HPT reliability: 97.90%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| chameleon      | 4.82 ms                                                                | 4.79 ms: 1.01x faster                                                |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (3): 2to3, docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_io, async_tree_memoization, async_tree_memoization_tg, async_tree_io_tg, async_tree_cpu_io_mixed_tg, async_tree_none_tg, async_tree_cpu_io_mixed, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 283 ms                                                                 | 282 ms: 1.00x faster                                                 |
| nbody          | 76.6 ms                                                                | 76.5 ms: 1.00x faster                                                |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_dna      | 152 ms                                                                 | 151 ms: 1.00x faster                                                 |
| regex_effbot   | 2.56 ms                                                                | 2.55 ms: 1.00x faster                                                |
| regex_v8       | 17.0 ms                                                                | 17.1 ms: 1.00x slower                                                |
| regex_compile  | 75.5 ms                                                                | 75.6 ms: 1.00x slower                                                |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_list          | 2.98 us                                                                | 2.93 us: 1.02x faster                                                |
| pickle               | 7.32 us                                                                | 7.24 us: 1.01x faster                                                |
| pickle_dict          | 18.2 us                                                                | 18.1 us: 1.01x faster                                                |
| tomli_loads          | 1.41 sec                                                               | 1.40 sec: 1.01x faster                                               |
| unpickle_pure_python | 159 us                                                                 | 158 us: 1.01x faster                                                 |
| pickle_pure_python   | 196 us                                                                 | 195 us: 1.00x faster                                                 |
| json_loads           | 17.0 us                                                                | 17.0 us: 1.00x slower                                                |
| xml_etree_process    | 38.7 ms                                                                | 38.8 ms: 1.00x slower                                                |
| xml_etree_generate   | 55.2 ms                                                                | 55.7 ms: 1.01x slower                                                |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (5): xml_etree_parse, xml_etree_iterparse, json_dumps, unpickle, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup_no_site | 11.9 ms                                                                | 12.1 ms: 1.01x slower                                                |
| python_startup         | 13.3 ms                                                                | 13.6 ms: 1.03x slower                                                |
| Geometric mean         | (ref)                                                                  | 1.02x slower                                                         |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark              | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| telco                  | 4.59 ms                                                                | 4.49 ms: 1.02x faster                                                |
| fannkuch               | 275 ms                                                                 | 270 ms: 1.02x faster                                                 |
| pickle_list            | 2.98 us                                                                | 2.93 us: 1.02x faster                                                |
| sqlite_synth           | 1.62 us                                                                | 1.60 us: 1.01x faster                                                |
| pathlib                | 24.3 ms                                                                | 24.0 ms: 1.01x faster                                                |
| sympy_str              | 143 ms                                                                 | 142 ms: 1.01x faster                                                 |
| deepcopy_memo          | 26.1 us                                                                | 25.8 us: 1.01x faster                                                |
| pickle                 | 7.32 us                                                                | 7.24 us: 1.01x faster                                                |
| sympy_expand           | 243 ms                                                                 | 241 ms: 1.01x faster                                                 |
| pickle_dict            | 18.2 us                                                                | 18.1 us: 1.01x faster                                                |
| tomli_loads            | 1.41 sec                                                               | 1.40 sec: 1.01x faster                                               |
| unpickle_pure_python   | 159 us                                                                 | 158 us: 1.01x faster                                                 |
| chameleon              | 4.82 ms                                                                | 4.79 ms: 1.01x faster                                                |
| mdp                    | 1.63 sec                                                               | 1.62 sec: 1.00x faster                                               |
| chaos                  | 41.5 ms                                                                | 41.3 ms: 1.00x faster                                                |
| sqlglot_parse          | 795 us                                                                 | 792 us: 1.00x faster                                                 |
| crypto_pyaes           | 49.1 ms                                                                | 48.9 ms: 1.00x faster                                                |
| pidigits               | 283 ms                                                                 | 282 ms: 1.00x faster                                                 |
| pickle_pure_python     | 196 us                                                                 | 195 us: 1.00x faster                                                 |
| comprehensions         | 12.6 us                                                                | 12.6 us: 1.00x faster                                                |
| nbody                  | 76.6 ms                                                                | 76.5 ms: 1.00x faster                                                |
| asyncio_websockets     | 409 ms                                                                 | 408 ms: 1.00x faster                                                 |
| spectral_norm          | 80.6 ms                                                                | 80.5 ms: 1.00x faster                                                |
| richards               | 32.0 ms                                                                | 31.9 ms: 1.00x faster                                                |
| scimark_sor            | 106 ms                                                                 | 106 ms: 1.00x faster                                                 |
| regex_dna              | 152 ms                                                                 | 151 ms: 1.00x faster                                                 |
| regex_effbot           | 2.56 ms                                                                | 2.55 ms: 1.00x faster                                                |
| richards_super         | 35.8 ms                                                                | 35.7 ms: 1.00x faster                                                |
| raytrace               | 177 ms                                                                 | 177 ms: 1.00x faster                                                 |
| scimark_monte_carlo    | 48.8 ms                                                                | 48.9 ms: 1.00x slower                                                |
| sqlglot_normalize      | 183 ms                                                                 | 183 ms: 1.00x slower                                                 |
| dulwich_log            | 29.7 ms                                                                | 29.8 ms: 1.00x slower                                                |
| gc_traversal           | 2.39 ms                                                                | 2.39 ms: 1.00x slower                                                |
| regex_v8               | 17.0 ms                                                                | 17.1 ms: 1.00x slower                                                |
| regex_compile          | 75.5 ms                                                                | 75.6 ms: 1.00x slower                                                |
| logging_silent         | 70.5 ns                                                                | 70.6 ns: 1.00x slower                                                |
| go                     | 109 ms                                                                 | 110 ms: 1.00x slower                                                 |
| json_loads             | 17.0 us                                                                | 17.0 us: 1.00x slower                                                |
| scimark_lu             | 74.8 ms                                                                | 75.0 ms: 1.00x slower                                                |
| deepcopy               | 224 us                                                                 | 225 us: 1.00x slower                                                 |
| xml_etree_process      | 38.7 ms                                                                | 38.8 ms: 1.00x slower                                                |
| bench_thread_pool      | 503 us                                                                 | 505 us: 1.00x slower                                                 |
| generators             | 28.2 ms                                                                | 28.3 ms: 1.00x slower                                                |
| hexiom                 | 5.01 ms                                                                | 5.04 ms: 1.00x slower                                                |
| logging_simple         | 3.45 us                                                                | 3.47 us: 1.00x slower                                                |
| async_generators       | 302 ms                                                                 | 304 ms: 1.01x slower                                                 |
| pprint_pformat         | 1.05 sec                                                               | 1.05 sec: 1.01x slower                                               |
| xml_etree_generate     | 55.2 ms                                                                | 55.7 ms: 1.01x slower                                                |
| json                   | 2.95 ms                                                                | 2.98 ms: 1.01x slower                                                |
| pprint_safe_repr       | 513 ms                                                                 | 519 ms: 1.01x slower                                                 |
| python_startup_no_site | 11.9 ms                                                                | 12.1 ms: 1.01x slower                                                |
| python_startup         | 13.3 ms                                                                | 13.6 ms: 1.03x slower                                                |
| Geometric mean         | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (41): asyncio_tcp, typing_runtime_protocols, deepcopy_reduce, xml_etree_parse, pycparser, async_tree_io, sympy_integrate, async_tree_memoization, async_tree_memoization_tg, xml_etree_iterparse, dask, mypy2, json_dumps, async_tree_io_tg, sqlglot_transpile, logging_format, coroutines, sqlglot_optimize, async_tree_cpu_io_mixed_tg, 2to3, docutils, meteor_contest, async_tree_none_tg, scimark_sparse_mat_mult, create_gc_cycles, unpickle, deltablue, scimark_fft, pyflate, async_tree_cpu_io_mixed, mako, float, unpack_sequence, unpickle_list, sympy_sum, async_tree_none, nqueens, bench_mp_pool, tornado_http, coverage, asyncio_tcp_ssl


# HPT report

- Reliability score: 97.90% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x