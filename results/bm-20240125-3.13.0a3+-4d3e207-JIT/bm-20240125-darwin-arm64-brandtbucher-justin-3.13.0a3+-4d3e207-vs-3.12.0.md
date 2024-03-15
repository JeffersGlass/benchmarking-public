
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin
- machine: darwin-arm64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.02x slower
- HPT reliability: 99.26%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.15x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 174 ms: 1.02x slower                                           |
| chameleon      | 4.70 ms                                                | 4.91 ms: 1.05x slower                                          |
| docutils       | 1.50 sec                                               | 1.48 sec: 1.02x faster                                         |
| Geometric mean | (ref)                                                  | 1.02x slower                                                   |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none        | 266 ms                                                 | 253 ms: 1.05x faster                                           |
| async_tree_io_tg       | 669 ms                                                 | 664 ms: 1.01x faster                                           |
| async_tree_none_tg     | 258 ms                                                 | 260 ms: 1.01x slower                                           |
| async_tree_io          | 668 ms                                                 | 698 ms: 1.05x slower                                           |
| async_tree_memoization | 312 ms                                                 | 328 ms: 1.05x slower                                           |
| Geometric mean         | (ref)                                                  | 1.00x slower                                                   |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pidigits       | 282 ms                                                 | 283 ms: 1.00x slower                                           |
| float          | 55.8 ms                                                | 56.2 ms: 1.01x slower                                          |
| nbody          | 68.8 ms                                                | 77.1 ms: 1.12x slower                                          |
| Geometric mean | (ref)                                                  | 1.04x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_compile  | 77.9 ms                                                | 76.5 ms: 1.02x faster                                          |
| regex_dna      | 154 ms                                                 | 156 ms: 1.01x slower                                           |
| regex_effbot   | 2.64 ms                                                | 2.75 ms: 1.04x slower                                          |
| regex_v8       | 16.0 ms                                                | 17.9 ms: 1.12x slower                                          |
| Geometric mean | (ref)                                                  | 1.04x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| pickle_pure_python   | 200 us                                                 | 197 us: 1.01x faster                                           |
| xml_etree_process    | 39.7 ms                                                | 39.1 ms: 1.01x faster                                          |
| json_loads           | 17.2 us                                                | 17.2 us: 1.00x faster                                          |
| unpickle             | 9.12 us                                                | 9.15 us: 1.00x slower                                          |
| pickle               | 7.23 us                                                | 7.26 us: 1.00x slower                                          |
| tomli_loads          | 1.39 sec                                               | 1.41 sec: 1.01x slower                                         |
| xml_etree_generate   | 55.8 ms                                                | 56.7 ms: 1.01x slower                                          |
| unpickle_list        | 3.02 us                                                | 3.07 us: 1.02x slower                                          |
| xml_etree_iterparse  | 74.0 ms                                                | 76.2 ms: 1.03x slower                                          |
| pickle_list          | 2.89 us                                                | 2.98 us: 1.03x slower                                          |
| unpickle_pure_python | 151 us                                                 | 158 us: 1.05x slower                                           |
| json_dumps           | 6.22 ms                                                | 6.54 ms: 1.05x slower                                          |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (2): xml_etree_parse, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 12.9 ms: 1.13x slower                                          |
| python_startup_no_site | 9.37 ms                                                | 11.3 ms: 1.20x slower                                          |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 7.71 ms                                                | 7.94 ms: 1.03x slower                                          |

All benchmarks:
===============

| Benchmark                | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------:|
| typing_runtime_protocols | 93.0 us                                                | 71.9 us: 1.29x faster                                          |
| raytrace                 | 212 ms                                                 | 179 ms: 1.18x faster                                           |
| comprehensions           | 14.5 us                                                | 12.9 us: 1.13x faster                                          |
| generators               | 31.1 ms                                                | 28.0 ms: 1.11x faster                                          |
| logging_silent           | 76.4 ns                                                | 69.6 ns: 1.10x faster                                          |
| deltablue                | 2.71 ms                                                | 2.51 ms: 1.08x faster                                          |
| deepcopy_memo            | 27.7 us                                                | 25.9 us: 1.07x faster                                          |
| unpack_sequence          | 31.5 ns                                                | 29.5 ns: 1.07x faster                                          |
| logging_simple           | 3.69 us                                                | 3.47 us: 1.06x faster                                          |
| sqlglot_parse            | 848 us                                                 | 800 us: 1.06x faster                                           |
| logging_format           | 3.98 us                                                | 3.76 us: 1.06x faster                                          |
| json                     | 3.09 ms                                                | 2.93 ms: 1.05x faster                                          |
| async_tree_none          | 266 ms                                                 | 253 ms: 1.05x faster                                           |
| sqlglot_transpile        | 1.02 ms                                                | 980 us: 1.04x faster                                           |
| deepcopy                 | 235 us                                                 | 225 us: 1.04x faster                                           |
| deepcopy_reduce          | 2.07 us                                                | 1.99 us: 1.04x faster                                          |
| sympy_str                | 148 ms                                                 | 143 ms: 1.04x faster                                           |
| crypto_pyaes             | 51.9 ms                                                | 50.4 ms: 1.03x faster                                          |
| coroutines               | 19.2 ms                                                | 18.9 ms: 1.02x faster                                          |
| regex_compile            | 77.9 ms                                                | 76.5 ms: 1.02x faster                                          |
| docutils                 | 1.50 sec                                               | 1.48 sec: 1.02x faster                                         |
| pickle_pure_python       | 200 us                                                 | 197 us: 1.01x faster                                           |
| xml_etree_process        | 39.7 ms                                                | 39.1 ms: 1.01x faster                                          |
| scimark_lu               | 76.0 ms                                                | 74.9 ms: 1.01x faster                                          |
| chaos                    | 42.5 ms                                                | 42.1 ms: 1.01x faster                                          |
| richards                 | 32.1 ms                                                | 31.8 ms: 1.01x faster                                          |
| richards_super           | 36.0 ms                                                | 35.7 ms: 1.01x faster                                          |
| sympy_sum                | 77.6 ms                                                | 76.9 ms: 1.01x faster                                          |
| async_tree_io_tg         | 669 ms                                                 | 664 ms: 1.01x faster                                           |
| sympy_integrate          | 11.4 ms                                                | 11.3 ms: 1.01x faster                                          |
| json_loads               | 17.2 us                                                | 17.2 us: 1.00x faster                                          |
| async_generators         | 304 ms                                                 | 303 ms: 1.00x faster                                           |
| sqlglot_normalize        | 186 ms                                                 | 186 ms: 1.00x faster                                           |
| gc_traversal             | 2.40 ms                                                | 2.40 ms: 1.00x slower                                          |
| unpickle                 | 9.12 us                                                | 9.15 us: 1.00x slower                                          |
| pidigits                 | 282 ms                                                 | 283 ms: 1.00x slower                                           |
| pickle                   | 7.23 us                                                | 7.26 us: 1.00x slower                                          |
| sympy_expand             | 241 ms                                                 | 242 ms: 1.00x slower                                           |
| create_gc_cycles         | 701 us                                                 | 705 us: 1.01x slower                                           |
| nqueens                  | 62.4 ms                                                | 62.8 ms: 1.01x slower                                          |
| float                    | 55.8 ms                                                | 56.2 ms: 1.01x slower                                          |
| dulwich_log              | 29.8 ms                                                | 30.1 ms: 1.01x slower                                          |
| async_tree_none_tg       | 258 ms                                                 | 260 ms: 1.01x slower                                           |
| regex_dna                | 154 ms                                                 | 156 ms: 1.01x slower                                           |
| tomli_loads              | 1.39 sec                                               | 1.41 sec: 1.01x slower                                         |
| bench_thread_pool        | 504 us                                                 | 509 us: 1.01x slower                                           |
| xml_etree_generate       | 55.8 ms                                                | 56.7 ms: 1.01x slower                                          |
| unpickle_list            | 3.02 us                                                | 3.07 us: 1.02x slower                                          |
| asyncio_tcp_ssl          | 1.24 sec                                               | 1.27 sec: 1.02x slower                                         |
| dask                     | 222 ms                                                 | 226 ms: 1.02x slower                                           |
| sqlite_synth             | 1.57 us                                                | 1.60 us: 1.02x slower                                          |
| 2to3                     | 169 ms                                                 | 174 ms: 1.02x slower                                           |
| mdp                      | 1.58 sec                                               | 1.62 sec: 1.03x slower                                         |
| bench_mp_pool            | 44.9 ms                                                | 46.1 ms: 1.03x slower                                          |
| sqlglot_optimize         | 34.0 ms                                                | 35.0 ms: 1.03x slower                                          |
| mako                     | 7.71 ms                                                | 7.94 ms: 1.03x slower                                          |
| xml_etree_iterparse      | 74.0 ms                                                | 76.2 ms: 1.03x slower                                          |
| pycparser                | 677 ms                                                 | 699 ms: 1.03x slower                                           |
| pickle_list              | 2.89 us                                                | 2.98 us: 1.03x slower                                          |
| meteor_contest           | 71.7 ms                                                | 74.3 ms: 1.04x slower                                          |
| regex_effbot             | 2.64 ms                                                | 2.75 ms: 1.04x slower                                          |
| pyflate                  | 316 ms                                                 | 329 ms: 1.04x slower                                           |
| async_tree_io            | 668 ms                                                 | 698 ms: 1.05x slower                                           |
| chameleon                | 4.70 ms                                                | 4.91 ms: 1.05x slower                                          |
| unpickle_pure_python     | 151 us                                                 | 158 us: 1.05x slower                                           |
| async_tree_memoization   | 312 ms                                                 | 328 ms: 1.05x slower                                           |
| json_dumps               | 6.22 ms                                                | 6.54 ms: 1.05x slower                                          |
| pprint_safe_repr         | 497 ms                                                 | 526 ms: 1.06x slower                                           |
| pprint_pformat           | 1.01 sec                                               | 1.08 sec: 1.07x slower                                         |
| spectral_norm            | 76.4 ms                                                | 82.0 ms: 1.07x slower                                          |
| scimark_sparse_mat_mult  | 3.14 ms                                                | 3.38 ms: 1.08x slower                                          |
| go                       | 102 ms                                                 | 110 ms: 1.09x slower                                           |
| scimark_monte_carlo      | 45.0 ms                                                | 49.1 ms: 1.09x slower                                          |
| fannkuch                 | 248 ms                                                 | 278 ms: 1.12x slower                                           |
| nbody                    | 68.8 ms                                                | 77.1 ms: 1.12x slower                                          |
| regex_v8                 | 16.0 ms                                                | 17.9 ms: 1.12x slower                                          |
| hexiom                   | 4.54 ms                                                | 5.10 ms: 1.12x slower                                          |
| scimark_fft              | 195 ms                                                 | 220 ms: 1.13x slower                                           |
| python_startup           | 11.4 ms                                                | 12.9 ms: 1.13x slower                                          |
| python_startup_no_site   | 9.37 ms                                                | 11.3 ms: 1.20x slower                                          |
| scimark_sor              | 87.4 ms                                                | 106 ms: 1.21x slower                                           |
| coverage                 | 38.9 ms                                                | 47.1 ms: 1.21x slower                                          |
| telco                    | 3.68 ms                                                | 4.63 ms: 1.26x slower                                          |
| mypy2                    | 380 ms                                                 | 526 ms: 1.38x slower                                           |
| Geometric mean           | (ref)                                                  | 1.02x slower                                                   |

Benchmark hidden because not significant (9): asyncio_tcp, async_tree_cpu_io_mixed, pathlib, async_tree_cpu_io_mixed_tg, xml_etree_parse, asyncio_websockets, pickle_dict, async_tree_memoization_tg, tornado_http
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.26% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.15x