
# Results vs. 3.12.0

- fork: python
- ref: 72f00f420afaba3bc873
- machine: darwin-arm64
- commit hash: 72f00f4
- commit date: 2022-05-30
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.82%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 153 ms: 1.10x faster                                                  |
| chameleon      | 4.70 ms                                                | 4.32 ms: 1.09x faster                                                 |
| docutils       | 1.50 sec                                               | 1.42 sec: 1.05x faster                                                |
| Geometric mean | (ref)                                                  | 1.06x faster                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 514 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 548 ms: 1.03x slower                                                  |
| async_tree_io              | 668 ms                                                 | 688 ms: 1.03x slower                                                  |
| async_tree_none            | 266 ms                                                 | 278 ms: 1.05x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 341 ms: 1.06x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 273 ms: 1.06x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 721 ms: 1.08x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 363 ms: 1.16x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.05x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 68.8 ms                                                | 65.5 ms: 1.05x faster                                                 |
| float          | 55.8 ms                                                | 54.4 ms: 1.03x faster                                                 |
| pidigits       | 282 ms                                                 | 280 ms: 1.00x faster                                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.22 ms: 1.19x faster                                                 |
| regex_compile  | 77.9 ms                                                | 73.8 ms: 1.05x faster                                                 |
| regex_dna      | 154 ms                                                 | 147 ms: 1.05x faster                                                  |
| regex_v8       | 16.0 ms                                                | 15.2 ms: 1.05x faster                                                 |
| Geometric mean | (ref)                                                  | 1.08x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|---------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_generate  | 55.8 ms                                                | 46.7 ms: 1.20x faster                                                 |
| xml_etree_process   | 39.7 ms                                                | 33.9 ms: 1.17x faster                                                 |
| pickle_dict         | 18.1 us                                                | 16.1 us: 1.12x faster                                                 |
| json_loads          | 17.2 us                                                | 15.4 us: 1.12x faster                                                 |
| pickle_list         | 2.89 us                                                | 2.59 us: 1.11x faster                                                 |
| unpickle            | 9.12 us                                                | 8.23 us: 1.11x faster                                                 |
| xml_etree_iterparse | 74.0 ms                                                | 66.9 ms: 1.11x faster                                                 |
| xml_etree_parse     | 106 ms                                                 | 97.2 ms: 1.09x faster                                                 |
| unpickle_list       | 3.02 us                                                | 2.80 us: 1.08x faster                                                 |
| tomli_loads         | 1.39 sec                                               | 1.30 sec: 1.07x faster                                                |
| pickle_pure_python  | 200 us                                                 | 194 us: 1.03x faster                                                  |
| pickle              | 7.23 us                                                | 7.03 us: 1.03x faster                                                 |
| json_dumps          | 6.22 ms                                                | 7.58 ms: 1.22x slower                                                 |
| Geometric mean      | (ref)                                                  | 1.07x faster                                                          |

Benchmark hidden because not significant (1): unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 9.31 ms: 1.01x faster                                                 |
| python_startup         | 11.4 ms                                                | 11.4 ms: 1.00x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.00x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 19.8 ms: 1.13x faster                                                 |
| mako            | 7.71 ms                                                | 8.11 ms: 1.05x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.03x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 191 ms: 1.60x faster                                                  |
| sqlite_synth               | 1.57 us                                                | 1.31 us: 1.20x faster                                                 |
| xml_etree_generate         | 55.8 ms                                                | 46.7 ms: 1.20x faster                                                 |
| regex_effbot               | 2.64 ms                                                | 2.22 ms: 1.19x faster                                                 |
| xml_etree_process          | 39.7 ms                                                | 33.9 ms: 1.17x faster                                                 |
| telco                      | 3.68 ms                                                | 3.17 ms: 1.16x faster                                                 |
| logging_silent             | 76.4 ns                                                | 66.3 ns: 1.15x faster                                                 |
| scimark_sor                | 87.4 ms                                                | 76.1 ms: 1.15x faster                                                 |
| nqueens                    | 62.4 ms                                                | 54.7 ms: 1.14x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 163 ms: 1.14x faster                                                  |
| coroutines                 | 19.2 ms                                                | 17.0 ms: 1.13x faster                                                 |
| django_template            | 22.3 ms                                                | 19.8 ms: 1.13x faster                                                 |
| pickle_dict                | 18.1 us                                                | 16.1 us: 1.12x faster                                                 |
| json_loads                 | 17.2 us                                                | 15.4 us: 1.12x faster                                                 |
| sqlglot_optimize           | 34.0 ms                                                | 30.4 ms: 1.12x faster                                                 |
| spectral_norm              | 76.4 ms                                                | 68.4 ms: 1.12x faster                                                 |
| pickle_list                | 2.89 us                                                | 2.59 us: 1.11x faster                                                 |
| scimark_lu                 | 76.0 ms                                                | 68.2 ms: 1.11x faster                                                 |
| pyflate                    | 316 ms                                                 | 285 ms: 1.11x faster                                                  |
| unpickle                   | 9.12 us                                                | 8.23 us: 1.11x faster                                                 |
| xml_etree_iterparse        | 74.0 ms                                                | 66.9 ms: 1.11x faster                                                 |
| json                       | 3.09 ms                                                | 2.79 ms: 1.11x faster                                                 |
| 2to3                       | 169 ms                                                 | 153 ms: 1.10x faster                                                  |
| logging_format             | 3.98 us                                                | 3.63 us: 1.10x faster                                                 |
| crypto_pyaes               | 51.9 ms                                                | 47.4 ms: 1.09x faster                                                 |
| logging_simple             | 3.69 us                                                | 3.37 us: 1.09x faster                                                 |
| xml_etree_parse            | 106 ms                                                 | 97.2 ms: 1.09x faster                                                 |
| chameleon                  | 4.70 ms                                                | 4.32 ms: 1.09x faster                                                 |
| bench_thread_pool          | 504 us                                                 | 466 us: 1.08x faster                                                  |
| bench_mp_pool              | 44.9 ms                                                | 41.6 ms: 1.08x faster                                                 |
| unpickle_list              | 3.02 us                                                | 2.80 us: 1.08x faster                                                 |
| deepcopy_reduce            | 2.07 us                                                | 1.93 us: 1.07x faster                                                 |
| tomli_loads                | 1.39 sec                                               | 1.30 sec: 1.07x faster                                                |
| scimark_fft                | 195 ms                                                 | 183 ms: 1.07x faster                                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 2.95 ms: 1.06x faster                                                 |
| raytrace                   | 212 ms                                                 | 200 ms: 1.06x faster                                                  |
| regex_compile              | 77.9 ms                                                | 73.8 ms: 1.05x faster                                                 |
| docutils                   | 1.50 sec                                               | 1.42 sec: 1.05x faster                                                |
| nbody                      | 68.8 ms                                                | 65.5 ms: 1.05x faster                                                 |
| regex_dna                  | 154 ms                                                 | 147 ms: 1.05x faster                                                  |
| sqlalchemy_declarative     | 62.3 ms                                                | 59.5 ms: 1.05x faster                                                 |
| regex_v8                   | 16.0 ms                                                | 15.2 ms: 1.05x faster                                                 |
| pathlib                    | 24.2 ms                                                | 23.2 ms: 1.04x faster                                                 |
| dulwich_log                | 29.8 ms                                                | 28.7 ms: 1.04x faster                                                 |
| generators                 | 31.1 ms                                                | 30.0 ms: 1.04x faster                                                 |
| sympy_expand               | 241 ms                                                 | 233 ms: 1.04x faster                                                  |
| sympy_str                  | 148 ms                                                 | 143 ms: 1.03x faster                                                  |
| deepcopy                   | 235 us                                                 | 228 us: 1.03x faster                                                  |
| pickle_pure_python         | 200 us                                                 | 194 us: 1.03x faster                                                  |
| pickle                     | 7.23 us                                                | 7.03 us: 1.03x faster                                                 |
| richards                   | 32.1 ms                                                | 31.3 ms: 1.03x faster                                                 |
| pycparser                  | 677 ms                                                 | 660 ms: 1.03x faster                                                  |
| float                      | 55.8 ms                                                | 54.4 ms: 1.03x faster                                                 |
| pprint_safe_repr           | 497 ms                                                 | 485 ms: 1.03x faster                                                  |
| pprint_pformat             | 1.01 sec                                               | 988 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 514 ms: 1.02x faster                                                  |
| sympy_integrate            | 11.4 ms                                                | 11.1 ms: 1.02x faster                                                 |
| fannkuch                   | 248 ms                                                 | 244 ms: 1.02x faster                                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 44.3 ms: 1.02x faster                                                 |
| dask                       | 222 ms                                                 | 219 ms: 1.02x faster                                                  |
| python_startup_no_site     | 9.37 ms                                                | 9.31 ms: 1.01x faster                                                 |
| gc_traversal               | 2.40 ms                                                | 2.38 ms: 1.01x faster                                                 |
| asyncio_websockets         | 409 ms                                                 | 407 ms: 1.01x faster                                                  |
| pidigits                   | 282 ms                                                 | 280 ms: 1.00x faster                                                  |
| python_startup             | 11.4 ms                                                | 11.4 ms: 1.00x slower                                                 |
| deepcopy_memo              | 27.7 us                                                | 27.8 us: 1.00x slower                                                 |
| deltablue                  | 2.71 ms                                                | 2.72 ms: 1.01x slower                                                 |
| sympy_sum                  | 77.6 ms                                                | 78.2 ms: 1.01x slower                                                 |
| hexiom                     | 4.54 ms                                                | 4.58 ms: 1.01x slower                                                 |
| meteor_contest             | 71.7 ms                                                | 72.5 ms: 1.01x slower                                                 |
| create_gc_cycles           | 701 us                                                 | 711 us: 1.01x slower                                                  |
| go                         | 102 ms                                                 | 103 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 548 ms: 1.03x slower                                                  |
| async_tree_io              | 668 ms                                                 | 688 ms: 1.03x slower                                                  |
| gunicorn                   | 1.15 ms                                                | 1.18 ms: 1.03x slower                                                 |
| unpack_sequence            | 31.5 ns                                                | 32.7 ns: 1.04x slower                                                 |
| sqlalchemy_imperative      | 6.68 ms                                                | 6.97 ms: 1.04x slower                                                 |
| async_tree_none            | 266 ms                                                 | 278 ms: 1.05x slower                                                  |
| richards_super             | 36.0 ms                                                | 37.8 ms: 1.05x slower                                                 |
| mako                       | 7.71 ms                                                | 8.11 ms: 1.05x slower                                                 |
| async_tree_memoization_tg  | 323 ms                                                 | 341 ms: 1.06x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 273 ms: 1.06x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 721 ms: 1.08x slower                                                  |
| mdp                        | 1.58 sec                                               | 1.74 sec: 1.10x slower                                                |
| chaos                      | 42.5 ms                                                | 47.8 ms: 1.12x slower                                                 |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.43 sec: 1.15x slower                                                |
| async_tree_memoization     | 312 ms                                                 | 363 ms: 1.16x slower                                                  |
| comprehensions             | 14.5 us                                                | 17.2 us: 1.18x slower                                                 |
| json_dumps                 | 6.22 ms                                                | 7.58 ms: 1.22x slower                                                 |
| sqlglot_transpile          | 1.02 ms                                                | 1.30 ms: 1.27x slower                                                 |
| sqlglot_parse              | 848 us                                                 | 1.14 ms: 1.34x slower                                                 |
| asyncio_tcp                | 449 ms                                                 | 665 ms: 1.48x slower                                                  |
| coverage                   | 38.9 ms                                                | 72.4 ms: 1.86x slower                                                 |
| typing_runtime_protocols   | 93.0 us                                                | 326 us: 3.50x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                          |

Benchmark hidden because not significant (3): tornado_http, unpickle_pure_python, aiohttp
Ignored benchmarks (1) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: mypy2
Ignored benchmarks (5) of results/bm-20220530-3.11.0b2-72f00f4/bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.82% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x