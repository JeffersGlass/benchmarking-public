
# Results vs. 3.11.0

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: darwin-arm64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.01x slower \*
- HPT reliability: 93.60%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 158 ms: 1.02x slower                                                  |
| chameleon      | 4.30 ms                                                | 4.21 ms: 1.02x faster                                                 |
| docutils       | 1.43 sec                                               | 1.41 sec: 1.01x faster                                                |
| html5lib       | 33.0 ms                                                | 32.3 ms: 1.02x faster                                                 |
| Geometric mean | (ref)                                                  | 1.01x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization     | 336 ms                                                 | 322 ms: 1.04x faster                                                  |
| async_tree_none_tg         | 276 ms                                                 | 266 ms: 1.04x faster                                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 340 ms: 1.04x faster                                                  |
| async_tree_io_tg           | 724 ms                                                 | 710 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 543 ms: 1.01x faster                                                  |
| async_tree_none            | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 521 ms: 1.00x slower                                                  |
| async_tree_io              | 697 ms                                                 | 728 ms: 1.04x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.01x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 280 ms: 1.00x faster                                                  |
| float          | 50.8 ms                                                | 55.5 ms: 1.09x slower                                                 |
| nbody          | 61.7 ms                                                | 67.7 ms: 1.10x slower                                                 |
| Geometric mean | (ref)                                                  | 1.06x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_v8       | 15.1 ms                                                | 15.0 ms: 1.01x faster                                                 |
| regex_compile  | 72.8 ms                                                | 72.1 ms: 1.01x faster                                                 |
| regex_dna      | 148 ms                                                 | 147 ms: 1.01x faster                                                  |
| regex_effbot   | 2.43 ms                                                | 2.44 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                  | 1.01x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 5.84 ms: 1.29x faster                                                 |
| unpickle_pure_python | 149 us                                                 | 137 us: 1.08x faster                                                  |
| xml_etree_parse      | 100 ms                                                 | 96.4 ms: 1.04x faster                                                 |
| pickle_pure_python   | 191 us                                                 | 190 us: 1.01x faster                                                  |
| pickle_dict          | 17.1 us                                                | 17.0 us: 1.00x faster                                                 |
| xml_etree_process    | 33.6 ms                                                | 33.8 ms: 1.01x slower                                                 |
| tomli_loads          | 1.27 sec                                               | 1.28 sec: 1.01x slower                                                |
| json_loads           | 15.3 us                                                | 15.5 us: 1.01x slower                                                 |
| unpickle             | 8.29 us                                                | 8.43 us: 1.02x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 46.9 ms: 1.02x slower                                                 |
| xml_etree_iterparse  | 68.3 ms                                                | 70.0 ms: 1.03x slower                                                 |
| unpickle_list        | 2.69 us                                                | 2.81 us: 1.05x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                          |

Benchmark hidden because not significant (2): pickle, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.4 ms: 1.06x slower                                                 |
| python_startup_no_site | 8.57 ms                                                | 9.54 ms: 1.11x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.09x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| genshi_xml      | 28.5 ms                                                | 27.3 ms: 1.05x faster                                                 |
| mako            | 7.93 ms                                                | 7.76 ms: 1.02x faster                                                 |
| genshi_text     | 14.4 ms                                                | 14.2 ms: 1.02x faster                                                 |
| django_template | 20.1 ms                                                | 20.8 ms: 1.03x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.01x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230110-darwin-arm64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| asyncio_tcp                | 643 ms                                                 | 430 ms: 1.49x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 5.84 ms: 1.29x faster                                                 |
| unpack_sequence            | 33.6 ns                                                | 30.2 ns: 1.11x faster                                                 |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.26 sec: 1.11x faster                                                |
| deltablue                  | 2.75 ms                                                | 2.51 ms: 1.10x faster                                                 |
| unpickle_pure_python       | 149 us                                                 | 137 us: 1.08x faster                                                  |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 2.66 ms: 1.06x faster                                                 |
| genshi_xml                 | 28.5 ms                                                | 27.3 ms: 1.05x faster                                                 |
| async_tree_memoization     | 336 ms                                                 | 322 ms: 1.04x faster                                                  |
| logging_silent             | 66.5 ns                                                | 63.9 ns: 1.04x faster                                                 |
| richards                   | 31.1 ms                                                | 29.8 ms: 1.04x faster                                                 |
| xml_etree_parse            | 100 ms                                                 | 96.4 ms: 1.04x faster                                                 |
| async_tree_none_tg         | 276 ms                                                 | 266 ms: 1.04x faster                                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 340 ms: 1.04x faster                                                  |
| create_gc_cycles           | 711 us                                                 | 686 us: 1.04x faster                                                  |
| richards_super             | 37.3 ms                                                | 36.0 ms: 1.04x faster                                                 |
| pycparser                  | 659 ms                                                 | 643 ms: 1.03x faster                                                  |
| mako                       | 7.93 ms                                                | 7.76 ms: 1.02x faster                                                 |
| chameleon                  | 4.30 ms                                                | 4.21 ms: 1.02x faster                                                 |
| logging_format             | 3.67 us                                                | 3.60 us: 1.02x faster                                                 |
| logging_simple             | 3.41 us                                                | 3.34 us: 1.02x faster                                                 |
| html5lib                   | 33.0 ms                                                | 32.3 ms: 1.02x faster                                                 |
| async_tree_io_tg           | 724 ms                                                 | 710 ms: 1.02x faster                                                  |
| genshi_text                | 14.4 ms                                                | 14.2 ms: 1.02x faster                                                 |
| sympy_integrate            | 11.3 ms                                                | 11.1 ms: 1.02x faster                                                 |
| dulwich_log                | 28.6 ms                                                | 28.2 ms: 1.01x faster                                                 |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 543 ms: 1.01x faster                                                  |
| docutils                   | 1.43 sec                                               | 1.41 sec: 1.01x faster                                                |
| bench_thread_pool          | 465 us                                                 | 460 us: 1.01x faster                                                  |
| regex_v8                   | 15.1 ms                                                | 15.0 ms: 1.01x faster                                                 |
| regex_compile              | 72.8 ms                                                | 72.1 ms: 1.01x faster                                                 |
| regex_dna                  | 148 ms                                                 | 147 ms: 1.01x faster                                                  |
| pickle_pure_python         | 191 us                                                 | 190 us: 1.01x faster                                                  |
| async_tree_none            | 282 ms                                                 | 280 ms: 1.01x faster                                                  |
| scimark_lu                 | 67.7 ms                                                | 67.3 ms: 1.01x faster                                                 |
| pickle_dict                | 17.1 us                                                | 17.0 us: 1.00x faster                                                 |
| pidigits                   | 280 ms                                                 | 280 ms: 1.00x faster                                                  |
| pprint_safe_repr           | 478 ms                                                 | 480 ms: 1.00x slower                                                  |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 521 ms: 1.00x slower                                                  |
| sympy_expand               | 229 ms                                                 | 230 ms: 1.00x slower                                                  |
| regex_effbot               | 2.43 ms                                                | 2.44 ms: 1.01x slower                                                 |
| xml_etree_process          | 33.6 ms                                                | 33.8 ms: 1.01x slower                                                 |
| tomli_loads                | 1.27 sec                                               | 1.28 sec: 1.01x slower                                                |
| json_loads                 | 15.3 us                                                | 15.5 us: 1.01x slower                                                 |
| sqlglot_optimize           | 29.6 ms                                                | 30.0 ms: 1.01x slower                                                 |
| json                       | 2.75 ms                                                | 2.79 ms: 1.01x slower                                                 |
| raytrace                   | 206 ms                                                 | 208 ms: 1.01x slower                                                  |
| fannkuch                   | 240 ms                                                 | 244 ms: 1.02x slower                                                  |
| telco                      | 3.17 ms                                                | 3.22 ms: 1.02x slower                                                 |
| coroutines                 | 17.2 ms                                                | 17.5 ms: 1.02x slower                                                 |
| unpickle                   | 8.29 us                                                | 8.43 us: 1.02x slower                                                 |
| sqlglot_normalize          | 162 ms                                                 | 165 ms: 1.02x slower                                                  |
| sympy_sum                  | 80.2 ms                                                | 81.7 ms: 1.02x slower                                                 |
| hexiom                     | 4.58 ms                                                | 4.66 ms: 1.02x slower                                                 |
| thrift                     | 410 us                                                 | 419 us: 1.02x slower                                                  |
| 2to3                       | 154 ms                                                 | 158 ms: 1.02x slower                                                  |
| nqueens                    | 55.9 ms                                                | 57.2 ms: 1.02x slower                                                 |
| xml_etree_generate         | 45.8 ms                                                | 46.9 ms: 1.02x slower                                                 |
| xml_etree_iterparse        | 68.3 ms                                                | 70.0 ms: 1.03x slower                                                 |
| django_template            | 20.1 ms                                                | 20.8 ms: 1.03x slower                                                 |
| bench_mp_pool              | 41.0 ms                                                | 42.5 ms: 1.04x slower                                                 |
| async_generators           | 192 ms                                                 | 200 ms: 1.04x slower                                                  |
| chaos                      | 47.4 ms                                                | 49.5 ms: 1.04x slower                                                 |
| async_tree_io              | 697 ms                                                 | 728 ms: 1.04x slower                                                  |
| unpickle_list              | 2.69 us                                                | 2.81 us: 1.05x slower                                                 |
| scimark_sor                | 79.2 ms                                                | 83.4 ms: 1.05x slower                                                 |
| deepcopy                   | 215 us                                                 | 227 us: 1.05x slower                                                  |
| scimark_fft                | 173 ms                                                 | 182 ms: 1.06x slower                                                  |
| pyflate                    | 284 ms                                                 | 301 ms: 1.06x slower                                                  |
| crypto_pyaes               | 47.5 ms                                                | 50.4 ms: 1.06x slower                                                 |
| python_startup             | 10.8 ms                                                | 11.4 ms: 1.06x slower                                                 |
| typing_runtime_protocols   | 301 us                                                 | 320 us: 1.06x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 70.6 ms: 1.07x slower                                                 |
| scimark_monte_carlo        | 43.5 ms                                                | 46.8 ms: 1.08x slower                                                 |
| deepcopy_memo              | 25.7 us                                                | 27.7 us: 1.08x slower                                                 |
| deepcopy_reduce            | 1.79 us                                                | 1.94 us: 1.08x slower                                                 |
| sqlite_synth               | 1.26 us                                                | 1.36 us: 1.09x slower                                                 |
| sqlglot_transpile          | 1.05 ms                                                | 1.15 ms: 1.09x slower                                                 |
| float                      | 50.8 ms                                                | 55.5 ms: 1.09x slower                                                 |
| nbody                      | 61.7 ms                                                | 67.7 ms: 1.10x slower                                                 |
| sqlglot_parse              | 890 us                                                 | 985 us: 1.11x slower                                                  |
| python_startup_no_site     | 8.57 ms                                                | 9.54 ms: 1.11x slower                                                 |
| mdp                        | 1.48 sec                                               | 1.70 sec: 1.14x slower                                                |
| comprehensions             | 14.4 us                                                | 16.6 us: 1.15x slower                                                 |
| generators                 | 30.3 ms                                                | 35.1 ms: 1.16x slower                                                 |
| dask                       | 219 ms                                                 | 309 ms: 1.41x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                          |

Benchmark hidden because not significant (9): pathlib, pprint_pformat, sympy_str, asyncio_websockets, gc_traversal, pickle, meteor_contest, go, pickle_list
Ignored benchmarks (9) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, tornado_http


# HPT report

- Reliability score: 93.60% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.97x