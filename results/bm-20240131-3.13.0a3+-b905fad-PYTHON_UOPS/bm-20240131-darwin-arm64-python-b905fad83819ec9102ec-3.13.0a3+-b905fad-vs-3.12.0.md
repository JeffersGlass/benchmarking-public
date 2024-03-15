
# Results vs. 3.12.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: darwin-arm64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 174 ms: 1.03x slower                                                   |
| chameleon      | 4.70 ms                                                | 4.95 ms: 1.05x slower                                                  |
| docutils       | 1.50 sec                                               | 1.50 sec: 1.00x faster                                                 |
| Geometric mean | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none           | 266 ms                                                 | 258 ms: 1.03x faster                                                   |
| async_tree_io_tg          | 669 ms                                                 | 676 ms: 1.01x slower                                                   |
| async_tree_memoization_tg | 323 ms                                                 | 330 ms: 1.02x slower                                                   |
| async_tree_none_tg        | 258 ms                                                 | 266 ms: 1.03x slower                                                   |
| async_tree_io             | 668 ms                                                 | 706 ms: 1.06x slower                                                   |
| async_tree_memoization    | 312 ms                                                 | 333 ms: 1.07x slower                                                   |
| Geometric mean            | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 283 ms: 1.01x slower                                                   |
| float          | 55.8 ms                                                | 68.3 ms: 1.22x slower                                                  |
| nbody          | 68.8 ms                                                | 85.3 ms: 1.24x slower                                                  |
| Geometric mean | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.56 ms: 1.03x faster                                                  |
| regex_dna      | 154 ms                                                 | 152 ms: 1.02x faster                                                   |
| regex_compile  | 77.9 ms                                                | 81.7 ms: 1.05x slower                                                  |
| regex_v8       | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_loads           | 17.2 us                                                | 17.0 us: 1.01x faster                                                  |
| pickle_pure_python   | 200 us                                                 | 198 us: 1.01x faster                                                   |
| pickle_dict          | 18.1 us                                                | 18.2 us: 1.01x slower                                                  |
| unpickle_list        | 3.02 us                                                | 3.08 us: 1.02x slower                                                  |
| xml_etree_process    | 39.7 ms                                                | 41.0 ms: 1.03x slower                                                  |
| pickle_list          | 2.89 us                                                | 2.99 us: 1.04x slower                                                  |
| xml_etree_generate   | 55.8 ms                                                | 58.8 ms: 1.05x slower                                                  |
| json_dumps           | 6.22 ms                                                | 6.57 ms: 1.06x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 163 us: 1.08x slower                                                   |
| xml_etree_iterparse  | 74.0 ms                                                | 80.5 ms: 1.09x slower                                                  |
| tomli_loads          | 1.39 sec                                               | 1.64 sec: 1.18x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.04x slower                                                           |

Benchmark hidden because not significant (3): pickle, unpickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 13.2 ms: 1.15x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 11.8 ms: 1.26x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.20x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 9.66 ms: 1.25x slower                                                  |

All benchmarks:
===============

| Benchmark                 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols  | 93.0 us                                                | 73.2 us: 1.27x faster                                                  |
| raytrace                  | 212 ms                                                 | 185 ms: 1.14x faster                                                   |
| generators                | 31.1 ms                                                | 28.7 ms: 1.08x faster                                                  |
| unpack_sequence           | 31.5 ns                                                | 29.1 ns: 1.08x faster                                                  |
| logging_silent            | 76.4 ns                                                | 71.3 ns: 1.07x faster                                                  |
| json                      | 3.09 ms                                                | 2.94 ms: 1.05x faster                                                  |
| sqlglot_parse             | 848 us                                                 | 813 us: 1.04x faster                                                   |
| logging_simple            | 3.69 us                                                | 3.56 us: 1.03x faster                                                  |
| deepcopy_memo             | 27.7 us                                                | 26.7 us: 1.03x faster                                                  |
| deepcopy                  | 235 us                                                 | 227 us: 1.03x faster                                                   |
| deepcopy_reduce           | 2.07 us                                                | 2.00 us: 1.03x faster                                                  |
| regex_effbot              | 2.64 ms                                                | 2.56 ms: 1.03x faster                                                  |
| async_tree_none           | 266 ms                                                 | 258 ms: 1.03x faster                                                   |
| logging_format            | 3.98 us                                                | 3.88 us: 1.03x faster                                                  |
| sqlglot_transpile         | 1.02 ms                                                | 998 us: 1.02x faster                                                   |
| async_generators          | 304 ms                                                 | 297 ms: 1.02x faster                                                   |
| regex_dna                 | 154 ms                                                 | 152 ms: 1.02x faster                                                   |
| json_loads                | 17.2 us                                                | 17.0 us: 1.01x faster                                                  |
| pickle_pure_python        | 200 us                                                 | 198 us: 1.01x faster                                                   |
| docutils                  | 1.50 sec                                               | 1.50 sec: 1.00x faster                                                 |
| asyncio_websockets        | 409 ms                                                 | 409 ms: 1.00x faster                                                   |
| create_gc_cycles          | 701 us                                                 | 704 us: 1.00x slower                                                   |
| pidigits                  | 282 ms                                                 | 283 ms: 1.01x slower                                                   |
| pickle_dict               | 18.1 us                                                | 18.2 us: 1.01x slower                                                  |
| dulwich_log               | 29.8 ms                                                | 30.1 ms: 1.01x slower                                                  |
| scimark_lu                | 76.0 ms                                                | 76.8 ms: 1.01x slower                                                  |
| async_tree_io_tg          | 669 ms                                                 | 676 ms: 1.01x slower                                                   |
| sympy_integrate           | 11.4 ms                                                | 11.5 ms: 1.01x slower                                                  |
| sympy_expand              | 241 ms                                                 | 244 ms: 1.01x slower                                                   |
| bench_thread_pool         | 504 us                                                 | 511 us: 1.01x slower                                                   |
| pathlib                   | 24.2 ms                                                | 24.6 ms: 1.02x slower                                                  |
| sympy_sum                 | 77.6 ms                                                | 79.1 ms: 1.02x slower                                                  |
| unpickle_list             | 3.02 us                                                | 3.08 us: 1.02x slower                                                  |
| mdp                       | 1.58 sec                                               | 1.62 sec: 1.02x slower                                                 |
| async_tree_memoization_tg | 323 ms                                                 | 330 ms: 1.02x slower                                                   |
| asyncio_tcp_ssl           | 1.24 sec                                               | 1.27 sec: 1.02x slower                                                 |
| coroutines                | 19.2 ms                                                | 19.7 ms: 1.02x slower                                                  |
| sqlglot_normalize         | 186 ms                                                 | 190 ms: 1.03x slower                                                   |
| richards_super            | 36.0 ms                                                | 37.0 ms: 1.03x slower                                                  |
| richards                  | 32.1 ms                                                | 33.0 ms: 1.03x slower                                                  |
| 2to3                      | 169 ms                                                 | 174 ms: 1.03x slower                                                   |
| async_tree_none_tg        | 258 ms                                                 | 266 ms: 1.03x slower                                                   |
| xml_etree_process         | 39.7 ms                                                | 41.0 ms: 1.03x slower                                                  |
| pickle_list               | 2.89 us                                                | 2.99 us: 1.04x slower                                                  |
| pycparser                 | 677 ms                                                 | 702 ms: 1.04x slower                                                   |
| crypto_pyaes              | 51.9 ms                                                | 54.0 ms: 1.04x slower                                                  |
| sqlite_synth              | 1.57 us                                                | 1.64 us: 1.05x slower                                                  |
| comprehensions            | 14.5 us                                                | 15.2 us: 1.05x slower                                                  |
| regex_compile             | 77.9 ms                                                | 81.7 ms: 1.05x slower                                                  |
| sqlglot_optimize          | 34.0 ms                                                | 35.8 ms: 1.05x slower                                                  |
| xml_etree_generate        | 55.8 ms                                                | 58.8 ms: 1.05x slower                                                  |
| chameleon                 | 4.70 ms                                                | 4.95 ms: 1.05x slower                                                  |
| json_dumps                | 6.22 ms                                                | 6.57 ms: 1.06x slower                                                  |
| async_tree_io             | 668 ms                                                 | 706 ms: 1.06x slower                                                   |
| async_tree_memoization    | 312 ms                                                 | 333 ms: 1.07x slower                                                   |
| regex_v8                  | 16.0 ms                                                | 17.1 ms: 1.07x slower                                                  |
| meteor_contest            | 71.7 ms                                                | 77.2 ms: 1.08x slower                                                  |
| chaos                     | 42.5 ms                                                | 45.9 ms: 1.08x slower                                                  |
| unpickle_pure_python      | 151 us                                                 | 163 us: 1.08x slower                                                   |
| xml_etree_iterparse       | 74.0 ms                                                | 80.5 ms: 1.09x slower                                                  |
| nqueens                   | 62.4 ms                                                | 67.9 ms: 1.09x slower                                                  |
| go                        | 102 ms                                                 | 111 ms: 1.09x slower                                                   |
| pprint_safe_repr          | 497 ms                                                 | 568 ms: 1.14x slower                                                   |
| pprint_pformat            | 1.01 sec                                               | 1.16 sec: 1.15x slower                                                 |
| python_startup            | 11.4 ms                                                | 13.2 ms: 1.15x slower                                                  |
| pyflate                   | 316 ms                                                 | 366 ms: 1.16x slower                                                   |
| tomli_loads               | 1.39 sec                                               | 1.64 sec: 1.18x slower                                                 |
| coverage                  | 38.9 ms                                                | 47.1 ms: 1.21x slower                                                  |
| scimark_sor               | 87.4 ms                                                | 106 ms: 1.21x slower                                                   |
| float                     | 55.8 ms                                                | 68.3 ms: 1.22x slower                                                  |
| nbody                     | 68.8 ms                                                | 85.3 ms: 1.24x slower                                                  |
| scimark_monte_carlo       | 45.0 ms                                                | 56.0 ms: 1.24x slower                                                  |
| scimark_fft               | 195 ms                                                 | 244 ms: 1.25x slower                                                   |
| mako                      | 7.71 ms                                                | 9.66 ms: 1.25x slower                                                  |
| python_startup_no_site    | 9.37 ms                                                | 11.8 ms: 1.26x slower                                                  |
| telco                     | 3.68 ms                                                | 4.70 ms: 1.28x slower                                                  |
| fannkuch                  | 248 ms                                                 | 319 ms: 1.28x slower                                                   |
| hexiom                    | 4.54 ms                                                | 5.85 ms: 1.29x slower                                                  |
| deltablue                 | 2.71 ms                                                | 3.53 ms: 1.30x slower                                                  |
| scimark_sparse_mat_mult   | 3.14 ms                                                | 4.09 ms: 1.31x slower                                                  |
| spectral_norm             | 76.4 ms                                                | 101 ms: 1.32x slower                                                   |
| mypy2                     | 380 ms                                                 | 524 ms: 1.38x slower                                                   |
| Geometric mean            | (ref)                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (11): asyncio_tcp, sympy_str, pickle, gc_traversal, async_tree_cpu_io_mixed, unpickle, async_tree_cpu_io_mixed_tg, tornado_http, xml_etree_parse, dask, bench_mp_pool
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.00x