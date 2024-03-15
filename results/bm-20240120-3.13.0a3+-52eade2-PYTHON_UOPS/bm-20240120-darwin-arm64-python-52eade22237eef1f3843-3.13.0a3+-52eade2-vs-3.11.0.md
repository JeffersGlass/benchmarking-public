
# Results vs. 3.11.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: darwin-arm64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.09x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 173 ms: 1.12x slower                                                   |
| chameleon      | 4.30 ms                                                | 5.02 ms: 1.17x slower                                                  |
| docutils       | 1.43 sec                                               | 1.51 sec: 1.06x slower                                                 |
| Geometric mean | (ref)                                                  | 1.09x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 261 ms: 1.08x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 682 ms: 1.06x faster                                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 333 ms: 1.06x faster                                                   |
| async_tree_none_tg         | 276 ms                                                 | 268 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 538 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 531 ms: 1.02x slower                                                   |
| async_tree_io              | 697 ms                                                 | 717 ms: 1.03x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 284 ms: 1.01x slower                                                   |
| float          | 50.8 ms                                                | 68.6 ms: 1.35x slower                                                  |
| nbody          | 61.7 ms                                                | 85.7 ms: 1.39x slower                                                  |
| Geometric mean | (ref)                                                  | 1.24x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 157 ms: 1.06x slower                                                   |
| regex_compile  | 72.8 ms                                                | 82.6 ms: 1.13x slower                                                  |
| regex_effbot   | 2.43 ms                                                | 2.85 ms: 1.17x slower                                                  |
| regex_v8       | 15.1 ms                                                | 18.1 ms: 1.20x slower                                                  |
| Geometric mean | (ref)                                                  | 1.14x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.61 ms: 1.14x faster                                                  |
| pickle_pure_python   | 191 us                                                 | 196 us: 1.03x slower                                                   |
| pickle_dict          | 17.1 us                                                | 18.1 us: 1.06x slower                                                  |
| pickle               | 6.98 us                                                | 7.45 us: 1.07x slower                                                  |
| xml_etree_parse      | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| unpickle             | 8.29 us                                                | 9.11 us: 1.10x slower                                                  |
| pickle_list          | 2.70 us                                                | 2.96 us: 1.10x slower                                                  |
| unpickle_pure_python | 149 us                                                 | 164 us: 1.10x slower                                                   |
| json_loads           | 15.3 us                                                | 17.1 us: 1.12x slower                                                  |
| unpickle_list        | 2.69 us                                                | 3.06 us: 1.14x slower                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 80.5 ms: 1.18x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 41.0 ms: 1.22x slower                                                  |
| xml_etree_generate   | 45.8 ms                                                | 59.5 ms: 1.30x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.67 sec: 1.31x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 12.6 ms: 1.17x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 11.2 ms: 1.30x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.24x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 7.93 ms                                                | 9.74 ms: 1.23x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-darwin-arm64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 73.6 us: 4.09x faster                                                  |
| asyncio_tcp                | 643 ms                                                 | 432 ms: 1.49x faster                                                   |
| unpack_sequence            | 33.6 ns                                                | 28.5 ns: 1.18x faster                                                  |
| json_dumps                 | 7.53 ms                                                | 6.61 ms: 1.14x faster                                                  |
| raytrace                   | 206 ms                                                 | 186 ms: 1.11x faster                                                   |
| sqlglot_parse              | 890 us                                                 | 811 us: 1.10x faster                                                   |
| async_tree_none            | 282 ms                                                 | 261 ms: 1.08x faster                                                   |
| async_tree_io_tg           | 724 ms                                                 | 682 ms: 1.06x faster                                                   |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.32 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 352 ms                                                 | 333 ms: 1.06x faster                                                   |
| sqlglot_transpile          | 1.05 ms                                                | 995 us: 1.06x faster                                                   |
| generators                 | 30.3 ms                                                | 28.7 ms: 1.06x faster                                                  |
| async_tree_none_tg         | 276 ms                                                 | 268 ms: 1.03x faster                                                   |
| richards_super             | 37.3 ms                                                | 36.5 ms: 1.02x faster                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 538 ms: 1.02x faster                                                   |
| chaos                      | 47.4 ms                                                | 46.5 ms: 1.02x faster                                                  |
| sympy_sum                  | 80.2 ms                                                | 79.6 ms: 1.01x faster                                                  |
| create_gc_cycles           | 711 us                                                 | 708 us: 1.00x faster                                                   |
| asyncio_websockets         | 408 ms                                                 | 410 ms: 1.00x slower                                                   |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                                  |
| pidigits                   | 280 ms                                                 | 284 ms: 1.01x slower                                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 531 ms: 1.02x slower                                                   |
| pickle_pure_python         | 191 us                                                 | 196 us: 1.03x slower                                                   |
| sympy_integrate            | 11.3 ms                                                | 11.6 ms: 1.03x slower                                                  |
| async_tree_io              | 697 ms                                                 | 717 ms: 1.03x slower                                                   |
| sympy_str                  | 144 ms                                                 | 149 ms: 1.03x slower                                                   |
| deepcopy_memo              | 25.7 us                                                | 26.7 us: 1.04x slower                                                  |
| logging_simple             | 3.41 us                                                | 3.56 us: 1.05x slower                                                  |
| dask                       | 219 ms                                                 | 229 ms: 1.05x slower                                                   |
| logging_format             | 3.67 us                                                | 3.85 us: 1.05x slower                                                  |
| richards                   | 31.1 ms                                                | 32.6 ms: 1.05x slower                                                  |
| dulwich_log                | 28.6 ms                                                | 30.1 ms: 1.05x slower                                                  |
| deepcopy                   | 215 us                                                 | 227 us: 1.05x slower                                                   |
| go                         | 105 ms                                                 | 111 ms: 1.06x slower                                                   |
| docutils                   | 1.43 sec                                               | 1.51 sec: 1.06x slower                                                 |
| pickle_dict                | 17.1 us                                                | 18.1 us: 1.06x slower                                                  |
| regex_dna                  | 148 ms                                                 | 157 ms: 1.06x slower                                                   |
| pycparser                  | 659 ms                                                 | 702 ms: 1.06x slower                                                   |
| pickle                     | 6.98 us                                                | 7.45 us: 1.07x slower                                                  |
| xml_etree_parse            | 100 ms                                                 | 107 ms: 1.07x slower                                                   |
| logging_silent             | 66.5 ns                                                | 71.1 ns: 1.07x slower                                                  |
| sympy_expand               | 229 ms                                                 | 245 ms: 1.07x slower                                                   |
| comprehensions             | 14.4 us                                                | 15.5 us: 1.07x slower                                                  |
| meteor_contest             | 71.1 ms                                                | 76.8 ms: 1.08x slower                                                  |
| json                       | 2.75 ms                                                | 2.99 ms: 1.09x slower                                                  |
| mdp                        | 1.48 sec                                               | 1.62 sec: 1.09x slower                                                 |
| bench_mp_pool              | 41.0 ms                                                | 44.7 ms: 1.09x slower                                                  |
| coroutines                 | 17.2 ms                                                | 18.8 ms: 1.10x slower                                                  |
| coverage                   | 43.9 ms                                                | 48.2 ms: 1.10x slower                                                  |
| unpickle                   | 8.29 us                                                | 9.11 us: 1.10x slower                                                  |
| pickle_list                | 2.70 us                                                | 2.96 us: 1.10x slower                                                  |
| pathlib                    | 23.2 ms                                                | 25.5 ms: 1.10x slower                                                  |
| unpickle_pure_python       | 149 us                                                 | 164 us: 1.10x slower                                                   |
| bench_thread_pool          | 465 us                                                 | 518 us: 1.11x slower                                                   |
| json_loads                 | 15.3 us                                                | 17.1 us: 1.12x slower                                                  |
| deepcopy_reduce            | 1.79 us                                                | 2.00 us: 1.12x slower                                                  |
| 2to3                       | 154 ms                                                 | 173 ms: 1.12x slower                                                   |
| scimark_lu                 | 67.7 ms                                                | 76.7 ms: 1.13x slower                                                  |
| regex_compile              | 72.8 ms                                                | 82.6 ms: 1.13x slower                                                  |
| unpickle_list              | 2.69 us                                                | 3.06 us: 1.14x slower                                                  |
| crypto_pyaes               | 47.5 ms                                                | 54.9 ms: 1.16x slower                                                  |
| chameleon                  | 4.30 ms                                                | 5.02 ms: 1.17x slower                                                  |
| python_startup             | 10.8 ms                                                | 12.6 ms: 1.17x slower                                                  |
| regex_effbot               | 2.43 ms                                                | 2.85 ms: 1.17x slower                                                  |
| sqlglot_normalize          | 162 ms                                                 | 190 ms: 1.18x slower                                                   |
| xml_etree_iterparse        | 68.3 ms                                                | 80.5 ms: 1.18x slower                                                  |
| pprint_safe_repr           | 478 ms                                                 | 572 ms: 1.20x slower                                                   |
| regex_v8                   | 15.1 ms                                                | 18.1 ms: 1.20x slower                                                  |
| pprint_pformat             | 979 ms                                                 | 1.17 sec: 1.20x slower                                                 |
| sqlglot_optimize           | 29.6 ms                                                | 35.9 ms: 1.21x slower                                                  |
| nqueens                    | 55.9 ms                                                | 68.1 ms: 1.22x slower                                                  |
| xml_etree_process          | 33.6 ms                                                | 41.0 ms: 1.22x slower                                                  |
| mako                       | 7.93 ms                                                | 9.74 ms: 1.23x slower                                                  |
| xml_etree_generate         | 45.8 ms                                                | 59.5 ms: 1.30x slower                                                  |
| hexiom                     | 4.58 ms                                                | 5.95 ms: 1.30x slower                                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 56.5 ms: 1.30x slower                                                  |
| python_startup_no_site     | 8.57 ms                                                | 11.2 ms: 1.30x slower                                                  |
| deltablue                  | 2.75 ms                                                | 3.59 ms: 1.31x slower                                                  |
| pyflate                    | 284 ms                                                 | 371 ms: 1.31x slower                                                   |
| tomli_loads                | 1.27 sec                                               | 1.67 sec: 1.31x slower                                                 |
| sqlite_synth               | 1.26 us                                                | 1.65 us: 1.31x slower                                                  |
| scimark_sor                | 79.2 ms                                                | 107 ms: 1.35x slower                                                   |
| float                      | 50.8 ms                                                | 68.6 ms: 1.35x slower                                                  |
| fannkuch                   | 240 ms                                                 | 326 ms: 1.36x slower                                                   |
| nbody                      | 61.7 ms                                                | 85.7 ms: 1.39x slower                                                  |
| mypy2                      | 372 ms                                                 | 531 ms: 1.42x slower                                                   |
| scimark_fft                | 173 ms                                                 | 247 ms: 1.43x slower                                                   |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 4.12 ms: 1.47x slower                                                  |
| telco                      | 3.17 ms                                                | 4.69 ms: 1.48x slower                                                  |
| async_generators           | 192 ms                                                 | 300 ms: 1.56x slower                                                   |
| spectral_norm              | 65.7 ms                                                | 105 ms: 1.60x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.09x slower                                                           |

Benchmark hidden because not significant (2): async_tree_memoization, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.05x


# Memory

- memory change: 1.04x