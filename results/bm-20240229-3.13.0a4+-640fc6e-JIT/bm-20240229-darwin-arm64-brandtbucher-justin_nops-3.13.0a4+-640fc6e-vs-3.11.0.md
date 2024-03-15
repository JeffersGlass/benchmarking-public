# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_nops
- machine: darwin-arm64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.08x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 188 ms: 1.22x slower                                                |
| chameleon      | 4.30 ms                                                | 4.82 ms: 1.12x slower                                               |
| docutils       | 1.43 sec                                               | 1.52 sec: 1.07x slower                                              |
| html5lib       | 33.0 ms                                                | 35.6 ms: 1.08x slower                                               |
| Geometric mean | (ref)                                                  | 1.10x slower                                                        |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none            | 282 ms                                                 | 251 ms: 1.12x faster                                                |
| async_tree_memoization_tg  | 352 ms                                                 | 321 ms: 1.10x faster                                                |
| async_tree_io_tg           | 724 ms                                                 | 667 ms: 1.09x faster                                                |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 529 ms: 1.04x faster                                                |
| async_tree_memoization     | 336 ms                                                 | 328 ms: 1.03x faster                                                |
| async_tree_io              | 697 ms                                                 | 701 ms: 1.01x slower                                                |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                        |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.00x slower                                                |
| float          | 50.8 ms                                                | 53.1 ms: 1.04x slower                                               |
| nbody          | 61.7 ms                                                | 71.3 ms: 1.16x slower                                               |
| Geometric mean | (ref)                                                  | 1.07x slower                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_dna      | 148 ms                                                 | 152 ms: 1.03x slower                                                |
| regex_effbot   | 2.43 ms                                                | 2.62 ms: 1.08x slower                                               |
| regex_v8       | 15.1 ms                                                | 17.2 ms: 1.14x slower                                               |
| regex_compile  | 72.8 ms                                                | 86.8 ms: 1.19x slower                                               |
| Geometric mean | (ref)                                                  | 1.11x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.50 ms: 1.16x faster                                               |
| pickle_pure_python   | 191 us                                                 | 196 us: 1.02x slower                                                |
| unpickle_pure_python | 149 us                                                 | 155 us: 1.04x slower                                                |
| pickle               | 6.98 us                                                | 7.29 us: 1.05x slower                                               |
| xml_etree_parse      | 100 ms                                                 | 106 ms: 1.05x slower                                                |
| pickle_dict          | 17.1 us                                                | 18.2 us: 1.07x slower                                               |
| tomli_loads          | 1.27 sec                                               | 1.37 sec: 1.07x slower                                              |
| pickle_list          | 2.70 us                                                | 2.93 us: 1.09x slower                                               |
| xml_etree_iterparse  | 68.3 ms                                                | 74.5 ms: 1.09x slower                                               |
| unpickle             | 8.29 us                                                | 9.13 us: 1.10x slower                                               |
| json_loads           | 15.3 us                                                | 17.0 us: 1.11x slower                                               |
| unpickle_list        | 2.69 us                                                | 3.07 us: 1.14x slower                                               |
| xml_etree_process    | 33.6 ms                                                | 39.2 ms: 1.17x slower                                               |
| xml_etree_generate   | 45.8 ms                                                | 55.8 ms: 1.22x slower                                               |
| Geometric mean       | (ref)                                                  | 1.07x slower                                                        |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 18.4 ms: 1.71x slower                                               |
| python_startup_no_site | 8.57 ms                                                | 16.8 ms: 1.96x slower                                               |
| Geometric mean         | (ref)                                                  | 1.83x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako            | 7.93 ms                                                | 6.82 ms: 1.16x faster                                               |
| django_template | 20.1 ms                                                | 21.8 ms: 1.08x slower                                               |
| genshi_text     | 14.4 ms                                                | 15.7 ms: 1.09x slower                                               |
| genshi_xml      | 28.5 ms                                                | 37.1 ms: 1.30x slower                                               |
| Geometric mean  | (ref)                                                  | 1.07x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-darwin-arm64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols   | 301 us                                                 | 71.3 us: 4.22x faster                                               |
| asyncio_tcp                | 643 ms                                                 | 411 ms: 1.57x faster                                                |
| pylint                     | 253 ms                                                 | 177 ms: 1.43x faster                                                |
| chaos                      | 47.4 ms                                                | 40.5 ms: 1.17x faster                                               |
| mako                       | 7.93 ms                                                | 6.82 ms: 1.16x faster                                               |
| json_dumps                 | 7.53 ms                                                | 6.50 ms: 1.16x faster                                               |
| async_tree_none            | 282 ms                                                 | 251 ms: 1.12x faster                                                |
| comprehensions             | 14.4 us                                                | 13.0 us: 1.11x faster                                               |
| async_tree_memoization_tg  | 352 ms                                                 | 321 ms: 1.10x faster                                                |
| async_tree_io_tg           | 724 ms                                                 | 667 ms: 1.09x faster                                                |
| deltablue                  | 2.75 ms                                                | 2.54 ms: 1.08x faster                                               |
| raytrace                   | 206 ms                                                 | 191 ms: 1.07x faster                                                |
| async_tree_none_tg         | 276 ms                                                 | 258 ms: 1.07x faster                                                |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.30 sec: 1.07x faster                                              |
| generators                 | 30.3 ms                                                | 28.4 ms: 1.07x faster                                               |
| sqlglot_parse              | 890 us                                                 | 834 us: 1.07x faster                                                |
| sympy_sum                  | 80.2 ms                                                | 76.9 ms: 1.04x faster                                               |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 529 ms: 1.04x faster                                                |
| async_tree_memoization     | 336 ms                                                 | 328 ms: 1.03x faster                                                |
| sqlglot_transpile          | 1.05 ms                                                | 1.03 ms: 1.02x faster                                               |
| pidigits                   | 280 ms                                                 | 282 ms: 1.00x slower                                                |
| async_tree_io              | 697 ms                                                 | 701 ms: 1.01x slower                                                |
| crypto_pyaes               | 47.5 ms                                                | 47.7 ms: 1.01x slower                                               |
| sympy_str                  | 144 ms                                                 | 145 ms: 1.01x slower                                                |
| create_gc_cycles           | 711 us                                                 | 716 us: 1.01x slower                                                |
| gc_traversal               | 2.38 ms                                                | 2.40 ms: 1.01x slower                                               |
| deepcopy_memo              | 25.7 us                                                | 26.1 us: 1.01x slower                                               |
| sympy_integrate            | 11.3 ms                                                | 11.5 ms: 1.02x slower                                               |
| logging_simple             | 3.41 us                                                | 3.49 us: 1.02x slower                                               |
| pickle_pure_python         | 191 us                                                 | 196 us: 1.02x slower                                                |
| regex_dna                  | 148 ms                                                 | 152 ms: 1.03x slower                                                |
| aiohttp                    | 1.02 ms                                                | 1.05 ms: 1.03x slower                                               |
| logging_format             | 3.67 us                                                | 3.80 us: 1.03x slower                                               |
| unpickle_pure_python       | 149 us                                                 | 155 us: 1.04x slower                                                |
| float                      | 50.8 ms                                                | 53.1 ms: 1.04x slower                                               |
| pickle                     | 6.98 us                                                | 7.29 us: 1.05x slower                                               |
| xml_etree_parse            | 100 ms                                                 | 106 ms: 1.05x slower                                                |
| meteor_contest             | 71.1 ms                                                | 75.0 ms: 1.06x slower                                               |
| coroutines                 | 17.2 ms                                                | 18.1 ms: 1.06x slower                                               |
| scimark_monte_carlo        | 43.5 ms                                                | 46.0 ms: 1.06x slower                                               |
| deepcopy                   | 215 us                                                 | 228 us: 1.06x slower                                                |
| pickle_dict                | 17.1 us                                                | 18.2 us: 1.07x slower                                               |
| docutils                   | 1.43 sec                                               | 1.52 sec: 1.07x slower                                              |
| json                       | 2.75 ms                                                | 2.95 ms: 1.07x slower                                               |
| tomli_loads                | 1.27 sec                                               | 1.37 sec: 1.07x slower                                              |
| coverage                   | 43.9 ms                                                | 47.2 ms: 1.08x slower                                               |
| sympy_expand               | 229 ms                                                 | 247 ms: 1.08x slower                                                |
| pprint_safe_repr           | 478 ms                                                 | 515 ms: 1.08x slower                                                |
| regex_effbot               | 2.43 ms                                                | 2.62 ms: 1.08x slower                                               |
| html5lib                   | 33.0 ms                                                | 35.6 ms: 1.08x slower                                               |
| django_template            | 20.1 ms                                                | 21.8 ms: 1.08x slower                                               |
| dulwich_log                | 28.6 ms                                                | 31.0 ms: 1.08x slower                                               |
| pprint_pformat             | 979 ms                                                 | 1.06 sec: 1.08x slower                                              |
| pickle_list                | 2.70 us                                                | 2.93 us: 1.09x slower                                               |
| genshi_text                | 14.4 ms                                                | 15.7 ms: 1.09x slower                                               |
| xml_etree_iterparse        | 68.3 ms                                                | 74.5 ms: 1.09x slower                                               |
| pathlib                    | 23.2 ms                                                | 25.3 ms: 1.09x slower                                               |
| logging_silent             | 66.5 ns                                                | 72.8 ns: 1.09x slower                                               |
| mdp                        | 1.48 sec                                               | 1.63 sec: 1.10x slower                                              |
| unpickle                   | 8.29 us                                                | 9.13 us: 1.10x slower                                               |
| pycparser                  | 659 ms                                                 | 727 ms: 1.10x slower                                                |
| go                         | 105 ms                                                 | 116 ms: 1.10x slower                                                |
| bench_thread_pool          | 465 us                                                 | 514 us: 1.10x slower                                                |
| deepcopy_reduce            | 1.79 us                                                | 1.98 us: 1.10x slower                                               |
| thrift                     | 410 us                                                 | 454 us: 1.11x slower                                                |
| json_loads                 | 15.3 us                                                | 17.0 us: 1.11x slower                                               |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 3.14 ms: 1.12x slower                                               |
| chameleon                  | 4.30 ms                                                | 4.82 ms: 1.12x slower                                               |
| sqlglot_normalize          | 162 ms                                                 | 183 ms: 1.13x slower                                                |
| regex_v8                   | 15.1 ms                                                | 17.2 ms: 1.14x slower                                               |
| unpickle_list              | 2.69 us                                                | 3.07 us: 1.14x slower                                               |
| nqueens                    | 55.9 ms                                                | 64.1 ms: 1.15x slower                                               |
| nbody                      | 61.7 ms                                                | 71.3 ms: 1.16x slower                                               |
| scimark_fft                | 173 ms                                                 | 200 ms: 1.16x slower                                                |
| hexiom                     | 4.58 ms                                                | 5.32 ms: 1.16x slower                                               |
| xml_etree_process          | 33.6 ms                                                | 39.2 ms: 1.17x slower                                               |
| richards_super             | 37.3 ms                                                | 43.5 ms: 1.17x slower                                               |
| regex_compile              | 72.8 ms                                                | 86.8 ms: 1.19x slower                                               |
| sqlglot_optimize           | 29.6 ms                                                | 35.6 ms: 1.20x slower                                               |
| xml_etree_generate         | 45.8 ms                                                | 55.8 ms: 1.22x slower                                               |
| pyflate                    | 284 ms                                                 | 346 ms: 1.22x slower                                                |
| 2to3                       | 154 ms                                                 | 188 ms: 1.22x slower                                                |
| spectral_norm              | 65.7 ms                                                | 81.6 ms: 1.24x slower                                               |
| scimark_lu                 | 67.7 ms                                                | 85.7 ms: 1.26x slower                                               |
| sqlite_synth               | 1.26 us                                                | 1.59 us: 1.27x slower                                               |
| richards                   | 31.1 ms                                                | 39.3 ms: 1.27x slower                                               |
| bench_mp_pool              | 41.0 ms                                                | 52.9 ms: 1.29x slower                                               |
| genshi_xml                 | 28.5 ms                                                | 37.1 ms: 1.30x slower                                               |
| fannkuch                   | 240 ms                                                 | 323 ms: 1.35x slower                                                |
| telco                      | 3.17 ms                                                | 4.47 ms: 1.41x slower                                               |
| scimark_sor                | 79.2 ms                                                | 113 ms: 1.43x slower                                                |
| mypy2                      | 372 ms                                                 | 539 ms: 1.45x slower                                                |
| dask                       | 219 ms                                                 | 334 ms: 1.52x slower                                                |
| async_generators           | 192 ms                                                 | 311 ms: 1.62x slower                                                |
| python_startup             | 10.8 ms                                                | 18.4 ms: 1.71x slower                                               |
| python_startup_no_site     | 8.57 ms                                                | 16.8 ms: 1.96x slower                                               |
| unpack_sequence            | 33.6 ns                                                | 114 ns: 3.38x slower                                                |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                        |

Benchmark hidden because not significant (4): asyncio_websockets, async_tree_cpu_io_mixed, gunicorn, tornado_http
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.90x