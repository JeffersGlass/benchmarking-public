
# Results vs. 3.11.0

- fork: python
- ref: 72f00f420afaba3bc873
- machine: darwin-arm64
- commit hash: 72f00f4
- commit date: 2022-05-30
- overall geometric mean: 1.02x slower \*
- HPT reliability: 92.27%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 153 ms: 1.01x faster                                                  |
| chameleon      | 4.30 ms                                                | 4.32 ms: 1.00x slower                                                 |
| docutils       | 1.43 sec                                               | 1.42 sec: 1.00x faster                                                |
| Geometric mean | (ref)                                                  | 1.00x faster                                                          |

Benchmark hidden because not significant (2): html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|---------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_memoization_tg | 352 ms                                                 | 341 ms: 1.03x faster                                                  |
| async_tree_none           | 282 ms                                                 | 278 ms: 1.01x faster                                                  |
| async_tree_io             | 697 ms                                                 | 688 ms: 1.01x faster                                                  |
| async_tree_none_tg        | 276 ms                                                 | 273 ms: 1.01x faster                                                  |
| async_tree_cpu_io_mixed   | 519 ms                                                 | 514 ms: 1.01x faster                                                  |
| async_tree_io_tg          | 724 ms                                                 | 721 ms: 1.00x faster                                                  |
| async_tree_memoization    | 336 ms                                                 | 363 ms: 1.08x slower                                                  |
| Geometric mean            | (ref)                                                  | 1.00x faster                                                          |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 61.7 ms                                                | 65.5 ms: 1.06x slower                                                 |
| float          | 50.8 ms                                                | 54.4 ms: 1.07x slower                                                 |
| Geometric mean | (ref)                                                  | 1.04x slower                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot   | 2.43 ms                                                | 2.22 ms: 1.09x faster                                                 |
| regex_dna      | 148 ms                                                 | 147 ms: 1.01x faster                                                  |
| regex_v8       | 15.1 ms                                                | 15.2 ms: 1.01x slower                                                 |
| regex_compile  | 72.8 ms                                                | 73.8 ms: 1.01x slower                                                 |
| Geometric mean | (ref)                                                  | 1.02x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_dict          | 17.1 us                                                | 16.1 us: 1.06x faster                                                 |
| pickle_list          | 2.70 us                                                | 2.59 us: 1.04x faster                                                 |
| xml_etree_parse      | 100 ms                                                 | 97.2 ms: 1.03x faster                                                 |
| xml_etree_iterparse  | 68.3 ms                                                | 66.9 ms: 1.02x faster                                                 |
| unpickle             | 8.29 us                                                | 8.23 us: 1.01x faster                                                 |
| json_dumps           | 7.53 ms                                                | 7.58 ms: 1.01x slower                                                 |
| pickle               | 6.98 us                                                | 7.03 us: 1.01x slower                                                 |
| xml_etree_process    | 33.6 ms                                                | 33.9 ms: 1.01x slower                                                 |
| unpickle_pure_python | 149 us                                                 | 151 us: 1.01x slower                                                  |
| pickle_pure_python   | 191 us                                                 | 194 us: 1.01x slower                                                  |
| xml_etree_generate   | 45.8 ms                                                | 46.7 ms: 1.02x slower                                                 |
| tomli_loads          | 1.27 sec                                               | 1.30 sec: 1.02x slower                                                |
| unpickle_list        | 2.69 us                                                | 2.80 us: 1.04x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                          |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.4 ms: 1.06x slower                                                 |
| python_startup_no_site | 8.57 ms                                                | 9.31 ms: 1.09x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.07x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| django_template | 20.1 ms                                                | 19.8 ms: 1.01x faster                                                 |
| genshi_xml      | 28.5 ms                                                | 28.8 ms: 1.01x slower                                                 |
| genshi_text     | 14.4 ms                                                | 14.6 ms: 1.02x slower                                                 |
| mako            | 7.93 ms                                                | 8.11 ms: 1.02x slower                                                 |
| Geometric mean  | (ref)                                                  | 1.01x slower                                                          |

All benchmarks:
===============

| Benchmark                 | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-darwin-arm64-python-72f00f420afaba3bc873-3.11.0b2-72f00f4 |
|---------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_effbot              | 2.43 ms                                                | 2.22 ms: 1.09x faster                                                 |
| pickle_dict               | 17.1 us                                                | 16.1 us: 1.06x faster                                                 |
| pickle_list               | 2.70 us                                                | 2.59 us: 1.04x faster                                                 |
| scimark_sor               | 79.2 ms                                                | 76.1 ms: 1.04x faster                                                 |
| async_tree_memoization_tg | 352 ms                                                 | 341 ms: 1.03x faster                                                  |
| xml_etree_parse           | 100 ms                                                 | 97.2 ms: 1.03x faster                                                 |
| raytrace                  | 206 ms                                                 | 200 ms: 1.03x faster                                                  |
| unpack_sequence           | 33.6 ns                                                | 32.7 ns: 1.03x faster                                                 |
| sympy_sum                 | 80.2 ms                                                | 78.2 ms: 1.03x faster                                                 |
| nqueens                   | 55.9 ms                                                | 54.7 ms: 1.02x faster                                                 |
| xml_etree_iterparse       | 68.3 ms                                                | 66.9 ms: 1.02x faster                                                 |
| go                        | 105 ms                                                 | 103 ms: 1.02x faster                                                  |
| django_template           | 20.1 ms                                                | 19.8 ms: 1.01x faster                                                 |
| async_tree_none           | 282 ms                                                 | 278 ms: 1.01x faster                                                  |
| async_tree_io             | 697 ms                                                 | 688 ms: 1.01x faster                                                  |
| async_tree_none_tg        | 276 ms                                                 | 273 ms: 1.01x faster                                                  |
| logging_simple            | 3.41 us                                                | 3.37 us: 1.01x faster                                                 |
| logging_format            | 3.67 us                                                | 3.63 us: 1.01x faster                                                 |
| generators                | 30.3 ms                                                | 30.0 ms: 1.01x faster                                                 |
| sympy_integrate           | 11.3 ms                                                | 11.1 ms: 1.01x faster                                                 |
| deltablue                 | 2.75 ms                                                | 2.72 ms: 1.01x faster                                                 |
| regex_dna                 | 148 ms                                                 | 147 ms: 1.01x faster                                                  |
| coroutines                | 17.2 ms                                                | 17.0 ms: 1.01x faster                                                 |
| async_tree_cpu_io_mixed   | 519 ms                                                 | 514 ms: 1.01x faster                                                  |
| async_generators          | 192 ms                                                 | 191 ms: 1.01x faster                                                  |
| unpickle                  | 8.29 us                                                | 8.23 us: 1.01x faster                                                 |
| 2to3                      | 154 ms                                                 | 153 ms: 1.01x faster                                                  |
| sympy_str                 | 144 ms                                                 | 143 ms: 1.00x faster                                                  |
| docutils                  | 1.43 sec                                               | 1.42 sec: 1.00x faster                                                |
| async_tree_io_tg          | 724 ms                                                 | 721 ms: 1.00x faster                                                  |
| asyncio_websockets        | 408 ms                                                 | 407 ms: 1.00x faster                                                  |
| logging_silent            | 66.5 ns                                                | 66.3 ns: 1.00x faster                                                 |
| crypto_pyaes              | 47.5 ms                                                | 47.4 ms: 1.00x faster                                                 |
| pyflate                   | 284 ms                                                 | 285 ms: 1.00x slower                                                  |
| chameleon                 | 4.30 ms                                                | 4.32 ms: 1.00x slower                                                 |
| sqlglot_normalize         | 162 ms                                                 | 163 ms: 1.01x slower                                                  |
| json_dumps                | 7.53 ms                                                | 7.58 ms: 1.01x slower                                                 |
| regex_v8                  | 15.1 ms                                                | 15.2 ms: 1.01x slower                                                 |
| scimark_lu                | 67.7 ms                                                | 68.2 ms: 1.01x slower                                                 |
| richards                  | 31.1 ms                                                | 31.3 ms: 1.01x slower                                                 |
| pickle                    | 6.98 us                                                | 7.03 us: 1.01x slower                                                 |
| pprint_pformat            | 979 ms                                                 | 988 ms: 1.01x slower                                                  |
| chaos                     | 47.4 ms                                                | 47.8 ms: 1.01x slower                                                 |
| genshi_xml                | 28.5 ms                                                | 28.8 ms: 1.01x slower                                                 |
| xml_etree_process         | 33.6 ms                                                | 33.9 ms: 1.01x slower                                                 |
| thrift                    | 410 us                                                 | 415 us: 1.01x slower                                                  |
| richards_super            | 37.3 ms                                                | 37.8 ms: 1.01x slower                                                 |
| unpickle_pure_python      | 149 us                                                 | 151 us: 1.01x slower                                                  |
| regex_compile             | 72.8 ms                                                | 73.8 ms: 1.01x slower                                                 |
| pprint_safe_repr          | 478 ms                                                 | 485 ms: 1.01x slower                                                  |
| pickle_pure_python        | 191 us                                                 | 194 us: 1.01x slower                                                  |
| json                      | 2.75 ms                                                | 2.79 ms: 1.01x slower                                                 |
| sympy_expand              | 229 ms                                                 | 233 ms: 1.02x slower                                                  |
| genshi_text               | 14.4 ms                                                | 14.6 ms: 1.02x slower                                                 |
| scimark_monte_carlo       | 43.5 ms                                                | 44.3 ms: 1.02x slower                                                 |
| xml_etree_generate        | 45.8 ms                                                | 46.7 ms: 1.02x slower                                                 |
| fannkuch                  | 240 ms                                                 | 244 ms: 1.02x slower                                                  |
| meteor_contest            | 71.1 ms                                                | 72.5 ms: 1.02x slower                                                 |
| mako                      | 7.93 ms                                                | 8.11 ms: 1.02x slower                                                 |
| tomli_loads               | 1.27 sec                                               | 1.30 sec: 1.02x slower                                                |
| asyncio_tcp_ssl           | 1.40 sec                                               | 1.43 sec: 1.03x slower                                                |
| sqlglot_optimize          | 29.6 ms                                                | 30.4 ms: 1.03x slower                                                 |
| asyncio_tcp               | 643 ms                                                 | 665 ms: 1.03x slower                                                  |
| spectral_norm             | 65.7 ms                                                | 68.4 ms: 1.04x slower                                                 |
| sqlite_synth              | 1.26 us                                                | 1.31 us: 1.04x slower                                                 |
| unpickle_list             | 2.69 us                                                | 2.80 us: 1.04x slower                                                 |
| scimark_sparse_mat_mult   | 2.81 ms                                                | 2.95 ms: 1.05x slower                                                 |
| deepcopy                  | 215 us                                                 | 228 us: 1.06x slower                                                  |
| scimark_fft               | 173 ms                                                 | 183 ms: 1.06x slower                                                  |
| nbody                     | 61.7 ms                                                | 65.5 ms: 1.06x slower                                                 |
| python_startup            | 10.8 ms                                                | 11.4 ms: 1.06x slower                                                 |
| float                     | 50.8 ms                                                | 54.4 ms: 1.07x slower                                                 |
| aiohttp                   | 1.02 ms                                                | 1.10 ms: 1.07x slower                                                 |
| deepcopy_reduce           | 1.79 us                                                | 1.93 us: 1.07x slower                                                 |
| deepcopy_memo             | 25.7 us                                                | 27.8 us: 1.08x slower                                                 |
| async_tree_memoization    | 336 ms                                                 | 363 ms: 1.08x slower                                                  |
| gunicorn                  | 1.10 ms                                                | 1.18 ms: 1.08x slower                                                 |
| typing_runtime_protocols  | 301 us                                                 | 326 us: 1.08x slower                                                  |
| python_startup_no_site    | 8.57 ms                                                | 9.31 ms: 1.09x slower                                                 |
| mdp                       | 1.48 sec                                               | 1.74 sec: 1.17x slower                                                |
| comprehensions            | 14.4 us                                                | 17.2 us: 1.19x slower                                                 |
| sqlglot_transpile         | 1.05 ms                                                | 1.30 ms: 1.23x slower                                                 |
| sqlglot_parse             | 890 us                                                 | 1.14 ms: 1.28x slower                                                 |
| coverage                  | 43.9 ms                                                | 72.4 ms: 1.65x slower                                                 |
| Geometric mean            | (ref)                                                  | 1.02x slower                                                          |

Benchmark hidden because not significant (18): html5lib, pylint, tornado_http, async_tree_cpu_io_mixed_tg, dask, sqlalchemy_imperative, pathlib, create_gc_cycles, pidigits, gc_traversal, pycparser, hexiom, bench_thread_pool, telco, json_loads, dulwich_log, sqlalchemy_declarative, bench_mp_pool
Ignored benchmarks (2) of results/bm-20221024-3.11.0-deaf509/bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, mypy2


# HPT report

- Reliability score: 92.27% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x