
# Results vs. 3.11.0

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: darwin-arm64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.07x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 178 ms: 1.16x slower                                                   |
| chameleon      | 4.30 ms                                                | 5.19 ms: 1.21x slower                                                  |
| docutils       | 1.43 sec                                               | 1.51 sec: 1.05x slower                                                 |
| tornado_http   | 69.1 ms                                                | 71.8 ms: 1.04x slower                                                  |
| Geometric mean | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 256 ms: 1.10x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 329 ms: 1.07x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 678 ms: 1.07x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 263 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 537 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 528 ms: 1.02x slower                                                   |
| async_tree_io              | 697 ms                                                 | 711 ms: 1.02x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.01x slower                                                   |
| float          | 50.8 ms                                                | 61.0 ms: 1.20x slower                                                  |
| nbody          | 61.7 ms                                                | 82.4 ms: 1.34x slower                                                  |
| Geometric mean | (ref)                                                  | 1.17x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 152 ms: 1.03x slower                                                   |
| regex_compile  | 72.8 ms                                                | 76.9 ms: 1.06x slower                                                  |
| regex_effbot   | 2.43 ms                                                | 2.72 ms: 1.12x slower                                                  |
| regex_v8       | 15.1 ms                                                | 17.7 ms: 1.17x slower                                                  |
| Geometric mean | (ref)                                                  | 1.09x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.66 ms: 1.13x faster                                                  |
| pickle_dict          | 17.1 us                                                | 17.9 us: 1.05x slower                                                  |
| pickle               | 6.98 us                                                | 7.44 us: 1.07x slower                                                  |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| pickle_list          | 2.70 us                                                | 2.91 us: 1.08x slower                                                  |
| pickle_pure_python   | 191 us                                                 | 208 us: 1.09x slower                                                   |
| unpickle             | 8.29 us                                                | 9.17 us: 1.11x slower                                                  |
| unpickle_pure_python | 149 us                                                 | 167 us: 1.12x slower                                                   |
| xml_etree_iterparse  | 68.3 ms                                                | 76.6 ms: 1.12x slower                                                  |
| json_loads           | 15.3 us                                                | 17.2 us: 1.12x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.11 us: 1.16x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 41.2 ms: 1.23x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.61 sec: 1.26x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 58.2 ms: 1.27x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.1 ms: 1.22x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 11.6 ms: 1.36x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.29x slower                                                           |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 75.0 us: 4.01x faster                                                  |
| asyncio_tcp                | 643 ms                                                 | 416 ms: 1.55x faster                                                   |
| generators                 | 30.3 ms                                                | 26.2 ms: 1.16x faster                                                  |
| comprehensions             | 14.4 us                                                | 12.7 us: 1.14x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 6.66 ms: 1.13x faster                                                  |
| chaos                      | 47.4 ms                                                | 42.0 ms: 1.13x faster                                                  |
| raytrace                   | 206 ms                                                 | 183 ms: 1.12x faster                                                   |
| unpack_sequence            | 33.6 ns                                                | 30.3 ns: 1.11x faster                                                  |
| async_tree_none            | 282 ms                                                 | 256 ms: 1.10x faster                                                   |
| deltablue                  | 2.75 ms                                                | 2.54 ms: 1.08x faster                                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.30 sec: 1.07x faster                                                 |
| async_tree_memoization_tg  | 352 ms                                                 | 329 ms: 1.07x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 678 ms: 1.07x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 263 ms: 1.05x faster                                                   |
| sympy_sum                  | 80.2 ms                                                | 76.7 ms: 1.05x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 537 ms: 1.02x faster                                                   |
| sqlglot_parse              | 890 us                                                 | 869 us: 1.02x faster                                                   |
| create_gc_cycles           | 711 us                                                 | 705 us: 1.01x faster                                                   |
| pidigits                   | 280 ms                                                 | 282 ms: 1.01x slower                                                   |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                                  |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 528 ms: 1.02x slower                                                   |
| async_tree_io              | 697 ms                                                 | 711 ms: 1.02x slower                                                   |
| deepcopy_memo              | 25.7 us                                                | 26.3 us: 1.02x slower                                                  |
| regex_dna                  | 148 ms                                                 | 152 ms: 1.03x slower                                                   |
| hexiom                     | 4.58 ms                                                | 4.71 ms: 1.03x slower                                                  |
| sympy_str                  | 144 ms                                                 | 149 ms: 1.03x slower                                                   |
| go                         | 105 ms                                                 | 109 ms: 1.03x slower                                                   |
| tornado_http               | 69.1 ms                                                | 71.8 ms: 1.04x slower                                                  |
| dask                       | 219 ms                                                 | 229 ms: 1.05x slower                                                   |
| meteor_contest             | 71.1 ms                                                | 74.5 ms: 1.05x slower                                                  |
| pickle_dict                | 17.1 us                                                | 17.9 us: 1.05x slower                                                  |
| docutils                   | 1.43 sec                                               | 1.51 sec: 1.05x slower                                                 |
| dulwich_log                | 28.6 ms                                                | 30.2 ms: 1.05x slower                                                  |
| regex_compile              | 72.8 ms                                                | 76.9 ms: 1.06x slower                                                  |
| crypto_pyaes               | 47.5 ms                                                | 50.2 ms: 1.06x slower                                                  |
| pickle                     | 6.98 us                                                | 7.44 us: 1.07x slower                                                  |
| richards_super             | 37.3 ms                                                | 39.8 ms: 1.07x slower                                                  |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| logging_simple             | 3.41 us                                                | 3.65 us: 1.07x slower                                                  |
| pathlib                    | 23.2 ms                                                | 24.9 ms: 1.07x slower                                                  |
| pickle_list                | 2.70 us                                                | 2.91 us: 1.08x slower                                                  |
| logging_format             | 3.67 us                                                | 3.99 us: 1.09x slower                                                  |
| pickle_pure_python         | 191 us                                                 | 208 us: 1.09x slower                                                   |
| deepcopy                   | 215 us                                                 | 235 us: 1.09x slower                                                   |
| coverage                   | 43.9 ms                                                | 47.8 ms: 1.09x slower                                                  |
| pycparser                  | 659 ms                                                 | 720 ms: 1.09x slower                                                   |
| logging_silent             | 66.5 ns                                                | 72.8 ns: 1.09x slower                                                  |
| unpickle                   | 8.29 us                                                | 9.17 us: 1.11x slower                                                  |
| json                       | 2.75 ms                                                | 3.04 ms: 1.11x slower                                                  |
| mdp                        | 1.48 sec                                               | 1.64 sec: 1.11x slower                                                 |
| bench_mp_pool              | 41.0 ms                                                | 45.7 ms: 1.12x slower                                                  |
| bench_thread_pool          | 465 us                                                 | 519 us: 1.12x slower                                                   |
| pprint_pformat             | 979 ms                                                 | 1.09 sec: 1.12x slower                                                 |
| regex_effbot               | 2.43 ms                                                | 2.72 ms: 1.12x slower                                                  |
| unpickle_pure_python       | 149 us                                                 | 167 us: 1.12x slower                                                   |
| sympy_expand               | 229 ms                                                 | 257 ms: 1.12x slower                                                   |
| xml_etree_iterparse        | 68.3 ms                                                | 76.6 ms: 1.12x slower                                                  |
| coroutines                 | 17.2 ms                                                | 19.3 ms: 1.12x slower                                                  |
| nqueens                    | 55.9 ms                                                | 62.8 ms: 1.12x slower                                                  |
| json_loads                 | 15.3 us                                                | 17.2 us: 1.12x slower                                                  |
| pprint_safe_repr           | 478 ms                                                 | 539 ms: 1.13x slower                                                   |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.20 ms: 1.14x slower                                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 49.8 ms: 1.15x slower                                                  |
| richards                   | 31.1 ms                                                | 35.7 ms: 1.15x slower                                                  |
| 2to3                       | 154 ms                                                 | 178 ms: 1.16x slower                                                   |
| scimark_lu                 | 67.7 ms                                                | 78.3 ms: 1.16x slower                                                  |
| unpickle_list              | 2.69 us                                                | 3.11 us: 1.16x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 76.1 ms: 1.16x slower                                                  |
| regex_v8                   | 15.1 ms                                                | 17.7 ms: 1.17x slower                                                  |
| deepcopy_reduce            | 1.79 us                                                | 2.11 us: 1.17x slower                                                  |
| sqlglot_normalize          | 162 ms                                                 | 193 ms: 1.19x slower                                                   |
| float                      | 50.8 ms                                                | 61.0 ms: 1.20x slower                                                  |
| chameleon                  | 4.30 ms                                                | 5.19 ms: 1.21x slower                                                  |
| sqlglot_optimize           | 29.6 ms                                                | 35.8 ms: 1.21x slower                                                  |
| python_startup             | 10.8 ms                                                | 13.1 ms: 1.22x slower                                                  |
| fannkuch                   | 240 ms                                                 | 293 ms: 1.22x slower                                                   |
| scimark_fft                | 173 ms                                                 | 211 ms: 1.22x slower                                                   |
| xml_etree_process          | 33.6 ms                                                | 41.2 ms: 1.23x slower                                                  |
| pyflate                    | 284 ms                                                 | 350 ms: 1.23x slower                                                   |
| tomli_loads                | 1.27 sec                                               | 1.61 sec: 1.26x slower                                                 |
| xml_etree_generate         | 45.8 ms                                                | 58.2 ms: 1.27x slower                                                  |
| sqlite_synth               | 1.26 us                                                | 1.65 us: 1.32x slower                                                  |
| nbody                      | 61.7 ms                                                | 82.4 ms: 1.34x slower                                                  |
| python_startup_no_site     | 8.57 ms                                                | 11.6 ms: 1.36x slower                                                  |
| scimark_sor                | 79.2 ms                                                | 108 ms: 1.37x slower                                                   |
| mypy2                      | 372 ms                                                 | 531 ms: 1.43x slower                                                   |
| telco                      | 3.17 ms                                                | 4.62 ms: 1.46x slower                                                  |
| async_generators           | 192 ms                                                 | 306 ms: 1.59x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.07x slower                                                           |

Benchmark hidden because not significant (5): async_tree_memoization, sympy_integrate, asyncio_websockets, sqlglot_transpile, mako
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.03x