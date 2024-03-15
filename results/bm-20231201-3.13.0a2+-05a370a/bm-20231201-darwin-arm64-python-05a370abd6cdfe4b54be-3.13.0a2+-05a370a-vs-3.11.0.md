
# Results vs. 3.11.0

- fork: python
- ref: 05a370abd6cdfe4b54be
- machine: darwin-arm64
- commit hash: 05a370a
- commit date: 2023-12-01
- overall geometric mean: 1.06x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 175 ms: 1.13x slower                                                   |
| chameleon      | 4.30 ms                                                | 5.13 ms: 1.19x slower                                                  |
| docutils       | 1.43 sec                                               | 1.50 sec: 1.05x slower                                                 |
| tornado_http   | 69.1 ms                                                | 71.9 ms: 1.04x slower                                                  |
| Geometric mean | (ref)                                                  | 1.10x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 256 ms: 1.10x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 333 ms: 1.06x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 686 ms: 1.06x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 268 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 543 ms: 1.01x faster                                                   |
| async_tree_io              | 697 ms                                                 | 706 ms: 1.01x slower                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 526 ms: 1.01x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                           |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.01x slower                                                   |
| float          | 50.8 ms                                                | 58.0 ms: 1.14x slower                                                  |
| nbody          | 61.7 ms                                                | 82.1 ms: 1.33x slower                                                  |
| Geometric mean | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 149 ms: 1.01x slower                                                   |
| regex_effbot   | 2.43 ms                                                | 2.57 ms: 1.06x slower                                                  |
| regex_compile  | 72.8 ms                                                | 79.3 ms: 1.09x slower                                                  |
| regex_v8       | 15.1 ms                                                | 16.9 ms: 1.12x slower                                                  |
| Geometric mean | (ref)                                                  | 1.07x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.59 ms: 1.14x faster                                                  |
| pickle_dict          | 17.1 us                                                | 17.9 us: 1.05x slower                                                  |
| pickle_list          | 2.70 us                                                | 2.88 us: 1.07x slower                                                  |
| pickle               | 6.98 us                                                | 7.47 us: 1.07x slower                                                  |
| xml_etree_parse      | 100 ms                                                 | 108 ms: 1.08x slower                                                   |
| pickle_pure_python   | 191 us                                                 | 208 us: 1.09x slower                                                   |
| unpickle             | 8.29 us                                                | 9.07 us: 1.09x slower                                                  |
| unpickle_pure_python | 149 us                                                 | 165 us: 1.11x slower                                                   |
| xml_etree_iterparse  | 68.3 ms                                                | 76.1 ms: 1.11x slower                                                  |
| json_loads           | 15.3 us                                                | 17.2 us: 1.12x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.14 us: 1.17x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 40.7 ms: 1.21x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.61 sec: 1.26x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 58.4 ms: 1.28x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.2 ms: 1.22x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 11.8 ms: 1.37x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 7.78 ms: 1.02x faster                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-darwin-arm64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 77.5 us: 3.88x faster                                                  |
| asyncio_tcp                | 643 ms                                                 | 412 ms: 1.56x faster                                                   |
| generators                 | 30.3 ms                                                | 26.1 ms: 1.16x faster                                                  |
| unpack_sequence            | 33.6 ns                                                | 29.0 ns: 1.16x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 6.59 ms: 1.14x faster                                                  |
| comprehensions             | 14.4 us                                                | 12.7 us: 1.14x faster                                                  |
| deltablue                  | 2.75 ms                                                | 2.45 ms: 1.12x faster                                                  |
| raytrace                   | 206 ms                                                 | 184 ms: 1.12x faster                                                   |
| async_tree_none            | 282 ms                                                 | 256 ms: 1.10x faster                                                   |
| chaos                      | 47.4 ms                                                | 43.2 ms: 1.10x faster                                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.30 sec: 1.07x faster                                                 |
| sqlglot_parse              | 890 us                                                 | 829 us: 1.07x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 333 ms: 1.06x faster                                                   |
| sympy_sum                  | 80.2 ms                                                | 75.9 ms: 1.06x faster                                                  |
| async_tree_io_tg           | 724 ms                                                 | 686 ms: 1.06x faster                                                   |
| sqlglot_transpile          | 1.05 ms                                                | 1.01 ms: 1.04x faster                                                  |
| async_tree_none_tg         | 276 ms                                                 | 268 ms: 1.03x faster                                                   |
| mako                       | 7.93 ms                                                | 7.78 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 543 ms: 1.01x faster                                                   |
| create_gc_cycles           | 711 us                                                 | 703 us: 1.01x faster                                                   |
| sympy_integrate            | 11.3 ms                                                | 11.2 ms: 1.01x faster                                                  |
| asyncio_websockets         | 408 ms                                                 | 410 ms: 1.00x slower                                                   |
| regex_dna                  | 148 ms                                                 | 149 ms: 1.01x slower                                                   |
| go                         | 105 ms                                                 | 106 ms: 1.01x slower                                                   |
| pidigits                   | 280 ms                                                 | 282 ms: 1.01x slower                                                   |
| deepcopy_memo              | 25.7 us                                                | 26.0 us: 1.01x slower                                                  |
| async_tree_io              | 697 ms                                                 | 706 ms: 1.01x slower                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 526 ms: 1.01x slower                                                   |
| sympy_str                  | 144 ms                                                 | 147 ms: 1.02x slower                                                   |
| crypto_pyaes               | 47.5 ms                                                | 48.9 ms: 1.03x slower                                                  |
| tornado_http               | 69.1 ms                                                | 71.9 ms: 1.04x slower                                                  |
| richards_super             | 37.3 ms                                                | 38.9 ms: 1.04x slower                                                  |
| dask                       | 219 ms                                                 | 229 ms: 1.05x slower                                                   |
| docutils                   | 1.43 sec                                               | 1.50 sec: 1.05x slower                                                 |
| pickle_dict                | 17.1 us                                                | 17.9 us: 1.05x slower                                                  |
| dulwich_log                | 28.6 ms                                                | 30.2 ms: 1.05x slower                                                  |
| regex_effbot               | 2.43 ms                                                | 2.57 ms: 1.06x slower                                                  |
| meteor_contest             | 71.1 ms                                                | 75.3 ms: 1.06x slower                                                  |
| logging_simple             | 3.41 us                                                | 3.63 us: 1.06x slower                                                  |
| gc_traversal               | 2.38 ms                                                | 2.54 ms: 1.07x slower                                                  |
| logging_silent             | 66.5 ns                                                | 71.0 ns: 1.07x slower                                                  |
| pathlib                    | 23.2 ms                                                | 24.8 ms: 1.07x slower                                                  |
| pickle_list                | 2.70 us                                                | 2.88 us: 1.07x slower                                                  |
| pickle                     | 6.98 us                                                | 7.47 us: 1.07x slower                                                  |
| logging_format             | 3.67 us                                                | 3.95 us: 1.07x slower                                                  |
| pycparser                  | 659 ms                                                 | 710 ms: 1.08x slower                                                   |
| xml_etree_parse            | 100 ms                                                 | 108 ms: 1.08x slower                                                   |
| deepcopy                   | 215 us                                                 | 232 us: 1.08x slower                                                   |
| pickle_pure_python         | 191 us                                                 | 208 us: 1.09x slower                                                   |
| regex_compile              | 72.8 ms                                                | 79.3 ms: 1.09x slower                                                  |
| coverage                   | 43.9 ms                                                | 48.0 ms: 1.09x slower                                                  |
| unpickle                   | 8.29 us                                                | 9.07 us: 1.09x slower                                                  |
| hexiom                     | 4.58 ms                                                | 5.02 ms: 1.10x slower                                                  |
| json                       | 2.75 ms                                                | 3.04 ms: 1.11x slower                                                  |
| bench_mp_pool              | 41.0 ms                                                | 45.3 ms: 1.11x slower                                                  |
| sympy_expand               | 229 ms                                                 | 254 ms: 1.11x slower                                                   |
| bench_thread_pool          | 465 us                                                 | 516 us: 1.11x slower                                                   |
| unpickle_pure_python       | 149 us                                                 | 165 us: 1.11x slower                                                   |
| pprint_pformat             | 979 ms                                                 | 1.09 sec: 1.11x slower                                                 |
| xml_etree_iterparse        | 68.3 ms                                                | 76.1 ms: 1.11x slower                                                  |
| regex_v8                   | 15.1 ms                                                | 16.9 ms: 1.12x slower                                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 48.5 ms: 1.12x slower                                                  |
| scimark_lu                 | 67.7 ms                                                | 75.9 ms: 1.12x slower                                                  |
| mdp                        | 1.48 sec                                               | 1.66 sec: 1.12x slower                                                 |
| json_loads                 | 15.3 us                                                | 17.2 us: 1.12x slower                                                  |
| pprint_safe_repr           | 478 ms                                                 | 536 ms: 1.12x slower                                                   |
| coroutines                 | 17.2 ms                                                | 19.3 ms: 1.12x slower                                                  |
| nqueens                    | 55.9 ms                                                | 63.0 ms: 1.13x slower                                                  |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.17 ms: 1.13x slower                                                  |
| 2to3                       | 154 ms                                                 | 175 ms: 1.13x slower                                                   |
| richards                   | 31.1 ms                                                | 35.2 ms: 1.14x slower                                                  |
| float                      | 50.8 ms                                                | 58.0 ms: 1.14x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 75.1 ms: 1.14x slower                                                  |
| deepcopy_reduce            | 1.79 us                                                | 2.07 us: 1.16x slower                                                  |
| unpickle_list              | 2.69 us                                                | 3.14 us: 1.17x slower                                                  |
| sqlglot_normalize          | 162 ms                                                 | 192 ms: 1.18x slower                                                   |
| chameleon                  | 4.30 ms                                                | 5.13 ms: 1.19x slower                                                  |
| sqlglot_optimize           | 29.6 ms                                                | 35.8 ms: 1.21x slower                                                  |
| fannkuch                   | 240 ms                                                 | 289 ms: 1.21x slower                                                   |
| xml_etree_process          | 33.6 ms                                                | 40.7 ms: 1.21x slower                                                  |
| pyflate                    | 284 ms                                                 | 344 ms: 1.21x slower                                                   |
| python_startup             | 10.8 ms                                                | 13.2 ms: 1.22x slower                                                  |
| scimark_fft                | 173 ms                                                 | 212 ms: 1.23x slower                                                   |
| tomli_loads                | 1.27 sec                                               | 1.61 sec: 1.26x slower                                                 |
| xml_etree_generate         | 45.8 ms                                                | 58.4 ms: 1.28x slower                                                  |
| sqlite_synth               | 1.26 us                                                | 1.65 us: 1.32x slower                                                  |
| nbody                      | 61.7 ms                                                | 82.1 ms: 1.33x slower                                                  |
| scimark_sor                | 79.2 ms                                                | 107 ms: 1.35x slower                                                   |
| python_startup_no_site     | 8.57 ms                                                | 11.8 ms: 1.37x slower                                                  |
| mypy2                      | 372 ms                                                 | 525 ms: 1.41x slower                                                   |
| telco                      | 3.17 ms                                                | 4.72 ms: 1.49x slower                                                  |
| async_generators           | 192 ms                                                 | 305 ms: 1.59x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.06x slower                                                           |

Benchmark hidden because not significant (1): async_tree_memoization
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.02x