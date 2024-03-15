
# Results vs. 3.11.0

- fork: python
- ref: ed7c3ff15680c1939fad
- machine: darwin-arm64
- commit hash: ed7c3ff
- commit date: 2022-09-11
- overall geometric mean: 1.02x slower \*
- HPT reliability: 87.32%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 153 ms: 1.01x faster                                                   |
| chameleon      | 4.30 ms                                                | 4.17 ms: 1.03x faster                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (3): docutils, html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 282 ms                                                 | 277 ms: 1.02x faster                                                   |
| async_tree_io           | 697 ms                                                 | 690 ms: 1.01x faster                                                   |
| async_tree_cpu_io_mixed | 519 ms                                                 | 515 ms: 1.01x faster                                                   |
| async_tree_none_tg      | 276 ms                                                 | 275 ms: 1.01x faster                                                   |
| async_tree_io_tg        | 724 ms                                                 | 722 ms: 1.00x faster                                                   |
| async_tree_memoization  | 336 ms                                                 | 347 ms: 1.03x slower                                                   |
| Geometric mean          | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 280 ms: 1.00x faster                                                   |
| float          | 50.8 ms                                                | 55.7 ms: 1.10x slower                                                  |
| nbody          | 61.7 ms                                                | 68.4 ms: 1.11x slower                                                  |
| Geometric mean | (ref)                                                  | 1.07x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 72.8 ms                                                | 73.6 ms: 1.01x slower                                                  |
| regex_effbot   | 2.43 ms                                                | 2.46 ms: 1.01x slower                                                  |
| regex_dna      | 148 ms                                                 | 150 ms: 1.01x slower                                                   |
| regex_v8       | 15.1 ms                                                | 15.5 ms: 1.02x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| xml_etree_parse      | 100 ms                                                 | 96.9 ms: 1.03x faster                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 67.1 ms: 1.02x faster                                                  |
| pickle_list          | 2.70 us                                                | 2.66 us: 1.01x faster                                                  |
| pickle_dict          | 17.1 us                                                | 17.0 us: 1.01x faster                                                  |
| json_dumps           | 7.53 ms                                                | 7.56 ms: 1.00x slower                                                  |
| json_loads           | 15.3 us                                                | 15.5 us: 1.01x slower                                                  |
| unpickle             | 8.29 us                                                | 8.37 us: 1.01x slower                                                  |
| xml_etree_process    | 33.6 ms                                                | 34.0 ms: 1.01x slower                                                  |
| xml_etree_generate   | 45.8 ms                                                | 46.7 ms: 1.02x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.31 sec: 1.03x slower                                                 |
| pickle               | 6.98 us                                                | 7.17 us: 1.03x slower                                                  |
| unpickle_list        | 2.69 us                                                | 2.77 us: 1.03x slower                                                  |
| unpickle_pure_python | 149 us                                                 | 163 us: 1.09x slower                                                   |
| pickle_pure_python   | 191 us                                                 | 210 us: 1.10x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 12.0 ms: 1.12x slower                                                  |
| python_startup_no_site | 8.57 ms                                                | 9.94 ms: 1.16x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.14x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| django_template | 20.1 ms                                                | 19.8 ms: 1.02x faster                                                  |
| genshi_xml      | 28.5 ms                                                | 28.1 ms: 1.02x faster                                                  |
| genshi_text     | 14.4 ms                                                | 14.5 ms: 1.01x slower                                                  |
| mako            | 7.93 ms                                                | 8.22 ms: 1.04x slower                                                  |
| Geometric mean  | (ref)                                                  | 1.00x slower                                                           |

All benchmarks:
===============

| Benchmark                | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-darwin-arm64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| coverage                 | 43.9 ms                                                | 41.3 ms: 1.06x faster                                                  |
| scimark_sor              | 79.2 ms                                                | 74.8 ms: 1.06x faster                                                  |
| coroutines               | 17.2 ms                                                | 16.4 ms: 1.05x faster                                                  |
| generators               | 30.3 ms                                                | 29.0 ms: 1.04x faster                                                  |
| unpack_sequence          | 33.6 ns                                                | 32.3 ns: 1.04x faster                                                  |
| xml_etree_parse          | 100 ms                                                 | 96.9 ms: 1.03x faster                                                  |
| logging_silent           | 66.5 ns                                                | 64.4 ns: 1.03x faster                                                  |
| go                       | 105 ms                                                 | 102 ms: 1.03x faster                                                   |
| chameleon                | 4.30 ms                                                | 4.17 ms: 1.03x faster                                                  |
| nqueens                  | 55.9 ms                                                | 54.3 ms: 1.03x faster                                                  |
| deltablue                | 2.75 ms                                                | 2.68 ms: 1.02x faster                                                  |
| bench_thread_pool        | 465 us                                                 | 457 us: 1.02x faster                                                   |
| sqlglot_transpile        | 1.05 ms                                                | 1.03 ms: 1.02x faster                                                  |
| sqlglot_parse            | 890 us                                                 | 874 us: 1.02x faster                                                   |
| django_template          | 20.1 ms                                                | 19.8 ms: 1.02x faster                                                  |
| xml_etree_iterparse      | 68.3 ms                                                | 67.1 ms: 1.02x faster                                                  |
| async_tree_none          | 282 ms                                                 | 277 ms: 1.02x faster                                                   |
| genshi_xml               | 28.5 ms                                                | 28.1 ms: 1.02x faster                                                  |
| richards_super           | 37.3 ms                                                | 36.8 ms: 1.01x faster                                                  |
| pickle_list              | 2.70 us                                                | 2.66 us: 1.01x faster                                                  |
| sqlglot_normalize        | 162 ms                                                 | 160 ms: 1.01x faster                                                   |
| async_tree_io            | 697 ms                                                 | 690 ms: 1.01x faster                                                   |
| sympy_integrate          | 11.3 ms                                                | 11.2 ms: 1.01x faster                                                  |
| hexiom                   | 4.58 ms                                                | 4.54 ms: 1.01x faster                                                  |
| async_tree_cpu_io_mixed  | 519 ms                                                 | 515 ms: 1.01x faster                                                   |
| richards                 | 31.1 ms                                                | 30.8 ms: 1.01x faster                                                  |
| pickle_dict              | 17.1 us                                                | 17.0 us: 1.01x faster                                                  |
| async_tree_none_tg       | 276 ms                                                 | 275 ms: 1.01x faster                                                   |
| 2to3                     | 154 ms                                                 | 153 ms: 1.01x faster                                                   |
| async_generators         | 192 ms                                                 | 191 ms: 1.00x faster                                                   |
| sqlglot_optimize         | 29.6 ms                                                | 29.5 ms: 1.00x faster                                                  |
| asyncio_websockets       | 408 ms                                                 | 407 ms: 1.00x faster                                                   |
| async_tree_io_tg         | 724 ms                                                 | 722 ms: 1.00x faster                                                   |
| pprint_safe_repr         | 478 ms                                                 | 477 ms: 1.00x faster                                                   |
| pidigits                 | 280 ms                                                 | 280 ms: 1.00x faster                                                   |
| pprint_pformat           | 979 ms                                                 | 977 ms: 1.00x faster                                                   |
| create_gc_cycles         | 711 us                                                 | 712 us: 1.00x slower                                                   |
| sympy_str                | 144 ms                                                 | 144 ms: 1.00x slower                                                   |
| json_dumps               | 7.53 ms                                                | 7.56 ms: 1.00x slower                                                  |
| json_loads               | 15.3 us                                                | 15.5 us: 1.01x slower                                                  |
| genshi_text              | 14.4 ms                                                | 14.5 ms: 1.01x slower                                                  |
| unpickle                 | 8.29 us                                                | 8.37 us: 1.01x slower                                                  |
| regex_compile            | 72.8 ms                                                | 73.6 ms: 1.01x slower                                                  |
| sympy_sum                | 80.2 ms                                                | 81.0 ms: 1.01x slower                                                  |
| regex_effbot             | 2.43 ms                                                | 2.46 ms: 1.01x slower                                                  |
| logging_simple           | 3.41 us                                                | 3.45 us: 1.01x slower                                                  |
| comprehensions           | 14.4 us                                                | 14.6 us: 1.01x slower                                                  |
| crypto_pyaes             | 47.5 ms                                                | 48.1 ms: 1.01x slower                                                  |
| logging_format           | 3.67 us                                                | 3.72 us: 1.01x slower                                                  |
| regex_dna                | 148 ms                                                 | 150 ms: 1.01x slower                                                   |
| xml_etree_process        | 33.6 ms                                                | 34.0 ms: 1.01x slower                                                  |
| chaos                    | 47.4 ms                                                | 48.2 ms: 1.02x slower                                                  |
| bench_mp_pool            | 41.0 ms                                                | 41.8 ms: 1.02x slower                                                  |
| xml_etree_generate       | 45.8 ms                                                | 46.7 ms: 1.02x slower                                                  |
| sqlalchemy_declarative   | 59.3 ms                                                | 60.5 ms: 1.02x slower                                                  |
| thrift                   | 410 us                                                 | 419 us: 1.02x slower                                                   |
| sympy_expand             | 229 ms                                                 | 235 ms: 1.02x slower                                                   |
| regex_v8                 | 15.1 ms                                                | 15.5 ms: 1.02x slower                                                  |
| tomli_loads              | 1.27 sec                                               | 1.31 sec: 1.03x slower                                                 |
| asyncio_tcp              | 643 ms                                                 | 661 ms: 1.03x slower                                                   |
| pickle                   | 6.98 us                                                | 7.17 us: 1.03x slower                                                  |
| dulwich_log              | 28.6 ms                                                | 29.5 ms: 1.03x slower                                                  |
| asyncio_tcp_ssl          | 1.40 sec                                               | 1.44 sec: 1.03x slower                                                 |
| sqlalchemy_imperative    | 6.98 ms                                                | 7.19 ms: 1.03x slower                                                  |
| unpickle_list            | 2.69 us                                                | 2.77 us: 1.03x slower                                                  |
| fannkuch                 | 240 ms                                                 | 247 ms: 1.03x slower                                                   |
| async_tree_memoization   | 336 ms                                                 | 347 ms: 1.03x slower                                                   |
| mako                     | 7.93 ms                                                | 8.22 ms: 1.04x slower                                                  |
| pyflate                  | 284 ms                                                 | 294 ms: 1.04x slower                                                   |
| flaskblogging            | 2.35 ms                                                | 2.45 ms: 1.04x slower                                                  |
| spectral_norm            | 65.7 ms                                                | 69.2 ms: 1.05x slower                                                  |
| meteor_contest           | 71.1 ms                                                | 75.0 ms: 1.05x slower                                                  |
| scimark_sparse_mat_mult  | 2.81 ms                                                | 3.00 ms: 1.07x slower                                                  |
| typing_runtime_protocols | 301 us                                                 | 322 us: 1.07x slower                                                   |
| scimark_fft              | 173 ms                                                 | 186 ms: 1.08x slower                                                   |
| sqlite_synth             | 1.26 us                                                | 1.36 us: 1.08x slower                                                  |
| deepcopy                 | 215 us                                                 | 233 us: 1.08x slower                                                   |
| scimark_monte_carlo      | 43.5 ms                                                | 47.2 ms: 1.09x slower                                                  |
| aiohttp                  | 1.02 ms                                                | 1.12 ms: 1.09x slower                                                  |
| unpickle_pure_python     | 149 us                                                 | 163 us: 1.09x slower                                                   |
| deepcopy_reduce          | 1.79 us                                                | 1.97 us: 1.10x slower                                                  |
| float                    | 50.8 ms                                                | 55.7 ms: 1.10x slower                                                  |
| pickle_pure_python       | 191 us                                                 | 210 us: 1.10x slower                                                   |
| nbody                    | 61.7 ms                                                | 68.4 ms: 1.11x slower                                                  |
| deepcopy_memo            | 25.7 us                                                | 28.7 us: 1.11x slower                                                  |
| python_startup           | 10.8 ms                                                | 12.0 ms: 1.12x slower                                                  |
| python_startup_no_site   | 8.57 ms                                                | 9.94 ms: 1.16x slower                                                  |
| mdp                      | 1.48 sec                                               | 1.74 sec: 1.17x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (15): pylint, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, docutils, gc_traversal, json, raytrace, scimark_lu, gunicorn, telco, pycparser, dask, pathlib, html5lib, tornado_http
Ignored benchmarks (1) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: mypy2


# HPT report

- Reliability score: 87.32% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x