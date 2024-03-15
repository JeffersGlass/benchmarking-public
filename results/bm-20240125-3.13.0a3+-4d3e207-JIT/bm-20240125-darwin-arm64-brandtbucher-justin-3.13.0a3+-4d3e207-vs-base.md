# Results vs. base

- fork: brandtbucher
- ref: justin
- machine: darwin-arm64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.02x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 1.15x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 168 ms                                                                 | 174 ms: 1.04x slower                                           |
| chameleon      | 4.84 ms                                                                | 4.91 ms: 1.02x slower                                          |
| docutils       | 1.45 sec                                                               | 1.48 sec: 1.02x slower                                         |
| tornado_http   | 66.0 ms                                                                | 70.7 ms: 1.07x slower                                          |
| Geometric mean | (ref)                                                                  | 1.04x slower                                                   |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_io_tg           | 660 ms                                                                 | 664 ms: 1.01x slower                                           |
| async_tree_io              | 693 ms                                                                 | 698 ms: 1.01x slower                                           |
| async_tree_cpu_io_mixed_tg | 526 ms                                                                 | 530 ms: 1.01x slower                                           |
| async_tree_cpu_io_mixed    | 516 ms                                                                 | 521 ms: 1.01x slower                                           |
| async_tree_none_tg         | 257 ms                                                                 | 260 ms: 1.01x slower                                           |
| Geometric mean             | (ref)                                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (3): async_tree_memoization_tg, async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| float          | 56.5 ms                                                                | 56.2 ms: 1.01x faster                                          |
| pidigits       | 282 ms                                                                 | 283 ms: 1.00x slower                                           |
| nbody          | 75.7 ms                                                                | 77.1 ms: 1.02x slower                                          |
| Geometric mean | (ref)                                                                  | 1.00x slower                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 155 ms                                                                 | 156 ms: 1.00x slower                                           |
| regex_effbot   | 2.74 ms                                                                | 2.75 ms: 1.00x slower                                          |
| regex_v8       | 17.8 ms                                                                | 17.9 ms: 1.01x slower                                          |
| regex_compile  | 72.7 ms                                                                | 76.5 ms: 1.05x slower                                          |
| Geometric mean | (ref)                                                                  | 1.02x slower                                                   |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| tomli_loads          | 1.54 sec                                                               | 1.41 sec: 1.09x faster                                         |
| pickle               | 7.32 us                                                                | 7.26 us: 1.01x faster                                          |
| pickle_dict          | 18.2 us                                                                | 18.1 us: 1.01x faster                                          |
| xml_etree_process    | 39.4 ms                                                                | 39.1 ms: 1.01x faster                                          |
| unpickle             | 9.19 us                                                                | 9.15 us: 1.00x faster                                          |
| xml_etree_iterparse  | 75.9 ms                                                                | 76.2 ms: 1.00x slower                                          |
| pickle_pure_python   | 196 us                                                                 | 197 us: 1.00x slower                                           |
| json_loads           | 17.0 us                                                                | 17.2 us: 1.01x slower                                          |
| unpickle_list        | 3.03 us                                                                | 3.07 us: 1.01x slower                                          |
| pickle_list          | 2.94 us                                                                | 2.98 us: 1.01x slower                                          |
| xml_etree_generate   | 55.8 ms                                                                | 56.7 ms: 1.02x slower                                          |
| unpickle_pure_python | 153 us                                                                 | 158 us: 1.03x slower                                           |
| Geometric mean       | (ref)                                                                  | 1.00x faster                                                   |

Benchmark hidden because not significant (2): json_dumps, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup_no_site | 11.2 ms                                                                | 11.3 ms: 1.01x slower                                          |
| python_startup         | 12.6 ms                                                                | 12.9 ms: 1.03x slower                                          |
| Geometric mean         | (ref)                                                                  | 1.02x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 7.64 ms                                                                | 7.94 ms: 1.04x slower                                          |

All benchmarks:
===============

| Benchmark                  | bm-20240126-darwin-arm64-python-841eacd07646e643f87d-3.13.0a3+-841eacd | bm-20240125-darwin-arm64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| tomli_loads                | 1.54 sec                                                               | 1.41 sec: 1.09x faster                                         |
| richards                   | 33.6 ms                                                                | 31.8 ms: 1.06x faster                                          |
| coroutines                 | 19.8 ms                                                                | 18.9 ms: 1.05x faster                                          |
| richards_super             | 37.1 ms                                                                | 35.7 ms: 1.04x faster                                          |
| pyflate                    | 338 ms                                                                 | 329 ms: 1.03x faster                                           |
| generators                 | 28.6 ms                                                                | 28.0 ms: 1.02x faster                                          |
| coverage                   | 48.0 ms                                                                | 47.1 ms: 1.02x faster                                          |
| logging_silent             | 70.4 ns                                                                | 69.6 ns: 1.01x faster                                          |
| pickle                     | 7.32 us                                                                | 7.26 us: 1.01x faster                                          |
| pickle_dict                | 18.2 us                                                                | 18.1 us: 1.01x faster                                          |
| xml_etree_process          | 39.4 ms                                                                | 39.1 ms: 1.01x faster                                          |
| create_gc_cycles           | 711 us                                                                 | 705 us: 1.01x faster                                           |
| json                       | 2.96 ms                                                                | 2.93 ms: 1.01x faster                                          |
| float                      | 56.5 ms                                                                | 56.2 ms: 1.01x faster                                          |
| unpickle                   | 9.19 us                                                                | 9.15 us: 1.00x faster                                          |
| regex_dna                  | 155 ms                                                                 | 156 ms: 1.00x slower                                           |
| pidigits                   | 282 ms                                                                 | 283 ms: 1.00x slower                                           |
| asyncio_websockets         | 408 ms                                                                 | 409 ms: 1.00x slower                                           |
| deepcopy_memo              | 25.8 us                                                                | 25.9 us: 1.00x slower                                          |
| regex_effbot               | 2.74 ms                                                                | 2.75 ms: 1.00x slower                                          |
| xml_etree_iterparse        | 75.9 ms                                                                | 76.2 ms: 1.00x slower                                          |
| pickle_pure_python         | 196 us                                                                 | 197 us: 1.00x slower                                           |
| typing_runtime_protocols   | 71.5 us                                                                | 71.9 us: 1.01x slower                                          |
| logging_format             | 3.74 us                                                                | 3.76 us: 1.01x slower                                          |
| async_tree_io_tg           | 660 ms                                                                 | 664 ms: 1.01x slower                                           |
| regex_v8                   | 17.8 ms                                                                | 17.9 ms: 1.01x slower                                          |
| deepcopy                   | 224 us                                                                 | 225 us: 1.01x slower                                           |
| async_tree_io              | 693 ms                                                                 | 698 ms: 1.01x slower                                           |
| python_startup_no_site     | 11.2 ms                                                                | 11.3 ms: 1.01x slower                                          |
| async_tree_cpu_io_mixed_tg | 526 ms                                                                 | 530 ms: 1.01x slower                                           |
| async_tree_cpu_io_mixed    | 516 ms                                                                 | 521 ms: 1.01x slower                                           |
| sqlite_synth               | 1.59 us                                                                | 1.60 us: 1.01x slower                                          |
| telco                      | 4.58 ms                                                                | 4.63 ms: 1.01x slower                                          |
| json_loads                 | 17.0 us                                                                | 17.2 us: 1.01x slower                                          |
| async_tree_none_tg         | 257 ms                                                                 | 260 ms: 1.01x slower                                           |
| unpickle_list              | 3.03 us                                                                | 3.07 us: 1.01x slower                                          |
| scimark_lu                 | 73.9 ms                                                                | 74.9 ms: 1.01x slower                                          |
| pycparser                  | 690 ms                                                                 | 699 ms: 1.01x slower                                           |
| scimark_sor                | 104 ms                                                                 | 106 ms: 1.01x slower                                           |
| deepcopy_reduce            | 1.96 us                                                                | 1.99 us: 1.01x slower                                          |
| pickle_list                | 2.94 us                                                                | 2.98 us: 1.01x slower                                          |
| xml_etree_generate         | 55.8 ms                                                                | 56.7 ms: 1.02x slower                                          |
| chameleon                  | 4.84 ms                                                                | 4.91 ms: 1.02x slower                                          |
| sympy_expand               | 238 ms                                                                 | 242 ms: 1.02x slower                                           |
| sqlglot_transpile          | 963 us                                                                 | 980 us: 1.02x slower                                           |
| sqlglot_parse              | 786 us                                                                 | 800 us: 1.02x slower                                           |
| nbody                      | 75.7 ms                                                                | 77.1 ms: 1.02x slower                                          |
| dulwich_log                | 29.5 ms                                                                | 30.1 ms: 1.02x slower                                          |
| docutils                   | 1.45 sec                                                               | 1.48 sec: 1.02x slower                                         |
| meteor_contest             | 72.9 ms                                                                | 74.3 ms: 1.02x slower                                          |
| pprint_safe_repr           | 515 ms                                                                 | 526 ms: 1.02x slower                                           |
| sqlglot_normalize          | 181 ms                                                                 | 186 ms: 1.02x slower                                           |
| async_generators           | 296 ms                                                                 | 303 ms: 1.02x slower                                           |
| fannkuch                   | 271 ms                                                                 | 278 ms: 1.02x slower                                           |
| sympy_str                  | 139 ms                                                                 | 143 ms: 1.03x slower                                           |
| unpickle_pure_python       | 153 us                                                                 | 158 us: 1.03x slower                                           |
| python_startup             | 12.6 ms                                                                | 12.9 ms: 1.03x slower                                          |
| dask                       | 220 ms                                                                 | 226 ms: 1.03x slower                                           |
| pprint_pformat             | 1.05 sec                                                               | 1.08 sec: 1.03x slower                                         |
| nqueens                    | 60.8 ms                                                                | 62.8 ms: 1.03x slower                                          |
| 2to3                       | 168 ms                                                                 | 174 ms: 1.04x slower                                           |
| sqlglot_optimize           | 33.7 ms                                                                | 35.0 ms: 1.04x slower                                          |
| deltablue                  | 2.42 ms                                                                | 2.51 ms: 1.04x slower                                          |
| mdp                        | 1.56 sec                                                               | 1.62 sec: 1.04x slower                                         |
| mako                       | 7.64 ms                                                                | 7.94 ms: 1.04x slower                                          |
| scimark_monte_carlo        | 47.2 ms                                                                | 49.1 ms: 1.04x slower                                          |
| crypto_pyaes               | 48.4 ms                                                                | 50.4 ms: 1.04x slower                                          |
| chaos                      | 40.3 ms                                                                | 42.1 ms: 1.04x slower                                          |
| go                         | 105 ms                                                                 | 110 ms: 1.05x slower                                           |
| raytrace                   | 170 ms                                                                 | 179 ms: 1.05x slower                                           |
| regex_compile              | 72.7 ms                                                                | 76.5 ms: 1.05x slower                                          |
| sympy_integrate            | 10.7 ms                                                                | 11.3 ms: 1.05x slower                                          |
| bench_mp_pool              | 43.7 ms                                                                | 46.1 ms: 1.05x slower                                          |
| sympy_sum                  | 72.7 ms                                                                | 76.9 ms: 1.06x slower                                          |
| bench_thread_pool          | 481 us                                                                 | 509 us: 1.06x slower                                           |
| unpack_sequence            | 27.8 ns                                                                | 29.5 ns: 1.06x slower                                          |
| tornado_http               | 66.0 ms                                                                | 70.7 ms: 1.07x slower                                          |
| scimark_fft                | 204 ms                                                                 | 220 ms: 1.08x slower                                           |
| comprehensions             | 12.0 us                                                                | 12.9 us: 1.08x slower                                          |
| scimark_sparse_mat_mult    | 3.11 ms                                                                | 3.38 ms: 1.08x slower                                          |
| spectral_norm              | 75.1 ms                                                                | 82.0 ms: 1.09x slower                                          |
| hexiom                     | 4.52 ms                                                                | 5.10 ms: 1.13x slower                                          |
| Geometric mean             | (ref)                                                                  | 1.02x slower                                                   |

Benchmark hidden because not significant (11): pathlib, asyncio_tcp_ssl, logging_simple, json_dumps, xml_etree_parse, gc_traversal, async_tree_memoization_tg, async_tree_memoization, async_tree_none, asyncio_tcp, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 1.15x