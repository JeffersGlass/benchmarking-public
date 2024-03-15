
# Results vs. 3.12.0

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: darwin-arm64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.00x slower \*
- HPT reliability: 79.21%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 160 ms: 1.06x faster                                                  |
| chameleon      | 4.70 ms                                                | 4.29 ms: 1.09x faster                                                 |
| docutils       | 1.50 sec                                               | 1.43 sec: 1.05x faster                                                |
| Geometric mean | (ref)                                                  | 1.04x faster                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 539 ms: 1.01x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 262 ms: 1.02x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 336 ms: 1.04x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 703 ms: 1.05x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 329 ms: 1.06x slower                                                  |
| async_tree_none            | 266 ms                                                 | 281 ms: 1.06x slower                                                  |
| async_tree_io              | 668 ms                                                 | 725 ms: 1.09x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                          |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| float          | 55.8 ms                                                | 56.0 ms: 1.00x slower                                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                                          |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.44 ms: 1.08x faster                                                 |
| regex_compile  | 77.9 ms                                                | 72.7 ms: 1.07x faster                                                 |
| regex_v8       | 16.0 ms                                                | 15.0 ms: 1.07x faster                                                 |
| regex_dna      | 154 ms                                                 | 147 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 46.0 ms: 1.21x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 34.2 ms: 1.16x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 95.4 ms: 1.12x faster                                                 |
| unpickle_list        | 3.02 us                                                | 2.73 us: 1.11x faster                                                 |
| json_loads           | 17.2 us                                                | 15.6 us: 1.10x faster                                                 |
| pickle_list          | 2.89 us                                                | 2.64 us: 1.09x faster                                                 |
| unpickle             | 9.12 us                                                | 8.39 us: 1.09x faster                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 69.2 ms: 1.07x faster                                                 |
| pickle_dict          | 18.1 us                                                | 17.1 us: 1.05x faster                                                 |
| json_dumps           | 6.22 ms                                                | 5.97 ms: 1.04x faster                                                 |
| pickle               | 7.23 us                                                | 7.14 us: 1.01x faster                                                 |
| unpickle_pure_python | 151 us                                                 | 149 us: 1.01x faster                                                  |
| tomli_loads          | 1.39 sec                                               | 1.40 sec: 1.00x slower                                                |
| Geometric mean       | (ref)                                                  | 1.07x faster                                                          |

Benchmark hidden because not significant (1): pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 11.4 ms: 1.00x faster                                                 |
| python_startup_no_site | 9.37 ms                                                | 9.43 ms: 1.01x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.00x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 19.7 ms: 1.13x faster                                                 |
| mako            | 7.71 ms                                                | 7.55 ms: 1.02x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.08x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 203 ms: 1.50x faster                                                  |
| xml_etree_generate         | 55.8 ms                                                | 46.0 ms: 1.21x faster                                                 |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 2.64 ms: 1.19x faster                                                 |
| logging_silent             | 76.4 ns                                                | 65.2 ns: 1.17x faster                                                 |
| telco                      | 3.68 ms                                                | 3.15 ms: 1.17x faster                                                 |
| xml_etree_process          | 39.7 ms                                                | 34.2 ms: 1.16x faster                                                 |
| scimark_lu                 | 76.0 ms                                                | 67.0 ms: 1.13x faster                                                 |
| django_template            | 22.3 ms                                                | 19.7 ms: 1.13x faster                                                 |
| xml_etree_parse            | 106 ms                                                 | 95.4 ms: 1.12x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 167 ms: 1.11x faster                                                  |
| sqlite_synth               | 1.57 us                                                | 1.42 us: 1.11x faster                                                 |
| sqlglot_optimize           | 34.0 ms                                                | 30.7 ms: 1.11x faster                                                 |
| unpickle_list              | 3.02 us                                                | 2.73 us: 1.11x faster                                                 |
| json                       | 3.09 ms                                                | 2.79 ms: 1.11x faster                                                 |
| json_loads                 | 17.2 us                                                | 15.6 us: 1.10x faster                                                 |
| chameleon                  | 4.70 ms                                                | 4.29 ms: 1.09x faster                                                 |
| pickle_list                | 2.89 us                                                | 2.64 us: 1.09x faster                                                 |
| bench_thread_pool          | 504 us                                                 | 463 us: 1.09x faster                                                  |
| unpickle                   | 9.12 us                                                | 8.39 us: 1.09x faster                                                 |
| regex_effbot               | 2.64 ms                                                | 2.44 ms: 1.08x faster                                                 |
| spectral_norm              | 76.4 ms                                                | 70.9 ms: 1.08x faster                                                 |
| deepcopy_reduce            | 2.07 us                                                | 1.92 us: 1.08x faster                                                 |
| regex_compile              | 77.9 ms                                                | 72.7 ms: 1.07x faster                                                 |
| xml_etree_iterparse        | 74.0 ms                                                | 69.2 ms: 1.07x faster                                                 |
| regex_v8                   | 16.0 ms                                                | 15.0 ms: 1.07x faster                                                 |
| richards                   | 32.1 ms                                                | 30.2 ms: 1.06x faster                                                 |
| bench_mp_pool              | 44.9 ms                                                | 42.2 ms: 1.06x faster                                                 |
| nqueens                    | 62.4 ms                                                | 58.8 ms: 1.06x faster                                                 |
| 2to3                       | 169 ms                                                 | 160 ms: 1.06x faster                                                  |
| crypto_pyaes               | 51.9 ms                                                | 49.0 ms: 1.06x faster                                                 |
| pickle_dict                | 18.1 us                                                | 17.1 us: 1.05x faster                                                 |
| regex_dna                  | 154 ms                                                 | 147 ms: 1.05x faster                                                  |
| pathlib                    | 24.2 ms                                                | 23.1 ms: 1.05x faster                                                 |
| scimark_fft                | 195 ms                                                 | 186 ms: 1.05x faster                                                  |
| docutils                   | 1.50 sec                                               | 1.43 sec: 1.05x faster                                                |
| logging_simple             | 3.69 us                                                | 3.53 us: 1.05x faster                                                 |
| logging_format             | 3.98 us                                                | 3.82 us: 1.04x faster                                                 |
| json_dumps                 | 6.22 ms                                                | 5.97 ms: 1.04x faster                                                 |
| deepcopy                   | 235 us                                                 | 225 us: 1.04x faster                                                  |
| dulwich_log                | 29.8 ms                                                | 28.7 ms: 1.04x faster                                                 |
| pprint_safe_repr           | 497 ms                                                 | 483 ms: 1.03x faster                                                  |
| create_gc_cycles           | 701 us                                                 | 683 us: 1.03x faster                                                  |
| pycparser                  | 677 ms                                                 | 660 ms: 1.03x faster                                                  |
| deepcopy_memo              | 27.7 us                                                | 27.1 us: 1.02x faster                                                 |
| mako                       | 7.71 ms                                                | 7.55 ms: 1.02x faster                                                 |
| deltablue                  | 2.71 ms                                                | 2.67 ms: 1.01x faster                                                 |
| pprint_pformat             | 1.01 sec                                               | 998 ms: 1.01x faster                                                  |
| sympy_expand               | 241 ms                                                 | 238 ms: 1.01x faster                                                  |
| pickle                     | 7.23 us                                                | 7.14 us: 1.01x faster                                                 |
| sympy_integrate            | 11.4 ms                                                | 11.2 ms: 1.01x faster                                                 |
| sympy_str                  | 148 ms                                                 | 146 ms: 1.01x faster                                                  |
| unpickle_pure_python       | 151 us                                                 | 149 us: 1.01x faster                                                  |
| pidigits                   | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| gc_traversal               | 2.40 ms                                                | 2.39 ms: 1.01x faster                                                 |
| python_startup             | 11.4 ms                                                | 11.4 ms: 1.00x faster                                                 |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                                  |
| float                      | 55.8 ms                                                | 56.0 ms: 1.00x slower                                                 |
| tomli_loads                | 1.39 sec                                               | 1.40 sec: 1.00x slower                                                |
| coroutines                 | 19.2 ms                                                | 19.3 ms: 1.00x slower                                                 |
| python_startup_no_site     | 9.37 ms                                                | 9.43 ms: 1.01x slower                                                 |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 539 ms: 1.01x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 262 ms: 1.02x slower                                                  |
| richards_super             | 36.0 ms                                                | 36.7 ms: 1.02x slower                                                 |
| raytrace                   | 212 ms                                                 | 220 ms: 1.04x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 336 ms: 1.04x slower                                                  |
| pyflate                    | 316 ms                                                 | 329 ms: 1.04x slower                                                  |
| fannkuch                   | 248 ms                                                 | 260 ms: 1.05x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 703 ms: 1.05x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 75.6 ms: 1.05x slower                                                 |
| async_tree_memoization     | 312 ms                                                 | 329 ms: 1.06x slower                                                  |
| async_tree_none            | 266 ms                                                 | 281 ms: 1.06x slower                                                  |
| hexiom                     | 4.54 ms                                                | 4.83 ms: 1.06x slower                                                 |
| sympy_sum                  | 77.6 ms                                                | 82.6 ms: 1.06x slower                                                 |
| unpack_sequence            | 31.5 ns                                                | 33.8 ns: 1.08x slower                                                 |
| async_tree_io              | 668 ms                                                 | 725 ms: 1.09x slower                                                  |
| sqlglot_transpile          | 1.02 ms                                                | 1.12 ms: 1.09x slower                                                 |
| comprehensions             | 14.5 us                                                | 15.9 us: 1.09x slower                                                 |
| mdp                        | 1.58 sec                                               | 1.74 sec: 1.10x slower                                                |
| sqlglot_parse              | 848 us                                                 | 954 us: 1.12x slower                                                  |
| go                         | 102 ms                                                 | 115 ms: 1.13x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.43 sec: 1.15x slower                                                |
| scimark_monte_carlo        | 45.0 ms                                                | 52.5 ms: 1.17x slower                                                 |
| chaos                      | 42.5 ms                                                | 49.7 ms: 1.17x slower                                                 |
| generators                 | 31.1 ms                                                | 36.6 ms: 1.18x slower                                                 |
| scimark_sor                | 87.4 ms                                                | 103 ms: 1.18x slower                                                  |
| dask                       | 222 ms                                                 | 320 ms: 1.44x slower                                                  |
| asyncio_tcp                | 449 ms                                                 | 658 ms: 1.47x slower                                                  |
| typing_runtime_protocols   | 93.0 us                                                | 325 us: 3.50x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                          |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed, nbody, pickle_pure_python, tornado_http
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, coverage, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20221114-3.12.0a2-3b9d793/bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 79.21% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.95x