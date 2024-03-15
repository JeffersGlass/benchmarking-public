# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_jumps
- machine: darwin-arm64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.08x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 188 ms: 1.22x slower                                                 |
| chameleon      | 4.30 ms                                                | 4.85 ms: 1.13x slower                                                |
| docutils       | 1.43 sec                                               | 1.53 sec: 1.07x slower                                               |
| Geometric mean | (ref)                                                  | 1.10x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 251 ms: 1.12x faster                                                 |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                                 |
| async_tree_io_tg           | 724 ms                                                 | 668 ms: 1.08x faster                                                 |
| async_tree_none_tg         | 276 ms                                                 | 259 ms: 1.07x faster                                                 |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 532 ms: 1.03x faster                                                 |
| async_tree_memoization     | 336 ms                                                 | 327 ms: 1.03x faster                                                 |
| async_tree_io              | 697 ms                                                 | 701 ms: 1.01x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                         |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.01x slower                                                 |
| float          | 50.8 ms                                                | 53.0 ms: 1.04x slower                                                |
| nbody          | 61.7 ms                                                | 70.6 ms: 1.14x slower                                                |
| Geometric mean | (ref)                                                  | 1.06x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 152 ms: 1.03x slower                                                 |
| regex_effbot   | 2.43 ms                                                | 2.63 ms: 1.08x slower                                                |
| regex_v8       | 15.1 ms                                                | 17.2 ms: 1.14x slower                                                |
| regex_compile  | 72.8 ms                                                | 86.7 ms: 1.19x slower                                                |
| Geometric mean | (ref)                                                  | 1.11x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.54 ms: 1.15x faster                                                |
| unpickle_pure_python | 149 us                                                 | 152 us: 1.02x slower                                                 |
| pickle_pure_python   | 191 us                                                 | 197 us: 1.03x slower                                                 |
| pickle               | 6.98 us                                                | 7.25 us: 1.04x slower                                                |
| pickle_dict          | 17.1 us                                                | 18.3 us: 1.07x slower                                                |
| xml_etree_parse      | 100 ms                                                 | 108 ms: 1.07x slower                                                 |
| tomli_loads          | 1.27 sec                                               | 1.38 sec: 1.08x slower                                               |
| pickle_list          | 2.70 us                                                | 2.96 us: 1.10x slower                                                |
| xml_etree_iterparse  | 68.3 ms                                                | 75.0 ms: 1.10x slower                                                |
| json_loads           | 15.3 us                                                | 16.9 us: 1.10x slower                                                |
| unpickle             | 8.29 us                                                | 9.15 us: 1.10x slower                                                |
| unpickle_list        | 2.69 us                                                | 3.07 us: 1.14x slower                                                |
| xml_etree_process    | 33.6 ms                                                | 39.0 ms: 1.16x slower                                                |
| xml_etree_generate   | 45.8 ms                                                | 57.8 ms: 1.26x slower                                                |
| Geometric mean       | (ref)                                                  | 1.08x slower                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 17.3 ms: 1.61x slower                                                |
| python_startup_no_site | 8.57 ms                                                | 15.9 ms: 1.85x slower                                                |
| Geometric mean         | (ref)                                                  | 1.73x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 6.85 ms: 1.16x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 72.1 us: 4.17x faster                                                |
| asyncio_tcp                | 643 ms                                                 | 407 ms: 1.58x faster                                                 |
| chaos                      | 47.4 ms                                                | 40.4 ms: 1.17x faster                                                |
| mako                       | 7.93 ms                                                | 6.85 ms: 1.16x faster                                                |
| json_dumps                 | 7.53 ms                                                | 6.54 ms: 1.15x faster                                                |
| async_tree_none            | 282 ms                                                 | 251 ms: 1.12x faster                                                 |
| comprehensions             | 14.4 us                                                | 13.0 us: 1.12x faster                                                |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                                 |
| async_tree_io_tg           | 724 ms                                                 | 668 ms: 1.08x faster                                                 |
| deltablue                  | 2.75 ms                                                | 2.54 ms: 1.08x faster                                                |
| raytrace                   | 206 ms                                                 | 192 ms: 1.07x faster                                                 |
| async_tree_none_tg         | 276 ms                                                 | 259 ms: 1.07x faster                                                 |
| generators                 | 30.3 ms                                                | 28.4 ms: 1.07x faster                                                |
| sqlglot_parse              | 890 us                                                 | 836 us: 1.06x faster                                                 |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.31 sec: 1.06x faster                                               |
| sympy_sum                  | 80.2 ms                                                | 77.4 ms: 1.04x faster                                                |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 532 ms: 1.03x faster                                                 |
| async_tree_memoization     | 336 ms                                                 | 327 ms: 1.03x faster                                                 |
| sqlglot_transpile          | 1.05 ms                                                | 1.03 ms: 1.02x faster                                                |
| asyncio_websockets         | 408 ms                                                 | 409 ms: 1.00x slower                                                 |
| async_tree_io              | 697 ms                                                 | 701 ms: 1.01x slower                                                 |
| pidigits                   | 280 ms                                                 | 282 ms: 1.01x slower                                                 |
| gc_traversal               | 2.38 ms                                                | 2.41 ms: 1.01x slower                                                |
| sympy_str                  | 144 ms                                                 | 146 ms: 1.01x slower                                                 |
| unpickle_pure_python       | 149 us                                                 | 152 us: 1.02x slower                                                 |
| sympy_integrate            | 11.3 ms                                                | 11.5 ms: 1.02x slower                                                |
| logging_simple             | 3.41 us                                                | 3.49 us: 1.02x slower                                                |
| pickle_pure_python         | 191 us                                                 | 197 us: 1.03x slower                                                 |
| regex_dna                  | 148 ms                                                 | 152 ms: 1.03x slower                                                 |
| logging_format             | 3.67 us                                                | 3.79 us: 1.03x slower                                                |
| deepcopy_memo              | 25.7 us                                                | 26.6 us: 1.03x slower                                                |
| pickle                     | 6.98 us                                                | 7.25 us: 1.04x slower                                                |
| float                      | 50.8 ms                                                | 53.0 ms: 1.04x slower                                                |
| meteor_contest             | 71.1 ms                                                | 74.5 ms: 1.05x slower                                                |
| scimark_monte_carlo        | 43.5 ms                                                | 46.0 ms: 1.06x slower                                                |
| deepcopy                   | 215 us                                                 | 228 us: 1.06x slower                                                 |
| docutils                   | 1.43 sec                                               | 1.53 sec: 1.07x slower                                               |
| pickle_dict                | 17.1 us                                                | 18.3 us: 1.07x slower                                                |
| xml_etree_parse            | 100 ms                                                 | 108 ms: 1.07x slower                                                 |
| json                       | 2.75 ms                                                | 2.96 ms: 1.07x slower                                                |
| sympy_expand               | 229 ms                                                 | 247 ms: 1.08x slower                                                 |
| pprint_safe_repr           | 478 ms                                                 | 517 ms: 1.08x slower                                                 |
| regex_effbot               | 2.43 ms                                                | 2.63 ms: 1.08x slower                                                |
| pprint_pformat             | 979 ms                                                 | 1.06 sec: 1.08x slower                                               |
| pathlib                    | 23.2 ms                                                | 25.2 ms: 1.08x slower                                                |
| tomli_loads                | 1.27 sec                                               | 1.38 sec: 1.08x slower                                               |
| coroutines                 | 17.2 ms                                                | 18.6 ms: 1.09x slower                                                |
| dulwich_log                | 28.6 ms                                                | 31.1 ms: 1.09x slower                                                |
| logging_silent             | 66.5 ns                                                | 72.6 ns: 1.09x slower                                                |
| bench_thread_pool          | 465 us                                                 | 510 us: 1.10x slower                                                 |
| pickle_list                | 2.70 us                                                | 2.96 us: 1.10x slower                                                |
| pycparser                  | 659 ms                                                 | 724 ms: 1.10x slower                                                 |
| go                         | 105 ms                                                 | 116 ms: 1.10x slower                                                 |
| xml_etree_iterparse        | 68.3 ms                                                | 75.0 ms: 1.10x slower                                                |
| mdp                        | 1.48 sec                                               | 1.64 sec: 1.10x slower                                               |
| json_loads                 | 15.3 us                                                | 16.9 us: 1.10x slower                                                |
| unpickle                   | 8.29 us                                                | 9.15 us: 1.10x slower                                                |
| coverage                   | 43.9 ms                                                | 48.5 ms: 1.11x slower                                                |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.14 ms: 1.12x slower                                                |
| deepcopy_reduce            | 1.79 us                                                | 2.00 us: 1.12x slower                                                |
| chameleon                  | 4.30 ms                                                | 4.85 ms: 1.13x slower                                                |
| regex_v8                   | 15.1 ms                                                | 17.2 ms: 1.14x slower                                                |
| sqlglot_normalize          | 162 ms                                                 | 184 ms: 1.14x slower                                                 |
| unpickle_list              | 2.69 us                                                | 3.07 us: 1.14x slower                                                |
| nbody                      | 61.7 ms                                                | 70.6 ms: 1.14x slower                                                |
| hexiom                     | 4.58 ms                                                | 5.32 ms: 1.16x slower                                                |
| scimark_fft                | 173 ms                                                 | 201 ms: 1.16x slower                                                 |
| xml_etree_process          | 33.6 ms                                                | 39.0 ms: 1.16x slower                                                |
| nqueens                    | 55.9 ms                                                | 65.0 ms: 1.16x slower                                                |
| richards_super             | 37.3 ms                                                | 43.8 ms: 1.17x slower                                                |
| regex_compile              | 72.8 ms                                                | 86.7 ms: 1.19x slower                                                |
| sqlglot_optimize           | 29.6 ms                                                | 35.6 ms: 1.20x slower                                                |
| 2to3                       | 154 ms                                                 | 188 ms: 1.22x slower                                                 |
| pyflate                    | 284 ms                                                 | 346 ms: 1.22x slower                                                 |
| spectral_norm              | 65.7 ms                                                | 80.2 ms: 1.22x slower                                                |
| xml_etree_generate         | 45.8 ms                                                | 57.8 ms: 1.26x slower                                                |
| scimark_lu                 | 67.7 ms                                                | 85.7 ms: 1.26x slower                                                |
| sqlite_synth               | 1.26 us                                                | 1.59 us: 1.27x slower                                                |
| bench_mp_pool              | 41.0 ms                                                | 52.0 ms: 1.27x slower                                                |
| richards                   | 31.1 ms                                                | 39.8 ms: 1.28x slower                                                |
| fannkuch                   | 240 ms                                                 | 316 ms: 1.32x slower                                                 |
| telco                      | 3.17 ms                                                | 4.48 ms: 1.41x slower                                                |
| scimark_sor                | 79.2 ms                                                | 116 ms: 1.46x slower                                                 |
| mypy2                      | 372 ms                                                 | 587 ms: 1.57x slower                                                 |
| async_generators           | 192 ms                                                 | 309 ms: 1.61x slower                                                 |
| python_startup             | 10.8 ms                                                | 17.3 ms: 1.61x slower                                                |
| python_startup_no_site     | 8.57 ms                                                | 15.9 ms: 1.85x slower                                                |
| unpack_sequence            | 33.6 ns                                                | 113 ns: 3.37x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                         |

Benchmark hidden because not significant (4): crypto_pyaes, create_gc_cycles, async_tree_cpu_io_mixed, tornado_http
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.90x