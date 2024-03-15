# Results vs. 3.11.0

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: darwin-arm64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.08x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 187 ms: 1.21x slower                                                   |
| chameleon      | 4.30 ms                                                | 4.84 ms: 1.13x slower                                                  |
| docutils       | 1.43 sec                                               | 1.51 sec: 1.06x slower                                                 |
| Geometric mean | (ref)                                                  | 1.10x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.10x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 670 ms: 1.08x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 259 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 530 ms: 1.04x faster                                                   |
| async_tree_io              | 697 ms                                                 | 701 ms: 1.01x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                           |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.00x slower                                                   |
| float          | 50.8 ms                                                | 52.9 ms: 1.04x slower                                                  |
| nbody          | 61.7 ms                                                | 70.0 ms: 1.14x slower                                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 145 ms: 1.02x faster                                                   |
| regex_effbot   | 2.43 ms                                                | 2.58 ms: 1.06x slower                                                  |
| regex_v8       | 15.1 ms                                                | 17.1 ms: 1.13x slower                                                  |
| regex_compile  | 72.8 ms                                                | 87.1 ms: 1.20x slower                                                  |
| Geometric mean | (ref)                                                  | 1.09x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.56 ms: 1.15x faster                                                  |
| unpickle_pure_python | 149 us                                                 | 152 us: 1.02x slower                                                   |
| pickle_pure_python   | 191 us                                                 | 196 us: 1.03x slower                                                   |
| pickle               | 6.98 us                                                | 7.27 us: 1.04x slower                                                  |
| pickle_dict          | 17.1 us                                                | 18.1 us: 1.06x slower                                                  |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| pickle_list          | 2.70 us                                                | 2.91 us: 1.08x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.39 sec: 1.09x slower                                                 |
| json_loads           | 15.3 us                                                | 16.9 us: 1.10x slower                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 75.4 ms: 1.10x slower                                                  |
| unpickle             | 8.29 us                                                | 9.19 us: 1.11x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.06 us: 1.14x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 40.0 ms: 1.19x slower                                                  |
| xml_etree_generate   | 45.8 ms                                                | 56.7 ms: 1.24x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.08x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 17.7 ms: 1.65x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 16.4 ms: 1.92x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.78x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 6.83 ms: 1.16x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 71.8 us: 4.19x faster                                                  |
| asyncio_tcp                | 643 ms                                                 | 399 ms: 1.61x faster                                                   |
| chaos                      | 47.4 ms                                                | 40.3 ms: 1.18x faster                                                  |
| mako                       | 7.93 ms                                                | 6.83 ms: 1.16x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 6.56 ms: 1.15x faster                                                  |
| comprehensions             | 14.4 us                                                | 12.9 us: 1.12x faster                                                  |
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.10x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 670 ms: 1.08x faster                                                   |
| deltablue                  | 2.75 ms                                                | 2.55 ms: 1.08x faster                                                  |
| raytrace                   | 206 ms                                                 | 191 ms: 1.08x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 259 ms: 1.07x faster                                                   |
| sqlglot_parse              | 890 us                                                 | 834 us: 1.07x faster                                                   |
| generators                 | 30.3 ms                                                | 28.5 ms: 1.06x faster                                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.32 sec: 1.06x faster                                                 |
| sympy_sum                  | 80.2 ms                                                | 77.1 ms: 1.04x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 530 ms: 1.04x faster                                                   |
| sqlglot_transpile          | 1.05 ms                                                | 1.03 ms: 1.03x faster                                                  |
| regex_dna                  | 148 ms                                                 | 145 ms: 1.02x faster                                                   |
| crypto_pyaes               | 47.5 ms                                                | 47.3 ms: 1.00x faster                                                  |
| create_gc_cycles           | 711 us                                                 | 713 us: 1.00x slower                                                   |
| pidigits                   | 280 ms                                                 | 282 ms: 1.00x slower                                                   |
| async_tree_io              | 697 ms                                                 | 701 ms: 1.01x slower                                                   |
| sympy_str                  | 144 ms                                                 | 145 ms: 1.01x slower                                                   |
| gc_traversal               | 2.38 ms                                                | 2.41 ms: 1.01x slower                                                  |
| sympy_integrate            | 11.3 ms                                                | 11.5 ms: 1.02x slower                                                  |
| unpickle_pure_python       | 149 us                                                 | 152 us: 1.02x slower                                                   |
| logging_simple             | 3.41 us                                                | 3.49 us: 1.02x slower                                                  |
| pickle_pure_python         | 191 us                                                 | 196 us: 1.03x slower                                                   |
| logging_format             | 3.67 us                                                | 3.77 us: 1.03x slower                                                  |
| deepcopy_memo              | 25.7 us                                                | 26.6 us: 1.03x slower                                                  |
| float                      | 50.8 ms                                                | 52.9 ms: 1.04x slower                                                  |
| meteor_contest             | 71.1 ms                                                | 74.1 ms: 1.04x slower                                                  |
| pickle                     | 6.98 us                                                | 7.27 us: 1.04x slower                                                  |
| pickle_dict                | 17.1 us                                                | 18.1 us: 1.06x slower                                                  |
| docutils                   | 1.43 sec                                               | 1.51 sec: 1.06x slower                                                 |
| scimark_monte_carlo        | 43.5 ms                                                | 46.1 ms: 1.06x slower                                                  |
| regex_effbot               | 2.43 ms                                                | 2.58 ms: 1.06x slower                                                  |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| deepcopy                   | 215 us                                                 | 231 us: 1.07x slower                                                   |
| dulwich_log                | 28.6 ms                                                | 30.9 ms: 1.08x slower                                                  |
| json                       | 2.75 ms                                                | 2.97 ms: 1.08x slower                                                  |
| pickle_list                | 2.70 us                                                | 2.91 us: 1.08x slower                                                  |
| sympy_expand               | 229 ms                                                 | 248 ms: 1.08x slower                                                   |
| pprint_safe_repr           | 478 ms                                                 | 517 ms: 1.08x slower                                                   |
| pprint_pformat             | 979 ms                                                 | 1.06 sec: 1.09x slower                                                 |
| coverage                   | 43.9 ms                                                | 47.7 ms: 1.09x slower                                                  |
| tomli_loads                | 1.27 sec                                               | 1.39 sec: 1.09x slower                                                 |
| logging_silent             | 66.5 ns                                                | 72.5 ns: 1.09x slower                                                  |
| coroutines                 | 17.2 ms                                                | 18.7 ms: 1.09x slower                                                  |
| pathlib                    | 23.2 ms                                                | 25.4 ms: 1.09x slower                                                  |
| go                         | 105 ms                                                 | 116 ms: 1.10x slower                                                   |
| mdp                        | 1.48 sec                                               | 1.63 sec: 1.10x slower                                                 |
| json_loads                 | 15.3 us                                                | 16.9 us: 1.10x slower                                                  |
| pycparser                  | 659 ms                                                 | 727 ms: 1.10x slower                                                   |
| xml_etree_iterparse        | 68.3 ms                                                | 75.4 ms: 1.10x slower                                                  |
| bench_thread_pool          | 465 us                                                 | 514 us: 1.10x slower                                                   |
| unpickle                   | 8.29 us                                                | 9.19 us: 1.11x slower                                                  |
| deepcopy_reduce            | 1.79 us                                                | 2.00 us: 1.11x slower                                                  |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.14 ms: 1.11x slower                                                  |
| chameleon                  | 4.30 ms                                                | 4.84 ms: 1.13x slower                                                  |
| regex_v8                   | 15.1 ms                                                | 17.1 ms: 1.13x slower                                                  |
| nbody                      | 61.7 ms                                                | 70.0 ms: 1.14x slower                                                  |
| sqlglot_normalize          | 162 ms                                                 | 184 ms: 1.14x slower                                                   |
| nqueens                    | 55.9 ms                                                | 63.7 ms: 1.14x slower                                                  |
| unpickle_list              | 2.69 us                                                | 3.06 us: 1.14x slower                                                  |
| scimark_fft                | 173 ms                                                 | 199 ms: 1.15x slower                                                   |
| richards_super             | 37.3 ms                                                | 43.4 ms: 1.16x slower                                                  |
| hexiom                     | 4.58 ms                                                | 5.33 ms: 1.16x slower                                                  |
| xml_etree_process          | 33.6 ms                                                | 40.0 ms: 1.19x slower                                                  |
| regex_compile              | 72.8 ms                                                | 87.1 ms: 1.20x slower                                                  |
| sqlglot_optimize           | 29.6 ms                                                | 35.5 ms: 1.20x slower                                                  |
| 2to3                       | 154 ms                                                 | 187 ms: 1.21x slower                                                   |
| pyflate                    | 284 ms                                                 | 346 ms: 1.22x slower                                                   |
| xml_etree_generate         | 45.8 ms                                                | 56.7 ms: 1.24x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 81.7 ms: 1.24x slower                                                  |
| scimark_lu                 | 67.7 ms                                                | 85.6 ms: 1.26x slower                                                  |
| bench_mp_pool              | 41.0 ms                                                | 52.2 ms: 1.28x slower                                                  |
| sqlite_synth               | 1.26 us                                                | 1.61 us: 1.28x slower                                                  |
| richards                   | 31.1 ms                                                | 40.4 ms: 1.30x slower                                                  |
| fannkuch                   | 240 ms                                                 | 325 ms: 1.36x slower                                                   |
| telco                      | 3.17 ms                                                | 4.48 ms: 1.42x slower                                                  |
| mypy2                      | 372 ms                                                 | 537 ms: 1.44x slower                                                   |
| scimark_sor                | 79.2 ms                                                | 115 ms: 1.45x slower                                                   |
| async_generators           | 192 ms                                                 | 311 ms: 1.62x slower                                                   |
| python_startup             | 10.8 ms                                                | 17.7 ms: 1.65x slower                                                  |
| python_startup_no_site     | 8.57 ms                                                | 16.4 ms: 1.92x slower                                                  |
| unpack_sequence            | 33.6 ns                                                | 114 ns: 3.37x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                           |

Benchmark hidden because not significant (4): async_tree_memoization, asyncio_websockets, async_tree_cpu_io_mixed, tornado_http
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.90x