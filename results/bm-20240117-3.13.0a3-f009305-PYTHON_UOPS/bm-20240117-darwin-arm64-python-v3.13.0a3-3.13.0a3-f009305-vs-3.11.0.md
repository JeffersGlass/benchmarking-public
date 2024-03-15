
# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a3
- machine: darwin-arm64
- commit hash: f009305
- commit date: 2024-01-17
- overall geometric mean: 1.09x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x slower
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-darwin-arm64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 173 ms: 1.12x slower                                       |
| chameleon      | 4.30 ms                                                | 5.03 ms: 1.17x slower                                      |
| docutils       | 1.43 sec                                               | 1.50 sec: 1.05x slower                                     |
| Geometric mean | (ref)                                                  | 1.09x slower                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-darwin-arm64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 261 ms: 1.08x faster                                       |
| async_tree_io_tg           | 724 ms                                                 | 682 ms: 1.06x faster                                       |
| async_tree_memoization_tg  | 352 ms                                                 | 335 ms: 1.05x faster                                       |
| async_tree_none_tg         | 276 ms                                                 | 267 ms: 1.03x faster                                       |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 538 ms: 1.02x faster                                       |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 530 ms: 1.02x slower                                       |
| async_tree_io              | 697 ms                                                 | 715 ms: 1.03x slower                                       |
| Geometric mean             | (ref)                                                  | 1.02x faster                                               |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-darwin-arm64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 284 ms: 1.01x slower                                       |
| float          | 50.8 ms                                                | 68.9 ms: 1.36x slower                                      |
| nbody          | 61.7 ms                                                | 86.4 ms: 1.40x slower                                      |
| Geometric mean | (ref)                                                  | 1.24x slower                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-darwin-arm64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 156 ms: 1.05x slower                                       |
| regex_compile  | 72.8 ms                                                | 82.6 ms: 1.13x slower                                      |
| regex_effbot   | 2.43 ms                                                | 2.77 ms: 1.14x slower                                      |
| regex_v8       | 15.1 ms                                                | 17.9 ms: 1.18x slower                                      |
| Geometric mean | (ref)                                                  | 1.13x slower                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-darwin-arm64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.61 ms: 1.14x faster                                      |
| pickle_pure_python   | 191 us                                                 | 196 us: 1.02x slower                                       |
| pickle_dict          | 17.1 us                                                | 18.1 us: 1.06x slower                                      |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.07x slower                                       |
| pickle               | 6.98 us                                                | 7.44 us: 1.07x slower                                      |
| pickle_list          | 2.70 us                                                | 2.97 us: 1.10x slower                                      |
| unpickle             | 8.29 us                                                | 9.16 us: 1.11x slower                                      |
| unpickle_pure_python | 149 us                                                 | 165 us: 1.11x slower                                       |
| json_loads           | 15.3 us                                                | 17.0 us: 1.11x slower                                      |
| unpickle_list        | 2.69 us                                                | 3.07 us: 1.14x slower                                      |
| xml_etree_iterparse  | 68.3 ms                                                | 80.9 ms: 1.19x slower                                      |
| xml_etree_process    | 33.6 ms                                                | 40.9 ms: 1.22x slower                                      |
| xml_etree_generate   | 45.8 ms                                                | 58.8 ms: 1.28x slower                                      |
| tomli_loads          | 1.27 sec                                               | 1.68 sec: 1.32x slower                                     |
| Geometric mean       | (ref)                                                  | 1.11x slower                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-darwin-arm64-python-v3.13.0a3-3.13.0a3-f009305 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 12.8 ms: 1.19x slower                                      |
| python_startup_no_site | 8.57 ms                                                | 11.4 ms: 1.34x slower                                      |
| Geometric mean         | (ref)                                                  | 1.26x slower                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-darwin-arm64-python-v3.13.0a3-3.13.0a3-f009305 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 7.93 ms                                                | 9.85 ms: 1.24x slower                                      |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-darwin-arm64-python-v3.13.0a3-3.13.0a3-f009305 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 74.1 us: 4.06x faster                                      |
| asyncio_tcp                | 643 ms                                                 | 426 ms: 1.51x faster                                       |
| unpack_sequence            | 33.6 ns                                                | 28.5 ns: 1.18x faster                                      |
| json_dumps                 | 7.53 ms                                                | 6.61 ms: 1.14x faster                                      |
| raytrace                   | 206 ms                                                 | 186 ms: 1.10x faster                                       |
| sqlglot_parse              | 890 us                                                 | 811 us: 1.10x faster                                       |
| async_tree_none            | 282 ms                                                 | 261 ms: 1.08x faster                                       |
| async_tree_io_tg           | 724 ms                                                 | 682 ms: 1.06x faster                                       |
| sqlglot_transpile          | 1.05 ms                                                | 994 us: 1.06x faster                                       |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.32 sec: 1.06x faster                                     |
| generators                 | 30.3 ms                                                | 28.7 ms: 1.06x faster                                      |
| async_tree_memoization_tg  | 352 ms                                                 | 335 ms: 1.05x faster                                       |
| async_tree_none_tg         | 276 ms                                                 | 267 ms: 1.03x faster                                       |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 538 ms: 1.02x faster                                       |
| richards_super             | 37.3 ms                                                | 36.6 ms: 1.02x faster                                      |
| chaos                      | 47.4 ms                                                | 46.7 ms: 1.01x faster                                      |
| create_gc_cycles           | 711 us                                                 | 703 us: 1.01x faster                                       |
| sympy_sum                  | 80.2 ms                                                | 79.4 ms: 1.01x faster                                      |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                      |
| pidigits                   | 280 ms                                                 | 284 ms: 1.01x slower                                       |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 530 ms: 1.02x slower                                       |
| pickle_pure_python         | 191 us                                                 | 196 us: 1.02x slower                                       |
| async_tree_io              | 697 ms                                                 | 715 ms: 1.03x slower                                       |
| sympy_integrate            | 11.3 ms                                                | 11.6 ms: 1.03x slower                                      |
| sympy_str                  | 144 ms                                                 | 149 ms: 1.03x slower                                       |
| dask                       | 219 ms                                                 | 227 ms: 1.04x slower                                       |
| deepcopy_memo              | 25.7 us                                                | 26.8 us: 1.04x slower                                      |
| docutils                   | 1.43 sec                                               | 1.50 sec: 1.05x slower                                     |
| logging_simple             | 3.41 us                                                | 3.58 us: 1.05x slower                                      |
| dulwich_log                | 28.6 ms                                                | 30.1 ms: 1.05x slower                                      |
| regex_dna                  | 148 ms                                                 | 156 ms: 1.05x slower                                       |
| richards                   | 31.1 ms                                                | 32.8 ms: 1.06x slower                                      |
| logging_format             | 3.67 us                                                | 3.88 us: 1.06x slower                                      |
| go                         | 105 ms                                                 | 112 ms: 1.06x slower                                       |
| deepcopy                   | 215 us                                                 | 229 us: 1.06x slower                                       |
| pickle_dict                | 17.1 us                                                | 18.1 us: 1.06x slower                                      |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.07x slower                                       |
| pickle                     | 6.98 us                                                | 7.44 us: 1.07x slower                                      |
| pycparser                  | 659 ms                                                 | 704 ms: 1.07x slower                                       |
| sympy_expand               | 229 ms                                                 | 247 ms: 1.08x slower                                       |
| meteor_contest             | 71.1 ms                                                | 76.8 ms: 1.08x slower                                      |
| logging_silent             | 66.5 ns                                                | 72.1 ns: 1.08x slower                                      |
| comprehensions             | 14.4 us                                                | 15.7 us: 1.09x slower                                      |
| mdp                        | 1.48 sec                                               | 1.62 sec: 1.09x slower                                     |
| coverage                   | 43.9 ms                                                | 47.9 ms: 1.09x slower                                      |
| coroutines                 | 17.2 ms                                                | 18.9 ms: 1.10x slower                                      |
| pathlib                    | 23.2 ms                                                | 25.5 ms: 1.10x slower                                      |
| bench_mp_pool              | 41.0 ms                                                | 45.1 ms: 1.10x slower                                      |
| pickle_list                | 2.70 us                                                | 2.97 us: 1.10x slower                                      |
| unpickle                   | 8.29 us                                                | 9.16 us: 1.11x slower                                      |
| json                       | 2.75 ms                                                | 3.04 ms: 1.11x slower                                      |
| unpickle_pure_python       | 149 us                                                 | 165 us: 1.11x slower                                       |
| json_loads                 | 15.3 us                                                | 17.0 us: 1.11x slower                                      |
| bench_thread_pool          | 465 us                                                 | 517 us: 1.11x slower                                       |
| deepcopy_reduce            | 1.79 us                                                | 2.01 us: 1.12x slower                                      |
| 2to3                       | 154 ms                                                 | 173 ms: 1.12x slower                                       |
| scimark_lu                 | 67.7 ms                                                | 76.7 ms: 1.13x slower                                      |
| regex_compile              | 72.8 ms                                                | 82.6 ms: 1.13x slower                                      |
| regex_effbot               | 2.43 ms                                                | 2.77 ms: 1.14x slower                                      |
| unpickle_list              | 2.69 us                                                | 3.07 us: 1.14x slower                                      |
| crypto_pyaes               | 47.5 ms                                                | 54.7 ms: 1.15x slower                                      |
| chameleon                  | 4.30 ms                                                | 5.03 ms: 1.17x slower                                      |
| sqlglot_normalize          | 162 ms                                                 | 191 ms: 1.18x slower                                       |
| regex_v8                   | 15.1 ms                                                | 17.9 ms: 1.18x slower                                      |
| xml_etree_iterparse        | 68.3 ms                                                | 80.9 ms: 1.19x slower                                      |
| python_startup             | 10.8 ms                                                | 12.8 ms: 1.19x slower                                      |
| pprint_safe_repr           | 478 ms                                                 | 575 ms: 1.20x slower                                       |
| pprint_pformat             | 979 ms                                                 | 1.18 sec: 1.20x slower                                     |
| sqlglot_optimize           | 29.6 ms                                                | 36.0 ms: 1.21x slower                                      |
| xml_etree_process          | 33.6 ms                                                | 40.9 ms: 1.22x slower                                      |
| nqueens                    | 55.9 ms                                                | 68.4 ms: 1.22x slower                                      |
| mako                       | 7.93 ms                                                | 9.85 ms: 1.24x slower                                      |
| xml_etree_generate         | 45.8 ms                                                | 58.8 ms: 1.28x slower                                      |
| sqlite_synth               | 1.26 us                                                | 1.64 us: 1.31x slower                                      |
| scimark_monte_carlo        | 43.5 ms                                                | 57.0 ms: 1.31x slower                                      |
| pyflate                    | 284 ms                                                 | 373 ms: 1.31x slower                                       |
| deltablue                  | 2.75 ms                                                | 3.63 ms: 1.32x slower                                      |
| tomli_loads                | 1.27 sec                                               | 1.68 sec: 1.32x slower                                     |
| hexiom                     | 4.58 ms                                                | 6.04 ms: 1.32x slower                                      |
| python_startup_no_site     | 8.57 ms                                                | 11.4 ms: 1.34x slower                                      |
| scimark_sor                | 79.2 ms                                                | 106 ms: 1.34x slower                                       |
| float                      | 50.8 ms                                                | 68.9 ms: 1.36x slower                                      |
| fannkuch                   | 240 ms                                                 | 328 ms: 1.37x slower                                       |
| nbody                      | 61.7 ms                                                | 86.4 ms: 1.40x slower                                      |
| mypy2                      | 372 ms                                                 | 530 ms: 1.42x slower                                       |
| scimark_fft                | 173 ms                                                 | 249 ms: 1.44x slower                                       |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 4.19 ms: 1.49x slower                                      |
| telco                      | 3.17 ms                                                | 4.73 ms: 1.49x slower                                      |
| async_generators           | 192 ms                                                 | 297 ms: 1.55x slower                                       |
| spectral_norm              | 65.7 ms                                                | 106 ms: 1.61x slower                                       |
| Geometric mean             | (ref)                                                  | 1.09x slower                                               |

Benchmark hidden because not significant (3): asyncio_websockets, async_tree_memoization, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.05x


# Memory

- memory change: 1.03x