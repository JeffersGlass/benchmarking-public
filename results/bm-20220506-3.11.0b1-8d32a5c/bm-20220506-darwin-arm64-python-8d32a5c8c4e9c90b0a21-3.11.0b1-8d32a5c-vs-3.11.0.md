
# Results vs. 3.11.0

- fork: python
- ref: 8d32a5c8c4e9c90b0a21
- machine: darwin-arm64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.03x slower \*
- HPT reliability: 99.94%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 152 ms: 1.01x faster                                                  |
| chameleon      | 4.30 ms                                                | 4.32 ms: 1.00x slower                                                 |
| docutils       | 1.43 sec                                               | 1.39 sec: 1.03x faster                                                |
| html5lib       | 33.0 ms                                                | 31.0 ms: 1.06x faster                                                 |
| Geometric mean | (ref)                                                  | 1.02x faster                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 277 ms: 1.02x faster                                                  |
| async_tree_io              | 697 ms                                                 | 690 ms: 1.01x faster                                                  |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 514 ms: 1.01x faster                                                  |
| async_tree_io_tg           | 724 ms                                                 | 737 ms: 1.02x slower                                                  |
| async_tree_memoization     | 336 ms                                                 | 353 ms: 1.05x slower                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 607 ms: 1.10x slower                                                  |
| async_tree_none_tg         | 276 ms                                                 | 332 ms: 1.20x slower                                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 434 ms: 1.23x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.07x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 50.8 ms                                                | 53.3 ms: 1.05x slower                                                 |
| nbody          | 61.7 ms                                                | 65.6 ms: 1.06x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.43 ms                                                | 2.26 ms: 1.07x faster                                                 |
| regex_dna      | 148 ms                                                 | 144 ms: 1.03x faster                                                  |
| regex_compile  | 72.8 ms                                                | 73.1 ms: 1.00x slower                                                 |
| regex_v8       | 15.1 ms                                                | 15.8 ms: 1.04x slower                                                 |
| Geometric mean | (ref)                                                  | 1.01x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_list          | 2.70 us                                                | 2.55 us: 1.06x faster                                                 |
| pickle_dict          | 17.1 us                                                | 16.2 us: 1.05x faster                                                 |
| xml_etree_parse      | 100 ms                                                 | 97.3 ms: 1.03x faster                                                 |
| xml_etree_iterparse  | 68.3 ms                                                | 67.2 ms: 1.02x faster                                                 |
| unpickle             | 8.29 us                                                | 8.32 us: 1.00x slower                                                 |
| json_dumps           | 7.53 ms                                                | 7.57 ms: 1.00x slower                                                 |
| json_loads           | 15.3 us                                                | 15.5 us: 1.01x slower                                                 |
| xml_etree_process    | 33.6 ms                                                | 34.2 ms: 1.02x slower                                                 |
| unpickle_pure_python | 149 us                                                 | 152 us: 1.02x slower                                                  |
| xml_etree_generate   | 45.8 ms                                                | 46.9 ms: 1.02x slower                                                 |
| pickle_pure_python   | 191 us                                                 | 196 us: 1.03x slower                                                  |
| tomli_loads          | 1.27 sec                                               | 1.31 sec: 1.03x slower                                                |
| unpickle_list        | 2.69 us                                                | 2.77 us: 1.03x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                          |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.4 ms: 1.06x slower                                                 |
| python_startup_no_site | 8.57 ms                                                | 9.27 ms: 1.08x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.07x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 20.1 ms                                                | 19.6 ms: 1.03x faster                                                 |
| genshi_xml      | 28.5 ms                                                | 28.7 ms: 1.01x slower                                                 |
| genshi_text     | 14.4 ms                                                | 14.5 ms: 1.01x slower                                                 |
| mako            | 7.93 ms                                                | 8.18 ms: 1.03x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.00x slower                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot               | 2.43 ms                                                | 2.26 ms: 1.07x faster                                                 |
| html5lib                   | 33.0 ms                                                | 31.0 ms: 1.06x faster                                                 |
| pickle_list                | 2.70 us                                                | 2.55 us: 1.06x faster                                                 |
| pickle_dict                | 17.1 us                                                | 16.2 us: 1.05x faster                                                 |
| xml_etree_parse            | 100 ms                                                 | 97.3 ms: 1.03x faster                                                 |
| regex_dna                  | 148 ms                                                 | 144 ms: 1.03x faster                                                  |
| docutils                   | 1.43 sec                                               | 1.39 sec: 1.03x faster                                                |
| sympy_sum                  | 80.2 ms                                                | 78.1 ms: 1.03x faster                                                 |
| nqueens                    | 55.9 ms                                                | 54.5 ms: 1.03x faster                                                 |
| django_template            | 20.1 ms                                                | 19.6 ms: 1.03x faster                                                 |
| unpack_sequence            | 33.6 ns                                                | 32.9 ns: 1.02x faster                                                 |
| coroutines                 | 17.2 ms                                                | 16.9 ms: 1.02x faster                                                 |
| async_tree_none            | 282 ms                                                 | 277 ms: 1.02x faster                                                  |
| deltablue                  | 2.75 ms                                                | 2.71 ms: 1.02x faster                                                 |
| go                         | 105 ms                                                 | 104 ms: 1.02x faster                                                  |
| xml_etree_iterparse        | 68.3 ms                                                | 67.2 ms: 1.02x faster                                                 |
| generators                 | 30.3 ms                                                | 29.9 ms: 1.01x faster                                                 |
| scimark_sor                | 79.2 ms                                                | 78.2 ms: 1.01x faster                                                 |
| raytrace                   | 206 ms                                                 | 203 ms: 1.01x faster                                                  |
| sympy_integrate            | 11.3 ms                                                | 11.1 ms: 1.01x faster                                                 |
| 2to3                       | 154 ms                                                 | 152 ms: 1.01x faster                                                  |
| async_tree_io              | 697 ms                                                 | 690 ms: 1.01x faster                                                  |
| logging_silent             | 66.5 ns                                                | 65.8 ns: 1.01x faster                                                 |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 514 ms: 1.01x faster                                                  |
| async_generators           | 192 ms                                                 | 190 ms: 1.01x faster                                                  |
| sympy_str                  | 144 ms                                                 | 143 ms: 1.00x faster                                                  |
| asyncio_websockets         | 408 ms                                                 | 407 ms: 1.00x faster                                                  |
| gc_traversal               | 2.38 ms                                                | 2.38 ms: 1.00x faster                                                 |
| hexiom                     | 4.58 ms                                                | 4.59 ms: 1.00x slower                                                 |
| telco                      | 3.17 ms                                                | 3.18 ms: 1.00x slower                                                 |
| unpickle                   | 8.29 us                                                | 8.32 us: 1.00x slower                                                 |
| regex_compile              | 72.8 ms                                                | 73.1 ms: 1.00x slower                                                 |
| json_dumps                 | 7.53 ms                                                | 7.57 ms: 1.00x slower                                                 |
| chameleon                  | 4.30 ms                                                | 4.32 ms: 1.00x slower                                                 |
| json                       | 2.75 ms                                                | 2.77 ms: 1.01x slower                                                 |
| create_gc_cycles           | 711 us                                                 | 715 us: 1.01x slower                                                  |
| crypto_pyaes               | 47.5 ms                                                | 47.8 ms: 1.01x slower                                                 |
| pprint_pformat             | 979 ms                                                 | 985 ms: 1.01x slower                                                  |
| genshi_xml                 | 28.5 ms                                                | 28.7 ms: 1.01x slower                                                 |
| genshi_text                | 14.4 ms                                                | 14.5 ms: 1.01x slower                                                 |
| sqlalchemy_declarative     | 59.3 ms                                                | 59.7 ms: 1.01x slower                                                 |
| pyflate                    | 284 ms                                                 | 286 ms: 1.01x slower                                                  |
| json_loads                 | 15.3 us                                                | 15.5 us: 1.01x slower                                                 |
| pprint_safe_repr           | 478 ms                                                 | 482 ms: 1.01x slower                                                  |
| scimark_lu                 | 67.7 ms                                                | 68.4 ms: 1.01x slower                                                 |
| flaskblogging              | 2.35 ms                                                | 2.38 ms: 1.01x slower                                                 |
| dulwich_log                | 28.6 ms                                                | 28.9 ms: 1.01x slower                                                 |
| sympy_expand               | 229 ms                                                 | 232 ms: 1.01x slower                                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 44.1 ms: 1.01x slower                                                 |
| sqlglot_normalize          | 162 ms                                                 | 164 ms: 1.01x slower                                                  |
| chaos                      | 47.4 ms                                                | 48.2 ms: 1.02x slower                                                 |
| bench_mp_pool              | 41.0 ms                                                | 41.7 ms: 1.02x slower                                                 |
| async_tree_io_tg           | 724 ms                                                 | 737 ms: 1.02x slower                                                  |
| xml_etree_process          | 33.6 ms                                                | 34.2 ms: 1.02x slower                                                 |
| meteor_contest             | 71.1 ms                                                | 72.5 ms: 1.02x slower                                                 |
| unpickle_pure_python       | 149 us                                                 | 152 us: 1.02x slower                                                  |
| sqlalchemy_imperative      | 6.98 ms                                                | 7.14 ms: 1.02x slower                                                 |
| xml_etree_generate         | 45.8 ms                                                | 46.9 ms: 1.02x slower                                                 |
| pickle_pure_python         | 191 us                                                 | 196 us: 1.03x slower                                                  |
| asyncio_tcp                | 643 ms                                                 | 660 ms: 1.03x slower                                                  |
| sqlglot_optimize           | 29.6 ms                                                | 30.5 ms: 1.03x slower                                                 |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.43 sec: 1.03x slower                                                |
| tomli_loads                | 1.27 sec                                               | 1.31 sec: 1.03x slower                                                |
| unpickle_list              | 2.69 us                                                | 2.77 us: 1.03x slower                                                 |
| fannkuch                   | 240 ms                                                 | 247 ms: 1.03x slower                                                  |
| mako                       | 7.93 ms                                                | 8.18 ms: 1.03x slower                                                 |
| bench_thread_pool          | 465 us                                                 | 480 us: 1.03x slower                                                  |
| spectral_norm              | 65.7 ms                                                | 68.2 ms: 1.04x slower                                                 |
| regex_v8                   | 15.1 ms                                                | 15.8 ms: 1.04x slower                                                 |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 2.95 ms: 1.05x slower                                                 |
| float                      | 50.8 ms                                                | 53.3 ms: 1.05x slower                                                 |
| async_tree_memoization     | 336 ms                                                 | 353 ms: 1.05x slower                                                  |
| scimark_fft                | 173 ms                                                 | 182 ms: 1.06x slower                                                  |
| deepcopy                   | 215 us                                                 | 228 us: 1.06x slower                                                  |
| sqlite_synth               | 1.26 us                                                | 1.33 us: 1.06x slower                                                 |
| python_startup             | 10.8 ms                                                | 11.4 ms: 1.06x slower                                                 |
| nbody                      | 61.7 ms                                                | 65.6 ms: 1.06x slower                                                 |
| gunicorn                   | 1.10 ms                                                | 1.18 ms: 1.08x slower                                                 |
| deepcopy_reduce            | 1.79 us                                                | 1.93 us: 1.08x slower                                                 |
| deepcopy_memo              | 25.7 us                                                | 27.8 us: 1.08x slower                                                 |
| aiohttp                    | 1.02 ms                                                | 1.11 ms: 1.08x slower                                                 |
| python_startup_no_site     | 8.57 ms                                                | 9.27 ms: 1.08x slower                                                 |
| typing_runtime_protocols   | 301 us                                                 | 327 us: 1.09x slower                                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 607 ms: 1.10x slower                                                  |
| mdp                        | 1.48 sec                                               | 1.73 sec: 1.17x slower                                                |
| comprehensions             | 14.4 us                                                | 17.1 us: 1.18x slower                                                 |
| async_tree_none_tg         | 276 ms                                                 | 332 ms: 1.20x slower                                                  |
| sqlglot_transpile          | 1.05 ms                                                | 1.29 ms: 1.22x slower                                                 |
| async_tree_memoization_tg  | 352 ms                                                 | 434 ms: 1.23x slower                                                  |
| sqlglot_parse              | 890 us                                                 | 1.12 ms: 1.26x slower                                                 |
| coverage                   | 43.9 ms                                                | 73.6 ms: 1.68x slower                                                 |
| Geometric mean             | (ref)                                                  | 1.03x slower                                                          |

Benchmark hidden because not significant (12): pathlib, logging_simple, pycparser, thrift, pickle, pylint, pidigits, logging_format, richards, dask, richards_super, tornado_http
Ignored benchmarks (1) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: mypy2


# HPT report

- Reliability score: 99.94% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x