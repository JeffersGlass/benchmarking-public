
# Results vs. 3.11.0

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: darwin-arm64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.03x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 159 ms: 1.03x slower                                                  |
| chameleon      | 4.30 ms                                                | 4.35 ms: 1.01x slower                                                 |
| docutils       | 1.43 sec                                               | 1.45 sec: 1.02x slower                                                |
| html5lib       | 33.0 ms                                                | 33.9 ms: 1.03x slower                                                 |
| Geometric mean | (ref)                                                  | 1.02x slower                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none_tg         | 276 ms                                                 | 262 ms: 1.05x faster                                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 336 ms: 1.05x faster                                                  |
| async_tree_memoization     | 336 ms                                                 | 322 ms: 1.04x faster                                                  |
| async_tree_io_tg           | 724 ms                                                 | 697 ms: 1.04x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 537 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 523 ms: 1.01x slower                                                  |
| async_tree_io              | 697 ms                                                 | 723 ms: 1.04x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                          |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 50.8 ms                                                | 55.9 ms: 1.10x slower                                                 |
| nbody          | 61.7 ms                                                | 69.0 ms: 1.12x slower                                                 |
| Geometric mean | (ref)                                                  | 1.07x slower                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_v8       | 15.1 ms                                                | 15.0 ms: 1.01x faster                                                 |
| regex_dna      | 148 ms                                                 | 148 ms: 1.00x faster                                                  |
| regex_compile  | 72.8 ms                                                | 73.0 ms: 1.00x slower                                                 |
| regex_effbot   | 2.43 ms                                                | 2.44 ms: 1.00x slower                                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.04 ms: 1.25x faster                                                 |
| xml_etree_parse      | 100 ms                                                 | 90.9 ms: 1.10x faster                                                 |
| unpickle_list        | 2.69 us                                                | 2.52 us: 1.07x faster                                                 |
| pickle_dict          | 17.1 us                                                | 16.9 us: 1.01x faster                                                 |
| xml_etree_generate   | 45.8 ms                                                | 46.0 ms: 1.00x slower                                                 |
| xml_etree_process    | 33.6 ms                                                | 33.8 ms: 1.01x slower                                                 |
| json_loads           | 15.3 us                                                | 15.6 us: 1.02x slower                                                 |
| pickle               | 6.98 us                                                | 7.13 us: 1.02x slower                                                 |
| unpickle_pure_python | 149 us                                                 | 154 us: 1.04x slower                                                  |
| pickle_pure_python   | 191 us                                                 | 201 us: 1.05x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.42 sec: 1.11x slower                                                |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                          |

Benchmark hidden because not significant (3): xml_etree_iterparse, unpickle, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.3 ms: 1.05x slower                                                 |
| python_startup_no_site | 8.57 ms                                                | 9.36 ms: 1.09x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.07x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.93 ms                                                | 7.66 ms: 1.04x faster                                                 |
| django_template | 20.1 ms                                                | 20.0 ms: 1.01x faster                                                 |
| genshi_xml      | 28.5 ms                                                | 28.4 ms: 1.01x faster                                                 |
| genshi_text     | 14.4 ms                                                | 14.6 ms: 1.01x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.01x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-darwin-arm64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps                 | 7.53 ms                                                | 6.04 ms: 1.25x faster                                                 |
| xml_etree_parse            | 100 ms                                                 | 90.9 ms: 1.10x faster                                                 |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 2.61 ms: 1.08x faster                                                 |
| unpickle_list              | 2.69 us                                                | 2.52 us: 1.07x faster                                                 |
| logging_silent             | 66.5 ns                                                | 63.1 ns: 1.05x faster                                                 |
| async_tree_none_tg         | 276 ms                                                 | 262 ms: 1.05x faster                                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 336 ms: 1.05x faster                                                  |
| async_tree_memoization     | 336 ms                                                 | 322 ms: 1.04x faster                                                  |
| async_tree_io_tg           | 724 ms                                                 | 697 ms: 1.04x faster                                                  |
| mako                       | 7.93 ms                                                | 7.66 ms: 1.04x faster                                                 |
| create_gc_cycles           | 711 us                                                 | 687 us: 1.03x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 537 ms: 1.02x faster                                                  |
| bench_thread_pool          | 465 us                                                 | 457 us: 1.02x faster                                                  |
| sympy_integrate            | 11.3 ms                                                | 11.1 ms: 1.02x faster                                                 |
| pickle_dict                | 17.1 us                                                | 16.9 us: 1.01x faster                                                 |
| django_template            | 20.1 ms                                                | 20.0 ms: 1.01x faster                                                 |
| regex_v8                   | 15.1 ms                                                | 15.0 ms: 1.01x faster                                                 |
| nqueens                    | 55.9 ms                                                | 55.6 ms: 1.01x faster                                                 |
| genshi_xml                 | 28.5 ms                                                | 28.4 ms: 1.01x faster                                                 |
| scimark_lu                 | 67.7 ms                                                | 67.4 ms: 1.01x faster                                                 |
| generators                 | 30.3 ms                                                | 30.2 ms: 1.00x faster                                                 |
| regex_dna                  | 148 ms                                                 | 148 ms: 1.00x faster                                                  |
| regex_compile              | 72.8 ms                                                | 73.0 ms: 1.00x slower                                                 |
| xml_etree_generate         | 45.8 ms                                                | 46.0 ms: 1.00x slower                                                 |
| regex_effbot               | 2.43 ms                                                | 2.44 ms: 1.00x slower                                                 |
| sympy_str                  | 144 ms                                                 | 144 ms: 1.00x slower                                                  |
| raytrace                   | 206 ms                                                 | 207 ms: 1.01x slower                                                  |
| dulwich_log                | 28.6 ms                                                | 28.8 ms: 1.01x slower                                                 |
| xml_etree_process          | 33.6 ms                                                | 33.8 ms: 1.01x slower                                                 |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 523 ms: 1.01x slower                                                  |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                                 |
| telco                      | 3.17 ms                                                | 3.20 ms: 1.01x slower                                                 |
| thrift                     | 410 us                                                 | 415 us: 1.01x slower                                                  |
| pprint_pformat             | 979 ms                                                 | 990 ms: 1.01x slower                                                  |
| pprint_safe_repr           | 478 ms                                                 | 484 ms: 1.01x slower                                                  |
| genshi_text                | 14.4 ms                                                | 14.6 ms: 1.01x slower                                                 |
| pycparser                  | 659 ms                                                 | 668 ms: 1.01x slower                                                  |
| chameleon                  | 4.30 ms                                                | 4.35 ms: 1.01x slower                                                 |
| unpack_sequence            | 33.6 ns                                                | 34.1 ns: 1.01x slower                                                 |
| docutils                   | 1.43 sec                                               | 1.45 sec: 1.02x slower                                                |
| sympy_sum                  | 80.2 ms                                                | 81.5 ms: 1.02x slower                                                 |
| async_generators           | 192 ms                                                 | 195 ms: 1.02x slower                                                  |
| json_loads                 | 15.3 us                                                | 15.6 us: 1.02x slower                                                 |
| bench_mp_pool              | 41.0 ms                                                | 41.7 ms: 1.02x slower                                                 |
| crypto_pyaes               | 47.5 ms                                                | 48.4 ms: 1.02x slower                                                 |
| pickle                     | 6.98 us                                                | 7.13 us: 1.02x slower                                                 |
| hexiom                     | 4.58 ms                                                | 4.68 ms: 1.02x slower                                                 |
| json                       | 2.75 ms                                                | 2.82 ms: 1.02x slower                                                 |
| sympy_expand               | 229 ms                                                 | 235 ms: 1.02x slower                                                  |
| asyncio_tcp                | 643 ms                                                 | 659 ms: 1.02x slower                                                  |
| chaos                      | 47.4 ms                                                | 48.6 ms: 1.03x slower                                                 |
| comprehensions             | 14.4 us                                                | 14.8 us: 1.03x slower                                                 |
| html5lib                   | 33.0 ms                                                | 33.9 ms: 1.03x slower                                                 |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.43 sec: 1.03x slower                                                |
| 2to3                       | 154 ms                                                 | 159 ms: 1.03x slower                                                  |
| sqlglot_normalize          | 162 ms                                                 | 167 ms: 1.03x slower                                                  |
| sqlglot_optimize           | 29.6 ms                                                | 30.5 ms: 1.03x slower                                                 |
| richards_super             | 37.3 ms                                                | 38.6 ms: 1.04x slower                                                 |
| unpickle_pure_python       | 149 us                                                 | 154 us: 1.04x slower                                                  |
| async_tree_io              | 697 ms                                                 | 723 ms: 1.04x slower                                                  |
| richards                   | 31.1 ms                                                | 32.5 ms: 1.05x slower                                                 |
| sqlglot_transpile          | 1.05 ms                                                | 1.10 ms: 1.05x slower                                                 |
| logging_format             | 3.67 us                                                | 3.85 us: 1.05x slower                                                 |
| logging_simple             | 3.41 us                                                | 3.58 us: 1.05x slower                                                 |
| coroutines                 | 17.2 ms                                                | 18.0 ms: 1.05x slower                                                 |
| pickle_pure_python         | 191 us                                                 | 201 us: 1.05x slower                                                  |
| deepcopy                   | 215 us                                                 | 227 us: 1.05x slower                                                  |
| python_startup             | 10.8 ms                                                | 11.3 ms: 1.05x slower                                                 |
| sqlglot_parse              | 890 us                                                 | 940 us: 1.06x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 69.5 ms: 1.06x slower                                                 |
| deepcopy_memo              | 25.7 us                                                | 27.3 us: 1.06x slower                                                 |
| typing_runtime_protocols   | 301 us                                                 | 321 us: 1.07x slower                                                  |
| deepcopy_reduce            | 1.79 us                                                | 1.92 us: 1.07x slower                                                 |
| scimark_fft                | 173 ms                                                 | 185 ms: 1.07x slower                                                  |
| meteor_contest             | 71.1 ms                                                | 76.4 ms: 1.07x slower                                                 |
| go                         | 105 ms                                                 | 114 ms: 1.09x slower                                                  |
| fannkuch                   | 240 ms                                                 | 260 ms: 1.09x slower                                                  |
| python_startup_no_site     | 8.57 ms                                                | 9.36 ms: 1.09x slower                                                 |
| float                      | 50.8 ms                                                | 55.9 ms: 1.10x slower                                                 |
| tomli_loads                | 1.27 sec                                               | 1.42 sec: 1.11x slower                                                |
| nbody                      | 61.7 ms                                                | 69.0 ms: 1.12x slower                                                 |
| sqlite_synth               | 1.26 us                                                | 1.42 us: 1.13x slower                                                 |
| mdp                        | 1.48 sec                                               | 1.71 sec: 1.15x slower                                                |
| pyflate                    | 284 ms                                                 | 331 ms: 1.17x slower                                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 52.9 ms: 1.22x slower                                                 |
| scimark_sor                | 79.2 ms                                                | 100 ms: 1.27x slower                                                  |
| dask                       | 219 ms                                                 | 322 ms: 1.47x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                          |

Benchmark hidden because not significant (10): xml_etree_iterparse, pathlib, unpickle, async_tree_none, pidigits, asyncio_websockets, deltablue, pickle_list, tornado_http, pylint
Ignored benchmarks (7) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x