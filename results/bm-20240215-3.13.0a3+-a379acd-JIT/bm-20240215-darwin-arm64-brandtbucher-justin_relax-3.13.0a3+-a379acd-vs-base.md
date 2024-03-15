# Results vs. base

- fork: brandtbucher
- ref: justin_relax
- machine: darwin-arm64
- commit hash: a379acd
- commit date: 2024-02-15
- overall geometric mean: 1.01x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 174 ms                                                                 | 193 ms: 1.11x slower                                                 |
| chameleon      | 4.82 ms                                                                | 4.79 ms: 1.01x faster                                                |
| docutils       | 1.47 sec                                                               | 1.46 sec: 1.01x faster                                               |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none_tg | 258 ms                                                                 | 256 ms: 1.01x faster                                                 |
| async_tree_io      | 696 ms                                                                 | 692 ms: 1.01x faster                                                 |
| async_tree_io_tg   | 661 ms                                                                 | 658 ms: 1.00x faster                                                 |
| Geometric mean     | (ref)                                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (5): async_tree_none, async_tree_memoization_tg, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 76.6 ms                                                                | 71.3 ms: 1.07x faster                                                |
| float          | 55.6 ms                                                                | 53.1 ms: 1.05x faster                                                |
| pidigits       | 283 ms                                                                 | 282 ms: 1.00x faster                                                 |
| Geometric mean | (ref)                                                                  | 1.04x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 75.5 ms                                                                | 73.7 ms: 1.02x faster                                                |
| regex_effbot   | 2.56 ms                                                                | 2.55 ms: 1.00x faster                                                |
| regex_v8       | 17.0 ms                                                                | 17.0 ms: 1.00x faster                                                |
| Geometric mean | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| tomli_loads          | 1.41 sec                                                               | 1.34 sec: 1.05x faster                                               |
| xml_etree_iterparse  | 75.7 ms                                                                | 73.6 ms: 1.03x faster                                                |
| unpickle_pure_python | 159 us                                                                 | 157 us: 1.01x faster                                                 |
| pickle_list          | 2.98 us                                                                | 2.95 us: 1.01x faster                                                |
| pickle               | 7.32 us                                                                | 7.25 us: 1.01x faster                                                |
| xml_etree_process    | 38.7 ms                                                                | 38.3 ms: 1.01x faster                                                |
| unpickle_list        | 3.09 us                                                                | 3.07 us: 1.01x faster                                                |
| xml_etree_generate   | 55.2 ms                                                                | 54.9 ms: 1.00x faster                                                |
| json_dumps           | 6.47 ms                                                                | 6.44 ms: 1.00x faster                                                |
| pickle_dict          | 18.2 us                                                                | 18.1 us: 1.00x faster                                                |
| pickle_pure_python   | 196 us                                                                 | 195 us: 1.00x faster                                                 |
| json_loads           | 17.0 us                                                                | 17.1 us: 1.01x slower                                                |
| Geometric mean       | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (2): xml_etree_parse, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 13.3 ms                                                                | 13.5 ms: 1.02x slower                                                |
| python_startup_no_site | 11.9 ms                                                                | 12.2 ms: 1.02x slower                                                |
| Geometric mean         | (ref)                                                                  | 1.02x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 7.80 ms                                                                | 6.98 ms: 1.12x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20240212-darwin-arm64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako                     | 7.80 ms                                                                | 6.98 ms: 1.12x faster                                                |
| asyncio_tcp              | 427 ms                                                                 | 394 ms: 1.08x faster                                                 |
| nbody                    | 76.6 ms                                                                | 71.3 ms: 1.07x faster                                                |
| scimark_fft              | 218 ms                                                                 | 205 ms: 1.07x faster                                                 |
| scimark_sparse_mat_mult  | 3.33 ms                                                                | 3.17 ms: 1.05x faster                                                |
| comprehensions           | 12.6 us                                                                | 12.0 us: 1.05x faster                                                |
| tomli_loads              | 1.41 sec                                                               | 1.34 sec: 1.05x faster                                               |
| hexiom                   | 5.01 ms                                                                | 4.79 ms: 1.05x faster                                                |
| float                    | 55.6 ms                                                                | 53.1 ms: 1.05x faster                                                |
| spectral_norm            | 80.6 ms                                                                | 77.1 ms: 1.05x faster                                                |
| fannkuch                 | 275 ms                                                                 | 263 ms: 1.04x faster                                                 |
| telco                    | 4.59 ms                                                                | 4.43 ms: 1.04x faster                                                |
| chaos                    | 41.5 ms                                                                | 40.0 ms: 1.04x faster                                                |
| pyflate                  | 327 ms                                                                 | 316 ms: 1.03x faster                                                 |
| crypto_pyaes             | 49.1 ms                                                                | 47.5 ms: 1.03x faster                                                |
| scimark_monte_carlo      | 48.8 ms                                                                | 47.3 ms: 1.03x faster                                                |
| xml_etree_iterparse      | 75.7 ms                                                                | 73.6 ms: 1.03x faster                                                |
| regex_compile            | 75.5 ms                                                                | 73.7 ms: 1.02x faster                                                |
| pprint_pformat           | 1.05 sec                                                               | 1.02 sec: 1.02x faster                                               |
| sqlite_synth             | 1.62 us                                                                | 1.59 us: 1.02x faster                                                |
| sympy_str                | 143 ms                                                                 | 141 ms: 1.02x faster                                                 |
| raytrace                 | 177 ms                                                                 | 174 ms: 1.02x faster                                                 |
| nqueens                  | 62.1 ms                                                                | 61.1 ms: 1.02x faster                                                |
| deepcopy_memo            | 26.1 us                                                                | 25.7 us: 1.01x faster                                                |
| meteor_contest           | 74.7 ms                                                                | 73.6 ms: 1.01x faster                                                |
| unpickle_pure_python     | 159 us                                                                 | 157 us: 1.01x faster                                                 |
| sqlglot_parse            | 795 us                                                                 | 785 us: 1.01x faster                                                 |
| deltablue                | 2.46 ms                                                                | 2.43 ms: 1.01x faster                                                |
| pprint_safe_repr         | 513 ms                                                                 | 507 ms: 1.01x faster                                                 |
| pickle_list              | 2.98 us                                                                | 2.95 us: 1.01x faster                                                |
| go                       | 109 ms                                                                 | 108 ms: 1.01x faster                                                 |
| mdp                      | 1.63 sec                                                               | 1.61 sec: 1.01x faster                                               |
| sympy_expand             | 243 ms                                                                 | 240 ms: 1.01x faster                                                 |
| sympy_integrate          | 11.3 ms                                                                | 11.2 ms: 1.01x faster                                                |
| sqlglot_optimize         | 34.5 ms                                                                | 34.2 ms: 1.01x faster                                                |
| richards                 | 32.0 ms                                                                | 31.7 ms: 1.01x faster                                                |
| pycparser                | 695 ms                                                                 | 688 ms: 1.01x faster                                                 |
| pickle                   | 7.32 us                                                                | 7.25 us: 1.01x faster                                                |
| richards_super           | 35.8 ms                                                                | 35.4 ms: 1.01x faster                                                |
| typing_runtime_protocols | 70.7 us                                                                | 70.0 us: 1.01x faster                                                |
| xml_etree_process        | 38.7 ms                                                                | 38.3 ms: 1.01x faster                                                |
| sqlglot_transpile        | 979 us                                                                 | 970 us: 1.01x faster                                                 |
| unpickle_list            | 3.09 us                                                                | 3.07 us: 1.01x faster                                                |
| sqlglot_normalize        | 183 ms                                                                 | 181 ms: 1.01x faster                                                 |
| async_tree_none_tg       | 258 ms                                                                 | 256 ms: 1.01x faster                                                 |
| sympy_sum                | 75.5 ms                                                                | 75.0 ms: 1.01x faster                                                |
| logging_format           | 3.78 us                                                                | 3.75 us: 1.01x faster                                                |
| logging_simple           | 3.45 us                                                                | 3.43 us: 1.01x faster                                                |
| deepcopy_reduce          | 2.00 us                                                                | 1.99 us: 1.01x faster                                                |
| docutils                 | 1.47 sec                                                               | 1.46 sec: 1.01x faster                                               |
| chameleon                | 4.82 ms                                                                | 4.79 ms: 1.01x faster                                                |
| async_tree_io            | 696 ms                                                                 | 692 ms: 1.01x faster                                                 |
| xml_etree_generate       | 55.2 ms                                                                | 54.9 ms: 1.00x faster                                                |
| json_dumps               | 6.47 ms                                                                | 6.44 ms: 1.00x faster                                                |
| pickle_dict              | 18.2 us                                                                | 18.1 us: 1.00x faster                                                |
| create_gc_cycles         | 706 us                                                                 | 703 us: 1.00x faster                                                 |
| async_tree_io_tg         | 661 ms                                                                 | 658 ms: 1.00x faster                                                 |
| scimark_lu               | 74.8 ms                                                                | 74.5 ms: 1.00x faster                                                |
| pickle_pure_python       | 196 us                                                                 | 195 us: 1.00x faster                                                 |
| scimark_sor              | 106 ms                                                                 | 105 ms: 1.00x faster                                                 |
| logging_silent           | 70.5 ns                                                                | 70.3 ns: 1.00x faster                                                |
| dulwich_log              | 29.7 ms                                                                | 29.6 ms: 1.00x faster                                                |
| regex_effbot             | 2.56 ms                                                                | 2.55 ms: 1.00x faster                                                |
| pidigits                 | 283 ms                                                                 | 282 ms: 1.00x faster                                                 |
| regex_v8                 | 17.0 ms                                                                | 17.0 ms: 1.00x faster                                                |
| deepcopy                 | 224 us                                                                 | 225 us: 1.01x slower                                                 |
| async_generators         | 302 ms                                                                 | 304 ms: 1.01x slower                                                 |
| json_loads               | 17.0 us                                                                | 17.1 us: 1.01x slower                                                |
| coverage                 | 47.2 ms                                                                | 47.9 ms: 1.01x slower                                                |
| python_startup           | 13.3 ms                                                                | 13.5 ms: 1.02x slower                                                |
| python_startup_no_site   | 11.9 ms                                                                | 12.2 ms: 1.02x slower                                                |
| coroutines               | 18.5 ms                                                                | 18.9 ms: 1.02x slower                                                |
| 2to3                     | 174 ms                                                                 | 193 ms: 1.11x slower                                                 |
| Geometric mean           | (ref)                                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (20): async_tree_none, async_tree_memoization_tg, async_tree_memoization, xml_etree_parse, json, async_tree_cpu_io_mixed, unpack_sequence, async_tree_cpu_io_mixed_tg, regex_dna, unpickle, asyncio_websockets, bench_mp_pool, dask, bench_thread_pool, tornado_http, generators, gc_traversal, pathlib, asyncio_tcp_ssl, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.99x