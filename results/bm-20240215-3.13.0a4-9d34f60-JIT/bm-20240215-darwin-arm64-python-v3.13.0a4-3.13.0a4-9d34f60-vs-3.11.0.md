# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a4
- machine: darwin-arm64
- commit hash: 9d34f60
- commit date: 2024-02-15
- overall geometric mean: 1.04x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.18x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 190 ms: 1.23x slower                                       |
| chameleon      | 4.30 ms                                                | 4.81 ms: 1.12x slower                                      |
| docutils       | 1.43 sec                                               | 1.48 sec: 1.03x slower                                     |
| Geometric mean | (ref)                                                  | 1.10x slower                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                       |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                       |
| async_tree_io_tg           | 724 ms                                                 | 666 ms: 1.09x faster                                       |
| async_tree_none_tg         | 276 ms                                                 | 259 ms: 1.07x faster                                       |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 530 ms: 1.04x faster                                       |
| async_tree_memoization     | 336 ms                                                 | 328 ms: 1.03x faster                                       |
| Geometric mean             | (ref)                                                  | 1.05x faster                                               |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 283 ms: 1.01x slower                                       |
| float          | 50.8 ms                                                | 55.5 ms: 1.09x slower                                      |
| nbody          | 61.7 ms                                                | 75.9 ms: 1.23x slower                                      |
| Geometric mean | (ref)                                                  | 1.11x slower                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 150 ms: 1.01x slower                                       |
| regex_compile  | 72.8 ms                                                | 75.1 ms: 1.03x slower                                      |
| regex_effbot   | 2.43 ms                                                | 2.54 ms: 1.05x slower                                      |
| regex_v8       | 15.1 ms                                                | 17.4 ms: 1.15x slower                                      |
| Geometric mean | (ref)                                                  | 1.06x slower                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.48 ms: 1.16x faster                                      |
| pickle_pure_python   | 191 us                                                 | 196 us: 1.02x slower                                       |
| pickle               | 6.98 us                                                | 7.33 us: 1.05x slower                                      |
| xml_etree_parse      | 100 ms                                                 | 105 ms: 1.05x slower                                       |
| unpickle_pure_python | 149 us                                                 | 158 us: 1.06x slower                                       |
| pickle_dict          | 17.1 us                                                | 18.2 us: 1.06x slower                                      |
| xml_etree_iterparse  | 68.3 ms                                                | 74.8 ms: 1.10x slower                                      |
| json_loads           | 15.3 us                                                | 16.9 us: 1.10x slower                                      |
| tomli_loads          | 1.27 sec                                               | 1.40 sec: 1.10x slower                                     |
| unpickle             | 8.29 us                                                | 9.18 us: 1.11x slower                                      |
| pickle_list          | 2.70 us                                                | 2.99 us: 1.11x slower                                      |
| unpickle_list        | 2.69 us                                                | 3.10 us: 1.15x slower                                      |
| xml_etree_process    | 33.6 ms                                                | 38.7 ms: 1.15x slower                                      |
| xml_etree_generate   | 45.8 ms                                                | 56.1 ms: 1.22x slower                                      |
| Geometric mean       | (ref)                                                  | 1.08x slower                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 13.1 ms: 1.22x slower                                      |
| python_startup_no_site | 8.57 ms                                                | 11.6 ms: 1.35x slower                                      |
| Geometric mean         | (ref)                                                  | 1.28x slower                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 7.93 ms                                                | 7.79 ms: 1.02x faster                                      |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-darwin-arm64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 70.9 us: 4.24x faster                                      |
| asyncio_tcp                | 643 ms                                                 | 401 ms: 1.60x faster                                       |
| unpack_sequence            | 33.6 ns                                                | 28.4 ns: 1.18x faster                                      |
| raytrace                   | 206 ms                                                 | 176 ms: 1.17x faster                                       |
| json_dumps                 | 7.53 ms                                                | 6.48 ms: 1.16x faster                                      |
| chaos                      | 47.4 ms                                                | 41.0 ms: 1.16x faster                                      |
| comprehensions             | 14.4 us                                                | 12.6 us: 1.15x faster                                      |
| sqlglot_parse              | 890 us                                                 | 787 us: 1.13x faster                                       |
| deltablue                  | 2.75 ms                                                | 2.45 ms: 1.12x faster                                      |
| async_tree_none            | 282 ms                                                 | 252 ms: 1.12x faster                                       |
| async_tree_memoization_tg  | 352 ms                                                 | 322 ms: 1.09x faster                                       |
| async_tree_io_tg           | 724 ms                                                 | 666 ms: 1.09x faster                                       |
| sqlglot_transpile          | 1.05 ms                                                | 973 us: 1.08x faster                                       |
| generators                 | 30.3 ms                                                | 28.3 ms: 1.07x faster                                      |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.31 sec: 1.07x faster                                     |
| async_tree_none_tg         | 276 ms                                                 | 259 ms: 1.07x faster                                       |
| sympy_sum                  | 80.2 ms                                                | 75.3 ms: 1.07x faster                                      |
| richards_super             | 37.3 ms                                                | 35.7 ms: 1.05x faster                                      |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 530 ms: 1.04x faster                                       |
| async_tree_memoization     | 336 ms                                                 | 328 ms: 1.03x faster                                       |
| sympy_str                  | 144 ms                                                 | 141 ms: 1.02x faster                                       |
| mako                       | 7.93 ms                                                | 7.79 ms: 1.02x faster                                      |
| sympy_integrate            | 11.3 ms                                                | 11.1 ms: 1.02x faster                                      |
| create_gc_cycles           | 711 us                                                 | 705 us: 1.01x faster                                       |
| asyncio_websockets         | 408 ms                                                 | 409 ms: 1.00x slower                                       |
| gc_traversal               | 2.38 ms                                                | 2.39 ms: 1.00x slower                                      |
| pidigits                   | 280 ms                                                 | 283 ms: 1.01x slower                                       |
| logging_simple             | 3.41 us                                                | 3.45 us: 1.01x slower                                      |
| regex_dna                  | 148 ms                                                 | 150 ms: 1.01x slower                                       |
| deepcopy_memo              | 25.7 us                                                | 26.3 us: 1.02x slower                                      |
| logging_format             | 3.67 us                                                | 3.76 us: 1.02x slower                                      |
| pickle_pure_python         | 191 us                                                 | 196 us: 1.02x slower                                       |
| richards                   | 31.1 ms                                                | 31.9 ms: 1.03x slower                                      |
| regex_compile              | 72.8 ms                                                | 75.1 ms: 1.03x slower                                      |
| crypto_pyaes               | 47.5 ms                                                | 49.1 ms: 1.03x slower                                      |
| docutils                   | 1.43 sec                                               | 1.48 sec: 1.03x slower                                     |
| dulwich_log                | 28.6 ms                                                | 29.8 ms: 1.04x slower                                      |
| go                         | 105 ms                                                 | 110 ms: 1.04x slower                                       |
| regex_effbot               | 2.43 ms                                                | 2.54 ms: 1.05x slower                                      |
| meteor_contest             | 71.1 ms                                                | 74.3 ms: 1.05x slower                                      |
| deepcopy                   | 215 us                                                 | 226 us: 1.05x slower                                       |
| pickle                     | 6.98 us                                                | 7.33 us: 1.05x slower                                      |
| pycparser                  | 659 ms                                                 | 693 ms: 1.05x slower                                       |
| xml_etree_parse            | 100 ms                                                 | 105 ms: 1.05x slower                                       |
| sympy_expand               | 229 ms                                                 | 241 ms: 1.05x slower                                       |
| logging_silent             | 66.5 ns                                                | 70.3 ns: 1.06x slower                                      |
| unpickle_pure_python       | 149 us                                                 | 158 us: 1.06x slower                                       |
| pickle_dict                | 17.1 us                                                | 18.2 us: 1.06x slower                                      |
| json                       | 2.75 ms                                                | 2.95 ms: 1.07x slower                                      |
| pprint_pformat             | 979 ms                                                 | 1.05 sec: 1.07x slower                                     |
| hexiom                     | 4.58 ms                                                | 4.91 ms: 1.07x slower                                      |
| pprint_safe_repr           | 478 ms                                                 | 515 ms: 1.08x slower                                       |
| coverage                   | 43.9 ms                                                | 47.5 ms: 1.08x slower                                      |
| bench_thread_pool          | 465 us                                                 | 504 us: 1.08x slower                                       |
| mdp                        | 1.48 sec                                               | 1.61 sec: 1.09x slower                                     |
| coroutines                 | 17.2 ms                                                | 18.7 ms: 1.09x slower                                      |
| float                      | 50.8 ms                                                | 55.5 ms: 1.09x slower                                      |
| pathlib                    | 23.2 ms                                                | 25.4 ms: 1.09x slower                                      |
| xml_etree_iterparse        | 68.3 ms                                                | 74.8 ms: 1.10x slower                                      |
| nqueens                    | 55.9 ms                                                | 61.6 ms: 1.10x slower                                      |
| json_loads                 | 15.3 us                                                | 16.9 us: 1.10x slower                                      |
| tomli_loads                | 1.27 sec                                               | 1.40 sec: 1.10x slower                                     |
| scimark_lu                 | 67.7 ms                                                | 74.8 ms: 1.10x slower                                      |
| deepcopy_reduce            | 1.79 us                                                | 1.98 us: 1.11x slower                                      |
| unpickle                   | 8.29 us                                                | 9.18 us: 1.11x slower                                      |
| pickle_list                | 2.70 us                                                | 2.99 us: 1.11x slower                                      |
| fannkuch                   | 240 ms                                                 | 267 ms: 1.11x slower                                       |
| scimark_monte_carlo        | 43.5 ms                                                | 48.5 ms: 1.12x slower                                      |
| chameleon                  | 4.30 ms                                                | 4.81 ms: 1.12x slower                                      |
| bench_mp_pool              | 41.0 ms                                                | 45.9 ms: 1.12x slower                                      |
| sqlglot_normalize          | 162 ms                                                 | 182 ms: 1.12x slower                                       |
| regex_v8                   | 15.1 ms                                                | 17.4 ms: 1.15x slower                                      |
| pyflate                    | 284 ms                                                 | 326 ms: 1.15x slower                                       |
| unpickle_list              | 2.69 us                                                | 3.10 us: 1.15x slower                                      |
| xml_etree_process          | 33.6 ms                                                | 38.7 ms: 1.15x slower                                      |
| sqlglot_optimize           | 29.6 ms                                                | 34.4 ms: 1.16x slower                                      |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.31 ms: 1.18x slower                                      |
| spectral_norm              | 65.7 ms                                                | 78.8 ms: 1.20x slower                                      |
| python_startup             | 10.8 ms                                                | 13.1 ms: 1.22x slower                                      |
| xml_etree_generate         | 45.8 ms                                                | 56.1 ms: 1.22x slower                                      |
| nbody                      | 61.7 ms                                                | 75.9 ms: 1.23x slower                                      |
| 2to3                       | 154 ms                                                 | 190 ms: 1.23x slower                                       |
| scimark_fft                | 173 ms                                                 | 213 ms: 1.23x slower                                       |
| sqlite_synth               | 1.26 us                                                | 1.59 us: 1.27x slower                                      |
| scimark_sor                | 79.2 ms                                                | 106 ms: 1.33x slower                                       |
| python_startup_no_site     | 8.57 ms                                                | 11.6 ms: 1.35x slower                                      |
| telco                      | 3.17 ms                                                | 4.51 ms: 1.42x slower                                      |
| dask                       | 219 ms                                                 | 335 ms: 1.53x slower                                       |
| mypy2                      | 372 ms                                                 | 577 ms: 1.55x slower                                       |
| async_generators           | 192 ms                                                 | 303 ms: 1.58x slower                                       |
| Geometric mean             | (ref)                                                  | 1.04x slower                                               |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_io, tornado_http
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.18x