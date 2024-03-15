
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: darwin-arm64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.00x faster
- HPT reliability: 81.25%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| chameleon      | 4.70 ms                                                | 4.89 ms: 1.04x slower                                                  |
| docutils       | 1.50 sec                                               | 1.45 sec: 1.03x faster                                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (2): 2to3, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 249 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 517 ms: 1.02x faster                                                   |
| async_tree_io_tg           | 669 ms                                                 | 664 ms: 1.01x faster                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 528 ms: 1.01x faster                                                   |
| async_tree_io              | 668 ms                                                 | 694 ms: 1.04x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 325 ms: 1.04x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| float          | 55.8 ms                                                | 56.4 ms: 1.01x slower                                                  |
| nbody          | 68.8 ms                                                | 75.0 ms: 1.09x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 77.9 ms                                                | 73.1 ms: 1.07x faster                                                  |
| regex_effbot   | 2.64 ms                                                | 2.56 ms: 1.03x faster                                                  |
| regex_dna      | 154 ms                                                 | 151 ms: 1.02x faster                                                   |
| regex_v8       | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_loads           | 17.2 us                                                | 16.9 us: 1.02x faster                                                  |
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                                   |
| xml_etree_parse      | 106 ms                                                 | 105 ms: 1.01x faster                                                   |
| pickle_dict          | 18.1 us                                                | 18.1 us: 1.00x slower                                                  |
| xml_etree_generate   | 55.8 ms                                                | 56.1 ms: 1.01x slower                                                  |
| unpickle             | 9.12 us                                                | 9.23 us: 1.01x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 153 us: 1.02x slower                                                   |
| xml_etree_iterparse  | 74.0 ms                                                | 75.5 ms: 1.02x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.09 us: 1.02x slower                                                  |
| pickle_list          | 2.89 us                                                | 2.97 us: 1.03x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.49 ms: 1.04x slower                                                  |
| tomli_loads          | 1.39 sec                                               | 1.54 sec: 1.11x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                           |

Benchmark hidden because not significant (2): xml_etree_process, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.0 ms: 1.14x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 11.6 ms: 1.24x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.19x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.59 ms: 1.02x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 70.8 us: 1.31x faster                                                  |
| raytrace                   | 212 ms                                                 | 170 ms: 1.25x faster                                                   |
| comprehensions             | 14.5 us                                                | 11.9 us: 1.22x faster                                                  |
| deltablue                  | 2.71 ms                                                | 2.43 ms: 1.11x faster                                                  |
| unpack_sequence            | 31.5 ns                                                | 28.4 ns: 1.11x faster                                                  |
| generators                 | 31.1 ms                                                | 28.3 ms: 1.10x faster                                                  |
| logging_silent             | 76.4 ns                                                | 70.1 ns: 1.09x faster                                                  |
| chaos                      | 42.5 ms                                                | 39.5 ms: 1.08x faster                                                  |
| sympy_sum                  | 77.6 ms                                                | 72.1 ms: 1.08x faster                                                  |
| deepcopy_memo              | 27.7 us                                                | 25.7 us: 1.08x faster                                                  |
| crypto_pyaes               | 51.9 ms                                                | 48.3 ms: 1.07x faster                                                  |
| logging_simple             | 3.69 us                                                | 3.45 us: 1.07x faster                                                  |
| sqlglot_parse              | 848 us                                                 | 793 us: 1.07x faster                                                   |
| async_tree_none            | 266 ms                                                 | 249 ms: 1.07x faster                                                   |
| regex_compile              | 77.9 ms                                                | 73.1 ms: 1.07x faster                                                  |
| sympy_integrate            | 11.4 ms                                                | 10.7 ms: 1.07x faster                                                  |
| sympy_str                  | 148 ms                                                 | 139 ms: 1.06x faster                                                   |
| logging_format             | 3.98 us                                                | 3.75 us: 1.06x faster                                                  |
| sqlglot_transpile          | 1.02 ms                                                | 971 us: 1.05x faster                                                   |
| json                       | 3.09 ms                                                | 2.94 ms: 1.05x faster                                                  |
| deepcopy                   | 235 us                                                 | 224 us: 1.05x faster                                                   |
| nqueens                    | 62.4 ms                                                | 60.1 ms: 1.04x faster                                                  |
| deepcopy_reduce            | 2.07 us                                                | 2.00 us: 1.04x faster                                                  |
| docutils                   | 1.50 sec                                               | 1.45 sec: 1.03x faster                                                 |
| async_generators           | 304 ms                                                 | 294 ms: 1.03x faster                                                   |
| regex_effbot               | 2.64 ms                                                | 2.56 ms: 1.03x faster                                                  |
| bench_thread_pool          | 504 us                                                 | 491 us: 1.03x faster                                                   |
| sqlglot_normalize          | 186 ms                                                 | 182 ms: 1.02x faster                                                   |
| spectral_norm              | 76.4 ms                                                | 74.7 ms: 1.02x faster                                                  |
| json_loads                 | 17.2 us                                                | 16.9 us: 1.02x faster                                                  |
| pickle_pure_python         | 200 us                                                 | 196 us: 1.02x faster                                                   |
| regex_dna                  | 154 ms                                                 | 151 ms: 1.02x faster                                                   |
| scimark_lu                 | 76.0 ms                                                | 74.7 ms: 1.02x faster                                                  |
| mako                       | 7.71 ms                                                | 7.59 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 517 ms: 1.02x faster                                                   |
| sympy_expand               | 241 ms                                                 | 237 ms: 1.02x faster                                                   |
| hexiom                     | 4.54 ms                                                | 4.47 ms: 1.02x faster                                                  |
| mdp                        | 1.58 sec                                               | 1.56 sec: 1.02x faster                                                 |
| dulwich_log                | 29.8 ms                                                | 29.5 ms: 1.01x faster                                                  |
| sqlglot_optimize           | 34.0 ms                                                | 33.7 ms: 1.01x faster                                                  |
| xml_etree_parse            | 106 ms                                                 | 105 ms: 1.01x faster                                                   |
| async_tree_io_tg           | 669 ms                                                 | 664 ms: 1.01x faster                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 528 ms: 1.01x faster                                                   |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.11 ms: 1.01x faster                                                  |
| pickle_dict                | 18.1 us                                                | 18.1 us: 1.00x slower                                                  |
| pidigits                   | 282 ms                                                 | 283 ms: 1.00x slower                                                   |
| xml_etree_generate         | 55.8 ms                                                | 56.1 ms: 1.01x slower                                                  |
| sqlite_synth               | 1.57 us                                                | 1.58 us: 1.01x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 72.4 ms: 1.01x slower                                                  |
| float                      | 55.8 ms                                                | 56.4 ms: 1.01x slower                                                  |
| unpickle                   | 9.12 us                                                | 9.23 us: 1.01x slower                                                  |
| coroutines                 | 19.2 ms                                                | 19.5 ms: 1.01x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.26 sec: 1.02x slower                                                 |
| pathlib                    | 24.2 ms                                                | 24.6 ms: 1.02x slower                                                  |
| unpickle_pure_python       | 151 us                                                 | 153 us: 1.02x slower                                                   |
| xml_etree_iterparse        | 74.0 ms                                                | 75.5 ms: 1.02x slower                                                  |
| pycparser                  | 677 ms                                                 | 691 ms: 1.02x slower                                                   |
| unpickle_list              | 3.02 us                                                | 3.09 us: 1.02x slower                                                  |
| go                         | 102 ms                                                 | 105 ms: 1.03x slower                                                   |
| pickle_list                | 2.89 us                                                | 2.97 us: 1.03x slower                                                  |
| pprint_pformat             | 1.01 sec                                               | 1.04 sec: 1.03x slower                                                 |
| pprint_safe_repr           | 497 ms                                                 | 513 ms: 1.03x slower                                                   |
| scimark_fft                | 195 ms                                                 | 203 ms: 1.04x slower                                                   |
| async_tree_io              | 668 ms                                                 | 694 ms: 1.04x slower                                                   |
| richards_super             | 36.0 ms                                                | 37.4 ms: 1.04x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 325 ms: 1.04x slower                                                   |
| chameleon                  | 4.70 ms                                                | 4.89 ms: 1.04x slower                                                  |
| richards                   | 32.1 ms                                                | 33.5 ms: 1.04x slower                                                  |
| json_dumps                 | 6.22 ms                                                | 6.49 ms: 1.04x slower                                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 47.2 ms: 1.05x slower                                                  |
| pyflate                    | 316 ms                                                 | 334 ms: 1.06x slower                                                   |
| regex_v8                   | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                  |
| nbody                      | 68.8 ms                                                | 75.0 ms: 1.09x slower                                                  |
| fannkuch                   | 248 ms                                                 | 271 ms: 1.09x slower                                                   |
| tomli_loads                | 1.39 sec                                               | 1.54 sec: 1.11x slower                                                 |
| python_startup             | 11.4 ms                                                | 13.0 ms: 1.14x slower                                                  |
| scimark_sor                | 87.4 ms                                                | 105 ms: 1.20x slower                                                   |
| telco                      | 3.68 ms                                                | 4.46 ms: 1.21x slower                                                  |
| coverage                   | 38.9 ms                                                | 47.6 ms: 1.22x slower                                                  |
| python_startup_no_site     | 9.37 ms                                                | 11.6 ms: 1.24x slower                                                  |
| mypy2                      | 380 ms                                                 | 511 ms: 1.34x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (12): asyncio_tcp, tornado_http, async_tree_memoization_tg, bench_mp_pool, dask, xml_etree_process, gc_traversal, create_gc_cycles, asyncio_websockets, pickle, async_tree_none_tg, 2to3
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 81.25% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x