
# Results vs. 3.12.0

- fork: python
- ref: ed7c3ff15680c1939fad
- machine: darwin-arm64
- commit hash: ed7c3ff
- commit date: 2022-09-11
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.62%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 153 ms: 1.10x faster                                                   |
| chameleon      | 4.70 ms                                                | 4.17 ms: 1.13x faster                                                  |
| docutils       | 1.50 sec                                               | 1.43 sec: 1.05x faster                                                 |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 515 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 547 ms: 1.03x slower                                                   |
| async_tree_io              | 668 ms                                                 | 690 ms: 1.03x slower                                                   |
| async_tree_none            | 266 ms                                                 | 277 ms: 1.04x slower                                                   |
| async_tree_none_tg         | 258 ms                                                 | 275 ms: 1.07x slower                                                   |
| async_tree_io_tg           | 669 ms                                                 | 722 ms: 1.08x slower                                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 351 ms: 1.09x slower                                                   |
| async_tree_memoization     | 312 ms                                                 | 347 ms: 1.11x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.05x slower                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 68.8 ms                                                | 68.4 ms: 1.01x faster                                                  |
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.46 ms: 1.07x faster                                                  |
| regex_compile  | 77.9 ms                                                | 73.6 ms: 1.06x faster                                                  |
| regex_v8       | 16.0 ms                                                | 15.5 ms: 1.03x faster                                                  |
| regex_dna      | 154 ms                                                 | 150 ms: 1.03x faster                                                   |
| Geometric mean | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 46.7 ms: 1.19x faster                                                  |
| xml_etree_process    | 39.7 ms                                                | 34.0 ms: 1.17x faster                                                  |
| json_loads           | 17.2 us                                                | 15.5 us: 1.11x faster                                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 67.1 ms: 1.10x faster                                                  |
| xml_etree_parse      | 106 ms                                                 | 96.9 ms: 1.10x faster                                                  |
| unpickle_list        | 3.02 us                                                | 2.77 us: 1.09x faster                                                  |
| unpickle             | 9.12 us                                                | 8.37 us: 1.09x faster                                                  |
| pickle_list          | 2.89 us                                                | 2.66 us: 1.09x faster                                                  |
| tomli_loads          | 1.39 sec                                               | 1.31 sec: 1.07x faster                                                 |
| pickle_dict          | 18.1 us                                                | 17.0 us: 1.06x faster                                                  |
| pickle               | 7.23 us                                                | 7.17 us: 1.01x faster                                                  |
| pickle_pure_python   | 200 us                                                 | 210 us: 1.05x slower                                                   |
| unpickle_pure_python | 151 us                                                 | 163 us: 1.08x slower                                                   |
| json_dumps           | 6.22 ms                                                | 7.56 ms: 1.22x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 12.0 ms: 1.06x slower                                                  |
| python_startup_no_site | 9.37 ms                                                | 9.94 ms: 1.06x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.06x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 19.8 ms: 1.13x faster                                                  |
| mako            | 7.71 ms                                                | 8.22 ms: 1.07x slower                                                  |
| Geometric mean  | (ref)                                                  | 1.03x faster                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 191 ms: 1.59x faster                                                   |
| xml_etree_generate         | 55.8 ms                                                | 46.7 ms: 1.19x faster                                                  |
| logging_silent             | 76.4 ns                                                | 64.4 ns: 1.19x faster                                                  |
| coroutines                 | 19.2 ms                                                | 16.4 ms: 1.17x faster                                                  |
| scimark_sor                | 87.4 ms                                                | 74.8 ms: 1.17x faster                                                  |
| xml_etree_process          | 39.7 ms                                                | 34.0 ms: 1.17x faster                                                  |
| sqlglot_normalize          | 186 ms                                                 | 160 ms: 1.16x faster                                                   |
| telco                      | 3.68 ms                                                | 3.18 ms: 1.16x faster                                                  |
| sqlite_synth               | 1.57 us                                                | 1.36 us: 1.16x faster                                                  |
| sqlglot_optimize           | 34.0 ms                                                | 29.5 ms: 1.15x faster                                                  |
| nqueens                    | 62.4 ms                                                | 54.3 ms: 1.15x faster                                                  |
| django_template            | 22.3 ms                                                | 19.8 ms: 1.13x faster                                                  |
| chameleon                  | 4.70 ms                                                | 4.17 ms: 1.13x faster                                                  |
| json                       | 3.09 ms                                                | 2.75 ms: 1.12x faster                                                  |
| scimark_lu                 | 76.0 ms                                                | 67.9 ms: 1.12x faster                                                  |
| json_loads                 | 17.2 us                                                | 15.5 us: 1.11x faster                                                  |
| 2to3                       | 169 ms                                                 | 153 ms: 1.10x faster                                                   |
| xml_etree_iterparse        | 74.0 ms                                                | 67.1 ms: 1.10x faster                                                  |
| bench_thread_pool          | 504 us                                                 | 457 us: 1.10x faster                                                   |
| spectral_norm              | 76.4 ms                                                | 69.2 ms: 1.10x faster                                                  |
| xml_etree_parse            | 106 ms                                                 | 96.9 ms: 1.10x faster                                                  |
| unpickle_list              | 3.02 us                                                | 2.77 us: 1.09x faster                                                  |
| unpickle                   | 9.12 us                                                | 8.37 us: 1.09x faster                                                  |
| pickle_list                | 2.89 us                                                | 2.66 us: 1.09x faster                                                  |
| crypto_pyaes               | 51.9 ms                                                | 48.1 ms: 1.08x faster                                                  |
| regex_effbot               | 2.64 ms                                                | 2.46 ms: 1.07x faster                                                  |
| bench_mp_pool              | 44.9 ms                                                | 41.8 ms: 1.07x faster                                                  |
| pyflate                    | 316 ms                                                 | 294 ms: 1.07x faster                                                   |
| generators                 | 31.1 ms                                                | 29.0 ms: 1.07x faster                                                  |
| logging_format             | 3.98 us                                                | 3.72 us: 1.07x faster                                                  |
| logging_simple             | 3.69 us                                                | 3.45 us: 1.07x faster                                                  |
| tomli_loads                | 1.39 sec                                               | 1.31 sec: 1.07x faster                                                 |
| pickle_dict                | 18.1 us                                                | 17.0 us: 1.06x faster                                                  |
| regex_compile              | 77.9 ms                                                | 73.6 ms: 1.06x faster                                                  |
| deepcopy_reduce            | 2.07 us                                                | 1.97 us: 1.05x faster                                                  |
| scimark_fft                | 195 ms                                                 | 186 ms: 1.05x faster                                                   |
| docutils                   | 1.50 sec                                               | 1.43 sec: 1.05x faster                                                 |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.00 ms: 1.05x faster                                                  |
| gunicorn                   | 1.15 ms                                                | 1.10 ms: 1.04x faster                                                  |
| pprint_safe_repr           | 497 ms                                                 | 477 ms: 1.04x faster                                                   |
| richards                   | 32.1 ms                                                | 30.8 ms: 1.04x faster                                                  |
| pathlib                    | 24.2 ms                                                | 23.4 ms: 1.03x faster                                                  |
| pprint_pformat             | 1.01 sec                                               | 977 ms: 1.03x faster                                                   |
| sqlalchemy_declarative     | 62.3 ms                                                | 60.5 ms: 1.03x faster                                                  |
| raytrace                   | 212 ms                                                 | 206 ms: 1.03x faster                                                   |
| sympy_expand               | 241 ms                                                 | 235 ms: 1.03x faster                                                   |
| regex_v8                   | 16.0 ms                                                | 15.5 ms: 1.03x faster                                                  |
| regex_dna                  | 154 ms                                                 | 150 ms: 1.03x faster                                                   |
| sympy_str                  | 148 ms                                                 | 144 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 515 ms: 1.02x faster                                                   |
| pycparser                  | 677 ms                                                 | 663 ms: 1.02x faster                                                   |
| sympy_integrate            | 11.4 ms                                                | 11.2 ms: 1.02x faster                                                  |
| dulwich_log                | 29.8 ms                                                | 29.5 ms: 1.01x faster                                                  |
| deltablue                  | 2.71 ms                                                | 2.68 ms: 1.01x faster                                                  |
| gc_traversal               | 2.40 ms                                                | 2.38 ms: 1.01x faster                                                  |
| pickle                     | 7.23 us                                                | 7.17 us: 1.01x faster                                                  |
| nbody                      | 68.8 ms                                                | 68.4 ms: 1.01x faster                                                  |
| pidigits                   | 282 ms                                                 | 280 ms: 1.01x faster                                                   |
| fannkuch                   | 248 ms                                                 | 247 ms: 1.01x faster                                                   |
| deepcopy                   | 235 us                                                 | 233 us: 1.01x faster                                                   |
| asyncio_websockets         | 409 ms                                                 | 407 ms: 1.01x faster                                                   |
| hexiom                     | 4.54 ms                                                | 4.54 ms: 1.00x faster                                                  |
| comprehensions             | 14.5 us                                                | 14.6 us: 1.01x slower                                                  |
| go                         | 102 ms                                                 | 102 ms: 1.01x slower                                                   |
| sqlglot_transpile          | 1.02 ms                                                | 1.03 ms: 1.01x slower                                                  |
| create_gc_cycles           | 701 us                                                 | 712 us: 1.02x slower                                                   |
| richards_super             | 36.0 ms                                                | 36.8 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 547 ms: 1.03x slower                                                   |
| unpack_sequence            | 31.5 ns                                                | 32.3 ns: 1.03x slower                                                  |
| sqlglot_parse              | 848 us                                                 | 874 us: 1.03x slower                                                   |
| async_tree_io              | 668 ms                                                 | 690 ms: 1.03x slower                                                   |
| deepcopy_memo              | 27.7 us                                                | 28.7 us: 1.04x slower                                                  |
| aiohttp                    | 1.08 ms                                                | 1.12 ms: 1.04x slower                                                  |
| async_tree_none            | 266 ms                                                 | 277 ms: 1.04x slower                                                   |
| sympy_sum                  | 77.6 ms                                                | 81.0 ms: 1.04x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 75.0 ms: 1.04x slower                                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 47.2 ms: 1.05x slower                                                  |
| pickle_pure_python         | 200 us                                                 | 210 us: 1.05x slower                                                   |
| python_startup             | 11.4 ms                                                | 12.0 ms: 1.06x slower                                                  |
| python_startup_no_site     | 9.37 ms                                                | 9.94 ms: 1.06x slower                                                  |
| coverage                   | 38.9 ms                                                | 41.3 ms: 1.06x slower                                                  |
| mako                       | 7.71 ms                                                | 8.22 ms: 1.07x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 275 ms: 1.07x slower                                                   |
| sqlalchemy_imperative      | 6.68 ms                                                | 7.19 ms: 1.08x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 722 ms: 1.08x slower                                                   |
| unpickle_pure_python       | 151 us                                                 | 163 us: 1.08x slower                                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 351 ms: 1.09x slower                                                   |
| mdp                        | 1.58 sec                                               | 1.74 sec: 1.10x slower                                                 |
| async_tree_memoization     | 312 ms                                                 | 347 ms: 1.11x slower                                                   |
| chaos                      | 42.5 ms                                                | 48.2 ms: 1.13x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.44 sec: 1.16x slower                                                 |
| json_dumps                 | 6.22 ms                                                | 7.56 ms: 1.22x slower                                                  |
| asyncio_tcp                | 449 ms                                                 | 661 ms: 1.47x slower                                                   |
| typing_runtime_protocols   | 93.0 us                                                | 322 us: 3.46x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (3): dask, float, tornado_http
Ignored benchmarks (1) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: mypy2
Ignored benchmarks (6) of results/bm-20220911-3.11.0rc2-ed7c3ff/bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.62% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x