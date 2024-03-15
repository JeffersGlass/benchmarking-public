
# Results vs. 3.11.0

- fork: python
- ref: 1ae7ceba29771baf8f2e
- machine: darwin-arm64
- commit hash: 1ae7ceb
- commit date: 2024-01-04
- overall geometric mean: 1.10x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x slower
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 178 ms: 1.15x slower                                                   |
| chameleon      | 4.30 ms                                                | 4.93 ms: 1.15x slower                                                  |
| docutils       | 1.43 sec                                               | 1.53 sec: 1.07x slower                                                 |
| tornado_http   | 69.1 ms                                                | 71.7 ms: 1.04x slower                                                  |
| Geometric mean | (ref)                                                  | 1.10x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 259 ms: 1.09x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 333 ms: 1.06x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 684 ms: 1.06x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 266 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 541 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 531 ms: 1.02x slower                                                   |
| async_tree_io              | 697 ms                                                 | 715 ms: 1.03x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 284 ms: 1.01x slower                                                   |
| float          | 50.8 ms                                                | 70.1 ms: 1.38x slower                                                  |
| nbody          | 61.7 ms                                                | 89.3 ms: 1.45x slower                                                  |
| Geometric mean | (ref)                                                  | 1.26x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 2.43 ms                                                | 2.49 ms: 1.03x slower                                                  |
| regex_v8       | 15.1 ms                                                | 17.0 ms: 1.12x slower                                                  |
| regex_compile  | 72.8 ms                                                | 84.4 ms: 1.16x slower                                                  |
| Geometric mean | (ref)                                                  | 1.07x slower                                                           |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.68 ms: 1.13x faster                                                  |
| pickle_pure_python   | 191 us                                                 | 200 us: 1.05x slower                                                   |
| pickle               | 6.98 us                                                | 7.42 us: 1.06x slower                                                  |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| pickle_list          | 2.70 us                                                | 2.88 us: 1.07x slower                                                  |
| pickle_dict          | 17.1 us                                                | 18.5 us: 1.09x slower                                                  |
| unpickle             | 8.29 us                                                | 9.20 us: 1.11x slower                                                  |
| json_loads           | 15.3 us                                                | 17.3 us: 1.12x slower                                                  |
| unpickle_pure_python | 149 us                                                 | 167 us: 1.13x slower                                                   |
| unpickle_list        | 2.69 us                                                | 3.18 us: 1.18x slower                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 81.2 ms: 1.19x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 41.8 ms: 1.25x slower                                                  |
| xml_etree_generate   | 45.8 ms                                                | 60.1 ms: 1.31x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.69 sec: 1.32x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.13x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.2 ms: 1.23x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 11.8 ms: 1.38x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 9.90 ms: 1.25x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240104-darwin-arm64-python-1ae7ceba29771baf8f2e-3.13.0a2+-1ae7ceb |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 76.3 us: 3.95x faster                                                  |
| asyncio_tcp                | 643 ms                                                 | 431 ms: 1.49x faster                                                   |
| unpack_sequence            | 33.6 ns                                                | 26.4 ns: 1.28x faster                                                  |
| generators                 | 30.3 ms                                                | 24.8 ms: 1.22x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 6.68 ms: 1.13x faster                                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.27 sec: 1.10x faster                                                 |
| raytrace                   | 206 ms                                                 | 188 ms: 1.09x faster                                                   |
| async_tree_none            | 282 ms                                                 | 259 ms: 1.09x faster                                                   |
| sqlglot_parse              | 890 us                                                 | 839 us: 1.06x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 333 ms: 1.06x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 684 ms: 1.06x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 266 ms: 1.04x faster                                                   |
| sqlglot_transpile          | 1.05 ms                                                | 1.03 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 541 ms: 1.02x faster                                                   |
| richards_super             | 37.3 ms                                                | 36.7 ms: 1.02x faster                                                  |
| chaos                      | 47.4 ms                                                | 47.1 ms: 1.01x faster                                                  |
| create_gc_cycles           | 711 us                                                 | 707 us: 1.01x faster                                                   |
| asyncio_websockets         | 408 ms                                                 | 409 ms: 1.00x slower                                                   |
| gc_traversal               | 2.38 ms                                                | 2.41 ms: 1.01x slower                                                  |
| pidigits                   | 280 ms                                                 | 284 ms: 1.01x slower                                                   |
| deepcopy_memo              | 25.7 us                                                | 26.2 us: 1.02x slower                                                  |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 531 ms: 1.02x slower                                                   |
| regex_effbot               | 2.43 ms                                                | 2.49 ms: 1.03x slower                                                  |
| async_tree_io              | 697 ms                                                 | 715 ms: 1.03x slower                                                   |
| sympy_sum                  | 80.2 ms                                                | 82.5 ms: 1.03x slower                                                  |
| tornado_http               | 69.1 ms                                                | 71.7 ms: 1.04x slower                                                  |
| coroutines                 | 17.2 ms                                                | 17.9 ms: 1.04x slower                                                  |
| pickle_pure_python         | 191 us                                                 | 200 us: 1.05x slower                                                   |
| dask                       | 219 ms                                                 | 230 ms: 1.05x slower                                                   |
| go                         | 105 ms                                                 | 111 ms: 1.05x slower                                                   |
| richards                   | 31.1 ms                                                | 32.7 ms: 1.05x slower                                                  |
| sympy_integrate            | 11.3 ms                                                | 11.9 ms: 1.06x slower                                                  |
| dulwich_log                | 28.6 ms                                                | 30.3 ms: 1.06x slower                                                  |
| pickle                     | 6.98 us                                                | 7.42 us: 1.06x slower                                                  |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| pickle_list                | 2.70 us                                                | 2.88 us: 1.07x slower                                                  |
| logging_simple             | 3.41 us                                                | 3.65 us: 1.07x slower                                                  |
| docutils                   | 1.43 sec                                               | 1.53 sec: 1.07x slower                                                 |
| pathlib                    | 23.2 ms                                                | 24.9 ms: 1.07x slower                                                  |
| pycparser                  | 659 ms                                                 | 708 ms: 1.07x slower                                                   |
| logging_format             | 3.67 us                                                | 3.96 us: 1.08x slower                                                  |
| deepcopy                   | 215 us                                                 | 233 us: 1.08x slower                                                   |
| pickle_dict                | 17.1 us                                                | 18.5 us: 1.09x slower                                                  |
| logging_silent             | 66.5 ns                                                | 72.4 ns: 1.09x slower                                                  |
| sympy_str                  | 144 ms                                                 | 156 ms: 1.09x slower                                                   |
| json                       | 2.75 ms                                                | 3.00 ms: 1.09x slower                                                  |
| coverage                   | 43.9 ms                                                | 48.2 ms: 1.10x slower                                                  |
| unpickle                   | 8.29 us                                                | 9.20 us: 1.11x slower                                                  |
| meteor_contest             | 71.1 ms                                                | 79.2 ms: 1.11x slower                                                  |
| comprehensions             | 14.4 us                                                | 16.1 us: 1.12x slower                                                  |
| regex_v8                   | 15.1 ms                                                | 17.0 ms: 1.12x slower                                                  |
| bench_thread_pool          | 465 us                                                 | 521 us: 1.12x slower                                                   |
| json_loads                 | 15.3 us                                                | 17.3 us: 1.12x slower                                                  |
| unpickle_pure_python       | 149 us                                                 | 167 us: 1.13x slower                                                   |
| bench_mp_pool              | 41.0 ms                                                | 46.2 ms: 1.13x slower                                                  |
| sympy_expand               | 229 ms                                                 | 259 ms: 1.13x slower                                                   |
| chameleon                  | 4.30 ms                                                | 4.93 ms: 1.15x slower                                                  |
| 2to3                       | 154 ms                                                 | 178 ms: 1.15x slower                                                   |
| deepcopy_reduce            | 1.79 us                                                | 2.08 us: 1.16x slower                                                  |
| regex_compile              | 72.8 ms                                                | 84.4 ms: 1.16x slower                                                  |
| scimark_lu                 | 67.7 ms                                                | 78.6 ms: 1.16x slower                                                  |
| crypto_pyaes               | 47.5 ms                                                | 55.7 ms: 1.17x slower                                                  |
| mdp                        | 1.48 sec                                               | 1.74 sec: 1.17x slower                                                 |
| unpickle_list              | 2.69 us                                                | 3.18 us: 1.18x slower                                                  |
| xml_etree_iterparse        | 68.3 ms                                                | 81.2 ms: 1.19x slower                                                  |
| sqlglot_normalize          | 162 ms                                                 | 196 ms: 1.21x slower                                                   |
| pprint_safe_repr           | 478 ms                                                 | 583 ms: 1.22x slower                                                   |
| pprint_pformat             | 979 ms                                                 | 1.20 sec: 1.22x slower                                                 |
| python_startup             | 10.8 ms                                                | 13.2 ms: 1.23x slower                                                  |
| nqueens                    | 55.9 ms                                                | 68.8 ms: 1.23x slower                                                  |
| xml_etree_process          | 33.6 ms                                                | 41.8 ms: 1.25x slower                                                  |
| mako                       | 7.93 ms                                                | 9.90 ms: 1.25x slower                                                  |
| sqlglot_optimize           | 29.6 ms                                                | 37.2 ms: 1.26x slower                                                  |
| hexiom                     | 4.58 ms                                                | 5.96 ms: 1.30x slower                                                  |
| xml_etree_generate         | 45.8 ms                                                | 60.1 ms: 1.31x slower                                                  |
| pyflate                    | 284 ms                                                 | 374 ms: 1.32x slower                                                   |
| deltablue                  | 2.75 ms                                                | 3.64 ms: 1.32x slower                                                  |
| tomli_loads                | 1.27 sec                                               | 1.69 sec: 1.32x slower                                                 |
| scimark_monte_carlo        | 43.5 ms                                                | 58.0 ms: 1.33x slower                                                  |
| sqlite_synth               | 1.26 us                                                | 1.71 us: 1.36x slower                                                  |
| scimark_sor                | 79.2 ms                                                | 109 ms: 1.37x slower                                                   |
| python_startup_no_site     | 8.57 ms                                                | 11.8 ms: 1.38x slower                                                  |
| float                      | 50.8 ms                                                | 70.1 ms: 1.38x slower                                                  |
| fannkuch                   | 240 ms                                                 | 341 ms: 1.42x slower                                                   |
| mypy2                      | 372 ms                                                 | 533 ms: 1.43x slower                                                   |
| nbody                      | 61.7 ms                                                | 89.3 ms: 1.45x slower                                                  |
| scimark_fft                | 173 ms                                                 | 257 ms: 1.49x slower                                                   |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 4.30 ms: 1.53x slower                                                  |
| telco                      | 3.17 ms                                                | 4.96 ms: 1.57x slower                                                  |
| async_generators           | 192 ms                                                 | 305 ms: 1.59x slower                                                   |
| spectral_norm              | 65.7 ms                                                | 110 ms: 1.68x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.10x slower                                                           |

Benchmark hidden because not significant (2): regex_dna, async_tree_memoization
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.07x
- 95% likely to have a slowdown of 1.06x
- 99% likely to have a slowdown of 1.05x


# Memory

- memory change: 1.03x