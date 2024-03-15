
# Results vs. 3.11.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: darwin-arm64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.12x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x slower
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 181 ms: 1.17x slower                                                   |
| chameleon      | 4.30 ms                                                | 5.34 ms: 1.24x slower                                                  |
| docutils       | 1.43 sec                                               | 1.56 sec: 1.09x slower                                                 |
| tornado_http   | 69.1 ms                                                | 74.9 ms: 1.08x slower                                                  |
| Geometric mean | (ref)                                                  | 1.14x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 264 ms: 1.07x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 691 ms: 1.05x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 338 ms: 1.04x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 271 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 546 ms: 1.01x faster                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 536 ms: 1.03x slower                                                   |
| async_tree_io              | 697 ms                                                 | 722 ms: 1.04x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 283 ms: 1.01x slower                                                   |
| float          | 50.8 ms                                                | 70.9 ms: 1.39x slower                                                  |
| nbody          | 61.7 ms                                                | 90.1 ms: 1.46x slower                                                  |
| Geometric mean | (ref)                                                  | 1.27x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 153 ms: 1.04x slower                                                   |
| regex_effbot   | 2.43 ms                                                | 2.72 ms: 1.12x slower                                                  |
| regex_v8       | 15.1 ms                                                | 17.8 ms: 1.17x slower                                                  |
| regex_compile  | 72.8 ms                                                | 87.5 ms: 1.20x slower                                                  |
| Geometric mean | (ref)                                                  | 1.13x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.69 ms: 1.13x faster                                                  |
| pickle_dict          | 17.1 us                                                | 18.0 us: 1.06x slower                                                  |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.06x slower                                                   |
| pickle               | 6.98 us                                                | 7.46 us: 1.07x slower                                                  |
| pickle_pure_python   | 191 us                                                 | 206 us: 1.07x slower                                                   |
| pickle_list          | 2.70 us                                                | 2.94 us: 1.09x slower                                                  |
| unpickle             | 8.29 us                                                | 9.16 us: 1.10x slower                                                  |
| json_loads           | 15.3 us                                                | 17.3 us: 1.12x slower                                                  |
| unpickle_pure_python | 149 us                                                 | 174 us: 1.17x slower                                                   |
| unpickle_list        | 2.69 us                                                | 3.15 us: 1.17x slower                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 81.1 ms: 1.19x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 42.7 ms: 1.27x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.70 sec: 1.33x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 62.3 ms: 1.36x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.13x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.2 ms: 1.22x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 11.7 ms: 1.37x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.29x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 9.93 ms: 1.25x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-darwin-arm64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 78.1 us: 3.85x faster                                                  |
| asyncio_tcp                | 643 ms                                                 | 432 ms: 1.49x faster                                                   |
| generators                 | 30.3 ms                                                | 25.6 ms: 1.18x faster                                                  |
| unpack_sequence            | 33.6 ns                                                | 28.9 ns: 1.16x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 6.69 ms: 1.13x faster                                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.31 sec: 1.07x faster                                                 |
| async_tree_none            | 282 ms                                                 | 264 ms: 1.07x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 691 ms: 1.05x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 338 ms: 1.04x faster                                                   |
| raytrace                   | 206 ms                                                 | 199 ms: 1.03x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 271 ms: 1.02x faster                                                   |
| create_gc_cycles           | 711 us                                                 | 704 us: 1.01x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 546 ms: 1.01x faster                                                   |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                                  |
| pidigits                   | 280 ms                                                 | 283 ms: 1.01x slower                                                   |
| chaos                      | 47.4 ms                                                | 48.2 ms: 1.02x slower                                                  |
| sqlglot_transpile          | 1.05 ms                                                | 1.08 ms: 1.02x slower                                                  |
| richards_super             | 37.3 ms                                                | 38.5 ms: 1.03x slower                                                  |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 536 ms: 1.03x slower                                                   |
| regex_dna                  | 148 ms                                                 | 153 ms: 1.04x slower                                                   |
| async_tree_io              | 697 ms                                                 | 722 ms: 1.04x slower                                                   |
| sympy_sum                  | 80.2 ms                                                | 83.4 ms: 1.04x slower                                                  |
| pickle_dict                | 17.1 us                                                | 18.0 us: 1.06x slower                                                  |
| deepcopy_memo              | 25.7 us                                                | 27.3 us: 1.06x slower                                                  |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.06x slower                                                   |
| dask                       | 219 ms                                                 | 234 ms: 1.07x slower                                                   |
| dulwich_log                | 28.6 ms                                                | 30.6 ms: 1.07x slower                                                  |
| pickle                     | 6.98 us                                                | 7.46 us: 1.07x slower                                                  |
| pickle_pure_python         | 191 us                                                 | 206 us: 1.07x slower                                                   |
| sympy_integrate            | 11.3 ms                                                | 12.1 ms: 1.07x slower                                                  |
| tornado_http               | 69.1 ms                                                | 74.9 ms: 1.08x slower                                                  |
| docutils                   | 1.43 sec                                               | 1.56 sec: 1.09x slower                                                 |
| pathlib                    | 23.2 ms                                                | 25.2 ms: 1.09x slower                                                  |
| pickle_list                | 2.70 us                                                | 2.94 us: 1.09x slower                                                  |
| go                         | 105 ms                                                 | 115 ms: 1.09x slower                                                   |
| logging_simple             | 3.41 us                                                | 3.72 us: 1.09x slower                                                  |
| json                       | 2.75 ms                                                | 3.01 ms: 1.09x slower                                                  |
| pycparser                  | 659 ms                                                 | 721 ms: 1.09x slower                                                   |
| logging_format             | 3.67 us                                                | 4.02 us: 1.10x slower                                                  |
| coroutines                 | 17.2 ms                                                | 18.8 ms: 1.10x slower                                                  |
| sympy_str                  | 144 ms                                                 | 158 ms: 1.10x slower                                                   |
| coverage                   | 43.9 ms                                                | 48.4 ms: 1.10x slower                                                  |
| unpickle                   | 8.29 us                                                | 9.16 us: 1.10x slower                                                  |
| deepcopy                   | 215 us                                                 | 239 us: 1.11x slower                                                   |
| richards                   | 31.1 ms                                                | 34.6 ms: 1.12x slower                                                  |
| regex_effbot               | 2.43 ms                                                | 2.72 ms: 1.12x slower                                                  |
| json_loads                 | 15.3 us                                                | 17.3 us: 1.12x slower                                                  |
| bench_mp_pool              | 41.0 ms                                                | 46.1 ms: 1.13x slower                                                  |
| comprehensions             | 14.4 us                                                | 16.3 us: 1.13x slower                                                  |
| logging_silent             | 66.5 ns                                                | 75.0 ns: 1.13x slower                                                  |
| meteor_contest             | 71.1 ms                                                | 80.3 ms: 1.13x slower                                                  |
| bench_thread_pool          | 465 us                                                 | 530 us: 1.14x slower                                                   |
| sympy_expand               | 229 ms                                                 | 262 ms: 1.14x slower                                                   |
| mdp                        | 1.48 sec                                               | 1.71 sec: 1.15x slower                                                 |
| scimark_lu                 | 67.7 ms                                                | 78.7 ms: 1.16x slower                                                  |
| unpickle_pure_python       | 149 us                                                 | 174 us: 1.17x slower                                                   |
| 2to3                       | 154 ms                                                 | 181 ms: 1.17x slower                                                   |
| unpickle_list              | 2.69 us                                                | 3.15 us: 1.17x slower                                                  |
| regex_v8                   | 15.1 ms                                                | 17.8 ms: 1.17x slower                                                  |
| crypto_pyaes               | 47.5 ms                                                | 55.9 ms: 1.18x slower                                                  |
| deepcopy_reduce            | 1.79 us                                                | 2.12 us: 1.18x slower                                                  |
| xml_etree_iterparse        | 68.3 ms                                                | 81.1 ms: 1.19x slower                                                  |
| regex_compile              | 72.8 ms                                                | 87.5 ms: 1.20x slower                                                  |
| python_startup             | 10.8 ms                                                | 13.2 ms: 1.22x slower                                                  |
| sqlglot_normalize          | 162 ms                                                 | 200 ms: 1.24x slower                                                   |
| chameleon                  | 4.30 ms                                                | 5.34 ms: 1.24x slower                                                  |
| pprint_safe_repr           | 478 ms                                                 | 594 ms: 1.24x slower                                                   |
| pprint_pformat             | 979 ms                                                 | 1.22 sec: 1.24x slower                                                 |
| nqueens                    | 55.9 ms                                                | 69.7 ms: 1.25x slower                                                  |
| mako                       | 7.93 ms                                                | 9.93 ms: 1.25x slower                                                  |
| xml_etree_process          | 33.6 ms                                                | 42.7 ms: 1.27x slower                                                  |
| sqlglot_optimize           | 29.6 ms                                                | 37.8 ms: 1.28x slower                                                  |
| hexiom                     | 4.58 ms                                                | 6.08 ms: 1.33x slower                                                  |
| pyflate                    | 284 ms                                                 | 377 ms: 1.33x slower                                                   |
| tomli_loads                | 1.27 sec                                               | 1.70 sec: 1.33x slower                                                 |
| deltablue                  | 2.75 ms                                                | 3.68 ms: 1.34x slower                                                  |
| xml_etree_generate         | 45.8 ms                                                | 62.3 ms: 1.36x slower                                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 59.3 ms: 1.36x slower                                                  |
| python_startup_no_site     | 8.57 ms                                                | 11.7 ms: 1.37x slower                                                  |
| sqlite_synth               | 1.26 us                                                | 1.72 us: 1.37x slower                                                  |
| scimark_sor                | 79.2 ms                                                | 110 ms: 1.39x slower                                                   |
| float                      | 50.8 ms                                                | 70.9 ms: 1.39x slower                                                  |
| fannkuch                   | 240 ms                                                 | 341 ms: 1.42x slower                                                   |
| mypy2                      | 372 ms                                                 | 542 ms: 1.46x slower                                                   |
| nbody                      | 61.7 ms                                                | 90.1 ms: 1.46x slower                                                  |
| scimark_fft                | 173 ms                                                 | 253 ms: 1.47x slower                                                   |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 4.21 ms: 1.50x slower                                                  |
| telco                      | 3.17 ms                                                | 4.83 ms: 1.53x slower                                                  |
| async_generators           | 192 ms                                                 | 309 ms: 1.61x slower                                                   |
| spectral_norm              | 65.7 ms                                                | 106 ms: 1.61x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.12x slower                                                           |

Benchmark hidden because not significant (3): sqlglot_parse, asyncio_websockets, async_tree_memoization
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.09x
- 95% likely to have a slowdown of 1.08x
- 99% likely to have a slowdown of 1.07x


# Memory

- memory change: 1.03x