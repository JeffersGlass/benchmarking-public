# Results vs. base

- fork: brandtbucher
- ref: justin
- machine: darwin-arm64
- commit hash: b63610e
- commit date: 2023-12-19
- overall geometric mean: 1.01x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.16x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| 2to3           | 178 ms                                                                 | 182 ms: 1.02x slower                                           |
| chameleon      | 5.19 ms                                                                | 5.12 ms: 1.01x faster                                          |
| docutils       | 1.51 sec                                                               | 1.54 sec: 1.02x slower                                         |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|--------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| async_tree_none_tg | 263 ms                                                                 | 264 ms: 1.00x slower                                           |
| async_tree_io      | 711 ms                                                                 | 714 ms: 1.00x slower                                           |
| Geometric mean     | (ref)                                                                  | 1.00x slower                                                   |

Benchmark hidden because not significant (6): async_tree_io_tg, async_tree_cpu_io_mixed, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| float          | 61.0 ms                                                                | 58.3 ms: 1.05x faster                                          |
| nbody          | 82.4 ms                                                                | 79.4 ms: 1.04x faster                                          |
| pidigits       | 282 ms                                                                 | 284 ms: 1.00x slower                                           |
| Geometric mean | (ref)                                                                  | 1.03x faster                                                   |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| regex_dna      | 152 ms                                                                 | 153 ms: 1.00x slower                                           |
| regex_v8       | 17.7 ms                                                                | 17.8 ms: 1.01x slower                                          |
| regex_compile  | 76.9 ms                                                                | 80.6 ms: 1.05x slower                                          |
| Geometric mean | (ref)                                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|----------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| tomli_loads          | 1.61 sec                                                               | 1.53 sec: 1.05x faster                                         |
| xml_etree_process    | 41.2 ms                                                                | 41.3 ms: 1.00x slower                                          |
| json_dumps           | 6.66 ms                                                                | 6.68 ms: 1.00x slower                                          |
| xml_etree_generate   | 58.2 ms                                                                | 58.6 ms: 1.01x slower                                          |
| pickle               | 7.44 us                                                                | 7.51 us: 1.01x slower                                          |
| xml_etree_parse      | 107 ms                                                                 | 109 ms: 1.01x slower                                           |
| unpickle_pure_python | 167 us                                                                 | 169 us: 1.01x slower                                           |
| xml_etree_iterparse  | 76.6 ms                                                                | 77.6 ms: 1.01x slower                                          |
| Geometric mean       | (ref)                                                                  | 1.00x slower                                                   |

Benchmark hidden because not significant (6): pickle_pure_python, unpickle, pickle_dict, json_loads, unpickle_list, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| python_startup         | 13.1 ms                                                                | 13.3 ms: 1.02x slower                                          |
| python_startup_no_site | 11.6 ms                                                                | 12.0 ms: 1.03x slower                                          |
| Geometric mean         | (ref)                                                                  | 1.02x slower                                                   |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|-----------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| mako      | 7.99 ms                                                                | 8.10 ms: 1.01x slower                                          |

All benchmarks:
===============

| Benchmark                | bm-20231218-darwin-arm64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f | bm-20231219-darwin-arm64-brandtbucher-justin-3.13.0a2+-b63610e |
|--------------------------|:----------------------------------------------------------------------:|:--------------------------------------------------------------:|
| tomli_loads              | 1.61 sec                                                               | 1.53 sec: 1.05x faster                                         |
| float                    | 61.0 ms                                                                | 58.3 ms: 1.05x faster                                          |
| richards_super           | 39.8 ms                                                                | 38.0 ms: 1.05x faster                                          |
| richards                 | 35.7 ms                                                                | 34.1 ms: 1.05x faster                                          |
| unpack_sequence          | 30.3 ns                                                                | 29.0 ns: 1.04x faster                                          |
| nbody                    | 82.4 ms                                                                | 79.4 ms: 1.04x faster                                          |
| generators               | 26.2 ms                                                                | 25.7 ms: 1.02x faster                                          |
| coroutines               | 19.3 ms                                                                | 19.0 ms: 1.01x faster                                          |
| chameleon                | 5.19 ms                                                                | 5.12 ms: 1.01x faster                                          |
| json                     | 3.04 ms                                                                | 3.02 ms: 1.01x faster                                          |
| gc_traversal             | 2.40 ms                                                                | 2.40 ms: 1.00x faster                                          |
| xml_etree_process        | 41.2 ms                                                                | 41.3 ms: 1.00x slower                                          |
| pyflate                  | 350 ms                                                                 | 351 ms: 1.00x slower                                           |
| json_dumps               | 6.66 ms                                                                | 6.68 ms: 1.00x slower                                          |
| regex_dna                | 152 ms                                                                 | 153 ms: 1.00x slower                                           |
| async_tree_none_tg       | 263 ms                                                                 | 264 ms: 1.00x slower                                           |
| async_tree_io            | 711 ms                                                                 | 714 ms: 1.00x slower                                           |
| pidigits                 | 282 ms                                                                 | 284 ms: 1.00x slower                                           |
| regex_v8                 | 17.7 ms                                                                | 17.8 ms: 1.01x slower                                          |
| pycparser                | 720 ms                                                                 | 725 ms: 1.01x slower                                           |
| xml_etree_generate       | 58.2 ms                                                                | 58.6 ms: 1.01x slower                                          |
| scimark_sor              | 108 ms                                                                 | 109 ms: 1.01x slower                                           |
| sqlite_synth             | 1.65 us                                                                | 1.67 us: 1.01x slower                                          |
| deepcopy_reduce          | 2.11 us                                                                | 2.13 us: 1.01x slower                                          |
| sqlglot_parse            | 869 us                                                                 | 878 us: 1.01x slower                                           |
| deepcopy_memo            | 26.3 us                                                                | 26.5 us: 1.01x slower                                          |
| pickle                   | 7.44 us                                                                | 7.51 us: 1.01x slower                                          |
| typing_runtime_protocols | 75.0 us                                                                | 75.8 us: 1.01x slower                                          |
| logging_simple           | 3.65 us                                                                | 3.69 us: 1.01x slower                                          |
| sqlglot_normalize        | 193 ms                                                                 | 195 ms: 1.01x slower                                           |
| logging_silent           | 72.8 ns                                                                | 73.6 ns: 1.01x slower                                          |
| dulwich_log              | 30.2 ms                                                                | 30.5 ms: 1.01x slower                                          |
| xml_etree_parse          | 107 ms                                                                 | 109 ms: 1.01x slower                                           |
| pprint_safe_repr         | 539 ms                                                                 | 546 ms: 1.01x slower                                           |
| sympy_expand             | 257 ms                                                                 | 260 ms: 1.01x slower                                           |
| unpickle_pure_python     | 167 us                                                                 | 169 us: 1.01x slower                                           |
| sqlglot_transpile        | 1.05 ms                                                                | 1.07 ms: 1.01x slower                                          |
| xml_etree_iterparse      | 76.6 ms                                                                | 77.6 ms: 1.01x slower                                          |
| mako                     | 7.99 ms                                                                | 8.10 ms: 1.01x slower                                          |
| crypto_pyaes             | 50.2 ms                                                                | 50.9 ms: 1.01x slower                                          |
| telco                    | 4.62 ms                                                                | 4.69 ms: 1.02x slower                                          |
| pprint_pformat           | 1.09 sec                                                               | 1.11 sec: 1.02x slower                                         |
| deepcopy                 | 235 us                                                                 | 238 us: 1.02x slower                                           |
| docutils                 | 1.51 sec                                                               | 1.54 sec: 1.02x slower                                         |
| python_startup           | 13.1 ms                                                                | 13.3 ms: 1.02x slower                                          |
| dask                     | 229 ms                                                                 | 234 ms: 1.02x slower                                           |
| bench_thread_pool        | 519 us                                                                 | 531 us: 1.02x slower                                           |
| 2to3                     | 178 ms                                                                 | 182 ms: 1.02x slower                                           |
| scimark_lu               | 78.3 ms                                                                | 80.4 ms: 1.03x slower                                          |
| python_startup_no_site   | 11.6 ms                                                                | 12.0 ms: 1.03x slower                                          |
| async_generators         | 306 ms                                                                 | 315 ms: 1.03x slower                                           |
| sqlglot_optimize         | 35.8 ms                                                                | 36.9 ms: 1.03x slower                                          |
| sympy_str                | 149 ms                                                                 | 153 ms: 1.03x slower                                           |
| raytrace                 | 183 ms                                                                 | 188 ms: 1.03x slower                                           |
| deltablue                | 2.54 ms                                                                | 2.62 ms: 1.03x slower                                          |
| fannkuch                 | 293 ms                                                                 | 302 ms: 1.03x slower                                           |
| mdp                      | 1.64 sec                                                               | 1.70 sec: 1.04x slower                                         |
| scimark_sparse_mat_mult  | 3.20 ms                                                                | 3.31 ms: 1.04x slower                                          |
| chaos                    | 42.0 ms                                                                | 43.6 ms: 1.04x slower                                          |
| meteor_contest           | 74.5 ms                                                                | 77.4 ms: 1.04x slower                                          |
| bench_mp_pool            | 45.7 ms                                                                | 47.8 ms: 1.05x slower                                          |
| scimark_monte_carlo      | 49.8 ms                                                                | 52.1 ms: 1.05x slower                                          |
| regex_compile            | 76.9 ms                                                                | 80.6 ms: 1.05x slower                                          |
| scimark_fft              | 211 ms                                                                 | 222 ms: 1.05x slower                                           |
| sympy_sum                | 76.7 ms                                                                | 80.8 ms: 1.05x slower                                          |
| nqueens                  | 62.8 ms                                                                | 66.2 ms: 1.05x slower                                          |
| go                       | 109 ms                                                                 | 115 ms: 1.06x slower                                           |
| sympy_integrate          | 11.2 ms                                                                | 12.0 ms: 1.07x slower                                          |
| comprehensions           | 12.7 us                                                                | 13.7 us: 1.08x slower                                          |
| spectral_norm            | 76.1 ms                                                                | 82.8 ms: 1.09x slower                                          |
| hexiom                   | 4.71 ms                                                                | 5.43 ms: 1.15x slower                                          |
| Geometric mean           | (ref)                                                                  | 1.01x slower                                                   |

Benchmark hidden because not significant (22): pickle_pure_python, create_gc_cycles, regex_effbot, pathlib, coverage, asyncio_websockets, unpickle, pickle_dict, json_loads, unpickle_list, async_tree_io_tg, logging_format, async_tree_cpu_io_mixed, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, asyncio_tcp_ssl, pickle_list, async_tree_none, tornado_http, mypy2, asyncio_tcp


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.16x