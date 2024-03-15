# Results vs. base

- fork: brandtbucher
- ref: justin_continue
- machine: darwin-arm64
- commit hash: 9e86002
- commit date: 2024-02-13
- overall geometric mean: 1.01x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| docutils       | 1.47 sec                                                               | 1.47 sec: 1.01x faster                                                  |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (3): 2to3, chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|--------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none_tg | 258 ms                                                                 | 257 ms: 1.00x faster                                                    |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                            |

Benchmark hidden because not significant (7): async_tree_memoization_tg, async_tree_io, async_tree_none, async_tree_io_tg, async_tree_cpu_io_mixed, async_tree_memoization, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 55.6 ms                                                                | 54.6 ms: 1.02x faster                                                   |
| nbody          | 76.6 ms                                                                | 75.6 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 75.5 ms                                                                | 74.2 ms: 1.02x faster                                                   |
| regex_dna      | 152 ms                                                                 | 151 ms: 1.00x faster                                                    |
| regex_effbot   | 2.56 ms                                                                | 2.55 ms: 1.00x faster                                                   |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| tomli_loads          | 1.41 sec                                                               | 1.37 sec: 1.03x faster                                                  |
| pickle_list          | 2.98 us                                                                | 2.95 us: 1.01x faster                                                   |
| pickle               | 7.32 us                                                                | 7.25 us: 1.01x faster                                                   |
| xml_etree_iterparse  | 75.7 ms                                                                | 75.1 ms: 1.01x faster                                                   |
| xml_etree_process    | 38.7 ms                                                                | 38.5 ms: 1.01x faster                                                   |
| pickle_dict          | 18.2 us                                                                | 18.1 us: 1.01x faster                                                   |
| unpickle_pure_python | 159 us                                                                 | 158 us: 1.01x faster                                                    |
| json_loads           | 17.0 us                                                                | 17.1 us: 1.01x slower                                                   |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                            |

Benchmark hidden because not significant (6): unpickle, json_dumps, xml_etree_generate, pickle_pure_python, xml_etree_parse, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup | 13.3 ms                                                                | 13.4 ms: 1.01x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                            |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-----------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 7.80 ms                                                                | 7.52 ms: 1.04x faster                                                   |

All benchmarks:
===============

| Benchmark               | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240213-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| fannkuch                | 275 ms                                                                 | 264 ms: 1.04x faster                                                    |
| mako                    | 7.80 ms                                                                | 7.52 ms: 1.04x faster                                                   |
| spectral_norm           | 80.6 ms                                                                | 78.1 ms: 1.03x faster                                                   |
| telco                   | 4.59 ms                                                                | 4.45 ms: 1.03x faster                                                   |
| hexiom                  | 5.01 ms                                                                | 4.87 ms: 1.03x faster                                                   |
| tomli_loads             | 1.41 sec                                                               | 1.37 sec: 1.03x faster                                                  |
| scimark_sparse_mat_mult | 3.33 ms                                                                | 3.26 ms: 1.02x faster                                                   |
| scimark_fft             | 218 ms                                                                 | 214 ms: 1.02x faster                                                    |
| comprehensions          | 12.6 us                                                                | 12.4 us: 1.02x faster                                                   |
| float                   | 55.6 ms                                                                | 54.6 ms: 1.02x faster                                                   |
| regex_compile           | 75.5 ms                                                                | 74.2 ms: 1.02x faster                                                   |
| mdp                     | 1.63 sec                                                               | 1.60 sec: 1.02x faster                                                  |
| sympy_str               | 143 ms                                                                 | 141 ms: 1.02x faster                                                    |
| sqlite_synth            | 1.62 us                                                                | 1.59 us: 1.02x faster                                                   |
| chaos                   | 41.5 ms                                                                | 40.9 ms: 1.01x faster                                                   |
| sympy_integrate         | 11.3 ms                                                                | 11.1 ms: 1.01x faster                                                   |
| pyflate                 | 327 ms                                                                 | 322 ms: 1.01x faster                                                    |
| pprint_pformat          | 1.05 sec                                                               | 1.03 sec: 1.01x faster                                                  |
| nbody                   | 76.6 ms                                                                | 75.6 ms: 1.01x faster                                                   |
| sympy_expand            | 243 ms                                                                 | 239 ms: 1.01x faster                                                    |
| pickle_list             | 2.98 us                                                                | 2.95 us: 1.01x faster                                                   |
| pprint_safe_repr        | 513 ms                                                                 | 507 ms: 1.01x faster                                                    |
| go                      | 109 ms                                                                 | 108 ms: 1.01x faster                                                    |
| scimark_monte_carlo     | 48.8 ms                                                                | 48.3 ms: 1.01x faster                                                   |
| sqlglot_parse           | 795 us                                                                 | 787 us: 1.01x faster                                                    |
| crypto_pyaes            | 49.1 ms                                                                | 48.6 ms: 1.01x faster                                                   |
| pickle                  | 7.32 us                                                                | 7.25 us: 1.01x faster                                                   |
| pycparser               | 695 ms                                                                 | 689 ms: 1.01x faster                                                    |
| deltablue               | 2.46 ms                                                                | 2.44 ms: 1.01x faster                                                   |
| xml_etree_iterparse     | 75.7 ms                                                                | 75.1 ms: 1.01x faster                                                   |
| deepcopy_reduce         | 2.00 us                                                                | 1.99 us: 1.01x faster                                                   |
| sympy_sum               | 75.5 ms                                                                | 74.9 ms: 1.01x faster                                                   |
| sqlglot_transpile       | 979 us                                                                 | 971 us: 1.01x faster                                                    |
| deepcopy_memo           | 26.1 us                                                                | 25.9 us: 1.01x faster                                                   |
| xml_etree_process       | 38.7 ms                                                                | 38.5 ms: 1.01x faster                                                   |
| richards_super          | 35.8 ms                                                                | 35.6 ms: 1.01x faster                                                   |
| pickle_dict             | 18.2 us                                                                | 18.1 us: 1.01x faster                                                   |
| raytrace                | 177 ms                                                                 | 176 ms: 1.01x faster                                                    |
| unpickle_pure_python    | 159 us                                                                 | 158 us: 1.01x faster                                                    |
| meteor_contest          | 74.7 ms                                                                | 74.3 ms: 1.01x faster                                                   |
| docutils                | 1.47 sec                                                               | 1.47 sec: 1.01x faster                                                  |
| sqlglot_optimize        | 34.5 ms                                                                | 34.4 ms: 1.00x faster                                                   |
| nqueens                 | 62.1 ms                                                                | 61.9 ms: 1.00x faster                                                   |
| async_tree_none_tg      | 258 ms                                                                 | 257 ms: 1.00x faster                                                    |
| richards                | 32.0 ms                                                                | 31.9 ms: 1.00x faster                                                   |
| regex_dna               | 152 ms                                                                 | 151 ms: 1.00x faster                                                    |
| regex_effbot            | 2.56 ms                                                                | 2.55 ms: 1.00x faster                                                   |
| sqlglot_normalize       | 183 ms                                                                 | 183 ms: 1.00x faster                                                    |
| scimark_sor             | 106 ms                                                                 | 106 ms: 1.00x faster                                                    |
| async_generators        | 302 ms                                                                 | 303 ms: 1.00x slower                                                    |
| gc_traversal            | 2.39 ms                                                                | 2.39 ms: 1.00x slower                                                   |
| generators              | 28.2 ms                                                                | 28.2 ms: 1.00x slower                                                   |
| logging_simple          | 3.45 us                                                                | 3.46 us: 1.00x slower                                                   |
| deepcopy                | 224 us                                                                 | 225 us: 1.00x slower                                                    |
| json_loads              | 17.0 us                                                                | 17.1 us: 1.01x slower                                                   |
| python_startup          | 13.3 ms                                                                | 13.4 ms: 1.01x slower                                                   |
| coverage                | 47.2 ms                                                                | 47.8 ms: 1.01x slower                                                   |
| coroutines              | 18.5 ms                                                                | 19.2 ms: 1.04x slower                                                   |
| Geometric mean          | (ref)                                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (35): tornado_http, pathlib, mypy2, 2to3, dask, async_tree_memoization_tg, typing_runtime_protocols, json, unpickle, bench_thread_pool, async_tree_io, async_tree_none, json_dumps, async_tree_io_tg, chameleon, xml_etree_generate, create_gc_cycles, async_tree_cpu_io_mixed, pickle_pure_python, async_tree_memoization, pidigits, asyncio_websockets, async_tree_cpu_io_mixed_tg, bench_mp_pool, unpack_sequence, regex_v8, dulwich_log, logging_format, logging_silent, scimark_lu, python_startup_no_site, asyncio_tcp_ssl, xml_etree_parse, unpickle_list, asyncio_tcp


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x