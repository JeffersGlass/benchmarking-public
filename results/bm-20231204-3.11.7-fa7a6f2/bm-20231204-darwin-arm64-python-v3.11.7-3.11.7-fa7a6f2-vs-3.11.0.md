
# Results vs. 3.11.0

- fork: python
- ref: v3.11.7
- machine: darwin-arm64
- commit hash: fa7a6f2
- commit date: 2023-12-04
- overall geometric mean: 1.02x slower
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 153 ms: 1.01x faster                                   |
| chameleon      | 4.30 ms                                                | 4.36 ms: 1.01x slower                                  |
| docutils       | 1.43 sec                                               | 1.41 sec: 1.02x faster                                 |
| html5lib       | 33.0 ms                                                | 33.8 ms: 1.03x slower                                  |
| Geometric mean | (ref)                                                  | 1.01x slower                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization     | 336 ms                                                 | 315 ms: 1.07x faster                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 334 ms: 1.05x faster                                   |
| async_tree_io_tg           | 724 ms                                                 | 700 ms: 1.03x faster                                   |
| async_tree_none_tg         | 276 ms                                                 | 271 ms: 1.02x faster                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 542 ms: 1.01x faster                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 516 ms: 1.01x faster                                   |
| Geometric mean             | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (2): async_tree_io, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 281 ms: 1.00x slower                                   |
| float          | 50.8 ms                                                | 53.5 ms: 1.05x slower                                  |
| nbody          | 61.7 ms                                                | 68.9 ms: 1.12x slower                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 152 ms: 1.03x slower                                   |
| regex_v8       | 15.1 ms                                                | 15.7 ms: 1.04x slower                                  |
| regex_effbot   | 2.43 ms                                                | 2.61 ms: 1.08x slower                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                           |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| xml_etree_parse      | 100 ms                                                 | 97.1 ms: 1.03x faster                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 67.8 ms: 1.01x faster                                  |
| pickle_dict          | 17.1 us                                                | 17.0 us: 1.01x faster                                  |
| pickle_list          | 2.70 us                                                | 2.69 us: 1.00x faster                                  |
| unpickle             | 8.29 us                                                | 8.32 us: 1.00x slower                                  |
| pickle_pure_python   | 191 us                                                 | 193 us: 1.01x slower                                   |
| json_dumps           | 7.53 ms                                                | 7.60 ms: 1.01x slower                                  |
| unpickle_pure_python | 149 us                                                 | 151 us: 1.01x slower                                   |
| xml_etree_process    | 33.6 ms                                                | 34.4 ms: 1.02x slower                                  |
| xml_etree_generate   | 45.8 ms                                                | 47.2 ms: 1.03x slower                                  |
| unpickle_list        | 2.69 us                                                | 2.78 us: 1.04x slower                                  |
| tomli_loads          | 1.27 sec                                               | 1.32 sec: 1.04x slower                                 |
| pickle               | 6.98 us                                                | 7.26 us: 1.04x slower                                  |
| Geometric mean       | (ref)                                                  | 1.01x slower                                           |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.9 ms: 1.10x slower                                  |
| python_startup_no_site | 8.57 ms                                                | 9.93 ms: 1.16x slower                                  |
| Geometric mean         | (ref)                                                  | 1.13x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 20.1 ms                                                | 19.7 ms: 1.02x faster                                  |
| genshi_xml      | 28.5 ms                                                | 28.9 ms: 1.01x slower                                  |
| genshi_text     | 14.4 ms                                                | 14.8 ms: 1.03x slower                                  |
| mako            | 7.93 ms                                                | 8.19 ms: 1.03x slower                                  |
| Geometric mean  | (ref)                                                  | 1.01x slower                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-darwin-arm64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization     | 336 ms                                                 | 315 ms: 1.07x faster                                   |
| async_tree_memoization_tg  | 352 ms                                                 | 334 ms: 1.05x faster                                   |
| scimark_sor                | 79.2 ms                                                | 76.4 ms: 1.04x faster                                  |
| async_tree_io_tg           | 724 ms                                                 | 700 ms: 1.03x faster                                   |
| xml_etree_parse            | 100 ms                                                 | 97.1 ms: 1.03x faster                                  |
| async_generators           | 192 ms                                                 | 187 ms: 1.03x faster                                   |
| pylint                     | 253 ms                                                 | 246 ms: 1.03x faster                                   |
| deepcopy                   | 215 us                                                 | 211 us: 1.02x faster                                   |
| async_tree_none_tg         | 276 ms                                                 | 271 ms: 1.02x faster                                   |
| django_template            | 20.1 ms                                                | 19.7 ms: 1.02x faster                                  |
| coroutines                 | 17.2 ms                                                | 16.9 ms: 1.02x faster                                  |
| generators                 | 30.3 ms                                                | 29.8 ms: 1.02x faster                                  |
| docutils                   | 1.43 sec                                               | 1.41 sec: 1.02x faster                                 |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 542 ms: 1.01x faster                                   |
| sympy_integrate            | 11.3 ms                                                | 11.1 ms: 1.01x faster                                  |
| deepcopy_memo              | 25.7 us                                                | 25.5 us: 1.01x faster                                  |
| coverage                   | 43.9 ms                                                | 43.5 ms: 1.01x faster                                  |
| 2to3                       | 154 ms                                                 | 153 ms: 1.01x faster                                   |
| comprehensions             | 14.4 us                                                | 14.3 us: 1.01x faster                                  |
| xml_etree_iterparse        | 68.3 ms                                                | 67.8 ms: 1.01x faster                                  |
| pickle_dict                | 17.1 us                                                | 17.0 us: 1.01x faster                                  |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 516 ms: 1.01x faster                                   |
| nqueens                    | 55.9 ms                                                | 55.7 ms: 1.00x faster                                  |
| logging_silent             | 66.5 ns                                                | 66.2 ns: 1.00x faster                                  |
| pickle_list                | 2.70 us                                                | 2.69 us: 1.00x faster                                  |
| bench_thread_pool          | 465 us                                                 | 464 us: 1.00x faster                                   |
| asyncio_websockets         | 408 ms                                                 | 407 ms: 1.00x faster                                   |
| create_gc_cycles           | 711 us                                                 | 713 us: 1.00x slower                                   |
| pidigits                   | 280 ms                                                 | 281 ms: 1.00x slower                                   |
| unpickle                   | 8.29 us                                                | 8.32 us: 1.00x slower                                  |
| deepcopy_reduce            | 1.79 us                                                | 1.80 us: 1.00x slower                                  |
| deltablue                  | 2.75 ms                                                | 2.77 ms: 1.01x slower                                  |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                  |
| pickle_pure_python         | 191 us                                                 | 193 us: 1.01x slower                                   |
| pprint_pformat             | 979 ms                                                 | 986 ms: 1.01x slower                                   |
| json                       | 2.75 ms                                                | 2.77 ms: 1.01x slower                                  |
| sqlglot_normalize          | 162 ms                                                 | 163 ms: 1.01x slower                                   |
| json_dumps                 | 7.53 ms                                                | 7.60 ms: 1.01x slower                                  |
| pprint_safe_repr           | 478 ms                                                 | 483 ms: 1.01x slower                                   |
| crypto_pyaes               | 47.5 ms                                                | 48.0 ms: 1.01x slower                                  |
| genshi_xml                 | 28.5 ms                                                | 28.9 ms: 1.01x slower                                  |
| chameleon                  | 4.30 ms                                                | 4.36 ms: 1.01x slower                                  |
| scimark_lu                 | 67.7 ms                                                | 68.7 ms: 1.01x slower                                  |
| sqlglot_optimize           | 29.6 ms                                                | 30.0 ms: 1.01x slower                                  |
| unpickle_pure_python       | 149 us                                                 | 151 us: 1.01x slower                                   |
| sqlglot_transpile          | 1.05 ms                                                | 1.07 ms: 1.01x slower                                  |
| sqlglot_parse              | 890 us                                                 | 904 us: 1.02x slower                                   |
| hexiom                     | 4.58 ms                                                | 4.65 ms: 1.02x slower                                  |
| meteor_contest             | 71.1 ms                                                | 72.3 ms: 1.02x slower                                  |
| raytrace                   | 206 ms                                                 | 209 ms: 1.02x slower                                   |
| sqlalchemy_declarative     | 59.3 ms                                                | 60.4 ms: 1.02x slower                                  |
| go                         | 105 ms                                                 | 108 ms: 1.02x slower                                   |
| xml_etree_process          | 33.6 ms                                                | 34.4 ms: 1.02x slower                                  |
| asyncio_tcp                | 643 ms                                                 | 659 ms: 1.02x slower                                   |
| html5lib                   | 33.0 ms                                                | 33.8 ms: 1.03x slower                                  |
| chaos                      | 47.4 ms                                                | 48.6 ms: 1.03x slower                                  |
| sqlalchemy_imperative      | 6.98 ms                                                | 7.16 ms: 1.03x slower                                  |
| logging_simple             | 3.41 us                                                | 3.50 us: 1.03x slower                                  |
| regex_dna                  | 148 ms                                                 | 152 ms: 1.03x slower                                   |
| sympy_expand               | 229 ms                                                 | 235 ms: 1.03x slower                                   |
| pathlib                    | 23.2 ms                                                | 23.9 ms: 1.03x slower                                  |
| richards                   | 31.1 ms                                                | 31.9 ms: 1.03x slower                                  |
| pyflate                    | 284 ms                                                 | 292 ms: 1.03x slower                                   |
| xml_etree_generate         | 45.8 ms                                                | 47.2 ms: 1.03x slower                                  |
| genshi_text                | 14.4 ms                                                | 14.8 ms: 1.03x slower                                  |
| aiohttp                    | 1.02 ms                                                | 1.06 ms: 1.03x slower                                  |
| logging_format             | 3.67 us                                                | 3.79 us: 1.03x slower                                  |
| mako                       | 7.93 ms                                                | 8.19 ms: 1.03x slower                                  |
| unpickle_list              | 2.69 us                                                | 2.78 us: 1.04x slower                                  |
| tomli_loads                | 1.27 sec                                               | 1.32 sec: 1.04x slower                                 |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.45 sec: 1.04x slower                                 |
| regex_v8                   | 15.1 ms                                                | 15.7 ms: 1.04x slower                                  |
| richards_super             | 37.3 ms                                                | 38.8 ms: 1.04x slower                                  |
| pickle                     | 6.98 us                                                | 7.26 us: 1.04x slower                                  |
| fannkuch                   | 240 ms                                                 | 250 ms: 1.04x slower                                   |
| flaskblogging              | 2.35 ms                                                | 2.47 ms: 1.05x slower                                  |
| float                      | 50.8 ms                                                | 53.5 ms: 1.05x slower                                  |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 2.99 ms: 1.06x slower                                  |
| spectral_norm              | 65.7 ms                                                | 70.5 ms: 1.07x slower                                  |
| regex_effbot               | 2.43 ms                                                | 2.61 ms: 1.08x slower                                  |
| scimark_fft                | 173 ms                                                 | 188 ms: 1.09x slower                                   |
| typing_runtime_protocols   | 301 us                                                 | 328 us: 1.09x slower                                   |
| scimark_monte_carlo        | 43.5 ms                                                | 47.6 ms: 1.09x slower                                  |
| python_startup             | 10.8 ms                                                | 11.9 ms: 1.10x slower                                  |
| nbody                      | 61.7 ms                                                | 68.9 ms: 1.12x slower                                  |
| python_startup_no_site     | 8.57 ms                                                | 9.93 ms: 1.16x slower                                  |
| mdp                        | 1.48 sec                                               | 1.75 sec: 1.18x slower                                 |
| mypy2                      | 372 ms                                                 | 583 ms: 1.57x slower                                   |
| Geometric mean             | (ref)                                                  | 1.02x slower                                           |

Benchmark hidden because not significant (16): sympy_sum, telco, pycparser, regex_compile, async_tree_io, sqlite_synth, thrift, async_tree_none, sympy_str, json_loads, dulwich_log, bench_mp_pool, unpack_sequence, dask, tornado_http, gunicorn


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x