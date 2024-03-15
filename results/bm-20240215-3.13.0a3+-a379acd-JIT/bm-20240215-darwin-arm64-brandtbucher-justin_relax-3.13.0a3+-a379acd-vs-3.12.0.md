
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_relax
- machine: darwin-arm64
- commit hash: a379acd
- commit date: 2024-02-15
- overall geometric mean: 1.00x faster \*
- HPT reliability: 70.75%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.14x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 193 ms: 1.14x slower                                                 |
| chameleon      | 4.70 ms                                                | 4.79 ms: 1.02x slower                                                |
| docutils       | 1.50 sec                                               | 1.46 sec: 1.03x faster                                               |
| Geometric mean | (ref)                                                  | 1.03x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 249 ms: 1.07x faster                                                 |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 516 ms: 1.02x faster                                                 |
| async_tree_io_tg           | 669 ms                                                 | 658 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 527 ms: 1.01x faster                                                 |
| async_tree_none_tg         | 258 ms                                                 | 256 ms: 1.01x faster                                                 |
| async_tree_io              | 668 ms                                                 | 692 ms: 1.04x slower                                                 |
| async_tree_memoization     | 312 ms                                                 | 325 ms: 1.04x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                         |

Benchmark hidden because not significant (1): async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 53.1 ms: 1.05x faster                                                |
| pidigits       | 282 ms                                                 | 282 ms: 1.00x slower                                                 |
| nbody          | 68.8 ms                                                | 71.3 ms: 1.04x slower                                                |
| Geometric mean | (ref)                                                  | 1.00x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 77.9 ms                                                | 73.7 ms: 1.06x faster                                                |
| regex_effbot   | 2.64 ms                                                | 2.55 ms: 1.03x faster                                                |
| regex_dna      | 154 ms                                                 | 151 ms: 1.02x faster                                                 |
| regex_v8       | 16.0 ms                                                | 17.0 ms: 1.07x slower                                                |
| Geometric mean | (ref)                                                  | 1.01x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| tomli_loads          | 1.39 sec                                               | 1.34 sec: 1.04x faster                                               |
| xml_etree_process    | 39.7 ms                                                | 38.3 ms: 1.03x faster                                                |
| pickle_pure_python   | 200 us                                                 | 195 us: 1.02x faster                                                 |
| xml_etree_generate   | 55.8 ms                                                | 54.9 ms: 1.02x faster                                                |
| json_loads           | 17.2 us                                                | 17.1 us: 1.01x faster                                                |
| xml_etree_iterparse  | 74.0 ms                                                | 73.6 ms: 1.01x faster                                                |
| pickle               | 7.23 us                                                | 7.25 us: 1.00x slower                                                |
| unpickle             | 9.12 us                                                | 9.15 us: 1.00x slower                                                |
| pickle_dict          | 18.1 us                                                | 18.1 us: 1.00x slower                                                |
| unpickle_list        | 3.02 us                                                | 3.07 us: 1.01x slower                                                |
| pickle_list          | 2.89 us                                                | 2.95 us: 1.02x slower                                                |
| json_dumps           | 6.22 ms                                                | 6.44 ms: 1.04x slower                                                |
| unpickle_pure_python | 151 us                                                 | 157 us: 1.04x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.5 ms: 1.18x slower                                                |
| python_startup_no_site | 9.37 ms                                                | 12.2 ms: 1.30x slower                                                |
| Geometric mean         | (ref)                                                  | 1.24x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 6.98 ms: 1.11x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240215-darwin-arm64-brandtbucher-justin_relax-3.13.0a3+-a379acd |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 70.0 us: 1.33x faster                                                |
| raytrace                   | 212 ms                                                 | 174 ms: 1.22x faster                                                 |
| comprehensions             | 14.5 us                                                | 12.0 us: 1.21x faster                                                |
| asyncio_tcp                | 449 ms                                                 | 394 ms: 1.14x faster                                                 |
| deltablue                  | 2.71 ms                                                | 2.43 ms: 1.11x faster                                                |
| unpack_sequence            | 31.5 ns                                                | 28.4 ns: 1.11x faster                                                |
| mako                       | 7.71 ms                                                | 6.98 ms: 1.11x faster                                                |
| generators                 | 31.1 ms                                                | 28.2 ms: 1.10x faster                                                |
| crypto_pyaes               | 51.9 ms                                                | 47.5 ms: 1.09x faster                                                |
| logging_silent             | 76.4 ns                                                | 70.3 ns: 1.09x faster                                                |
| sqlglot_parse              | 848 us                                                 | 785 us: 1.08x faster                                                 |
| deepcopy_memo              | 27.7 us                                                | 25.7 us: 1.07x faster                                                |
| logging_simple             | 3.69 us                                                | 3.43 us: 1.07x faster                                                |
| async_tree_none            | 266 ms                                                 | 249 ms: 1.07x faster                                                 |
| chaos                      | 42.5 ms                                                | 40.0 ms: 1.06x faster                                                |
| logging_format             | 3.98 us                                                | 3.75 us: 1.06x faster                                                |
| regex_compile              | 77.9 ms                                                | 73.7 ms: 1.06x faster                                                |
| sqlglot_transpile          | 1.02 ms                                                | 970 us: 1.05x faster                                                 |
| float                      | 55.8 ms                                                | 53.1 ms: 1.05x faster                                                |
| json                       | 3.09 ms                                                | 2.94 ms: 1.05x faster                                                |
| sympy_str                  | 148 ms                                                 | 141 ms: 1.05x faster                                                 |
| deepcopy                   | 235 us                                                 | 225 us: 1.04x faster                                                 |
| deepcopy_reduce            | 2.07 us                                                | 1.99 us: 1.04x faster                                                |
| tomli_loads                | 1.39 sec                                               | 1.34 sec: 1.04x faster                                               |
| sympy_sum                  | 77.6 ms                                                | 75.0 ms: 1.04x faster                                                |
| xml_etree_process          | 39.7 ms                                                | 38.3 ms: 1.03x faster                                                |
| regex_effbot               | 2.64 ms                                                | 2.55 ms: 1.03x faster                                                |
| docutils                   | 1.50 sec                                               | 1.46 sec: 1.03x faster                                               |
| pickle_pure_python         | 200 us                                                 | 195 us: 1.02x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 181 ms: 1.02x faster                                                 |
| nqueens                    | 62.4 ms                                                | 61.1 ms: 1.02x faster                                                |
| coroutines                 | 19.2 ms                                                | 18.9 ms: 1.02x faster                                                |
| scimark_lu                 | 76.0 ms                                                | 74.5 ms: 1.02x faster                                                |
| regex_dna                  | 154 ms                                                 | 151 ms: 1.02x faster                                                 |
| sympy_integrate            | 11.4 ms                                                | 11.2 ms: 1.02x faster                                                |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 516 ms: 1.02x faster                                                 |
| xml_etree_generate         | 55.8 ms                                                | 54.9 ms: 1.02x faster                                                |
| richards_super             | 36.0 ms                                                | 35.4 ms: 1.02x faster                                                |
| async_tree_io_tg           | 669 ms                                                 | 658 ms: 1.02x faster                                                 |
| richards                   | 32.1 ms                                                | 31.7 ms: 1.02x faster                                                |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 527 ms: 1.01x faster                                                 |
| json_loads                 | 17.2 us                                                | 17.1 us: 1.01x faster                                                |
| async_tree_none_tg         | 258 ms                                                 | 256 ms: 1.01x faster                                                 |
| xml_etree_iterparse        | 74.0 ms                                                | 73.6 ms: 1.01x faster                                                |
| dulwich_log                | 29.8 ms                                                | 29.6 ms: 1.01x faster                                                |
| sympy_expand               | 241 ms                                                 | 240 ms: 1.01x faster                                                 |
| pidigits                   | 282 ms                                                 | 282 ms: 1.00x slower                                                 |
| create_gc_cycles           | 701 us                                                 | 703 us: 1.00x slower                                                 |
| pickle                     | 7.23 us                                                | 7.25 us: 1.00x slower                                                |
| sqlglot_optimize           | 34.0 ms                                                | 34.2 ms: 1.00x slower                                                |
| unpickle                   | 9.12 us                                                | 9.15 us: 1.00x slower                                                |
| pickle_dict                | 18.1 us                                                | 18.1 us: 1.00x slower                                                |
| spectral_norm              | 76.4 ms                                                | 77.1 ms: 1.01x slower                                                |
| sqlite_synth               | 1.57 us                                                | 1.59 us: 1.01x slower                                                |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.17 ms: 1.01x slower                                                |
| pprint_pformat             | 1.01 sec                                               | 1.02 sec: 1.01x slower                                               |
| unpickle_list              | 3.02 us                                                | 3.07 us: 1.01x slower                                                |
| dask                       | 222 ms                                                 | 226 ms: 1.02x slower                                                 |
| pycparser                  | 677 ms                                                 | 688 ms: 1.02x slower                                                 |
| mdp                        | 1.58 sec                                               | 1.61 sec: 1.02x slower                                               |
| pprint_safe_repr           | 497 ms                                                 | 507 ms: 1.02x slower                                                 |
| chameleon                  | 4.70 ms                                                | 4.79 ms: 1.02x slower                                                |
| pickle_list                | 2.89 us                                                | 2.95 us: 1.02x slower                                                |
| meteor_contest             | 71.7 ms                                                | 73.6 ms: 1.03x slower                                                |
| json_dumps                 | 6.22 ms                                                | 6.44 ms: 1.04x slower                                                |
| nbody                      | 68.8 ms                                                | 71.3 ms: 1.04x slower                                                |
| async_tree_io              | 668 ms                                                 | 692 ms: 1.04x slower                                                 |
| async_tree_memoization     | 312 ms                                                 | 325 ms: 1.04x slower                                                 |
| unpickle_pure_python       | 151 us                                                 | 157 us: 1.04x slower                                                 |
| bench_mp_pool              | 44.9 ms                                                | 47.0 ms: 1.05x slower                                                |
| scimark_fft                | 195 ms                                                 | 205 ms: 1.05x slower                                                 |
| scimark_monte_carlo        | 45.0 ms                                                | 47.3 ms: 1.05x slower                                                |
| hexiom                     | 4.54 ms                                                | 4.79 ms: 1.05x slower                                                |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.31 sec: 1.06x slower                                               |
| fannkuch                   | 248 ms                                                 | 263 ms: 1.06x slower                                                 |
| go                         | 102 ms                                                 | 108 ms: 1.06x slower                                                 |
| regex_v8                   | 16.0 ms                                                | 17.0 ms: 1.07x slower                                                |
| 2to3                       | 169 ms                                                 | 193 ms: 1.14x slower                                                 |
| python_startup             | 11.4 ms                                                | 13.5 ms: 1.18x slower                                                |
| telco                      | 3.68 ms                                                | 4.43 ms: 1.20x slower                                                |
| scimark_sor                | 87.4 ms                                                | 105 ms: 1.21x slower                                                 |
| coverage                   | 38.9 ms                                                | 47.9 ms: 1.23x slower                                                |
| python_startup_no_site     | 9.37 ms                                                | 12.2 ms: 1.30x slower                                                |
| mypy2                      | 380 ms                                                 | 590 ms: 1.55x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                         |

Benchmark hidden because not significant (9): async_tree_memoization_tg, xml_etree_parse, gc_traversal, bench_thread_pool, asyncio_websockets, async_generators, pyflate, pathlib, tornado_http
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 70.75% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.14x