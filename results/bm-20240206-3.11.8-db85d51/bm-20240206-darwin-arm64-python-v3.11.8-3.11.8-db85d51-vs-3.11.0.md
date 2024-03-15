
# Results vs. 3.11.0

- fork: python
- ref: v3.11.8
- machine: darwin-arm64
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.01x slower \*
- HPT reliability: 90.49%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 154 ms                                                 | 151 ms: 1.02x faster                                   |
| chameleon      | 4.30 ms                                                | 4.32 ms: 1.00x slower                                  |
| docutils       | 1.43 sec                                               | 1.42 sec: 1.01x faster                                 |
| Geometric mean | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (2): html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization_tg  | 352 ms                                                 | 332 ms: 1.06x faster                                   |
| async_tree_memoization     | 336 ms                                                 | 321 ms: 1.05x faster                                   |
| async_tree_io_tg           | 724 ms                                                 | 692 ms: 1.05x faster                                   |
| async_tree_none_tg         | 276 ms                                                 | 268 ms: 1.03x faster                                   |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 543 ms: 1.01x faster                                   |
| async_tree_io              | 697 ms                                                 | 693 ms: 1.01x faster                                   |
| Geometric mean             | (ref)                                                  | 1.03x faster                                           |

Benchmark hidden because not significant (2): async_tree_none, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 50.8 ms                                                | 53.4 ms: 1.05x slower                                  |
| nbody          | 61.7 ms                                                | 68.5 ms: 1.11x slower                                  |
| Geometric mean | (ref)                                                  | 1.05x slower                                           |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 72.8 ms                                                | 70.9 ms: 1.03x faster                                  |
| regex_dna      | 148 ms                                                 | 152 ms: 1.03x slower                                   |
| regex_v8       | 15.1 ms                                                | 16.3 ms: 1.08x slower                                  |
| regex_effbot   | 2.43 ms                                                | 2.64 ms: 1.09x slower                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| unpickle_pure_python | 149 us                                                 | 145 us: 1.02x faster                                   |
| pickle_list          | 2.70 us                                                | 2.64 us: 1.02x faster                                  |
| xml_etree_generate   | 45.8 ms                                                | 45.1 ms: 1.02x faster                                  |
| unpickle_list        | 2.69 us                                                | 2.64 us: 1.02x faster                                  |
| xml_etree_process    | 33.6 ms                                                | 33.2 ms: 1.01x faster                                  |
| unpickle             | 8.29 us                                                | 8.21 us: 1.01x faster                                  |
| json_loads           | 15.3 us                                                | 15.3 us: 1.00x faster                                  |
| json_dumps           | 7.53 ms                                                | 7.55 ms: 1.00x slower                                  |
| pickle_dict          | 17.1 us                                                | 17.3 us: 1.01x slower                                  |
| tomli_loads          | 1.27 sec                                               | 1.29 sec: 1.01x slower                                 |
| pickle_pure_python   | 191 us                                                 | 196 us: 1.02x slower                                   |
| Geometric mean       | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (3): xml_etree_iterparse, pickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 10.8 ms                                                | 11.6 ms: 1.08x slower                                  |
| python_startup_no_site | 8.57 ms                                                | 9.53 ms: 1.11x slower                                  |
| Geometric mean         | (ref)                                                  | 1.10x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 20.1 ms                                                | 19.6 ms: 1.02x faster                                  |
| genshi_text     | 14.4 ms                                                | 14.2 ms: 1.02x faster                                  |
| genshi_xml      | 28.5 ms                                                | 28.3 ms: 1.01x faster                                  |
| mako            | 7.93 ms                                                | 7.97 ms: 1.00x slower                                  |
| Geometric mean  | (ref)                                                  | 1.01x faster                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-darwin-arm64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-darwin-arm64-python-v3.11.8-3.11.8-db85d51 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization_tg  | 352 ms                                                 | 332 ms: 1.06x faster                                   |
| deepcopy                   | 215 us                                                 | 204 us: 1.05x faster                                   |
| deltablue                  | 2.75 ms                                                | 2.62 ms: 1.05x faster                                  |
| async_tree_memoization     | 336 ms                                                 | 321 ms: 1.05x faster                                   |
| async_tree_io_tg           | 724 ms                                                 | 692 ms: 1.05x faster                                   |
| comprehensions             | 14.4 us                                                | 13.9 us: 1.04x faster                                  |
| deepcopy_memo              | 25.7 us                                                | 24.9 us: 1.03x faster                                  |
| generators                 | 30.3 ms                                                | 29.4 ms: 1.03x faster                                  |
| async_tree_none_tg         | 276 ms                                                 | 268 ms: 1.03x faster                                   |
| regex_compile              | 72.8 ms                                                | 70.9 ms: 1.03x faster                                  |
| async_generators           | 192 ms                                                 | 187 ms: 1.03x faster                                   |
| django_template            | 20.1 ms                                                | 19.6 ms: 1.02x faster                                  |
| sympy_str                  | 144 ms                                                 | 140 ms: 1.02x faster                                   |
| unpickle_pure_python       | 149 us                                                 | 145 us: 1.02x faster                                   |
| sympy_sum                  | 80.2 ms                                                | 78.5 ms: 1.02x faster                                  |
| go                         | 105 ms                                                 | 103 ms: 1.02x faster                                   |
| deepcopy_reduce            | 1.79 us                                                | 1.76 us: 1.02x faster                                  |
| pickle_list                | 2.70 us                                                | 2.64 us: 1.02x faster                                  |
| sympy_integrate            | 11.3 ms                                                | 11.1 ms: 1.02x faster                                  |
| 2to3                       | 154 ms                                                 | 151 ms: 1.02x faster                                   |
| coroutines                 | 17.2 ms                                                | 16.9 ms: 1.02x faster                                  |
| xml_etree_generate         | 45.8 ms                                                | 45.1 ms: 1.02x faster                                  |
| unpickle_list              | 2.69 us                                                | 2.64 us: 1.02x faster                                  |
| genshi_text                | 14.4 ms                                                | 14.2 ms: 1.02x faster                                  |
| async_tree_cpu_io_mixed_tg | 550 ms                                                 | 543 ms: 1.01x faster                                   |
| nqueens                    | 55.9 ms                                                | 55.3 ms: 1.01x faster                                  |
| raytrace                   | 206 ms                                                 | 203 ms: 1.01x faster                                   |
| sympy_expand               | 229 ms                                                 | 227 ms: 1.01x faster                                   |
| xml_etree_process          | 33.6 ms                                                | 33.2 ms: 1.01x faster                                  |
| coverage                   | 43.9 ms                                                | 43.4 ms: 1.01x faster                                  |
| sqlglot_transpile          | 1.05 ms                                                | 1.04 ms: 1.01x faster                                  |
| sqlglot_normalize          | 162 ms                                                 | 160 ms: 1.01x faster                                   |
| unpickle                   | 8.29 us                                                | 8.21 us: 1.01x faster                                  |
| bench_thread_pool          | 465 us                                                 | 461 us: 1.01x faster                                   |
| hexiom                     | 4.58 ms                                                | 4.53 ms: 1.01x faster                                  |
| genshi_xml                 | 28.5 ms                                                | 28.3 ms: 1.01x faster                                  |
| flaskblogging              | 2.35 ms                                                | 2.33 ms: 1.01x faster                                  |
| docutils                   | 1.43 sec                                               | 1.42 sec: 1.01x faster                                 |
| logging_simple             | 3.41 us                                                | 3.39 us: 1.01x faster                                  |
| logging_silent             | 66.5 ns                                                | 66.0 ns: 1.01x faster                                  |
| telco                      | 3.17 ms                                                | 3.15 ms: 1.01x faster                                  |
| mdp                        | 1.48 sec                                               | 1.48 sec: 1.01x faster                                 |
| async_tree_io              | 697 ms                                                 | 693 ms: 1.01x faster                                   |
| json                       | 2.75 ms                                                | 2.74 ms: 1.01x faster                                  |
| json_loads                 | 15.3 us                                                | 15.3 us: 1.00x faster                                  |
| sqlglot_optimize           | 29.6 ms                                                | 29.5 ms: 1.00x faster                                  |
| asyncio_websockets         | 408 ms                                                 | 407 ms: 1.00x faster                                   |
| crypto_pyaes               | 47.5 ms                                                | 47.3 ms: 1.00x faster                                  |
| pprint_pformat             | 979 ms                                                 | 976 ms: 1.00x faster                                   |
| scimark_lu                 | 67.7 ms                                                | 67.6 ms: 1.00x faster                                  |
| sqlite_synth               | 1.26 us                                                | 1.26 us: 1.00x slower                                  |
| json_dumps                 | 7.53 ms                                                | 7.55 ms: 1.00x slower                                  |
| thrift                     | 410 us                                                 | 411 us: 1.00x slower                                   |
| mako                       | 7.93 ms                                                | 7.97 ms: 1.00x slower                                  |
| chameleon                  | 4.30 ms                                                | 4.32 ms: 1.00x slower                                  |
| typing_runtime_protocols   | 301 us                                                 | 303 us: 1.01x slower                                   |
| sqlalchemy_declarative     | 59.3 ms                                                | 59.6 ms: 1.01x slower                                  |
| sqlalchemy_imperative      | 6.98 ms                                                | 7.03 ms: 1.01x slower                                  |
| richards                   | 31.1 ms                                                | 31.3 ms: 1.01x slower                                  |
| pickle_dict                | 17.1 us                                                | 17.3 us: 1.01x slower                                  |
| tomli_loads                | 1.27 sec                                               | 1.29 sec: 1.01x slower                                 |
| richards_super             | 37.3 ms                                                | 37.8 ms: 1.01x slower                                  |
| chaos                      | 47.4 ms                                                | 48.1 ms: 1.01x slower                                  |
| pyflate                    | 284 ms                                                 | 289 ms: 1.02x slower                                   |
| asyncio_tcp                | 643 ms                                                 | 656 ms: 1.02x slower                                   |
| pickle_pure_python         | 191 us                                                 | 196 us: 1.02x slower                                   |
| scimark_sor                | 79.2 ms                                                | 81.0 ms: 1.02x slower                                  |
| asyncio_tcp_ssl            | 1.40 sec                                               | 1.43 sec: 1.02x slower                                 |
| fannkuch                   | 240 ms                                                 | 246 ms: 1.02x slower                                   |
| regex_dna                  | 148 ms                                                 | 152 ms: 1.03x slower                                   |
| aiohttp                    | 1.02 ms                                                | 1.06 ms: 1.04x slower                                  |
| float                      | 50.8 ms                                                | 53.4 ms: 1.05x slower                                  |
| gunicorn                   | 1.10 ms                                                | 1.15 ms: 1.05x slower                                  |
| scimark_sparse_mat_mult    | 2.81 ms                                                | 2.98 ms: 1.06x slower                                  |
| scimark_monte_carlo        | 43.5 ms                                                | 46.2 ms: 1.06x slower                                  |
| spectral_norm              | 65.7 ms                                                | 70.0 ms: 1.06x slower                                  |
| scimark_fft                | 173 ms                                                 | 186 ms: 1.08x slower                                   |
| python_startup             | 10.8 ms                                                | 11.6 ms: 1.08x slower                                  |
| regex_v8                   | 15.1 ms                                                | 16.3 ms: 1.08x slower                                  |
| regex_effbot               | 2.43 ms                                                | 2.64 ms: 1.09x slower                                  |
| nbody                      | 61.7 ms                                                | 68.5 ms: 1.11x slower                                  |
| python_startup_no_site     | 8.57 ms                                                | 9.53 ms: 1.11x slower                                  |
| mypy2                      | 372 ms                                                 | 573 ms: 1.54x slower                                   |
| Geometric mean             | (ref)                                                  | 1.01x slower                                           |

Benchmark hidden because not significant (21): pylint, dask, async_tree_none, pycparser, xml_etree_iterparse, logging_format, pickle, sqlglot_parse, pprint_safe_repr, dulwich_log, pidigits, gc_traversal, create_gc_cycles, meteor_contest, pathlib, async_tree_cpu_io_mixed, tornado_http, unpack_sequence, xml_etree_parse, bench_mp_pool, html5lib


# HPT report

- Reliability score: 90.49% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x