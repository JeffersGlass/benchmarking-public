
# Results vs. 3.12.0

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: darwin-arm64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.01x faster \*
- HPT reliability: 88.33%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 159 ms: 1.07x faster                                                  |
| chameleon      | 4.70 ms                                                | 4.35 ms: 1.08x faster                                                 |
| docutils       | 1.50 sec                                               | 1.45 sec: 1.03x faster                                                |
| Geometric mean | (ref)                                                  | 1.04x faster                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 537 ms: 1.01x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 262 ms: 1.02x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 322 ms: 1.03x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 697 ms: 1.04x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 336 ms: 1.04x slower                                                  |
| async_tree_none            | 266 ms                                                 | 281 ms: 1.06x slower                                                  |
| async_tree_io              | 668 ms                                                 | 723 ms: 1.08x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                          |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| nbody          | 68.8 ms                                                | 69.0 ms: 1.00x slower                                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                                          |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.44 ms: 1.08x faster                                                 |
| regex_compile  | 77.9 ms                                                | 73.0 ms: 1.07x faster                                                 |
| regex_v8       | 16.0 ms                                                | 15.0 ms: 1.06x faster                                                 |
| regex_dna      | 154 ms                                                 | 148 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.06x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 46.0 ms: 1.21x faster                                                 |
| unpickle_list        | 3.02 us                                                | 2.52 us: 1.20x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 33.8 ms: 1.17x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 90.9 ms: 1.17x faster                                                 |
| json_loads           | 17.2 us                                                | 15.6 us: 1.10x faster                                                 |
| unpickle             | 9.12 us                                                | 8.27 us: 1.10x faster                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 67.9 ms: 1.09x faster                                                 |
| pickle_list          | 2.89 us                                                | 2.70 us: 1.07x faster                                                 |
| pickle_dict          | 18.1 us                                                | 16.9 us: 1.07x faster                                                 |
| json_dumps           | 6.22 ms                                                | 6.04 ms: 1.03x faster                                                 |
| pickle               | 7.23 us                                                | 7.13 us: 1.01x faster                                                 |
| pickle_pure_python   | 200 us                                                 | 201 us: 1.01x slower                                                  |
| tomli_loads          | 1.39 sec                                               | 1.42 sec: 1.02x slower                                                |
| unpickle_pure_python | 151 us                                                 | 154 us: 1.02x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.08x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 11.3 ms: 1.01x faster                                                 |
| python_startup_no_site | 9.37 ms                                                | 9.36 ms: 1.00x faster                                                 |
| Geometric mean         | (ref)                                                  | 1.00x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 20.0 ms: 1.12x faster                                                 |
| mako            | 7.71 ms                                                | 7.66 ms: 1.01x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.06x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 195 ms: 1.56x faster                                                  |
| xml_etree_generate         | 55.8 ms                                                | 46.0 ms: 1.21x faster                                                 |
| logging_silent             | 76.4 ns                                                | 63.1 ns: 1.21x faster                                                 |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 2.61 ms: 1.20x faster                                                 |
| unpickle_list              | 3.02 us                                                | 2.52 us: 1.20x faster                                                 |
| xml_etree_process          | 39.7 ms                                                | 33.8 ms: 1.17x faster                                                 |
| xml_etree_parse            | 106 ms                                                 | 90.9 ms: 1.17x faster                                                 |
| telco                      | 3.68 ms                                                | 3.20 ms: 1.15x faster                                                 |
| scimark_lu                 | 76.0 ms                                                | 67.4 ms: 1.13x faster                                                 |
| nqueens                    | 62.4 ms                                                | 55.6 ms: 1.12x faster                                                 |
| django_template            | 22.3 ms                                                | 20.0 ms: 1.12x faster                                                 |
| sqlglot_optimize           | 34.0 ms                                                | 30.5 ms: 1.12x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 167 ms: 1.12x faster                                                  |
| sqlite_synth               | 1.57 us                                                | 1.42 us: 1.11x faster                                                 |
| bench_thread_pool          | 504 us                                                 | 457 us: 1.10x faster                                                  |
| json_loads                 | 17.2 us                                                | 15.6 us: 1.10x faster                                                 |
| unpickle                   | 9.12 us                                                | 8.27 us: 1.10x faster                                                 |
| spectral_norm              | 76.4 ms                                                | 69.5 ms: 1.10x faster                                                 |
| json                       | 3.09 ms                                                | 2.82 ms: 1.10x faster                                                 |
| xml_etree_iterparse        | 74.0 ms                                                | 67.9 ms: 1.09x faster                                                 |
| regex_effbot               | 2.64 ms                                                | 2.44 ms: 1.08x faster                                                 |
| deepcopy_reduce            | 2.07 us                                                | 1.92 us: 1.08x faster                                                 |
| chameleon                  | 4.70 ms                                                | 4.35 ms: 1.08x faster                                                 |
| bench_mp_pool              | 44.9 ms                                                | 41.7 ms: 1.07x faster                                                 |
| crypto_pyaes               | 51.9 ms                                                | 48.4 ms: 1.07x faster                                                 |
| 2to3                       | 169 ms                                                 | 159 ms: 1.07x faster                                                  |
| pickle_list                | 2.89 us                                                | 2.70 us: 1.07x faster                                                 |
| coroutines                 | 19.2 ms                                                | 18.0 ms: 1.07x faster                                                 |
| regex_compile              | 77.9 ms                                                | 73.0 ms: 1.07x faster                                                 |
| pickle_dict                | 18.1 us                                                | 16.9 us: 1.07x faster                                                 |
| regex_v8                   | 16.0 ms                                                | 15.0 ms: 1.06x faster                                                 |
| scimark_fft                | 195 ms                                                 | 185 ms: 1.06x faster                                                  |
| pathlib                    | 24.2 ms                                                | 23.1 ms: 1.05x faster                                                 |
| regex_dna                  | 154 ms                                                 | 148 ms: 1.04x faster                                                  |
| dulwich_log                | 29.8 ms                                                | 28.8 ms: 1.04x faster                                                 |
| deepcopy                   | 235 us                                                 | 227 us: 1.04x faster                                                  |
| docutils                   | 1.50 sec                                               | 1.45 sec: 1.03x faster                                                |
| logging_format             | 3.98 us                                                | 3.85 us: 1.03x faster                                                 |
| logging_simple             | 3.69 us                                                | 3.58 us: 1.03x faster                                                 |
| generators                 | 31.1 ms                                                | 30.2 ms: 1.03x faster                                                 |
| json_dumps                 | 6.22 ms                                                | 6.04 ms: 1.03x faster                                                 |
| pprint_safe_repr           | 497 ms                                                 | 484 ms: 1.03x faster                                                  |
| sympy_expand               | 241 ms                                                 | 235 ms: 1.03x faster                                                  |
| sympy_integrate            | 11.4 ms                                                | 11.1 ms: 1.03x faster                                                 |
| raytrace                   | 212 ms                                                 | 207 ms: 1.02x faster                                                  |
| sympy_str                  | 148 ms                                                 | 144 ms: 1.02x faster                                                  |
| pprint_pformat             | 1.01 sec                                               | 990 ms: 1.02x faster                                                  |
| create_gc_cycles           | 701 us                                                 | 687 us: 1.02x faster                                                  |
| deepcopy_memo              | 27.7 us                                                | 27.3 us: 1.02x faster                                                 |
| pycparser                  | 677 ms                                                 | 668 ms: 1.01x faster                                                  |
| pickle                     | 7.23 us                                                | 7.13 us: 1.01x faster                                                 |
| python_startup             | 11.4 ms                                                | 11.3 ms: 1.01x faster                                                 |
| mako                       | 7.71 ms                                                | 7.66 ms: 1.01x faster                                                 |
| pidigits                   | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                                  |
| python_startup_no_site     | 9.37 ms                                                | 9.36 ms: 1.00x faster                                                 |
| gc_traversal               | 2.40 ms                                                | 2.40 ms: 1.00x slower                                                 |
| nbody                      | 68.8 ms                                                | 69.0 ms: 1.00x slower                                                 |
| pickle_pure_python         | 200 us                                                 | 201 us: 1.01x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 537 ms: 1.01x slower                                                  |
| richards                   | 32.1 ms                                                | 32.5 ms: 1.01x slower                                                 |
| tomli_loads                | 1.39 sec                                               | 1.42 sec: 1.02x slower                                                |
| deltablue                  | 2.71 ms                                                | 2.75 ms: 1.02x slower                                                 |
| async_tree_none_tg         | 258 ms                                                 | 262 ms: 1.02x slower                                                  |
| comprehensions             | 14.5 us                                                | 14.8 us: 1.02x slower                                                 |
| unpickle_pure_python       | 151 us                                                 | 154 us: 1.02x slower                                                  |
| hexiom                     | 4.54 ms                                                | 4.68 ms: 1.03x slower                                                 |
| async_tree_memoization     | 312 ms                                                 | 322 ms: 1.03x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 697 ms: 1.04x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 336 ms: 1.04x slower                                                  |
| fannkuch                   | 248 ms                                                 | 260 ms: 1.05x slower                                                  |
| pyflate                    | 316 ms                                                 | 331 ms: 1.05x slower                                                  |
| sympy_sum                  | 77.6 ms                                                | 81.5 ms: 1.05x slower                                                 |
| async_tree_none            | 266 ms                                                 | 281 ms: 1.06x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 76.4 ms: 1.06x slower                                                 |
| richards_super             | 36.0 ms                                                | 38.6 ms: 1.07x slower                                                 |
| sqlglot_transpile          | 1.02 ms                                                | 1.10 ms: 1.08x slower                                                 |
| mdp                        | 1.58 sec                                               | 1.71 sec: 1.08x slower                                                |
| async_tree_io              | 668 ms                                                 | 723 ms: 1.08x slower                                                  |
| unpack_sequence            | 31.5 ns                                                | 34.1 ns: 1.08x slower                                                 |
| sqlglot_parse              | 848 us                                                 | 940 us: 1.11x slower                                                  |
| go                         | 102 ms                                                 | 114 ms: 1.13x slower                                                  |
| chaos                      | 42.5 ms                                                | 48.6 ms: 1.14x slower                                                 |
| scimark_sor                | 87.4 ms                                                | 100 ms: 1.15x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.43 sec: 1.15x slower                                                |
| scimark_monte_carlo        | 45.0 ms                                                | 52.9 ms: 1.18x slower                                                 |
| dask                       | 222 ms                                                 | 322 ms: 1.45x slower                                                  |
| asyncio_tcp                | 449 ms                                                 | 659 ms: 1.47x slower                                                  |
| typing_runtime_protocols   | 93.0 us                                                | 321 us: 3.46x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                          |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, tornado_http, float
Ignored benchmarks (6) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, coverage, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20221025-3.12.0a1-4ae1a0e/bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 88.33% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x