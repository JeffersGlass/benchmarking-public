
# Results vs. 3.11.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: darwin-arm64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.18x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x slower
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 196 ms: 1.27x slower                                                   |
| chameleon      | 4.30 ms                                                | 5.51 ms: 1.28x slower                                                  |
| docutils       | 1.43 sec                                               | 1.67 sec: 1.17x slower                                                 |
| tornado_http   | 69.1 ms                                                | 83.4 ms: 1.21x slower                                                  |
| Geometric mean | (ref)                                                  | 1.23x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_io_tg           | 724 ms                                                 | 735 ms: 1.02x slower                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 360 ms: 1.02x slower                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 574 ms: 1.04x slower                                                   |
| async_tree_none_tg         | 276 ms                                                 | 289 ms: 1.04x slower                                                   |
| async_tree_memoization     | 336 ms                                                 | 360 ms: 1.07x slower                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 564 ms: 1.09x slower                                                   |
| async_tree_io              | 697 ms                                                 | 767 ms: 1.10x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 294 ms: 1.05x slower                                                   |
| float          | 50.8 ms                                                | 74.2 ms: 1.46x slower                                                  |
| nbody          | 61.7 ms                                                | 92.7 ms: 1.50x slower                                                  |
| Geometric mean | (ref)                                                  | 1.32x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 161 ms: 1.08x slower                                                   |
| regex_effbot   | 2.43 ms                                                | 2.84 ms: 1.17x slower                                                  |
| regex_v8       | 15.1 ms                                                | 18.4 ms: 1.22x slower                                                  |
| regex_compile  | 72.8 ms                                                | 89.4 ms: 1.23x slower                                                  |
| Geometric mean | (ref)                                                  | 1.17x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.97 ms: 1.08x faster                                                  |
| pickle_dict          | 17.1 us                                                | 18.6 us: 1.09x slower                                                  |
| pickle               | 6.98 us                                                | 7.67 us: 1.10x slower                                                  |
| pickle_pure_python   | 191 us                                                 | 212 us: 1.11x slower                                                   |
| xml_etree_parse      | 100 ms                                                 | 113 ms: 1.12x slower                                                   |
| pickle_list          | 2.70 us                                                | 3.04 us: 1.13x slower                                                  |
| unpickle             | 8.29 us                                                | 9.49 us: 1.15x slower                                                  |
| json_loads           | 15.3 us                                                | 17.9 us: 1.16x slower                                                  |
| unpickle_pure_python | 149 us                                                 | 180 us: 1.21x slower                                                   |
| unpickle_list        | 2.69 us                                                | 3.27 us: 1.22x slower                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 86.0 ms: 1.26x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 44.4 ms: 1.32x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.76 sec: 1.38x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 64.3 ms: 1.40x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.18x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 15.6 ms: 1.45x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 14.0 ms: 1.63x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.54x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 10.5 ms: 1.32x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 80.6 us: 3.73x faster                                                  |
| generators                 | 30.3 ms                                                | 26.6 ms: 1.14x faster                                                  |
| unpack_sequence            | 33.6 ns                                                | 29.8 ns: 1.13x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 6.97 ms: 1.08x faster                                                  |
| asyncio_tcp                | 643 ms                                                 | 595 ms: 1.08x faster                                                   |
| raytrace                   | 206 ms                                                 | 203 ms: 1.01x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 735 ms: 1.02x slower                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 360 ms: 1.02x slower                                                   |
| sqlglot_parse              | 890 us                                                 | 924 us: 1.04x slower                                                   |
| create_gc_cycles           | 711 us                                                 | 740 us: 1.04x slower                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 574 ms: 1.04x slower                                                   |
| async_tree_none_tg         | 276 ms                                                 | 289 ms: 1.04x slower                                                   |
| pidigits                   | 280 ms                                                 | 294 ms: 1.05x slower                                                   |
| chaos                      | 47.4 ms                                                | 50.1 ms: 1.06x slower                                                  |
| richards_super             | 37.3 ms                                                | 39.9 ms: 1.07x slower                                                  |
| asyncio_websockets         | 408 ms                                                 | 437 ms: 1.07x slower                                                   |
| async_tree_memoization     | 336 ms                                                 | 360 ms: 1.07x slower                                                   |
| gc_traversal               | 2.38 ms                                                | 2.56 ms: 1.07x slower                                                  |
| sqlglot_transpile          | 1.05 ms                                                | 1.13 ms: 1.07x slower                                                  |
| regex_dna                  | 148 ms                                                 | 161 ms: 1.08x slower                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 564 ms: 1.09x slower                                                   |
| pickle_dict                | 17.1 us                                                | 18.6 us: 1.09x slower                                                  |
| sympy_sum                  | 80.2 ms                                                | 87.7 ms: 1.09x slower                                                  |
| async_tree_io              | 697 ms                                                 | 767 ms: 1.10x slower                                                   |
| pickle                     | 6.98 us                                                | 7.67 us: 1.10x slower                                                  |
| deepcopy_memo              | 25.7 us                                                | 28.4 us: 1.10x slower                                                  |
| pickle_pure_python         | 191 us                                                 | 212 us: 1.11x slower                                                   |
| dulwich_log                | 28.6 ms                                                | 32.0 ms: 1.12x slower                                                  |
| xml_etree_parse            | 100 ms                                                 | 113 ms: 1.12x slower                                                   |
| pickle_list                | 2.70 us                                                | 3.04 us: 1.13x slower                                                  |
| go                         | 105 ms                                                 | 119 ms: 1.13x slower                                                   |
| coroutines                 | 17.2 ms                                                | 19.4 ms: 1.13x slower                                                  |
| coverage                   | 43.9 ms                                                | 49.9 ms: 1.14x slower                                                  |
| sympy_integrate            | 11.3 ms                                                | 12.8 ms: 1.14x slower                                                  |
| logging_simple             | 3.41 us                                                | 3.89 us: 1.14x slower                                                  |
| unpickle                   | 8.29 us                                                | 9.49 us: 1.15x slower                                                  |
| deepcopy                   | 215 us                                                 | 247 us: 1.15x slower                                                   |
| logging_format             | 3.67 us                                                | 4.22 us: 1.15x slower                                                  |
| json                       | 2.75 ms                                                | 3.16 ms: 1.15x slower                                                  |
| dask                       | 219 ms                                                 | 252 ms: 1.15x slower                                                   |
| richards                   | 31.1 ms                                                | 35.9 ms: 1.16x slower                                                  |
| sympy_str                  | 144 ms                                                 | 167 ms: 1.16x slower                                                   |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.62 sec: 1.16x slower                                                 |
| json_loads                 | 15.3 us                                                | 17.9 us: 1.16x slower                                                  |
| logging_silent             | 66.5 ns                                                | 77.5 ns: 1.16x slower                                                  |
| pycparser                  | 659 ms                                                 | 769 ms: 1.17x slower                                                   |
| comprehensions             | 14.4 us                                                | 16.9 us: 1.17x slower                                                  |
| docutils                   | 1.43 sec                                               | 1.67 sec: 1.17x slower                                                 |
| regex_effbot               | 2.43 ms                                                | 2.84 ms: 1.17x slower                                                  |
| meteor_contest             | 71.1 ms                                                | 83.9 ms: 1.18x slower                                                  |
| pathlib                    | 23.2 ms                                                | 27.5 ms: 1.18x slower                                                  |
| sympy_expand               | 229 ms                                                 | 274 ms: 1.20x slower                                                   |
| scimark_lu                 | 67.7 ms                                                | 81.4 ms: 1.20x slower                                                  |
| crypto_pyaes               | 47.5 ms                                                | 57.3 ms: 1.21x slower                                                  |
| tornado_http               | 69.1 ms                                                | 83.4 ms: 1.21x slower                                                  |
| unpickle_pure_python       | 149 us                                                 | 180 us: 1.21x slower                                                   |
| unpickle_list              | 2.69 us                                                | 3.27 us: 1.22x slower                                                  |
| regex_v8                   | 15.1 ms                                                | 18.4 ms: 1.22x slower                                                  |
| deepcopy_reduce            | 1.79 us                                                | 2.19 us: 1.22x slower                                                  |
| regex_compile              | 72.8 ms                                                | 89.4 ms: 1.23x slower                                                  |
| mdp                        | 1.48 sec                                               | 1.85 sec: 1.25x slower                                                 |
| bench_thread_pool          | 465 us                                                 | 582 us: 1.25x slower                                                   |
| bench_mp_pool              | 41.0 ms                                                | 51.6 ms: 1.26x slower                                                  |
| xml_etree_iterparse        | 68.3 ms                                                | 86.0 ms: 1.26x slower                                                  |
| 2to3                       | 154 ms                                                 | 196 ms: 1.27x slower                                                   |
| chameleon                  | 4.30 ms                                                | 5.51 ms: 1.28x slower                                                  |
| pprint_pformat             | 979 ms                                                 | 1.26 sec: 1.28x slower                                                 |
| pprint_safe_repr           | 478 ms                                                 | 615 ms: 1.29x slower                                                   |
| nqueens                    | 55.9 ms                                                | 72.2 ms: 1.29x slower                                                  |
| sqlglot_normalize          | 162 ms                                                 | 211 ms: 1.31x slower                                                   |
| mako                       | 7.93 ms                                                | 10.5 ms: 1.32x slower                                                  |
| xml_etree_process          | 33.6 ms                                                | 44.4 ms: 1.32x slower                                                  |
| sqlglot_optimize           | 29.6 ms                                                | 39.5 ms: 1.33x slower                                                  |
| hexiom                     | 4.58 ms                                                | 6.31 ms: 1.38x slower                                                  |
| tomli_loads                | 1.27 sec                                               | 1.76 sec: 1.38x slower                                                 |
| deltablue                  | 2.75 ms                                                | 3.83 ms: 1.39x slower                                                  |
| xml_etree_generate         | 45.8 ms                                                | 64.3 ms: 1.40x slower                                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 61.4 ms: 1.41x slower                                                  |
| sqlite_synth               | 1.26 us                                                | 1.78 us: 1.42x slower                                                  |
| scimark_sor                | 79.2 ms                                                | 114 ms: 1.44x slower                                                   |
| python_startup             | 10.8 ms                                                | 15.6 ms: 1.45x slower                                                  |
| pyflate                    | 284 ms                                                 | 411 ms: 1.45x slower                                                   |
| float                      | 50.8 ms                                                | 74.2 ms: 1.46x slower                                                  |
| fannkuch                   | 240 ms                                                 | 360 ms: 1.50x slower                                                   |
| nbody                      | 61.7 ms                                                | 92.7 ms: 1.50x slower                                                  |
| scimark_fft                | 173 ms                                                 | 261 ms: 1.51x slower                                                   |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 4.38 ms: 1.56x slower                                                  |
| telco                      | 3.17 ms                                                | 4.95 ms: 1.56x slower                                                  |
| mypy2                      | 372 ms                                                 | 595 ms: 1.60x slower                                                   |
| spectral_norm              | 65.7 ms                                                | 106 ms: 1.61x slower                                                   |
| python_startup_no_site     | 8.57 ms                                                | 14.0 ms: 1.63x slower                                                  |
| async_generators           | 192 ms                                                 | 322 ms: 1.68x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.18x slower                                                           |

Benchmark hidden because not significant (1): async_tree_none
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.16x
- 95% likely to have a slowdown of 1.15x
- 99% likely to have a slowdown of 1.14x


# Memory

- memory change: 1.03x