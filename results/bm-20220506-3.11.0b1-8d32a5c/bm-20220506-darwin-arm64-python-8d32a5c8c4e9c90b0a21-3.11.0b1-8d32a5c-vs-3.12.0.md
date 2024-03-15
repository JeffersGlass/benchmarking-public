
# Results vs. 3.12.0

- fork: python
- ref: 8d32a5c8c4e9c90b0a21
- machine: darwin-arm64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.00x faster \*
- HPT reliability: 99.68%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 152 ms: 1.11x faster                                                  |
| chameleon      | 4.70 ms                                                | 4.32 ms: 1.09x faster                                                 |
| docutils       | 1.50 sec                                               | 1.39 sec: 1.08x faster                                                |
| Geometric mean | (ref)                                                  | 1.07x faster                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 526 ms                                                 | 514 ms: 1.02x faster                                                  |
| async_tree_io              | 668 ms                                                 | 690 ms: 1.03x slower                                                  |
| async_tree_none            | 266 ms                                                 | 277 ms: 1.04x slower                                                  |
| async_tree_io_tg           | 669 ms                                                 | 737 ms: 1.10x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 353 ms: 1.13x slower                                                  |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 607 ms: 1.14x slower                                                  |
| async_tree_none_tg         | 258 ms                                                 | 332 ms: 1.29x slower                                                  |
| async_tree_memoization_tg  | 323 ms                                                 | 434 ms: 1.34x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.13x slower                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 68.8 ms                                                | 65.6 ms: 1.05x faster                                                 |
| float          | 55.8 ms                                                | 53.3 ms: 1.05x faster                                                 |
| pidigits       | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.64 ms                                                | 2.26 ms: 1.17x faster                                                 |
| regex_dna      | 154 ms                                                 | 144 ms: 1.07x faster                                                  |
| regex_compile  | 77.9 ms                                                | 73.1 ms: 1.06x faster                                                 |
| regex_v8       | 16.0 ms                                                | 15.8 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.08x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| xml_etree_generate   | 55.8 ms                                                | 46.9 ms: 1.19x faster                                                 |
| xml_etree_process    | 39.7 ms                                                | 34.2 ms: 1.16x faster                                                 |
| pickle_list          | 2.89 us                                                | 2.55 us: 1.13x faster                                                 |
| pickle_dict          | 18.1 us                                                | 16.2 us: 1.11x faster                                                 |
| json_loads           | 17.2 us                                                | 15.5 us: 1.11x faster                                                 |
| xml_etree_iterparse  | 74.0 ms                                                | 67.2 ms: 1.10x faster                                                 |
| unpickle             | 9.12 us                                                | 8.32 us: 1.10x faster                                                 |
| xml_etree_parse      | 106 ms                                                 | 97.3 ms: 1.09x faster                                                 |
| unpickle_list        | 3.02 us                                                | 2.77 us: 1.09x faster                                                 |
| tomli_loads          | 1.39 sec                                               | 1.31 sec: 1.06x faster                                                |
| pickle               | 7.23 us                                                | 6.98 us: 1.04x faster                                                 |
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                                  |
| unpickle_pure_python | 151 us                                                 | 152 us: 1.01x slower                                                  |
| json_dumps           | 6.22 ms                                                | 7.57 ms: 1.22x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.07x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup_no_site | 9.37 ms                                                | 9.27 ms: 1.01x faster                                                 |
| Geometric mean         | (ref)                                                  | 1.01x faster                                                          |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 22.3 ms                                                | 19.6 ms: 1.14x faster                                                 |
| mako            | 7.71 ms                                                | 8.18 ms: 1.06x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.04x faster                                                          |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_generators           | 304 ms                                                 | 190 ms: 1.60x faster                                                  |
| xml_etree_generate         | 55.8 ms                                                | 46.9 ms: 1.19x faster                                                 |
| sqlite_synth               | 1.57 us                                                | 1.33 us: 1.18x faster                                                 |
| regex_effbot               | 2.64 ms                                                | 2.26 ms: 1.17x faster                                                 |
| logging_silent             | 76.4 ns                                                | 65.8 ns: 1.16x faster                                                 |
| xml_etree_process          | 39.7 ms                                                | 34.2 ms: 1.16x faster                                                 |
| telco                      | 3.68 ms                                                | 3.18 ms: 1.16x faster                                                 |
| nqueens                    | 62.4 ms                                                | 54.5 ms: 1.15x faster                                                 |
| coroutines                 | 19.2 ms                                                | 16.9 ms: 1.14x faster                                                 |
| django_template            | 22.3 ms                                                | 19.6 ms: 1.14x faster                                                 |
| pickle_list                | 2.89 us                                                | 2.55 us: 1.13x faster                                                 |
| sqlglot_normalize          | 186 ms                                                 | 164 ms: 1.13x faster                                                  |
| spectral_norm              | 76.4 ms                                                | 68.2 ms: 1.12x faster                                                 |
| scimark_sor                | 87.4 ms                                                | 78.2 ms: 1.12x faster                                                 |
| sqlglot_optimize           | 34.0 ms                                                | 30.5 ms: 1.12x faster                                                 |
| json                       | 3.09 ms                                                | 2.77 ms: 1.12x faster                                                 |
| pickle_dict                | 18.1 us                                                | 16.2 us: 1.11x faster                                                 |
| json_loads                 | 17.2 us                                                | 15.5 us: 1.11x faster                                                 |
| 2to3                       | 169 ms                                                 | 152 ms: 1.11x faster                                                  |
| scimark_lu                 | 76.0 ms                                                | 68.4 ms: 1.11x faster                                                 |
| pyflate                    | 316 ms                                                 | 286 ms: 1.10x faster                                                  |
| xml_etree_iterparse        | 74.0 ms                                                | 67.2 ms: 1.10x faster                                                 |
| unpickle                   | 9.12 us                                                | 8.32 us: 1.10x faster                                                 |
| xml_etree_parse            | 106 ms                                                 | 97.3 ms: 1.09x faster                                                 |
| unpickle_list              | 3.02 us                                                | 2.77 us: 1.09x faster                                                 |
| chameleon                  | 4.70 ms                                                | 4.32 ms: 1.09x faster                                                 |
| crypto_pyaes               | 51.9 ms                                                | 47.8 ms: 1.09x faster                                                 |
| logging_format             | 3.98 us                                                | 3.68 us: 1.08x faster                                                 |
| logging_simple             | 3.69 us                                                | 3.41 us: 1.08x faster                                                 |
| docutils                   | 1.50 sec                                               | 1.39 sec: 1.08x faster                                                |
| bench_mp_pool              | 44.9 ms                                                | 41.7 ms: 1.08x faster                                                 |
| scimark_fft                | 195 ms                                                 | 182 ms: 1.07x faster                                                  |
| regex_dna                  | 154 ms                                                 | 144 ms: 1.07x faster                                                  |
| deepcopy_reduce            | 2.07 us                                                | 1.93 us: 1.07x faster                                                 |
| regex_compile              | 77.9 ms                                                | 73.1 ms: 1.06x faster                                                 |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 2.95 ms: 1.06x faster                                                 |
| tomli_loads                | 1.39 sec                                               | 1.31 sec: 1.06x faster                                                |
| bench_thread_pool          | 504 us                                                 | 480 us: 1.05x faster                                                  |
| nbody                      | 68.8 ms                                                | 65.6 ms: 1.05x faster                                                 |
| pathlib                    | 24.2 ms                                                | 23.1 ms: 1.05x faster                                                 |
| float                      | 55.8 ms                                                | 53.3 ms: 1.05x faster                                                 |
| sqlalchemy_declarative     | 62.3 ms                                                | 59.7 ms: 1.04x faster                                                 |
| raytrace                   | 212 ms                                                 | 203 ms: 1.04x faster                                                  |
| sympy_expand               | 241 ms                                                 | 232 ms: 1.04x faster                                                  |
| generators                 | 31.1 ms                                                | 29.9 ms: 1.04x faster                                                 |
| pickle                     | 7.23 us                                                | 6.98 us: 1.04x faster                                                 |
| richards                   | 32.1 ms                                                | 31.1 ms: 1.03x faster                                                 |
| sympy_str                  | 148 ms                                                 | 143 ms: 1.03x faster                                                  |
| dulwich_log                | 29.8 ms                                                | 28.9 ms: 1.03x faster                                                 |
| pprint_safe_repr           | 497 ms                                                 | 482 ms: 1.03x faster                                                  |
| deepcopy                   | 235 us                                                 | 228 us: 1.03x faster                                                  |
| pycparser                  | 677 ms                                                 | 659 ms: 1.03x faster                                                  |
| pprint_pformat             | 1.01 sec                                               | 985 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 514 ms: 1.02x faster                                                  |
| scimark_monte_carlo        | 45.0 ms                                                | 44.1 ms: 1.02x faster                                                 |
| sympy_integrate            | 11.4 ms                                                | 11.1 ms: 1.02x faster                                                 |
| pickle_pure_python         | 200 us                                                 | 196 us: 1.02x faster                                                  |
| python_startup_no_site     | 9.37 ms                                                | 9.27 ms: 1.01x faster                                                 |
| regex_v8                   | 16.0 ms                                                | 15.8 ms: 1.01x faster                                                 |
| gc_traversal               | 2.40 ms                                                | 2.38 ms: 1.01x faster                                                 |
| fannkuch                   | 248 ms                                                 | 247 ms: 1.01x faster                                                  |
| asyncio_websockets         | 409 ms                                                 | 407 ms: 1.01x faster                                                  |
| pidigits                   | 282 ms                                                 | 281 ms: 1.00x faster                                                  |
| deepcopy_memo              | 27.7 us                                                | 27.8 us: 1.00x slower                                                 |
| sympy_sum                  | 77.6 ms                                                | 78.1 ms: 1.01x slower                                                 |
| hexiom                     | 4.54 ms                                                | 4.59 ms: 1.01x slower                                                 |
| unpickle_pure_python       | 151 us                                                 | 152 us: 1.01x slower                                                  |
| meteor_contest             | 71.7 ms                                                | 72.5 ms: 1.01x slower                                                 |
| create_gc_cycles           | 701 us                                                 | 715 us: 1.02x slower                                                  |
| go                         | 102 ms                                                 | 104 ms: 1.02x slower                                                  |
| aiohttp                    | 1.08 ms                                                | 1.11 ms: 1.03x slower                                                 |
| gunicorn                   | 1.15 ms                                                | 1.18 ms: 1.03x slower                                                 |
| async_tree_io              | 668 ms                                                 | 690 ms: 1.03x slower                                                  |
| richards_super             | 36.0 ms                                                | 37.4 ms: 1.04x slower                                                 |
| async_tree_none            | 266 ms                                                 | 277 ms: 1.04x slower                                                  |
| unpack_sequence            | 31.5 ns                                                | 32.9 ns: 1.04x slower                                                 |
| mako                       | 7.71 ms                                                | 8.18 ms: 1.06x slower                                                 |
| sqlalchemy_imperative      | 6.68 ms                                                | 7.14 ms: 1.07x slower                                                 |
| mdp                        | 1.58 sec                                               | 1.73 sec: 1.10x slower                                                |
| async_tree_io_tg           | 669 ms                                                 | 737 ms: 1.10x slower                                                  |
| async_tree_memoization     | 312 ms                                                 | 353 ms: 1.13x slower                                                  |
| chaos                      | 42.5 ms                                                | 48.2 ms: 1.13x slower                                                 |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 607 ms: 1.14x slower                                                  |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.43 sec: 1.15x slower                                                |
| comprehensions             | 14.5 us                                                | 17.1 us: 1.18x slower                                                 |
| json_dumps                 | 6.22 ms                                                | 7.57 ms: 1.22x slower                                                 |
| sqlglot_transpile          | 1.02 ms                                                | 1.29 ms: 1.26x slower                                                 |
| async_tree_none_tg         | 258 ms                                                 | 332 ms: 1.29x slower                                                  |
| sqlglot_parse              | 848 us                                                 | 1.12 ms: 1.33x slower                                                 |
| async_tree_memoization_tg  | 323 ms                                                 | 434 ms: 1.34x slower                                                  |
| asyncio_tcp                | 449 ms                                                 | 660 ms: 1.47x slower                                                  |
| coverage                   | 38.9 ms                                                | 73.6 ms: 1.89x slower                                                 |
| typing_runtime_protocols   | 93.0 us                                                | 327 us: 3.51x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                          |

Benchmark hidden because not significant (4): dask, deltablue, python_startup, tornado_http
Ignored benchmarks (1) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: mypy2
Ignored benchmarks (6) of results/bm-20220506-3.11.0b1-8d32a5c/bm-20220506-darwin-arm64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.68% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.96x