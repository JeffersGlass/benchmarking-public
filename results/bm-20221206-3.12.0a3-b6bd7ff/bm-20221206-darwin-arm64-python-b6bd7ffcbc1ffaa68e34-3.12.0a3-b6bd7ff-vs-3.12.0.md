
# Results vs. 3.12.0

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: darwin-arm64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.04x slower \*
- HPT reliability: 99.32%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 166 ms: 1.02x faster                                                  |
| chameleon      | 4.70 ms                                                | 4.68 ms: 1.00x faster                                                 |
| docutils       | 1.50 sec                                               | 1.48 sec: 1.01x faster                                                |
| Geometric mean | (ref)                                                  | 1.01x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 539 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 553 ms: 1.04x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 333 ms: 1.07x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 276 ms: 1.07x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 350 ms: 1.08x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 733 ms: 1.10x slower                                                  |
| async_tree_none            | 266 ms                                                 | 295 ms: 1.11x slower                                                  |
| async_tree_io              | 668 ms                                                 | 758 ms: 1.13x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| nbody          | 68.8 ms                                                | 68.4 ms: 1.01x faster                                                 |
| float          | 55.8 ms                                                | 57.6 ms: 1.03x slower                                                 |
| Geometric mean | (ref)                                                  | 1.01x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.45 ms: 1.08x faster                                                 |
| regex_v8       | 16.0 ms                                                | 15.1 ms: 1.05x faster                                                 |
| regex_dna      | 154 ms                                                 | 147 ms: 1.05x faster                                                  |
| regex_compile  | 77.9 ms                                                | 78.1 ms: 1.00x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 47.5 ms: 1.18x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 96.5 ms: 1.10x faster                                                 |
| unpickle_list        | 3.02 us                                                | 2.75 us: 1.10x faster                                                 |
| json_loads           | 17.2 us                                                | 15.8 us: 1.09x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 36.4 ms: 1.09x faster                                                 |
| pickle_list          | 2.89 us                                                | 2.67 us: 1.08x faster                                                 |
| unpickle             | 9.12 us                                                | 8.45 us: 1.08x faster                                                 |
| pickle_dict          | 18.1 us                                                | 17.0 us: 1.06x faster                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 70.3 ms: 1.05x faster                                                 |
| pickle               | 7.23 us                                                | 7.13 us: 1.01x faster                                                 |
| json_dumps           | 6.22 ms                                                | 6.15 ms: 1.01x faster                                                 |
| pickle_pure_python   | 200 us                                                 | 213 us: 1.06x slower                                                  |
| unpickle_pure_python | 151 us                                                 | 160 us: 1.06x slower                                                  |
| tomli_loads          | 1.39 sec                                               | 1.51 sec: 1.08x slower                                                |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 11.4 ms: 1.00x slower                                                 |
| python_startup_no_site | 9.37 ms                                                | 9.48 ms: 1.01x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.71 ms                                                | 7.45 ms: 1.04x faster                                                 |
| django_template | 22.3 ms                                                | 21.9 ms: 1.02x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.03x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 208 ms: 1.46x faster                                                  |
| telco                      | 3.68 ms                                                | 3.09 ms: 1.19x faster                                                 |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 2.65 ms: 1.18x faster                                                 |
| xml_etree_generate         | 55.8 ms                                                | 47.5 ms: 1.18x faster                                                 |
| xml_etree_parse            | 106 ms                                                 | 96.5 ms: 1.10x faster                                                 |
| sqlite_synth               | 1.57 us                                                | 1.43 us: 1.10x faster                                                 |
| unpickle_list              | 3.02 us                                                | 2.75 us: 1.10x faster                                                 |
| json_loads                 | 17.2 us                                                | 15.8 us: 1.09x faster                                                 |
| xml_etree_process          | 39.7 ms                                                | 36.4 ms: 1.09x faster                                                 |
| pickle_list                | 2.89 us                                                | 2.67 us: 1.08x faster                                                 |
| json                       | 3.09 ms                                                | 2.85 ms: 1.08x faster                                                 |
| unpickle                   | 9.12 us                                                | 8.45 us: 1.08x faster                                                 |
| regex_effbot               | 2.64 ms                                                | 2.45 ms: 1.08x faster                                                 |
| pickle_dict                | 18.1 us                                                | 17.0 us: 1.06x faster                                                 |
| regex_v8                   | 16.0 ms                                                | 15.1 ms: 1.05x faster                                                 |
| xml_etree_iterparse        | 74.0 ms                                                | 70.3 ms: 1.05x faster                                                 |
| bench_mp_pool              | 44.9 ms                                                | 42.6 ms: 1.05x faster                                                 |
| scimark_fft                | 195 ms                                                 | 186 ms: 1.05x faster                                                  |
| regex_dna                  | 154 ms                                                 | 147 ms: 1.05x faster                                                  |
| nqueens                    | 62.4 ms                                                | 60.0 ms: 1.04x faster                                                 |
| pathlib                    | 24.2 ms                                                | 23.3 ms: 1.04x faster                                                 |
| bench_thread_pool          | 504 us                                                 | 485 us: 1.04x faster                                                  |
| mako                       | 7.71 ms                                                | 7.45 ms: 1.04x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 180 ms: 1.03x faster                                                  |
| sqlglot_optimize           | 34.0 ms                                                | 33.1 ms: 1.03x faster                                                 |
| create_gc_cycles           | 701 us                                                 | 682 us: 1.03x faster                                                  |
| 2to3                       | 169 ms                                                 | 166 ms: 1.02x faster                                                  |
| django_template            | 22.3 ms                                                | 21.9 ms: 1.02x faster                                                 |
| dulwich_log                | 29.8 ms                                                | 29.4 ms: 1.02x faster                                                 |
| docutils                   | 1.50 sec                                               | 1.48 sec: 1.01x faster                                                |
| pickle                     | 7.23 us                                                | 7.13 us: 1.01x faster                                                 |
| json_dumps                 | 6.22 ms                                                | 6.15 ms: 1.01x faster                                                 |
| gc_traversal               | 2.40 ms                                                | 2.38 ms: 1.01x faster                                                 |
| crypto_pyaes               | 51.9 ms                                                | 51.5 ms: 1.01x faster                                                 |
| pidigits                   | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| nbody                      | 68.8 ms                                                | 68.4 ms: 1.01x faster                                                 |
| chameleon                  | 4.70 ms                                                | 4.68 ms: 1.00x faster                                                 |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                                  |
| regex_compile              | 77.9 ms                                                | 78.1 ms: 1.00x slower                                                 |
| python_startup             | 11.4 ms                                                | 11.4 ms: 1.00x slower                                                 |
| deepcopy_reduce            | 2.07 us                                                | 2.09 us: 1.01x slower                                                 |
| python_startup_no_site     | 9.37 ms                                                | 9.48 ms: 1.01x slower                                                 |
| pycparser                  | 677 ms                                                 | 686 ms: 1.01x slower                                                  |
| pprint_safe_repr           | 497 ms                                                 | 507 ms: 1.02x slower                                                  |
| sympy_expand               | 241 ms                                                 | 246 ms: 1.02x slower                                                  |
| deepcopy                   | 235 us                                                 | 240 us: 1.02x slower                                                  |
| pprint_pformat             | 1.01 sec                                               | 1.03 sec: 1.02x slower                                                |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 539 ms: 1.02x slower                                                  |
| unpack_sequence            | 31.5 ns                                                | 32.3 ns: 1.03x slower                                                 |
| raytrace                   | 212 ms                                                 | 218 ms: 1.03x slower                                                  |
| logging_format             | 3.98 us                                                | 4.10 us: 1.03x slower                                                 |
| float                      | 55.8 ms                                                | 57.6 ms: 1.03x slower                                                 |
| logging_simple             | 3.69 us                                                | 3.81 us: 1.03x slower                                                 |
| sympy_str                  | 148 ms                                                 | 153 ms: 1.04x slower                                                  |
| deepcopy_memo              | 27.7 us                                                | 28.7 us: 1.04x slower                                                 |
| logging_silent             | 76.4 ns                                                | 79.3 ns: 1.04x slower                                                 |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 553 ms: 1.04x slower                                                  |
| spectral_norm              | 76.4 ms                                                | 79.6 ms: 1.04x slower                                                 |
| sympy_integrate            | 11.4 ms                                                | 11.9 ms: 1.05x slower                                                 |
| deltablue                  | 2.71 ms                                                | 2.83 ms: 1.05x slower                                                 |
| meteor_contest             | 71.7 ms                                                | 75.9 ms: 1.06x slower                                                 |
| pickle_pure_python         | 200 us                                                 | 213 us: 1.06x slower                                                  |
| coroutines                 | 19.2 ms                                                | 20.5 ms: 1.06x slower                                                 |
| unpickle_pure_python       | 151 us                                                 | 160 us: 1.06x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 333 ms: 1.07x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 276 ms: 1.07x slower                                                  |
| fannkuch                   | 248 ms                                                 | 267 ms: 1.07x slower                                                  |
| scimark_lu                 | 76.0 ms                                                | 81.7 ms: 1.08x slower                                                 |
| pyflate                    | 316 ms                                                 | 340 ms: 1.08x slower                                                  |
| richards                   | 32.1 ms                                                | 34.7 ms: 1.08x slower                                                 |
| tomli_loads                | 1.39 sec                                               | 1.51 sec: 1.08x slower                                                |
| async_tree_memoization_tg  | 323 ms                                                 | 350 ms: 1.08x slower                                                  |
| hexiom                     | 4.54 ms                                                | 4.97 ms: 1.09x slower                                                 |
| async_tree_io_tg           | 669 ms                                                 | 733 ms: 1.10x slower                                                  |
| sympy_sum                  | 77.6 ms                                                | 85.0 ms: 1.10x slower                                                 |
| async_tree_none            | 266 ms                                                 | 295 ms: 1.11x slower                                                  |
| mdp                        | 1.58 sec                                               | 1.77 sec: 1.12x slower                                                |
| async_tree_io              | 668 ms                                                 | 758 ms: 1.13x slower                                                  |
| richards_super             | 36.0 ms                                                | 41.5 ms: 1.15x slower                                                 |
| go                         | 102 ms                                                 | 118 ms: 1.16x slower                                                  |
| sqlglot_transpile          | 1.02 ms                                                | 1.19 ms: 1.17x slower                                                 |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.46 sec: 1.17x slower                                                |
| comprehensions             | 14.5 us                                                | 17.3 us: 1.19x slower                                                 |
| scimark_monte_carlo        | 45.0 ms                                                | 53.6 ms: 1.19x slower                                                 |
| scimark_sor                | 87.4 ms                                                | 105 ms: 1.20x slower                                                  |
| generators                 | 31.1 ms                                                | 37.2 ms: 1.20x slower                                                 |
| sqlglot_parse              | 848 us                                                 | 1.02 ms: 1.20x slower                                                 |
| chaos                      | 42.5 ms                                                | 51.4 ms: 1.21x slower                                                 |
| asyncio_tcp                | 449 ms                                                 | 661 ms: 1.47x slower                                                  |
| dask                       | 222 ms                                                 | 331 ms: 1.49x slower                                                  |
| typing_runtime_protocols   | 93.0 us                                                | 329 us: 3.54x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                          |
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, coverage, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http
Ignored benchmarks (4) of results/bm-20221206-3.12.0a3-b6bd7ff/bm-20221206-darwin-arm64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 99.32% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.96x