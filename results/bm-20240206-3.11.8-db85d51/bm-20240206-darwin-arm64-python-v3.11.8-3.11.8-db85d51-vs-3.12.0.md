
# Results vs. 3.12.0

- fork: python
- ref: v3.11.8
- machine: darwin-arm64
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 151 ms: 1.12x faster                                   |
| chameleon      | 4.70 ms                                                | 4.32 ms: 1.09x faster                                  |
| docutils       | 1.50 sec                                               | 1.42 sec: 1.06x faster                                 |
| Geometric mean | (ref)                                                  | 1.07x faster                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 520 ms: 1.01x faster                                   |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 543 ms: 1.02x slower                                   |
| async_tree_memoization     | 312 ms                                                 | 321 ms: 1.03x slower                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 332 ms: 1.03x slower                                   |
| async_tree_io_tg           | 669 ms                                                 | 692 ms: 1.03x slower                                   |
| async_tree_io              | 668 ms                                                 | 693 ms: 1.04x slower                                   |
| async_tree_none_tg         | 258 ms                                                 | 268 ms: 1.04x slower                                   |
| async_tree_none            | 266 ms                                                 | 280 ms: 1.06x slower                                   |
| Geometric mean             | (ref)                                                  | 1.03x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 55.8 ms                                                | 53.4 ms: 1.05x faster                                  |
| pidigits       | 282 ms                                                 | 280 ms: 1.00x faster                                   |
| nbody          | 68.8 ms                                                | 68.5 ms: 1.00x faster                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 77.9 ms                                                | 70.9 ms: 1.10x faster                                  |
| regex_dna      | 154 ms                                                 | 152 ms: 1.01x faster                                   |
| regex_effbot   | 2.64 ms                                                | 2.64 ms: 1.00x slower                                  |
| regex_v8       | 16.0 ms                                                | 16.3 ms: 1.02x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 45.1 ms: 1.24x faster                                  |
| xml_etree_process    | 39.7 ms                                                | 33.2 ms: 1.19x faster                                  |
| unpickle_list        | 3.02 us                                                | 2.64 us: 1.14x faster                                  |
| json_loads           | 17.2 us                                                | 15.3 us: 1.13x faster                                  |
| unpickle             | 9.12 us                                                | 8.21 us: 1.11x faster                                  |
| pickle_list          | 2.89 us                                                | 2.64 us: 1.09x faster                                  |
| xml_etree_iterparse  | 74.0 ms                                                | 68.0 ms: 1.09x faster                                  |
| tomli_loads          | 1.39 sec                                               | 1.29 sec: 1.08x faster                                 |
| xml_etree_parse      | 106 ms                                                 | 101 ms: 1.06x faster                                   |
| pickle_dict          | 18.1 us                                                | 17.3 us: 1.04x faster                                  |
| pickle               | 7.23 us                                                | 6.96 us: 1.04x faster                                  |
| unpickle_pure_python | 151 us                                                 | 145 us: 1.04x faster                                   |
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                   |
| json_dumps           | 6.22 ms                                                | 7.55 ms: 1.21x slower                                  |
| Geometric mean       | (ref)                                                  | 1.07x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 11.6 ms: 1.02x slower                                  |
| python_startup_no_site | 9.37 ms                                                | 9.53 ms: 1.02x slower                                  |
| Geometric mean         | (ref)                                                  | 1.02x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 22.3 ms                                                | 19.6 ms: 1.14x faster                                  |
| mako            | 7.71 ms                                                | 7.97 ms: 1.03x slower                                  |
| Geometric mean  | (ref)                                                  | 1.05x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 187 ms: 1.62x faster                                   |
| sqlite_synth               | 1.57 us                                                | 1.26 us: 1.25x faster                                  |
| xml_etree_generate         | 55.8 ms                                                | 45.1 ms: 1.24x faster                                  |
| xml_etree_process          | 39.7 ms                                                | 33.2 ms: 1.19x faster                                  |
| deepcopy_reduce            | 2.07 us                                                | 1.76 us: 1.18x faster                                  |
| telco                      | 3.68 ms                                                | 3.15 ms: 1.17x faster                                  |
| sqlglot_normalize          | 186 ms                                                 | 160 ms: 1.16x faster                                   |
| logging_silent             | 76.4 ns                                                | 66.0 ns: 1.16x faster                                  |
| sqlglot_optimize           | 34.0 ms                                                | 29.5 ms: 1.15x faster                                  |
| deepcopy                   | 235 us                                                 | 204 us: 1.15x faster                                   |
| unpickle_list              | 3.02 us                                                | 2.64 us: 1.14x faster                                  |
| coroutines                 | 19.2 ms                                                | 16.9 ms: 1.14x faster                                  |
| django_template            | 22.3 ms                                                | 19.6 ms: 1.14x faster                                  |
| nqueens                    | 62.4 ms                                                | 55.3 ms: 1.13x faster                                  |
| json                       | 3.09 ms                                                | 2.74 ms: 1.13x faster                                  |
| json_loads                 | 17.2 us                                                | 15.3 us: 1.13x faster                                  |
| scimark_lu                 | 76.0 ms                                                | 67.6 ms: 1.12x faster                                  |
| 2to3                       | 169 ms                                                 | 151 ms: 1.12x faster                                   |
| deepcopy_memo              | 27.7 us                                                | 24.9 us: 1.11x faster                                  |
| unpickle                   | 9.12 us                                                | 8.21 us: 1.11x faster                                  |
| regex_compile              | 77.9 ms                                                | 70.9 ms: 1.10x faster                                  |
| crypto_pyaes               | 51.9 ms                                                | 47.3 ms: 1.10x faster                                  |
| bench_thread_pool          | 504 us                                                 | 461 us: 1.09x faster                                   |
| pyflate                    | 316 ms                                                 | 289 ms: 1.09x faster                                   |
| pickle_list                | 2.89 us                                                | 2.64 us: 1.09x faster                                  |
| spectral_norm              | 76.4 ms                                                | 70.0 ms: 1.09x faster                                  |
| logging_simple             | 3.69 us                                                | 3.39 us: 1.09x faster                                  |
| xml_etree_iterparse        | 74.0 ms                                                | 68.0 ms: 1.09x faster                                  |
| bench_mp_pool              | 44.9 ms                                                | 41.2 ms: 1.09x faster                                  |
| chameleon                  | 4.70 ms                                                | 4.32 ms: 1.09x faster                                  |
| logging_format             | 3.98 us                                                | 3.67 us: 1.09x faster                                  |
| tomli_loads                | 1.39 sec                                               | 1.29 sec: 1.08x faster                                 |
| scimark_sor                | 87.4 ms                                                | 81.0 ms: 1.08x faster                                  |
| mdp                        | 1.58 sec                                               | 1.48 sec: 1.07x faster                                 |
| sympy_expand               | 241 ms                                                 | 227 ms: 1.06x faster                                   |
| docutils                   | 1.50 sec                                               | 1.42 sec: 1.06x faster                                 |
| generators                 | 31.1 ms                                                | 29.4 ms: 1.06x faster                                  |
| xml_etree_parse            | 106 ms                                                 | 101 ms: 1.06x faster                                   |
| sympy_str                  | 148 ms                                                 | 140 ms: 1.05x faster                                   |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 2.98 ms: 1.05x faster                                  |
| comprehensions             | 14.5 us                                                | 13.9 us: 1.05x faster                                  |
| scimark_fft                | 195 ms                                                 | 186 ms: 1.05x faster                                   |
| float                      | 55.8 ms                                                | 53.4 ms: 1.05x faster                                  |
| sqlalchemy_declarative     | 62.3 ms                                                | 59.6 ms: 1.05x faster                                  |
| pickle_dict                | 18.1 us                                                | 17.3 us: 1.04x faster                                  |
| dulwich_log                | 29.8 ms                                                | 28.6 ms: 1.04x faster                                  |
| raytrace                   | 212 ms                                                 | 203 ms: 1.04x faster                                   |
| pathlib                    | 24.2 ms                                                | 23.2 ms: 1.04x faster                                  |
| pprint_safe_repr           | 497 ms                                                 | 478 ms: 1.04x faster                                   |
| pickle                     | 7.23 us                                                | 6.96 us: 1.04x faster                                  |
| unpickle_pure_python       | 151 us                                                 | 145 us: 1.04x faster                                   |
| pprint_pformat             | 1.01 sec                                               | 976 ms: 1.04x faster                                   |
| deltablue                  | 2.71 ms                                                | 2.62 ms: 1.03x faster                                  |
| pycparser                  | 677 ms                                                 | 657 ms: 1.03x faster                                   |
| sympy_integrate            | 11.4 ms                                                | 11.1 ms: 1.03x faster                                  |
| richards                   | 32.1 ms                                                | 31.3 ms: 1.03x faster                                  |
| pickle_pure_python         | 200 us                                                 | 196 us: 1.02x faster                                   |
| dask                       | 222 ms                                                 | 218 ms: 1.02x faster                                   |
| regex_dna                  | 154 ms                                                 | 152 ms: 1.01x faster                                   |
| fannkuch                   | 248 ms                                                 | 246 ms: 1.01x faster                                   |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 520 ms: 1.01x faster                                   |
| meteor_contest             | 71.7 ms                                                | 71.1 ms: 1.01x faster                                  |
| gc_traversal               | 2.40 ms                                                | 2.39 ms: 1.01x faster                                  |
| asyncio_websockets         | 409 ms                                                 | 407 ms: 1.01x faster                                   |
| pidigits                   | 282 ms                                                 | 280 ms: 1.00x faster                                   |
| nbody                      | 68.8 ms                                                | 68.5 ms: 1.00x faster                                  |
| hexiom                     | 4.54 ms                                                | 4.53 ms: 1.00x faster                                  |
| regex_effbot               | 2.64 ms                                                | 2.64 ms: 1.00x slower                                  |
| sympy_sum                  | 77.6 ms                                                | 78.5 ms: 1.01x slower                                  |
| create_gc_cycles           | 701 us                                                 | 712 us: 1.01x slower                                   |
| python_startup             | 11.4 ms                                                | 11.6 ms: 1.02x slower                                  |
| go                         | 102 ms                                                 | 103 ms: 1.02x slower                                   |
| python_startup_no_site     | 9.37 ms                                                | 9.53 ms: 1.02x slower                                  |
| sqlglot_transpile          | 1.02 ms                                                | 1.04 ms: 1.02x slower                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 543 ms: 1.02x slower                                   |
| regex_v8                   | 16.0 ms                                                | 16.3 ms: 1.02x slower                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 46.2 ms: 1.03x slower                                  |
| async_tree_memoization     | 312 ms                                                 | 321 ms: 1.03x slower                                   |
| async_tree_memoization_tg  | 323 ms                                                 | 332 ms: 1.03x slower                                   |
| mako                       | 7.71 ms                                                | 7.97 ms: 1.03x slower                                  |
| async_tree_io_tg           | 669 ms                                                 | 692 ms: 1.03x slower                                   |
| async_tree_io              | 668 ms                                                 | 693 ms: 1.04x slower                                   |
| async_tree_none_tg         | 258 ms                                                 | 268 ms: 1.04x slower                                   |
| sqlglot_parse              | 848 us                                                 | 889 us: 1.05x slower                                   |
| richards_super             | 36.0 ms                                                | 37.8 ms: 1.05x slower                                  |
| sqlalchemy_imperative      | 6.68 ms                                                | 7.03 ms: 1.05x slower                                  |
| async_tree_none            | 266 ms                                                 | 280 ms: 1.06x slower                                   |
| unpack_sequence            | 31.5 ns                                                | 33.8 ns: 1.07x slower                                  |
| coverage                   | 38.9 ms                                                | 43.4 ms: 1.12x slower                                  |
| chaos                      | 42.5 ms                                                | 48.1 ms: 1.13x slower                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.43 sec: 1.15x slower                                 |
| json_dumps                 | 6.22 ms                                                | 7.55 ms: 1.21x slower                                  |
| asyncio_tcp                | 449 ms                                                 | 656 ms: 1.46x slower                                   |
| mypy2                      | 380 ms                                                 | 573 ms: 1.51x slower                                   |
| typing_runtime_protocols   | 93.0 us                                                | 303 us: 3.25x slower                                   |
| Geometric mean             | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (3): aiohttp, tornado_http, gunicorn
Ignored benchmarks (6) of results/bm-20240206-3.11.8-db85d51/bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.98x