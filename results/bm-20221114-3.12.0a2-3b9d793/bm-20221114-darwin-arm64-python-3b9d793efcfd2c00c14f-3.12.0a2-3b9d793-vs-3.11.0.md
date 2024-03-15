
# Results vs. 3.11.0

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: darwin-arm64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.03x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 160 ms: 1.04x slower                                                  |
| docutils       | 1.43 sec                                               | 1.43 sec: 1.00x slower                                                |
| html5lib       | 33.0 ms                                                | 33.4 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                  | 1.02x slower                                                          |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none_tg         | 276 ms                                                 | 262 ms: 1.06x faster                                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 336 ms: 1.05x faster                                                  |
| async_tree_io_tg           | 724 ms                                                 | 703 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 539 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 522 ms: 1.01x slower                                                  |
| async_tree_io              | 697 ms                                                 | 725 ms: 1.04x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                          |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 50.8 ms                                                | 56.0 ms: 1.10x slower                                                 |
| nbody          | 61.7 ms                                                | 68.8 ms: 1.11x slower                                                 |
| Geometric mean | (ref)                                                  | 1.07x slower                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_v8       | 15.1 ms                                                | 15.0 ms: 1.01x faster                                                 |
| regex_dna      | 148 ms                                                 | 147 ms: 1.01x faster                                                  |
| regex_compile  | 72.8 ms                                                | 72.7 ms: 1.00x faster                                                 |
| regex_effbot   | 2.43 ms                                                | 2.44 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 5.97 ms: 1.26x faster                                                 |
| xml_etree_parse      | 100 ms                                                 | 95.4 ms: 1.05x faster                                                 |
| pickle_list          | 2.70 us                                                | 2.64 us: 1.02x faster                                                 |
| pickle_dict          | 17.1 us                                                | 17.1 us: 1.00x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 46.0 ms: 1.00x slower                                                 |
| unpickle_pure_python | 149 us                                                 | 149 us: 1.00x slower                                                  |
| unpickle             | 8.29 us                                                | 8.39 us: 1.01x slower                                                 |
| xml_etree_iterparse  | 68.3 ms                                                | 69.2 ms: 1.01x slower                                                 |
| unpickle_list        | 2.69 us                                                | 2.73 us: 1.02x slower                                                 |
| json_loads           | 15.3 us                                                | 15.6 us: 1.02x slower                                                 |
| xml_etree_process    | 33.6 ms                                                | 34.2 ms: 1.02x slower                                                 |
| pickle               | 6.98 us                                                | 7.14 us: 1.02x slower                                                 |
| pickle_pure_python   | 191 us                                                 | 200 us: 1.04x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.40 sec: 1.10x slower                                                |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.4 ms: 1.06x slower                                                 |
| python_startup_no_site | 8.57 ms                                                | 9.43 ms: 1.10x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.08x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.93 ms                                                | 7.55 ms: 1.05x faster                                                 |
| django_template | 20.1 ms                                                | 19.7 ms: 1.02x faster                                                 |
| genshi_xml      | 28.5 ms                                                | 28.3 ms: 1.01x faster                                                 |
| genshi_text     | 14.4 ms                                                | 14.9 ms: 1.03x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.01x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-darwin-arm64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps                 | 7.53 ms                                                | 5.97 ms: 1.26x faster                                                 |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 2.64 ms: 1.07x faster                                                 |
| async_tree_none_tg         | 276 ms                                                 | 262 ms: 1.06x faster                                                  |
| xml_etree_parse            | 100 ms                                                 | 95.4 ms: 1.05x faster                                                 |
| mako                       | 7.93 ms                                                | 7.55 ms: 1.05x faster                                                 |
| async_tree_memoization_tg  | 352 ms                                                 | 336 ms: 1.05x faster                                                  |
| create_gc_cycles           | 711 us                                                 | 683 us: 1.04x faster                                                  |
| deltablue                  | 2.75 ms                                                | 2.67 ms: 1.03x faster                                                 |
| async_tree_io_tg           | 724 ms                                                 | 703 ms: 1.03x faster                                                  |
| richards                   | 31.1 ms                                                | 30.2 ms: 1.03x faster                                                 |
| django_template            | 20.1 ms                                                | 19.7 ms: 1.02x faster                                                 |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 539 ms: 1.02x faster                                                  |
| pickle_list                | 2.70 us                                                | 2.64 us: 1.02x faster                                                 |
| logging_silent             | 66.5 ns                                                | 65.2 ns: 1.02x faster                                                 |
| richards_super             | 37.3 ms                                                | 36.7 ms: 1.02x faster                                                 |
| regex_v8                   | 15.1 ms                                                | 15.0 ms: 1.01x faster                                                 |
| scimark_lu                 | 67.7 ms                                                | 67.0 ms: 1.01x faster                                                 |
| regex_dna                  | 148 ms                                                 | 147 ms: 1.01x faster                                                  |
| genshi_xml                 | 28.5 ms                                                | 28.3 ms: 1.01x faster                                                 |
| telco                      | 3.17 ms                                                | 3.15 ms: 1.01x faster                                                 |
| bench_thread_pool          | 465 us                                                 | 463 us: 1.01x faster                                                  |
| regex_compile              | 72.8 ms                                                | 72.7 ms: 1.00x faster                                                 |
| pickle_dict                | 17.1 us                                                | 17.1 us: 1.00x slower                                                 |
| docutils                   | 1.43 sec                                               | 1.43 sec: 1.00x slower                                                |
| xml_etree_generate         | 45.8 ms                                                | 46.0 ms: 1.00x slower                                                 |
| unpickle_pure_python       | 149 us                                                 | 149 us: 1.00x slower                                                  |
| regex_effbot               | 2.43 ms                                                | 2.44 ms: 1.01x slower                                                 |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 522 ms: 1.01x slower                                                  |
| pprint_safe_repr           | 478 ms                                                 | 483 ms: 1.01x slower                                                  |
| unpickle                   | 8.29 us                                                | 8.39 us: 1.01x slower                                                 |
| xml_etree_iterparse        | 68.3 ms                                                | 69.2 ms: 1.01x slower                                                 |
| html5lib                   | 33.0 ms                                                | 33.4 ms: 1.01x slower                                                 |
| json                       | 2.75 ms                                                | 2.79 ms: 1.01x slower                                                 |
| unpickle_list              | 2.69 us                                                | 2.73 us: 1.02x slower                                                 |
| json_loads                 | 15.3 us                                                | 15.6 us: 1.02x slower                                                 |
| xml_etree_process          | 33.6 ms                                                | 34.2 ms: 1.02x slower                                                 |
| sympy_str                  | 144 ms                                                 | 146 ms: 1.02x slower                                                  |
| pprint_pformat             | 979 ms                                                 | 998 ms: 1.02x slower                                                  |
| asyncio_tcp                | 643 ms                                                 | 658 ms: 1.02x slower                                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.43 sec: 1.02x slower                                                |
| pickle                     | 6.98 us                                                | 7.14 us: 1.02x slower                                                 |
| bench_mp_pool              | 41.0 ms                                                | 42.2 ms: 1.03x slower                                                 |
| sympy_sum                  | 80.2 ms                                                | 82.6 ms: 1.03x slower                                                 |
| sqlglot_normalize          | 162 ms                                                 | 167 ms: 1.03x slower                                                  |
| thrift                     | 410 us                                                 | 424 us: 1.03x slower                                                  |
| crypto_pyaes               | 47.5 ms                                                | 49.0 ms: 1.03x slower                                                 |
| genshi_text                | 14.4 ms                                                | 14.9 ms: 1.03x slower                                                 |
| logging_simple             | 3.41 us                                                | 3.53 us: 1.03x slower                                                 |
| sqlglot_optimize           | 29.6 ms                                                | 30.7 ms: 1.04x slower                                                 |
| 2to3                       | 154 ms                                                 | 160 ms: 1.04x slower                                                  |
| async_tree_io              | 697 ms                                                 | 725 ms: 1.04x slower                                                  |
| logging_format             | 3.67 us                                                | 3.82 us: 1.04x slower                                                 |
| sympy_expand               | 229 ms                                                 | 238 ms: 1.04x slower                                                  |
| pickle_pure_python         | 191 us                                                 | 200 us: 1.04x slower                                                  |
| deepcopy                   | 215 us                                                 | 225 us: 1.05x slower                                                  |
| chaos                      | 47.4 ms                                                | 49.7 ms: 1.05x slower                                                 |
| deepcopy_memo              | 25.7 us                                                | 27.1 us: 1.05x slower                                                 |
| nqueens                    | 55.9 ms                                                | 58.8 ms: 1.05x slower                                                 |
| hexiom                     | 4.58 ms                                                | 4.83 ms: 1.05x slower                                                 |
| async_generators           | 192 ms                                                 | 203 ms: 1.06x slower                                                  |
| python_startup             | 10.8 ms                                                | 11.4 ms: 1.06x slower                                                 |
| sqlglot_transpile          | 1.05 ms                                                | 1.12 ms: 1.06x slower                                                 |
| meteor_contest             | 71.1 ms                                                | 75.6 ms: 1.06x slower                                                 |
| raytrace                   | 206 ms                                                 | 220 ms: 1.07x slower                                                  |
| deepcopy_reduce            | 1.79 us                                                | 1.92 us: 1.07x slower                                                 |
| sqlglot_parse              | 890 us                                                 | 954 us: 1.07x slower                                                  |
| scimark_fft                | 173 ms                                                 | 186 ms: 1.08x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 70.9 ms: 1.08x slower                                                 |
| typing_runtime_protocols   | 301 us                                                 | 325 us: 1.08x slower                                                  |
| fannkuch                   | 240 ms                                                 | 260 ms: 1.09x slower                                                  |
| go                         | 105 ms                                                 | 115 ms: 1.09x slower                                                  |
| tomli_loads                | 1.27 sec                                               | 1.40 sec: 1.10x slower                                                |
| python_startup_no_site     | 8.57 ms                                                | 9.43 ms: 1.10x slower                                                 |
| float                      | 50.8 ms                                                | 56.0 ms: 1.10x slower                                                 |
| comprehensions             | 14.4 us                                                | 15.9 us: 1.10x slower                                                 |
| nbody                      | 61.7 ms                                                | 68.8 ms: 1.11x slower                                                 |
| coroutines                 | 17.2 ms                                                | 19.3 ms: 1.13x slower                                                 |
| sqlite_synth               | 1.26 us                                                | 1.42 us: 1.13x slower                                                 |
| pyflate                    | 284 ms                                                 | 329 ms: 1.16x slower                                                  |
| mdp                        | 1.48 sec                                               | 1.74 sec: 1.17x slower                                                |
| generators                 | 30.3 ms                                                | 36.6 ms: 1.21x slower                                                 |
| scimark_monte_carlo        | 43.5 ms                                                | 52.5 ms: 1.21x slower                                                 |
| scimark_sor                | 79.2 ms                                                | 103 ms: 1.30x slower                                                  |
| dask                       | 219 ms                                                 | 320 ms: 1.46x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                          |

Benchmark hidden because not significant (12): async_tree_memoization, pathlib, sympy_integrate, async_tree_none, chameleon, pidigits, asyncio_websockets, gc_traversal, pycparser, dulwich_log, unpack_sequence, tornado_http
Ignored benchmarks (8) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.98x