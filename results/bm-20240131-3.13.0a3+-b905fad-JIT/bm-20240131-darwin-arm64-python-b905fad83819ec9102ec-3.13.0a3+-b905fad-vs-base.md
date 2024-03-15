# Results vs. base

- fork: python
- ref: b905fad83819ec9102ec
- machine: darwin-arm64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.01x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.15x

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 170 ms                                                                                                            | 174 ms: 1.03x slower                                                                                                  |
| docutils       | 1.45 sec                                                                                                          | 1.48 sec: 1.02x slower                                                                                                |
| Geometric mean | (ref)                                                                                                             | 1.02x slower                                                                                                          |

Benchmark hidden because not significant (2): chameleon, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|--------------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| async_tree_none_tg | 258 ms                                                                                                            | 259 ms: 1.01x slower                                                                                                  |
| Geometric mean     | (ref)                                                                                                             | 1.00x slower                                                                                                          |

Benchmark hidden because not significant (7): async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_io, async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_memoization, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| float          | 56.4 ms                                                                                                           | 55.9 ms: 1.01x faster                                                                                                 |
| nbody          | 75.0 ms                                                                                                           | 76.8 ms: 1.02x slower                                                                                                 |
| Geometric mean | (ref)                                                                                                             | 1.01x slower                                                                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| regex_effbot   | 2.56 ms                                                                                                           | 2.55 ms: 1.00x faster                                                                                                 |
| regex_dna      | 151 ms                                                                                                            | 152 ms: 1.00x slower                                                                                                  |
| regex_v8       | 17.1 ms                                                                                                           | 17.1 ms: 1.00x slower                                                                                                 |
| regex_compile  | 73.1 ms                                                                                                           | 76.3 ms: 1.04x slower                                                                                                 |
| Geometric mean | (ref)                                                                                                             | 1.01x slower                                                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| tomli_loads          | 1.54 sec                                                                                                          | 1.40 sec: 1.10x faster                                                                                                |
| unpickle             | 9.23 us                                                                                                           | 9.02 us: 1.02x faster                                                                                                 |
| json_loads           | 16.9 us                                                                                                           | 16.9 us: 1.00x slower                                                                                                 |
| pickle_pure_python   | 196 us                                                                                                            | 197 us: 1.00x slower                                                                                                  |
| xml_etree_iterparse  | 75.5 ms                                                                                                           | 76.2 ms: 1.01x slower                                                                                                 |
| pickle_dict          | 18.1 us                                                                                                           | 18.3 us: 1.01x slower                                                                                                 |
| pickle               | 7.23 us                                                                                                           | 7.31 us: 1.01x slower                                                                                                 |
| xml_etree_parse      | 105 ms                                                                                                            | 108 ms: 1.02x slower                                                                                                  |
| unpickle_pure_python | 153 us                                                                                                            | 158 us: 1.03x slower                                                                                                  |
| Geometric mean       | (ref)                                                                                                             | 1.00x faster                                                                                                          |

Benchmark hidden because not significant (5): unpickle_list, xml_etree_process, xml_etree_generate, json_dumps, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|------------------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| python_startup         | 13.0 ms                                                                                                           | 13.2 ms: 1.01x slower                                                                                                 |
| python_startup_no_site | 11.6 ms                                                                                                           | 11.8 ms: 1.01x slower                                                                                                 |
| Geometric mean         | (ref)                                                                                                             | 1.01x slower                                                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|-----------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| mako      | 7.59 ms                                                                                                           | 7.94 ms: 1.05x slower                                                                                                 |

All benchmarks:
===============

| Benchmark                | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-darwin-arm64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|--------------------------|:-----------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------:|
| tomli_loads              | 1.54 sec                                                                                                          | 1.40 sec: 1.10x faster                                                                                                |
| richards                 | 33.5 ms                                                                                                           | 32.2 ms: 1.04x faster                                                                                                 |
| richards_super           | 37.4 ms                                                                                                           | 36.1 ms: 1.04x faster                                                                                                 |
| unpickle                 | 9.23 us                                                                                                           | 9.02 us: 1.02x faster                                                                                                 |
| pyflate                  | 334 ms                                                                                                            | 327 ms: 1.02x faster                                                                                                  |
| coroutines               | 19.5 ms                                                                                                           | 19.1 ms: 1.02x faster                                                                                                 |
| generators               | 28.3 ms                                                                                                           | 27.9 ms: 1.01x faster                                                                                                 |
| float                    | 56.4 ms                                                                                                           | 55.9 ms: 1.01x faster                                                                                                 |
| coverage                 | 47.6 ms                                                                                                           | 47.3 ms: 1.01x faster                                                                                                 |
| regex_effbot             | 2.56 ms                                                                                                           | 2.55 ms: 1.00x faster                                                                                                 |
| regex_dna                | 151 ms                                                                                                            | 152 ms: 1.00x slower                                                                                                  |
| regex_v8                 | 17.1 ms                                                                                                           | 17.1 ms: 1.00x slower                                                                                                 |
| json_loads               | 16.9 us                                                                                                           | 16.9 us: 1.00x slower                                                                                                 |
| pickle_pure_python       | 196 us                                                                                                            | 197 us: 1.00x slower                                                                                                  |
| async_tree_none_tg       | 258 ms                                                                                                            | 259 ms: 1.01x slower                                                                                                  |
| create_gc_cycles         | 701 us                                                                                                            | 705 us: 1.01x slower                                                                                                  |
| scimark_sor              | 105 ms                                                                                                            | 106 ms: 1.01x slower                                                                                                  |
| pprint_safe_repr         | 513 ms                                                                                                            | 516 ms: 1.01x slower                                                                                                  |
| sqlglot_parse            | 793 us                                                                                                            | 799 us: 1.01x slower                                                                                                  |
| logging_silent           | 70.1 ns                                                                                                           | 70.7 ns: 1.01x slower                                                                                                 |
| logging_simple           | 3.45 us                                                                                                           | 3.48 us: 1.01x slower                                                                                                 |
| deepcopy_memo            | 25.7 us                                                                                                           | 25.9 us: 1.01x slower                                                                                                 |
| xml_etree_iterparse      | 75.5 ms                                                                                                           | 76.2 ms: 1.01x slower                                                                                                 |
| python_startup           | 13.0 ms                                                                                                           | 13.2 ms: 1.01x slower                                                                                                 |
| pickle_dict              | 18.1 us                                                                                                           | 18.3 us: 1.01x slower                                                                                                 |
| sqlglot_transpile        | 971 us                                                                                                            | 982 us: 1.01x slower                                                                                                  |
| pickle                   | 7.23 us                                                                                                           | 7.31 us: 1.01x slower                                                                                                 |
| pycparser                | 691 ms                                                                                                            | 699 ms: 1.01x slower                                                                                                  |
| pprint_pformat           | 1.04 sec                                                                                                          | 1.06 sec: 1.01x slower                                                                                                |
| deepcopy                 | 224 us                                                                                                            | 227 us: 1.01x slower                                                                                                  |
| dulwich_log              | 29.5 ms                                                                                                           | 29.9 ms: 1.01x slower                                                                                                 |
| python_startup_no_site   | 11.6 ms                                                                                                           | 11.8 ms: 1.01x slower                                                                                                 |
| telco                    | 4.46 ms                                                                                                           | 4.53 ms: 1.02x slower                                                                                                 |
| typing_runtime_protocols | 70.8 us                                                                                                           | 72.0 us: 1.02x slower                                                                                                 |
| sqlite_synth             | 1.58 us                                                                                                           | 1.60 us: 1.02x slower                                                                                                 |
| logging_format           | 3.75 us                                                                                                           | 3.82 us: 1.02x slower                                                                                                 |
| dask                     | 222 ms                                                                                                            | 225 ms: 1.02x slower                                                                                                  |
| docutils                 | 1.45 sec                                                                                                          | 1.48 sec: 1.02x slower                                                                                                |
| crypto_pyaes             | 48.3 ms                                                                                                           | 49.2 ms: 1.02x slower                                                                                                 |
| sqlglot_normalize        | 182 ms                                                                                                            | 185 ms: 1.02x slower                                                                                                  |
| sympy_expand             | 237 ms                                                                                                            | 242 ms: 1.02x slower                                                                                                  |
| xml_etree_parse          | 105 ms                                                                                                            | 108 ms: 1.02x slower                                                                                                  |
| meteor_contest           | 72.4 ms                                                                                                           | 74.1 ms: 1.02x slower                                                                                                 |
| nbody                    | 75.0 ms                                                                                                           | 76.8 ms: 1.02x slower                                                                                                 |
| bench_thread_pool        | 491 us                                                                                                            | 503 us: 1.02x slower                                                                                                  |
| fannkuch                 | 271 ms                                                                                                            | 278 ms: 1.02x slower                                                                                                  |
| sympy_str                | 139 ms                                                                                                            | 142 ms: 1.03x slower                                                                                                  |
| 2to3                     | 170 ms                                                                                                            | 174 ms: 1.03x slower                                                                                                  |
| sqlglot_optimize         | 33.7 ms                                                                                                           | 34.8 ms: 1.03x slower                                                                                                 |
| unpickle_pure_python     | 153 us                                                                                                            | 158 us: 1.03x slower                                                                                                  |
| deltablue                | 2.43 ms                                                                                                           | 2.51 ms: 1.03x slower                                                                                                 |
| async_generators         | 294 ms                                                                                                            | 304 ms: 1.03x slower                                                                                                  |
| mdp                      | 1.56 sec                                                                                                          | 1.62 sec: 1.04x slower                                                                                                |
| scimark_monte_carlo      | 47.2 ms                                                                                                           | 49.2 ms: 1.04x slower                                                                                                 |
| raytrace                 | 170 ms                                                                                                            | 177 ms: 1.04x slower                                                                                                  |
| regex_compile            | 73.1 ms                                                                                                           | 76.3 ms: 1.04x slower                                                                                                 |
| nqueens                  | 60.1 ms                                                                                                           | 62.8 ms: 1.04x slower                                                                                                 |
| bench_mp_pool            | 44.7 ms                                                                                                           | 46.7 ms: 1.05x slower                                                                                                 |
| mako                     | 7.59 ms                                                                                                           | 7.94 ms: 1.05x slower                                                                                                 |
| go                       | 105 ms                                                                                                            | 110 ms: 1.05x slower                                                                                                  |
| sympy_sum                | 72.1 ms                                                                                                           | 76.1 ms: 1.06x slower                                                                                                 |
| sympy_integrate          | 10.7 ms                                                                                                           | 11.3 ms: 1.06x slower                                                                                                 |
| comprehensions           | 11.9 us                                                                                                           | 12.7 us: 1.07x slower                                                                                                 |
| chaos                    | 39.5 ms                                                                                                           | 42.2 ms: 1.07x slower                                                                                                 |
| scimark_sparse_mat_mult  | 3.11 ms                                                                                                           | 3.34 ms: 1.07x slower                                                                                                 |
| scimark_fft              | 203 ms                                                                                                            | 218 ms: 1.08x slower                                                                                                  |
| spectral_norm            | 74.7 ms                                                                                                           | 82.9 ms: 1.11x slower                                                                                                 |
| hexiom                   | 4.47 ms                                                                                                           | 5.09 ms: 1.14x slower                                                                                                 |
| Geometric mean           | (ref)                                                                                                             | 1.01x slower                                                                                                          |

Benchmark hidden because not significant (25): asyncio_tcp, pathlib, unpack_sequence, unpickle_list, asyncio_tcp_ssl, scimark_lu, json, xml_etree_process, chameleon, xml_etree_generate, gc_traversal, asyncio_websockets, pidigits, async_tree_cpu_io_mixed_tg, deepcopy_reduce, async_tree_io_tg, json_dumps, async_tree_io, pickle_list, async_tree_memoization_tg, async_tree_cpu_io_mixed, async_tree_memoization, async_tree_none, tornado_http, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.15x