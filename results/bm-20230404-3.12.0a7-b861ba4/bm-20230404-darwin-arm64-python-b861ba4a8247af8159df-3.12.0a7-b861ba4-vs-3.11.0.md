
# Results vs. 3.11.0

- fork: python
- ref: b861ba4a8247af8159df
- machine: darwin-arm64
- commit hash: b861ba4
- commit date: 2023-04-04
- overall geometric mean: 1.06x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 170 ms: 1.10x slower                                                  |
| chameleon      | 4.30 ms                                                | 4.73 ms: 1.10x slower                                                 |
| docutils       | 1.43 sec                                               | 1.51 sec: 1.05x slower                                                |
| html5lib       | 33.0 ms                                                | 35.6 ms: 1.08x slower                                                 |
| Geometric mean | (ref)                                                  | 1.07x slower                                                          |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|---------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization    | 336 ms                                                 | 325 ms: 1.03x faster                                                  |
| async_tree_memoization_tg | 352 ms                                                 | 343 ms: 1.03x faster                                                  |
| async_tree_none_tg        | 276 ms                                                 | 271 ms: 1.02x faster                                                  |
| async_tree_io_tg          | 724 ms                                                 | 721 ms: 1.00x faster                                                  |
| async_tree_none           | 282 ms                                                 | 288 ms: 1.02x slower                                                  |
| async_tree_cpu_io_mixed   | 519 ms                                                 | 537 ms: 1.04x slower                                                  |
| async_tree_io             | 697 ms                                                 | 740 ms: 1.06x slower                                                  |
| Geometric mean            | (ref)                                                  | 1.00x slower                                                          |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pidigits       | 280 ms                                                 | 282 ms: 1.00x slower                                                  |
| nbody          | 61.7 ms                                                | 64.0 ms: 1.04x slower                                                 |
| float          | 50.8 ms                                                | 54.3 ms: 1.07x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_v8       | 15.1 ms                                                | 15.2 ms: 1.00x slower                                                 |
| regex_effbot   | 2.43 ms                                                | 2.46 ms: 1.01x slower                                                 |
| regex_compile  | 72.8 ms                                                | 78.7 ms: 1.08x slower                                                 |
| Geometric mean | (ref)                                                  | 1.02x slower                                                          |

Benchmark hidden because not significant (1): regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| json_dumps           | 7.53 ms                                                | 6.01 ms: 1.25x faster                                                 |
| xml_etree_parse      | 100 ms                                                 | 98.6 ms: 1.02x faster                                                 |
| unpickle_list        | 2.69 us                                                | 2.70 us: 1.01x slower                                                 |
| unpickle             | 8.29 us                                                | 8.39 us: 1.01x slower                                                 |
| pickle_dict          | 17.1 us                                                | 17.3 us: 1.01x slower                                                 |
| pickle_list          | 2.70 us                                                | 2.76 us: 1.02x slower                                                 |
| pickle               | 6.98 us                                                | 7.16 us: 1.03x slower                                                 |
| json_loads           | 15.3 us                                                | 15.8 us: 1.03x slower                                                 |
| unpickle_pure_python | 149 us                                                 | 158 us: 1.06x slower                                                  |
| pickle_pure_python   | 191 us                                                 | 206 us: 1.07x slower                                                  |
| xml_etree_iterparse  | 68.3 ms                                                | 73.5 ms: 1.08x slower                                                 |
| xml_etree_generate   | 45.8 ms                                                | 49.6 ms: 1.08x slower                                                 |
| tomli_loads          | 1.27 sec                                               | 1.43 sec: 1.13x slower                                                |
| xml_etree_process    | 33.6 ms                                                | 39.0 ms: 1.16x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.03x slower                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.8 ms: 1.10x slower                                                 |
| python_startup_no_site | 8.57 ms                                                | 9.57 ms: 1.12x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.11x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 7.93 ms                                                | 7.17 ms: 1.11x faster                                                 |
| django_template | 20.1 ms                                                | 22.2 ms: 1.10x slower                                                 |
| genshi_xml      | 28.5 ms                                                | 31.5 ms: 1.10x slower                                                 |
| genshi_text     | 14.4 ms                                                | 16.2 ms: 1.12x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.05x slower                                                          |

All benchmarks:
===============

| Benchmark                 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-darwin-arm64-python-b861ba4a8247af8159df-3.12.0a7-b861ba4 |
|---------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| asyncio_tcp               | 643 ms                                                 | 434 ms: 1.48x faster                                                  |
| json_dumps                | 7.53 ms                                                | 6.01 ms: 1.25x faster                                                 |
| mako                      | 7.93 ms                                                | 7.17 ms: 1.11x faster                                                 |
| asyncio_tcp_ssl           | 1.40 sec                                               | 1.31 sec: 1.06x faster                                                |
| scimark_sparse_mat_mult   | 2.81 ms                                                | 2.72 ms: 1.04x faster                                                 |
| async_tree_memoization    | 336 ms                                                 | 325 ms: 1.03x faster                                                  |
| async_tree_memoization_tg | 352 ms                                                 | 343 ms: 1.03x faster                                                  |
| async_tree_none_tg        | 276 ms                                                 | 271 ms: 1.02x faster                                                  |
| create_gc_cycles          | 711 us                                                 | 698 us: 1.02x faster                                                  |
| xml_etree_parse           | 100 ms                                                 | 98.6 ms: 1.02x faster                                                 |
| async_tree_io_tg          | 724 ms                                                 | 721 ms: 1.00x faster                                                  |
| regex_v8                  | 15.1 ms                                                | 15.2 ms: 1.00x slower                                                 |
| pidigits                  | 280 ms                                                 | 282 ms: 1.00x slower                                                  |
| hexiom                    | 4.58 ms                                                | 4.60 ms: 1.00x slower                                                 |
| unpickle_list             | 2.69 us                                                | 2.70 us: 1.01x slower                                                 |
| gc_traversal              | 2.38 ms                                                | 2.40 ms: 1.01x slower                                                 |
| deltablue                 | 2.75 ms                                                | 2.77 ms: 1.01x slower                                                 |
| regex_effbot              | 2.43 ms                                                | 2.46 ms: 1.01x slower                                                 |
| unpickle                  | 8.29 us                                                | 8.39 us: 1.01x slower                                                 |
| pickle_dict               | 17.1 us                                                | 17.3 us: 1.01x slower                                                 |
| chaos                     | 47.4 ms                                                | 48.1 ms: 1.02x slower                                                 |
| meteor_contest            | 71.1 ms                                                | 72.3 ms: 1.02x slower                                                 |
| json                      | 2.75 ms                                                | 2.80 ms: 1.02x slower                                                 |
| dask                      | 219 ms                                                 | 224 ms: 1.02x slower                                                  |
| sqlalchemy_imperative     | 6.98 ms                                                | 7.13 ms: 1.02x slower                                                 |
| async_tree_none           | 282 ms                                                 | 288 ms: 1.02x slower                                                  |
| pickle_list               | 2.70 us                                                | 2.76 us: 1.02x slower                                                 |
| pycparser                 | 659 ms                                                 | 676 ms: 1.02x slower                                                  |
| dulwich_log               | 28.6 ms                                                | 29.3 ms: 1.02x slower                                                 |
| pickle                    | 6.98 us                                                | 7.16 us: 1.03x slower                                                 |
| json_loads                | 15.3 us                                                | 15.8 us: 1.03x slower                                                 |
| scimark_fft               | 173 ms                                                 | 177 ms: 1.03x slower                                                  |
| telco                     | 3.17 ms                                                | 3.27 ms: 1.03x slower                                                 |
| async_tree_cpu_io_mixed   | 519 ms                                                 | 537 ms: 1.04x slower                                                  |
| nbody                     | 61.7 ms                                                | 64.0 ms: 1.04x slower                                                 |
| sympy_integrate           | 11.3 ms                                                | 11.8 ms: 1.05x slower                                                 |
| pathlib                   | 23.2 ms                                                | 24.4 ms: 1.05x slower                                                 |
| docutils                  | 1.43 sec                                               | 1.51 sec: 1.05x slower                                                |
| pprint_pformat            | 979 ms                                                 | 1.03 sec: 1.05x slower                                                |
| pprint_safe_repr          | 478 ms                                                 | 505 ms: 1.06x slower                                                  |
| sqlalchemy_declarative    | 59.3 ms                                                | 62.6 ms: 1.06x slower                                                 |
| sympy_str                 | 144 ms                                                 | 152 ms: 1.06x slower                                                  |
| async_tree_io             | 697 ms                                                 | 740 ms: 1.06x slower                                                  |
| unpickle_pure_python      | 149 us                                                 | 158 us: 1.06x slower                                                  |
| float                     | 50.8 ms                                                | 54.3 ms: 1.07x slower                                                 |
| sqlite_synth              | 1.26 us                                                | 1.34 us: 1.07x slower                                                 |
| bench_thread_pool         | 465 us                                                 | 498 us: 1.07x slower                                                  |
| sympy_sum                 | 80.2 ms                                                | 85.9 ms: 1.07x slower                                                 |
| pickle_pure_python        | 191 us                                                 | 206 us: 1.07x slower                                                  |
| sympy_expand              | 229 ms                                                 | 246 ms: 1.08x slower                                                  |
| xml_etree_iterparse       | 68.3 ms                                                | 73.5 ms: 1.08x slower                                                 |
| html5lib                  | 33.0 ms                                                | 35.6 ms: 1.08x slower                                                 |
| regex_compile             | 72.8 ms                                                | 78.7 ms: 1.08x slower                                                 |
| fannkuch                  | 240 ms                                                 | 260 ms: 1.08x slower                                                  |
| xml_etree_generate        | 45.8 ms                                                | 49.6 ms: 1.08x slower                                                 |
| raytrace                  | 206 ms                                                 | 223 ms: 1.09x slower                                                  |
| deepcopy_memo             | 25.7 us                                                | 27.9 us: 1.09x slower                                                 |
| mdp                       | 1.48 sec                                               | 1.62 sec: 1.09x slower                                                |
| nqueens                   | 55.9 ms                                                | 61.1 ms: 1.09x slower                                                 |
| deepcopy                  | 215 us                                                 | 236 us: 1.09x slower                                                  |
| python_startup            | 10.8 ms                                                | 11.8 ms: 1.10x slower                                                 |
| chameleon                 | 4.30 ms                                                | 4.73 ms: 1.10x slower                                                 |
| django_template           | 20.1 ms                                                | 22.2 ms: 1.10x slower                                                 |
| 2to3                      | 154 ms                                                 | 170 ms: 1.10x slower                                                  |
| genshi_xml                | 28.5 ms                                                | 31.5 ms: 1.10x slower                                                 |
| crypto_pyaes              | 47.5 ms                                                | 52.4 ms: 1.10x slower                                                 |
| go                        | 105 ms                                                 | 117 ms: 1.11x slower                                                  |
| bench_mp_pool             | 41.0 ms                                                | 45.4 ms: 1.11x slower                                                 |
| sqlglot_optimize          | 29.6 ms                                                | 33.0 ms: 1.11x slower                                                 |
| sqlglot_normalize         | 162 ms                                                 | 181 ms: 1.12x slower                                                  |
| python_startup_no_site    | 8.57 ms                                                | 9.57 ms: 1.12x slower                                                 |
| thrift                    | 410 us                                                 | 459 us: 1.12x slower                                                  |
| genshi_text               | 14.4 ms                                                | 16.2 ms: 1.12x slower                                                 |
| tomli_loads               | 1.27 sec                                               | 1.43 sec: 1.13x slower                                                |
| richards_super            | 37.3 ms                                                | 42.3 ms: 1.14x slower                                                 |
| deepcopy_reduce           | 1.79 us                                                | 2.04 us: 1.14x slower                                                 |
| richards                  | 31.1 ms                                                | 35.3 ms: 1.14x slower                                                 |
| logging_format            | 3.67 us                                                | 4.21 us: 1.14x slower                                                 |
| scimark_sor               | 79.2 ms                                                | 90.7 ms: 1.15x slower                                                 |
| logging_simple            | 3.41 us                                                | 3.93 us: 1.15x slower                                                 |
| xml_etree_process         | 33.6 ms                                                | 39.0 ms: 1.16x slower                                                 |
| generators                | 30.3 ms                                                | 35.4 ms: 1.17x slower                                                 |
| logging_silent            | 66.5 ns                                                | 77.7 ns: 1.17x slower                                                 |
| pyflate                   | 284 ms                                                 | 332 ms: 1.17x slower                                                  |
| sqlglot_transpile         | 1.05 ms                                                | 1.24 ms: 1.17x slower                                                 |
| scimark_monte_carlo       | 43.5 ms                                                | 51.1 ms: 1.18x slower                                                 |
| comprehensions            | 14.4 us                                                | 17.0 us: 1.18x slower                                                 |
| sqlglot_parse             | 890 us                                                 | 1.07 ms: 1.20x slower                                                 |
| spectral_norm             | 65.7 ms                                                | 80.5 ms: 1.23x slower                                                 |
| coroutines                | 17.2 ms                                                | 21.4 ms: 1.25x slower                                                 |
| scimark_lu                | 67.7 ms                                                | 84.7 ms: 1.25x slower                                                 |
| typing_runtime_protocols  | 301 us                                                 | 392 us: 1.30x slower                                                  |
| async_generators          | 192 ms                                                 | 260 ms: 1.35x slower                                                  |
| Geometric mean            | (ref)                                                  | 1.06x slower                                                          |

Benchmark hidden because not significant (5): async_tree_cpu_io_mixed_tg, unpack_sequence, asyncio_websockets, regex_dna, tornado_http
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, coverage, flaskblogging, gunicorn, mypy2, pylint


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.05x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.02x