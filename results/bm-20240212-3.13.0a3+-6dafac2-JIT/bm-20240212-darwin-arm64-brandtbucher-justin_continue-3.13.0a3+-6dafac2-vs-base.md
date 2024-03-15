# Results vs. base

- fork: brandtbucher
- ref: justin_continue
- machine: darwin-arm64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.01x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 174 ms                                                                 | 173 ms: 1.01x faster                                                    |
| chameleon      | 4.82 ms                                                                | 4.77 ms: 1.01x faster                                                   |
| docutils       | 1.47 sec                                                               | 1.47 sec: 1.00x faster                                                  |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_memoization_tg, async_tree_none_tg, async_tree_io_tg, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| nbody          | 76.6 ms                                                                | 75.5 ms: 1.01x faster                                                   |
| float          | 55.6 ms                                                                | 54.8 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 75.5 ms                                                                | 74.6 ms: 1.01x faster                                                   |
| regex_effbot   | 2.56 ms                                                                | 2.55 ms: 1.00x faster                                                   |
| regex_dna      | 152 ms                                                                 | 152 ms: 1.00x slower                                                    |
| Geometric mean | (ref)                                                                  | 1.00x faster                                                            |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| tomli_loads          | 1.41 sec                                                               | 1.37 sec: 1.03x faster                                                  |
| xml_etree_iterparse  | 75.7 ms                                                                | 74.9 ms: 1.01x faster                                                   |
| pickle_list          | 2.98 us                                                                | 2.95 us: 1.01x faster                                                   |
| unpickle_pure_python | 159 us                                                                 | 158 us: 1.01x faster                                                    |
| pickle               | 7.32 us                                                                | 7.27 us: 1.01x faster                                                   |
| xml_etree_process    | 38.7 ms                                                                | 38.5 ms: 1.01x faster                                                   |
| pickle_dict          | 18.2 us                                                                | 18.1 us: 1.00x faster                                                   |
| json_loads           | 17.0 us                                                                | 17.1 us: 1.01x slower                                                   |
| xml_etree_generate   | 55.2 ms                                                                | 55.8 ms: 1.01x slower                                                   |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                            |

Benchmark hidden because not significant (5): pickle_pure_python, unpickle_list, json_dumps, unpickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup | 13.3 ms                                                                | 13.3 ms: 1.00x slower                                                   |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                            |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 7.80 ms                                                                | 7.47 ms: 1.04x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240212-darwin-arm64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|--------------------------|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------:|
| comprehensions           | 12.6 us                                                                | 12.0 us: 1.05x faster                                                   |
| hexiom                   | 5.01 ms                                                                | 4.78 ms: 1.05x faster                                                   |
| fannkuch                 | 275 ms                                                                 | 263 ms: 1.05x faster                                                    |
| mako                     | 7.80 ms                                                                | 7.47 ms: 1.04x faster                                                   |
| telco                    | 4.59 ms                                                                | 4.45 ms: 1.03x faster                                                   |
| spectral_norm            | 80.6 ms                                                                | 78.1 ms: 1.03x faster                                                   |
| pathlib                  | 24.3 ms                                                                | 23.5 ms: 1.03x faster                                                   |
| pprint_pformat           | 1.05 sec                                                               | 1.01 sec: 1.03x faster                                                  |
| tomli_loads              | 1.41 sec                                                               | 1.37 sec: 1.03x faster                                                  |
| sqlite_synth             | 1.62 us                                                                | 1.58 us: 1.03x faster                                                   |
| pprint_safe_repr         | 513 ms                                                                 | 501 ms: 1.02x faster                                                    |
| scimark_fft              | 218 ms                                                                 | 213 ms: 1.02x faster                                                    |
| mdp                      | 1.63 sec                                                               | 1.59 sec: 1.02x faster                                                  |
| scimark_monte_carlo      | 48.8 ms                                                                | 47.8 ms: 1.02x faster                                                   |
| scimark_sparse_mat_mult  | 3.33 ms                                                                | 3.27 ms: 1.02x faster                                                   |
| chaos                    | 41.5 ms                                                                | 40.7 ms: 1.02x faster                                                   |
| pyflate                  | 327 ms                                                                 | 321 ms: 1.02x faster                                                    |
| nbody                    | 76.6 ms                                                                | 75.5 ms: 1.01x faster                                                   |
| sympy_str                | 143 ms                                                                 | 141 ms: 1.01x faster                                                    |
| float                    | 55.6 ms                                                                | 54.8 ms: 1.01x faster                                                   |
| sympy_integrate          | 11.3 ms                                                                | 11.1 ms: 1.01x faster                                                   |
| sqlglot_parse            | 795 us                                                                 | 785 us: 1.01x faster                                                    |
| crypto_pyaes             | 49.1 ms                                                                | 48.4 ms: 1.01x faster                                                   |
| deepcopy_memo            | 26.1 us                                                                | 25.8 us: 1.01x faster                                                   |
| sympy_expand             | 243 ms                                                                 | 240 ms: 1.01x faster                                                    |
| xml_etree_iterparse      | 75.7 ms                                                                | 74.9 ms: 1.01x faster                                                   |
| regex_compile            | 75.5 ms                                                                | 74.6 ms: 1.01x faster                                                   |
| typing_runtime_protocols | 70.7 us                                                                | 70.0 us: 1.01x faster                                                   |
| pickle_list              | 2.98 us                                                                | 2.95 us: 1.01x faster                                                   |
| chameleon                | 4.82 ms                                                                | 4.77 ms: 1.01x faster                                                   |
| sympy_sum                | 75.5 ms                                                                | 74.8 ms: 1.01x faster                                                   |
| nqueens                  | 62.1 ms                                                                | 61.5 ms: 1.01x faster                                                   |
| sqlglot_optimize         | 34.5 ms                                                                | 34.2 ms: 1.01x faster                                                   |
| deltablue                | 2.46 ms                                                                | 2.44 ms: 1.01x faster                                                   |
| bench_thread_pool        | 503 us                                                                 | 499 us: 1.01x faster                                                    |
| 2to3                     | 174 ms                                                                 | 173 ms: 1.01x faster                                                    |
| raytrace                 | 177 ms                                                                 | 176 ms: 1.01x faster                                                    |
| unpickle_pure_python     | 159 us                                                                 | 158 us: 1.01x faster                                                    |
| pickle                   | 7.32 us                                                                | 7.27 us: 1.01x faster                                                   |
| richards_super           | 35.8 ms                                                                | 35.6 ms: 1.01x faster                                                   |
| sqlglot_transpile        | 979 us                                                                 | 972 us: 1.01x faster                                                    |
| meteor_contest           | 74.7 ms                                                                | 74.3 ms: 1.01x faster                                                   |
| deepcopy_reduce          | 2.00 us                                                                | 1.99 us: 1.01x faster                                                   |
| go                       | 109 ms                                                                 | 109 ms: 1.01x faster                                                    |
| xml_etree_process        | 38.7 ms                                                                | 38.5 ms: 1.01x faster                                                   |
| docutils                 | 1.47 sec                                                               | 1.47 sec: 1.00x faster                                                  |
| pickle_dict              | 18.2 us                                                                | 18.1 us: 1.00x faster                                                   |
| coroutines               | 18.5 ms                                                                | 18.4 ms: 1.00x faster                                                   |
| sqlglot_normalize        | 183 ms                                                                 | 182 ms: 1.00x faster                                                    |
| richards                 | 32.0 ms                                                                | 31.9 ms: 1.00x faster                                                   |
| create_gc_cycles         | 706 us                                                                 | 704 us: 1.00x faster                                                    |
| asyncio_websockets       | 409 ms                                                                 | 408 ms: 1.00x faster                                                    |
| async_generators         | 302 ms                                                                 | 301 ms: 1.00x faster                                                    |
| regex_effbot             | 2.56 ms                                                                | 2.55 ms: 1.00x faster                                                   |
| scimark_sor              | 106 ms                                                                 | 106 ms: 1.00x faster                                                    |
| regex_dna                | 152 ms                                                                 | 152 ms: 1.00x slower                                                    |
| logging_format           | 3.78 us                                                                | 3.79 us: 1.00x slower                                                   |
| logging_simple           | 3.45 us                                                                | 3.46 us: 1.00x slower                                                   |
| python_startup           | 13.3 ms                                                                | 13.3 ms: 1.00x slower                                                   |
| json                     | 2.95 ms                                                                | 2.97 ms: 1.01x slower                                                   |
| coverage                 | 47.2 ms                                                                | 47.5 ms: 1.01x slower                                                   |
| deepcopy                 | 224 us                                                                 | 226 us: 1.01x slower                                                    |
| generators               | 28.2 ms                                                                | 28.4 ms: 1.01x slower                                                   |
| json_loads               | 17.0 us                                                                | 17.1 us: 1.01x slower                                                   |
| xml_etree_generate       | 55.2 ms                                                                | 55.8 ms: 1.01x slower                                                   |
| Geometric mean           | (ref)                                                                  | 1.01x faster                                                            |

Benchmark hidden because not significant (28): asyncio_tcp, tornado_http, dask, pycparser, mypy2, bench_mp_pool, async_tree_memoization_tg, async_tree_none_tg, async_tree_io_tg, pickle_pure_python, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_none, unpickle_list, scimark_lu, regex_v8, asyncio_tcp_ssl, pidigits, dulwich_log, async_tree_io, gc_traversal, json_dumps, logging_silent, async_tree_memoization, unpack_sequence, unpickle, python_startup_no_site, xml_etree_parse


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x