# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_nops
- machine: darwin-arm64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.05x slower \*
- HPT reliability: 99.30%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.82x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 169 ms                                                 | 188 ms: 1.11x slower                                                |
| chameleon      | 4.70 ms                                                | 4.82 ms: 1.03x slower                                               |
| docutils       | 1.50 sec                                               | 1.52 sec: 1.02x slower                                              |
| Geometric mean | (ref)                                                  | 1.04x slower                                                        |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none            | 266 ms                                                 | 251 ms: 1.06x faster                                                |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 518 ms: 1.01x faster                                                |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 529 ms: 1.01x faster                                                |
| async_tree_io_tg           | 669 ms                                                 | 667 ms: 1.00x faster                                                |
| async_tree_memoization     | 312 ms                                                 | 328 ms: 1.05x slower                                                |
| async_tree_io              | 668 ms                                                 | 701 ms: 1.05x slower                                                |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (2): async_tree_memoization_tg, async_tree_none_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| float          | 55.8 ms                                                | 53.1 ms: 1.05x faster                                               |
| nbody          | 68.8 ms                                                | 71.3 ms: 1.04x slower                                               |
| Geometric mean | (ref)                                                  | 1.00x faster                                                        |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_dna      | 154 ms                                                 | 152 ms: 1.01x faster                                                |
| regex_effbot   | 2.64 ms                                                | 2.62 ms: 1.01x faster                                               |
| regex_v8       | 16.0 ms                                                | 17.2 ms: 1.08x slower                                               |
| regex_compile  | 77.9 ms                                                | 86.8 ms: 1.12x slower                                               |
| Geometric mean | (ref)                                                  | 1.04x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| tomli_loads          | 1.39 sec                                               | 1.37 sec: 1.02x faster                                              |
| pickle_pure_python   | 200 us                                                 | 196 us: 1.02x faster                                                |
| json_loads           | 17.2 us                                                | 17.0 us: 1.01x faster                                               |
| xml_etree_process    | 39.7 ms                                                | 39.2 ms: 1.01x faster                                               |
| xml_etree_generate   | 55.8 ms                                                | 55.8 ms: 1.00x faster                                               |
| xml_etree_iterparse  | 74.0 ms                                                | 74.5 ms: 1.01x slower                                               |
| pickle_dict          | 18.1 us                                                | 18.2 us: 1.01x slower                                               |
| pickle               | 7.23 us                                                | 7.29 us: 1.01x slower                                               |
| pickle_list          | 2.89 us                                                | 2.93 us: 1.02x slower                                               |
| unpickle_list        | 3.02 us                                                | 3.07 us: 1.02x slower                                               |
| unpickle_pure_python | 151 us                                                 | 155 us: 1.03x slower                                                |
| json_dumps           | 6.22 ms                                                | 6.50 ms: 1.05x slower                                               |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                        |

Benchmark hidden because not significant (2): xml_etree_parse, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 11.4 ms                                                | 18.4 ms: 1.61x slower                                               |
| python_startup_no_site | 9.37 ms                                                | 16.8 ms: 1.79x slower                                               |
| Geometric mean         | (ref)                                                  | 1.70x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako            | 7.71 ms                                                | 6.82 ms: 1.13x faster                                               |
| django_template | 22.3 ms                                                | 21.8 ms: 1.03x faster                                               |
| Geometric mean  | (ref)                                                  | 1.08x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols   | 93.0 us                                                | 71.3 us: 1.30x faster                                               |
| mako                       | 7.71 ms                                                | 6.82 ms: 1.13x faster                                               |
| comprehensions             | 14.5 us                                                | 13.0 us: 1.12x faster                                               |
| raytrace                   | 212 ms                                                 | 191 ms: 1.11x faster                                                |
| generators                 | 31.1 ms                                                | 28.4 ms: 1.09x faster                                               |
| asyncio_tcp                | 449 ms                                                 | 411 ms: 1.09x faster                                                |
| crypto_pyaes               | 51.9 ms                                                | 47.7 ms: 1.09x faster                                               |
| deltablue                  | 2.71 ms                                                | 2.54 ms: 1.07x faster                                               |
| coroutines                 | 19.2 ms                                                | 18.1 ms: 1.06x faster                                               |
| deepcopy_memo              | 27.7 us                                                | 26.1 us: 1.06x faster                                               |
| async_tree_none            | 266 ms                                                 | 251 ms: 1.06x faster                                                |
| logging_simple             | 3.69 us                                                | 3.49 us: 1.06x faster                                               |
| chaos                      | 42.5 ms                                                | 40.5 ms: 1.05x faster                                               |
| float                      | 55.8 ms                                                | 53.1 ms: 1.05x faster                                               |
| logging_silent             | 76.4 ns                                                | 72.8 ns: 1.05x faster                                               |
| logging_format             | 3.98 us                                                | 3.80 us: 1.05x faster                                               |
| json                       | 3.09 ms                                                | 2.95 ms: 1.05x faster                                               |
| deepcopy_reduce            | 2.07 us                                                | 1.98 us: 1.05x faster                                               |
| gunicorn                   | 1.15 ms                                                | 1.10 ms: 1.04x faster                                               |
| deepcopy                   | 235 us                                                 | 228 us: 1.03x faster                                                |
| django_template            | 22.3 ms                                                | 21.8 ms: 1.03x faster                                               |
| aiohttp                    | 1.08 ms                                                | 1.05 ms: 1.02x faster                                               |
| tomli_loads                | 1.39 sec                                               | 1.37 sec: 1.02x faster                                              |
| sympy_str                  | 148 ms                                                 | 145 ms: 1.02x faster                                                |
| pickle_pure_python         | 200 us                                                 | 196 us: 1.02x faster                                                |
| sqlglot_parse              | 848 us                                                 | 834 us: 1.02x faster                                                |
| json_loads                 | 17.2 us                                                | 17.0 us: 1.01x faster                                               |
| regex_dna                  | 154 ms                                                 | 152 ms: 1.01x faster                                                |
| async_tree_cpu_io_mixed    | 526 ms                                                 | 518 ms: 1.01x faster                                                |
| sqlglot_normalize          | 186 ms                                                 | 183 ms: 1.01x faster                                                |
| xml_etree_process          | 39.7 ms                                                | 39.2 ms: 1.01x faster                                               |
| sympy_sum                  | 77.6 ms                                                | 76.9 ms: 1.01x faster                                               |
| async_tree_cpu_io_mixed_tg | 532 ms                                                 | 529 ms: 1.01x faster                                                |
| regex_effbot               | 2.64 ms                                                | 2.62 ms: 1.01x faster                                               |
| async_tree_io_tg           | 669 ms                                                 | 667 ms: 1.00x faster                                                |
| asyncio_websockets         | 409 ms                                                 | 408 ms: 1.00x faster                                                |
| xml_etree_generate         | 55.8 ms                                                | 55.8 ms: 1.00x faster                                               |
| gc_traversal               | 2.40 ms                                                | 2.40 ms: 1.00x slower                                               |
| scimark_sparse_mat_mult    | 3.14 ms                                                | 3.14 ms: 1.00x slower                                               |
| xml_etree_iterparse        | 74.0 ms                                                | 74.5 ms: 1.01x slower                                               |
| sqlglot_transpile          | 1.02 ms                                                | 1.03 ms: 1.01x slower                                               |
| pickle_dict                | 18.1 us                                                | 18.2 us: 1.01x slower                                               |
| pickle                     | 7.23 us                                                | 7.29 us: 1.01x slower                                               |
| sympy_integrate            | 11.4 ms                                                | 11.5 ms: 1.01x slower                                               |
| sqlite_synth               | 1.57 us                                                | 1.59 us: 1.01x slower                                               |
| docutils                   | 1.50 sec                                               | 1.52 sec: 1.02x slower                                              |
| pickle_list                | 2.89 us                                                | 2.93 us: 1.02x slower                                               |
| unpickle_list              | 3.02 us                                                | 3.07 us: 1.02x slower                                               |
| bench_thread_pool          | 504 us                                                 | 514 us: 1.02x slower                                                |
| create_gc_cycles           | 701 us                                                 | 716 us: 1.02x slower                                                |
| scimark_monte_carlo        | 45.0 ms                                                | 46.0 ms: 1.02x slower                                               |
| sympy_expand               | 241 ms                                                 | 247 ms: 1.02x slower                                                |
| async_generators           | 304 ms                                                 | 311 ms: 1.02x slower                                                |
| scimark_fft                | 195 ms                                                 | 200 ms: 1.02x slower                                                |
| nqueens                    | 62.4 ms                                                | 64.1 ms: 1.03x slower                                               |
| chameleon                  | 4.70 ms                                                | 4.82 ms: 1.03x slower                                               |
| unpickle_pure_python       | 151 us                                                 | 155 us: 1.03x slower                                                |
| mdp                        | 1.58 sec                                               | 1.63 sec: 1.03x slower                                              |
| pprint_safe_repr           | 497 ms                                                 | 515 ms: 1.04x slower                                                |
| nbody                      | 68.8 ms                                                | 71.3 ms: 1.04x slower                                               |
| dulwich_log                | 29.8 ms                                                | 31.0 ms: 1.04x slower                                               |
| sqlglot_optimize           | 34.0 ms                                                | 35.6 ms: 1.04x slower                                               |
| meteor_contest             | 71.7 ms                                                | 75.0 ms: 1.05x slower                                               |
| json_dumps                 | 6.22 ms                                                | 6.50 ms: 1.05x slower                                               |
| pathlib                    | 24.2 ms                                                | 25.3 ms: 1.05x slower                                               |
| pprint_pformat             | 1.01 sec                                               | 1.06 sec: 1.05x slower                                              |
| async_tree_memoization     | 312 ms                                                 | 328 ms: 1.05x slower                                                |
| async_tree_io              | 668 ms                                                 | 701 ms: 1.05x slower                                                |
| asyncio_tcp_ssl            | 1.24 sec                                               | 1.30 sec: 1.05x slower                                              |
| spectral_norm              | 76.4 ms                                                | 81.6 ms: 1.07x slower                                               |
| pycparser                  | 677 ms                                                 | 727 ms: 1.07x slower                                                |
| regex_v8                   | 16.0 ms                                                | 17.2 ms: 1.08x slower                                               |
| pyflate                    | 316 ms                                                 | 346 ms: 1.10x slower                                                |
| 2to3                       | 169 ms                                                 | 188 ms: 1.11x slower                                                |
| regex_compile              | 77.9 ms                                                | 86.8 ms: 1.12x slower                                               |
| scimark_lu                 | 76.0 ms                                                | 85.7 ms: 1.13x slower                                               |
| go                         | 102 ms                                                 | 116 ms: 1.15x slower                                                |
| hexiom                     | 4.54 ms                                                | 5.32 ms: 1.17x slower                                               |
| bench_mp_pool              | 44.9 ms                                                | 52.9 ms: 1.18x slower                                               |
| richards_super             | 36.0 ms                                                | 43.5 ms: 1.21x slower                                               |
| telco                      | 3.68 ms                                                | 4.47 ms: 1.22x slower                                               |
| coverage                   | 38.9 ms                                                | 47.2 ms: 1.22x slower                                               |
| richards                   | 32.1 ms                                                | 39.3 ms: 1.22x slower                                               |
| scimark_sor                | 87.4 ms                                                | 113 ms: 1.29x slower                                                |
| fannkuch                   | 248 ms                                                 | 323 ms: 1.30x slower                                                |
| mypy2                      | 380 ms                                                 | 539 ms: 1.42x slower                                                |
| dask                       | 222 ms                                                 | 334 ms: 1.50x slower                                                |
| python_startup             | 11.4 ms                                                | 18.4 ms: 1.61x slower                                               |
| python_startup_no_site     | 9.37 ms                                                | 16.8 ms: 1.79x slower                                               |
| unpack_sequence            | 31.5 ns                                                | 114 ns: 3.61x slower                                                |
| Geometric mean             | (ref)                                                  | 1.05x slower                                                        |

Benchmark hidden because not significant (6): xml_etree_parse, async_tree_memoization_tg, pidigits, async_tree_none_tg, unpickle, tornado_http
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-darwin-arm64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240229-3.13.0a4+-640fc6e-JIT/bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.30% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.82x