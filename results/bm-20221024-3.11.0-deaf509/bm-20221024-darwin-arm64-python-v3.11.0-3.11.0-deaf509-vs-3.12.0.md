
# Results vs. 3.12.0

- fork: python
- ref: v3.11.0
- machine: darwin-arm64
- commit hash: deaf509
- commit date: 2022-10-24
- overall geometric mean: 1.03x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 154 ms: 1.10x faster                                   |
| chameleon      | 4.70 ms                                                | 4.30 ms: 1.09x faster                                  |
| docutils       | 1.50 sec                                               | 1.43 sec: 1.05x faster                                 |
| Geometric mean | (ref)                                                  | 1.06x faster                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 519 ms: 1.01x faster                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 550 ms: 1.03x slower                                   |
| async_tree_io              | 668 ms                                                 | 697 ms: 1.04x slower                                   |
| async_tree_none            | 266 ms                                                 | 282 ms: 1.06x slower                                   |
| async_tree_none_tg         | 258 ms                                                 | 276 ms: 1.07x slower                                   |
| async_tree_memoization     | 312 ms                                                 | 336 ms: 1.08x slower                                   |
| async_tree_io_tg           | 669 ms                                                 | 724 ms: 1.08x slower                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 352 ms: 1.09x slower                                   |
| Geometric mean             | (ref)                                                  | 1.06x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 68.8 ms                                                | 61.7 ms: 1.12x faster                                  |
| float          | 55.8 ms                                                | 50.8 ms: 1.10x faster                                  |
| pidigits       | 282 ms                                                 | 280 ms: 1.00x faster                                   |
| Geometric mean | (ref)                                                  | 1.07x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.43 ms: 1.09x faster                                  |
| regex_compile  | 77.9 ms                                                | 72.8 ms: 1.07x faster                                  |
| regex_v8       | 16.0 ms                                                | 15.1 ms: 1.05x faster                                  |
| regex_dna      | 154 ms                                                 | 148 ms: 1.04x faster                                   |
| Geometric mean | (ref)                                                  | 1.06x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 45.8 ms: 1.22x faster                                  |
| xml_etree_process    | 39.7 ms                                                | 33.6 ms: 1.18x faster                                  |
| unpickle_list        | 3.02 us                                                | 2.69 us: 1.12x faster                                  |
| json_loads           | 17.2 us                                                | 15.3 us: 1.12x faster                                  |
| unpickle             | 9.12 us                                                | 8.29 us: 1.10x faster                                  |
| tomli_loads          | 1.39 sec                                               | 1.27 sec: 1.09x faster                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 68.3 ms: 1.08x faster                                  |
| pickle_list          | 2.89 us                                                | 2.70 us: 1.07x faster                                  |
| xml_etree_parse      | 106 ms                                                 | 100 ms: 1.06x faster                                   |
| pickle_dict          | 18.1 us                                                | 17.1 us: 1.06x faster                                  |
| pickle_pure_python   | 200 us                                                 | 191 us: 1.04x faster                                   |
| pickle               | 7.23 us                                                | 6.98 us: 1.04x faster                                  |
| unpickle_pure_python | 151 us                                                 | 149 us: 1.01x faster                                   |
| json_dumps           | 6.22 ms                                                | 7.53 ms: 1.21x slower                                  |
| Geometric mean       | (ref)                                                  | 1.07x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 8.57 ms: 1.09x faster                                  |
| python_startup         | 11.4 ms                                                | 10.8 ms: 1.06x faster                                  |
| Geometric mean         | (ref)                                                  | 1.08x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 22.3 ms                                                | 20.1 ms: 1.11x faster                                  |
| mako            | 7.71 ms                                                | 7.93 ms: 1.03x slower                                  |
| Geometric mean  | (ref)                                                  | 1.04x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 192 ms: 1.58x faster                                   |
| sqlite_synth               | 1.57 us                                                | 1.26 us: 1.25x faster                                  |
| xml_etree_generate         | 55.8 ms                                                | 45.8 ms: 1.22x faster                                  |
| xml_etree_process          | 39.7 ms                                                | 33.6 ms: 1.18x faster                                  |
| spectral_norm              | 76.4 ms                                                | 65.7 ms: 1.16x faster                                  |
| telco                      | 3.68 ms                                                | 3.17 ms: 1.16x faster                                  |
| deepcopy_reduce            | 2.07 us                                                | 1.79 us: 1.15x faster                                  |
| logging_silent             | 76.4 ns                                                | 66.5 ns: 1.15x faster                                  |
| sqlglot_optimize           | 34.0 ms                                                | 29.6 ms: 1.15x faster                                  |
| sqlglot_normalize          | 186 ms                                                 | 162 ms: 1.15x faster                                   |
| scimark_fft                | 195 ms                                                 | 173 ms: 1.13x faster                                   |
| unpickle_list              | 3.02 us                                                | 2.69 us: 1.12x faster                                  |
| json_loads                 | 17.2 us                                                | 15.3 us: 1.12x faster                                  |
| json                       | 3.09 ms                                                | 2.75 ms: 1.12x faster                                  |
| scimark_lu                 | 76.0 ms                                                | 67.7 ms: 1.12x faster                                  |
| coroutines                 | 19.2 ms                                                | 17.2 ms: 1.12x faster                                  |
| nqueens                    | 62.4 ms                                                | 55.9 ms: 1.12x faster                                  |
| nbody                      | 68.8 ms                                                | 61.7 ms: 1.12x faster                                  |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 2.81 ms: 1.11x faster                                  |
| pyflate                    | 316 ms                                                 | 284 ms: 1.11x faster                                   |
| django_template            | 22.3 ms                                                | 20.1 ms: 1.11x faster                                  |
| scimark_sor                | 87.4 ms                                                | 79.2 ms: 1.10x faster                                  |
| unpickle                   | 9.12 us                                                | 8.29 us: 1.10x faster                                  |
| 2to3                       | 169 ms                                                 | 154 ms: 1.10x faster                                   |
| float                      | 55.8 ms                                                | 50.8 ms: 1.10x faster                                  |
| bench_mp_pool              | 44.9 ms                                                | 41.0 ms: 1.09x faster                                  |
| tomli_loads                | 1.39 sec                                               | 1.27 sec: 1.09x faster                                 |
| python_startup_no_site     | 9.37 ms                                                | 8.57 ms: 1.09x faster                                  |
| crypto_pyaes               | 51.9 ms                                                | 47.5 ms: 1.09x faster                                  |
| chameleon                  | 4.70 ms                                                | 4.30 ms: 1.09x faster                                  |
| deepcopy                   | 235 us                                                 | 215 us: 1.09x faster                                   |
| regex_effbot               | 2.64 ms                                                | 2.43 ms: 1.09x faster                                  |
| xml_etree_iterparse        | 74.0 ms                                                | 68.3 ms: 1.08x faster                                  |
| logging_format             | 3.98 us                                                | 3.67 us: 1.08x faster                                  |
| bench_thread_pool          | 504 us                                                 | 465 us: 1.08x faster                                   |
| logging_simple             | 3.69 us                                                | 3.41 us: 1.08x faster                                  |
| deepcopy_memo              | 27.7 us                                                | 25.7 us: 1.07x faster                                  |
| pickle_list                | 2.89 us                                                | 2.70 us: 1.07x faster                                  |
| regex_compile              | 77.9 ms                                                | 72.8 ms: 1.07x faster                                  |
| mdp                        | 1.58 sec                                               | 1.48 sec: 1.06x faster                                 |
| python_startup             | 11.4 ms                                                | 10.8 ms: 1.06x faster                                  |
| xml_etree_parse            | 106 ms                                                 | 100 ms: 1.06x faster                                   |
| pickle_dict                | 18.1 us                                                | 17.1 us: 1.06x faster                                  |
| aiohttp                    | 1.08 ms                                                | 1.02 ms: 1.05x faster                                  |
| regex_v8                   | 16.0 ms                                                | 15.1 ms: 1.05x faster                                  |
| sympy_expand               | 241 ms                                                 | 229 ms: 1.05x faster                                   |
| sqlalchemy_declarative     | 62.3 ms                                                | 59.3 ms: 1.05x faster                                  |
| docutils                   | 1.50 sec                                               | 1.43 sec: 1.05x faster                                 |
| gunicorn                   | 1.15 ms                                                | 1.10 ms: 1.05x faster                                  |
| pickle_pure_python         | 200 us                                                 | 191 us: 1.04x faster                                   |
| pathlib                    | 24.2 ms                                                | 23.2 ms: 1.04x faster                                  |
| dulwich_log                | 29.8 ms                                                | 28.6 ms: 1.04x faster                                  |
| regex_dna                  | 154 ms                                                 | 148 ms: 1.04x faster                                   |
| pprint_safe_repr           | 497 ms                                                 | 478 ms: 1.04x faster                                   |
| fannkuch                   | 248 ms                                                 | 240 ms: 1.04x faster                                   |
| pickle                     | 7.23 us                                                | 6.98 us: 1.04x faster                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 43.5 ms: 1.04x faster                                  |
| richards                   | 32.1 ms                                                | 31.1 ms: 1.03x faster                                  |
| pprint_pformat             | 1.01 sec                                               | 979 ms: 1.03x faster                                   |
| raytrace                   | 212 ms                                                 | 206 ms: 1.03x faster                                   |
| sympy_str                  | 148 ms                                                 | 144 ms: 1.03x faster                                   |
| pycparser                  | 677 ms                                                 | 659 ms: 1.03x faster                                   |
| generators                 | 31.1 ms                                                | 30.3 ms: 1.03x faster                                  |
| mypy2                      | 380 ms                                                 | 372 ms: 1.02x faster                                   |
| dask                       | 222 ms                                                 | 219 ms: 1.01x faster                                   |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 519 ms: 1.01x faster                                   |
| unpickle_pure_python       | 151 us                                                 | 149 us: 1.01x faster                                   |
| meteor_contest             | 71.7 ms                                                | 71.1 ms: 1.01x faster                                  |
| sympy_integrate            | 11.4 ms                                                | 11.3 ms: 1.01x faster                                  |
| comprehensions             | 14.5 us                                                | 14.4 us: 1.01x faster                                  |
| gc_traversal               | 2.40 ms                                                | 2.38 ms: 1.01x faster                                  |
| pidigits                   | 282 ms                                                 | 280 ms: 1.00x faster                                   |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                   |
| hexiom                     | 4.54 ms                                                | 4.58 ms: 1.01x slower                                  |
| create_gc_cycles           | 701 us                                                 | 711 us: 1.01x slower                                   |
| deltablue                  | 2.71 ms                                                | 2.75 ms: 1.02x slower                                  |
| mako                       | 7.71 ms                                                | 7.93 ms: 1.03x slower                                  |
| sqlglot_transpile          | 1.02 ms                                                | 1.05 ms: 1.03x slower                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 550 ms: 1.03x slower                                   |
| sympy_sum                  | 77.6 ms                                                | 80.2 ms: 1.03x slower                                  |
| richards_super             | 36.0 ms                                                | 37.3 ms: 1.03x slower                                  |
| go                         | 102 ms                                                 | 105 ms: 1.04x slower                                   |
| async_tree_io              | 668 ms                                                 | 697 ms: 1.04x slower                                   |
| sqlalchemy_imperative      | 6.68 ms                                                | 6.98 ms: 1.04x slower                                  |
| sqlglot_parse              | 848 us                                                 | 890 us: 1.05x slower                                   |
| async_tree_none            | 266 ms                                                 | 282 ms: 1.06x slower                                   |
| unpack_sequence            | 31.5 ns                                                | 33.6 ns: 1.07x slower                                  |
| async_tree_none_tg         | 258 ms                                                 | 276 ms: 1.07x slower                                   |
| async_tree_memoization     | 312 ms                                                 | 336 ms: 1.08x slower                                   |
| async_tree_io_tg           | 669 ms                                                 | 724 ms: 1.08x slower                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 352 ms: 1.09x slower                                   |
| chaos                      | 42.5 ms                                                | 47.4 ms: 1.11x slower                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.40 sec: 1.12x slower                                 |
| coverage                   | 38.9 ms                                                | 43.9 ms: 1.13x slower                                  |
| json_dumps                 | 6.22 ms                                                | 7.53 ms: 1.21x slower                                  |
| asyncio_tcp                | 449 ms                                                 | 643 ms: 1.43x slower                                   |
| typing_runtime_protocols   | 93.0 us                                                | 301 us: 3.24x slower                                   |
| Geometric mean             | (ref)                                                  | 1.03x faster                                           |

Benchmark hidden because not significant (1): tornado_http
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.98x