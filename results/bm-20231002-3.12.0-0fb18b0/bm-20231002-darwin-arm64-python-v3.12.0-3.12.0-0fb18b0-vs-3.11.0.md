
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0
- machine: darwin-arm64
- commit hash: 0fb18b0
- commit date: 2023-10-02
- overall geometric mean: 1.03x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 169 ms: 1.10x slower                                   |
| chameleon      | 4.30 ms                                                | 4.70 ms: 1.09x slower                                  |
| docutils       | 1.43 sec                                               | 1.50 sec: 1.05x slower                                 |
| Geometric mean | (ref)                                                  | 1.06x slower                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization_tg  | 352 ms                                                 | 323 ms: 1.09x faster                                   |
| async_tree_io_tg           | 724 ms                                                 | 669 ms: 1.08x faster                                   |
| async_tree_memoization     | 336 ms                                                 | 312 ms: 1.08x faster                                   |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                   |
| async_tree_none            | 282 ms                                                 | 266 ms: 1.06x faster                                   |
| async_tree_io              | 697 ms                                                 | 668 ms: 1.04x faster                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 532 ms: 1.03x faster                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 526 ms: 1.01x slower                                   |
| Geometric mean             | (ref)                                                  | 1.06x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.00x slower                                   |
| float          | 50.8 ms                                                | 55.8 ms: 1.10x slower                                  |
| nbody          | 61.7 ms                                                | 68.8 ms: 1.12x slower                                  |
| Geometric mean | (ref)                                                  | 1.07x slower                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 154 ms: 1.04x slower                                   |
| regex_v8       | 15.1 ms                                                | 16.0 ms: 1.05x slower                                  |
| regex_compile  | 72.8 ms                                                | 77.9 ms: 1.07x slower                                  |
| regex_effbot   | 2.43 ms                                                | 2.64 ms: 1.09x slower                                  |
| Geometric mean | (ref)                                                  | 1.06x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.22 ms: 1.21x faster                                  |
| unpickle_pure_python | 149 us                                                 | 151 us: 1.01x slower                                   |
| pickle               | 6.98 us                                                | 7.23 us: 1.04x slower                                  |
| pickle_pure_python   | 191 us                                                 | 200 us: 1.04x slower                                   |
| pickle_dict          | 17.1 us                                                | 18.1 us: 1.06x slower                                  |
| xml_etree_parse      | 100 ms                                                 | 106 ms: 1.06x slower                                   |
| pickle_list          | 2.70 us                                                | 2.89 us: 1.07x slower                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 74.0 ms: 1.08x slower                                  |
| tomli_loads          | 1.27 sec                                               | 1.39 sec: 1.09x slower                                 |
| unpickle             | 8.29 us                                                | 9.12 us: 1.10x slower                                  |
| json_loads           | 15.3 us                                                | 17.2 us: 1.12x slower                                  |
| unpickle_list        | 2.69 us                                                | 3.02 us: 1.12x slower                                  |
| xml_etree_process    | 33.6 ms                                                | 39.7 ms: 1.18x slower                                  |
| xml_etree_generate   | 45.8 ms                                                | 55.8 ms: 1.22x slower                                  |
| Geometric mean       | (ref)                                                  | 1.07x slower                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.4 ms: 1.06x slower                                  |
| python_startup_no_site | 8.57 ms                                                | 9.37 ms: 1.09x slower                                  |
| Geometric mean         | (ref)                                                  | 1.08x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 7.93 ms                                                | 7.71 ms: 1.03x faster                                  |
| django_template | 20.1 ms                                                | 22.3 ms: 1.11x slower                                  |
| Geometric mean  | (ref)                                                  | 1.04x slower                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 93.0 us: 3.24x faster                                  |
| asyncio_tcp                | 643 ms                                                 | 449 ms: 1.43x faster                                   |
| json_dumps                 | 7.53 ms                                                | 6.22 ms: 1.21x faster                                  |
| coverage                   | 43.9 ms                                                | 38.9 ms: 1.13x faster                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.24 sec: 1.12x faster                                 |
| chaos                      | 47.4 ms                                                | 42.5 ms: 1.11x faster                                  |
| async_tree_memoization_tg  | 352 ms                                                 | 323 ms: 1.09x faster                                   |
| async_tree_io_tg           | 724 ms                                                 | 669 ms: 1.08x faster                                   |
| async_tree_memoization     | 336 ms                                                 | 312 ms: 1.08x faster                                   |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                   |
| unpack_sequence            | 33.6 ns                                                | 31.5 ns: 1.07x faster                                  |
| async_tree_none            | 282 ms                                                 | 266 ms: 1.06x faster                                   |
| sqlglot_parse              | 890 us                                                 | 848 us: 1.05x faster                                   |
| sqlalchemy_imperative      | 6.98 ms                                                | 6.68 ms: 1.04x faster                                  |
| async_tree_io              | 697 ms                                                 | 668 ms: 1.04x faster                                   |
| go                         | 105 ms                                                 | 102 ms: 1.04x faster                                   |
| richards_super             | 37.3 ms                                                | 36.0 ms: 1.03x faster                                  |
| sympy_sum                  | 80.2 ms                                                | 77.6 ms: 1.03x faster                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 532 ms: 1.03x faster                                   |
| sqlglot_transpile          | 1.05 ms                                                | 1.02 ms: 1.03x faster                                  |
| mako                       | 7.93 ms                                                | 7.71 ms: 1.03x faster                                  |
| deltablue                  | 2.75 ms                                                | 2.71 ms: 1.02x faster                                  |
| create_gc_cycles           | 711 us                                                 | 701 us: 1.01x faster                                   |
| hexiom                     | 4.58 ms                                                | 4.54 ms: 1.01x faster                                  |
| asyncio_websockets         | 408 ms                                                 | 409 ms: 1.00x slower                                   |
| pidigits                   | 280 ms                                                 | 282 ms: 1.00x slower                                   |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                  |
| comprehensions             | 14.4 us                                                | 14.5 us: 1.01x slower                                  |
| sympy_integrate            | 11.3 ms                                                | 11.4 ms: 1.01x slower                                  |
| meteor_contest             | 71.1 ms                                                | 71.7 ms: 1.01x slower                                  |
| unpickle_pure_python       | 149 us                                                 | 151 us: 1.01x slower                                   |
| async_tree_cpu_io_mixed    | 519 ms                                                 | 526 ms: 1.01x slower                                   |
| dask                       | 219 ms                                                 | 222 ms: 1.01x slower                                   |
| mypy2                      | 372 ms                                                 | 380 ms: 1.02x slower                                   |
| generators                 | 30.3 ms                                                | 31.1 ms: 1.03x slower                                  |
| pycparser                  | 659 ms                                                 | 677 ms: 1.03x slower                                   |
| sympy_str                  | 144 ms                                                 | 148 ms: 1.03x slower                                   |
| raytrace                   | 206 ms                                                 | 212 ms: 1.03x slower                                   |
| pprint_pformat             | 979 ms                                                 | 1.01 sec: 1.03x slower                                 |
| richards                   | 31.1 ms                                                | 32.1 ms: 1.03x slower                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 45.0 ms: 1.04x slower                                  |
| pickle                     | 6.98 us                                                | 7.23 us: 1.04x slower                                  |
| fannkuch                   | 240 ms                                                 | 248 ms: 1.04x slower                                   |
| pprint_safe_repr           | 478 ms                                                 | 497 ms: 1.04x slower                                   |
| regex_dna                  | 148 ms                                                 | 154 ms: 1.04x slower                                   |
| dulwich_log                | 28.6 ms                                                | 29.8 ms: 1.04x slower                                  |
| pathlib                    | 23.2 ms                                                | 24.2 ms: 1.04x slower                                  |
| pickle_pure_python         | 191 us                                                 | 200 us: 1.04x slower                                   |
| gunicorn                   | 1.10 ms                                                | 1.15 ms: 1.05x slower                                  |
| docutils                   | 1.43 sec                                               | 1.50 sec: 1.05x slower                                 |
| sqlalchemy_declarative     | 59.3 ms                                                | 62.3 ms: 1.05x slower                                  |
| sympy_expand               | 229 ms                                                 | 241 ms: 1.05x slower                                   |
| regex_v8                   | 15.1 ms                                                | 16.0 ms: 1.05x slower                                  |
| aiohttp                    | 1.02 ms                                                | 1.08 ms: 1.05x slower                                  |
| pickle_dict                | 17.1 us                                                | 18.1 us: 1.06x slower                                  |
| xml_etree_parse            | 100 ms                                                 | 106 ms: 1.06x slower                                   |
| python_startup             | 10.8 ms                                                | 11.4 ms: 1.06x slower                                  |
| mdp                        | 1.48 sec                                               | 1.58 sec: 1.06x slower                                 |
| regex_compile              | 72.8 ms                                                | 77.9 ms: 1.07x slower                                  |
| pickle_list                | 2.70 us                                                | 2.89 us: 1.07x slower                                  |
| deepcopy_memo              | 25.7 us                                                | 27.7 us: 1.07x slower                                  |
| logging_simple             | 3.41 us                                                | 3.69 us: 1.08x slower                                  |
| bench_thread_pool          | 465 us                                                 | 504 us: 1.08x slower                                   |
| logging_format             | 3.67 us                                                | 3.98 us: 1.08x slower                                  |
| xml_etree_iterparse        | 68.3 ms                                                | 74.0 ms: 1.08x slower                                  |
| regex_effbot               | 2.43 ms                                                | 2.64 ms: 1.09x slower                                  |
| deepcopy                   | 215 us                                                 | 235 us: 1.09x slower                                   |
| chameleon                  | 4.30 ms                                                | 4.70 ms: 1.09x slower                                  |
| crypto_pyaes               | 47.5 ms                                                | 51.9 ms: 1.09x slower                                  |
| python_startup_no_site     | 8.57 ms                                                | 9.37 ms: 1.09x slower                                  |
| tomli_loads                | 1.27 sec                                               | 1.39 sec: 1.09x slower                                 |
| bench_mp_pool              | 41.0 ms                                                | 44.9 ms: 1.09x slower                                  |
| float                      | 50.8 ms                                                | 55.8 ms: 1.10x slower                                  |
| 2to3                       | 154 ms                                                 | 169 ms: 1.10x slower                                   |
| unpickle                   | 8.29 us                                                | 9.12 us: 1.10x slower                                  |
| scimark_sor                | 79.2 ms                                                | 87.4 ms: 1.10x slower                                  |
| django_template            | 20.1 ms                                                | 22.3 ms: 1.11x slower                                  |
| pyflate                    | 284 ms                                                 | 316 ms: 1.11x slower                                   |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.14 ms: 1.11x slower                                  |
| nbody                      | 61.7 ms                                                | 68.8 ms: 1.12x slower                                  |
| nqueens                    | 55.9 ms                                                | 62.4 ms: 1.12x slower                                  |
| coroutines                 | 17.2 ms                                                | 19.2 ms: 1.12x slower                                  |
| scimark_lu                 | 67.7 ms                                                | 76.0 ms: 1.12x slower                                  |
| json                       | 2.75 ms                                                | 3.09 ms: 1.12x slower                                  |
| json_loads                 | 15.3 us                                                | 17.2 us: 1.12x slower                                  |
| unpickle_list              | 2.69 us                                                | 3.02 us: 1.12x slower                                  |
| scimark_fft                | 173 ms                                                 | 195 ms: 1.13x slower                                   |
| sqlglot_normalize          | 162 ms                                                 | 186 ms: 1.15x slower                                   |
| sqlglot_optimize           | 29.6 ms                                                | 34.0 ms: 1.15x slower                                  |
| logging_silent             | 66.5 ns                                                | 76.4 ns: 1.15x slower                                  |
| deepcopy_reduce            | 1.79 us                                                | 2.07 us: 1.15x slower                                  |
| telco                      | 3.17 ms                                                | 3.68 ms: 1.16x slower                                  |
| spectral_norm              | 65.7 ms                                                | 76.4 ms: 1.16x slower                                  |
| xml_etree_process          | 33.6 ms                                                | 39.7 ms: 1.18x slower                                  |
| xml_etree_generate         | 45.8 ms                                                | 55.8 ms: 1.22x slower                                  |
| sqlite_synth               | 1.26 us                                                | 1.57 us: 1.25x slower                                  |
| async_generators           | 192 ms                                                 | 304 ms: 1.58x slower                                   |
| Geometric mean             | (ref)                                                  | 1.03x slower                                           |

Benchmark hidden because not significant (1): tornado_http
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.04x