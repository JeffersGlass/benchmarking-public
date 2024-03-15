
# Results vs. 3.11.0

- fork: python
- ref: 52eade22237eef1f3843
- machine: linux-x86_64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.07x faster
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 293 ms: 1.02x slower                                                         |
| chameleon      | 7.92 ms                                                      | 7.16 ms: 1.11x faster                                                        |
| docutils       | 2.85 sec                                                     | 2.83 sec: 1.01x faster                                                       |
| tornado_http   | 124 ms                                                       | 117 ms: 1.06x faster                                                         |
| Geometric mean | (ref)                                                        | 1.04x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 432 ms: 1.20x faster                                                         |
| async_tree_memoization     | 629 ms                                                       | 547 ms: 1.15x faster                                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 543 ms: 1.10x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 431 ms: 1.10x faster                                                         |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 698 ms: 1.08x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 701 ms: 1.07x faster                                                         |
| Geometric mean             | (ref)                                                        | 1.11x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 88.6 ms: 1.05x faster                                                        |
| pidigits       | 251 ms                                                       | 264 ms: 1.05x slower                                                         |
| float          | 74.9 ms                                                      | 79.9 ms: 1.07x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 140 ms: 1.11x faster                                                         |
| regex_dna      | 227 ms                                                       | 239 ms: 1.05x slower                                                         |
| regex_effbot   | 3.34 ms                                                      | 3.59 ms: 1.07x slower                                                        |
| regex_v8       | 24.4 ms                                                      | 26.7 ms: 1.09x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                        |
| json_loads           | 28.9 us                                                      | 25.0 us: 1.16x faster                                                        |
| unpickle_pure_python | 238 us                                                       | 211 us: 1.13x faster                                                         |
| pickle_dict          | 32.3 us                                                      | 30.7 us: 1.05x faster                                                        |
| pickle_pure_python   | 316 us                                                       | 307 us: 1.03x faster                                                         |
| xml_etree_process    | 55.9 ms                                                      | 57.3 ms: 1.03x slower                                                        |
| tomli_loads          | 2.25 sec                                                     | 2.31 sec: 1.03x slower                                                       |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                        |
| unpickle_list        | 4.60 us                                                      | 4.88 us: 1.06x slower                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 84.7 ms: 1.06x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.39 us: 1.11x slower                                                        |
| unpickle             | 13.3 us                                                      | 14.8 us: 1.12x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                                 |

Benchmark hidden because not significant (2): xml_etree_iterparse, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.17x slower                                                        |
| python_startup_no_site | 7.73 ms                                                      | 11.0 ms: 1.43x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.4 ms: 1.06x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240120-pythonperf2-x86_64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 114 us: 4.66x faster                                                         |
| asyncio_tcp                | 747 ms                                                       | 365 ms: 2.05x faster                                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                                       |
| generators                 | 54.6 ms                                                      | 33.8 ms: 1.62x faster                                                        |
| comprehensions             | 25.1 us                                                      | 16.5 us: 1.51x faster                                                        |
| chaos                      | 74.9 ms                                                      | 58.9 ms: 1.27x faster                                                        |
| coroutines                 | 27.8 ms                                                      | 22.1 ms: 1.25x faster                                                        |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                        |
| sympy_sum                  | 186 ms                                                       | 152 ms: 1.22x faster                                                         |
| async_tree_none            | 518 ms                                                       | 432 ms: 1.20x faster                                                         |
| crypto_pyaes               | 83.3 ms                                                      | 70.0 ms: 1.19x faster                                                        |
| scimark_lu                 | 114 ms                                                       | 96.1 ms: 1.19x faster                                                        |
| raytrace                   | 309 ms                                                       | 263 ms: 1.18x faster                                                         |
| nqueens                    | 103 ms                                                       | 87.6 ms: 1.17x faster                                                        |
| sympy_str                  | 337 ms                                                       | 290 ms: 1.16x faster                                                         |
| json_loads                 | 28.9 us                                                      | 25.0 us: 1.16x faster                                                        |
| async_tree_memoization     | 629 ms                                                       | 547 ms: 1.15x faster                                                         |
| unpickle_pure_python       | 238 us                                                       | 211 us: 1.13x faster                                                         |
| sympy_expand               | 553 ms                                                       | 491 ms: 1.13x faster                                                         |
| deltablue                  | 3.97 ms                                                      | 3.53 ms: 1.12x faster                                                        |
| mdp                        | 2.77 sec                                                     | 2.47 sec: 1.12x faster                                                       |
| sympy_integrate            | 25.8 ms                                                      | 23.1 ms: 1.12x faster                                                        |
| logging_simple             | 7.24 us                                                      | 6.50 us: 1.11x faster                                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.36 ms: 1.11x faster                                                        |
| regex_compile              | 156 ms                                                       | 140 ms: 1.11x faster                                                         |
| chameleon                  | 7.92 ms                                                      | 7.16 ms: 1.11x faster                                                        |
| async_tree_memoization_tg  | 600 ms                                                       | 543 ms: 1.10x faster                                                         |
| async_tree_none_tg         | 474 ms                                                       | 431 ms: 1.10x faster                                                         |
| logging_format             | 7.71 us                                                      | 7.04 us: 1.09x faster                                                        |
| async_tree_io              | 1.17 sec                                                     | 1.07 sec: 1.09x faster                                                       |
| hexiom                     | 6.98 ms                                                      | 6.39 ms: 1.09x faster                                                        |
| fannkuch                   | 416 ms                                                       | 382 ms: 1.09x faster                                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.77 ms: 1.08x faster                                                        |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                       |
| richards_super             | 63.6 ms                                                      | 58.9 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 698 ms: 1.08x faster                                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 701 ms: 1.07x faster                                                         |
| deepcopy                   | 391 us                                                       | 367 us: 1.07x faster                                                         |
| sqlglot_normalize          | 122 ms                                                       | 115 ms: 1.06x faster                                                         |
| tornado_http               | 124 ms                                                       | 117 ms: 1.06x faster                                                         |
| mako                       | 11.0 ms                                                      | 10.4 ms: 1.06x faster                                                        |
| pickle_dict                | 32.3 us                                                      | 30.7 us: 1.05x faster                                                        |
| json                       | 5.58 ms                                                      | 5.30 ms: 1.05x faster                                                        |
| scimark_monte_carlo        | 69.8 ms                                                      | 66.3 ms: 1.05x faster                                                        |
| nbody                      | 92.9 ms                                                      | 88.6 ms: 1.05x faster                                                        |
| logging_silent             | 100 ns                                                       | 95.8 ns: 1.05x faster                                                        |
| spectral_norm              | 95.1 ms                                                      | 91.4 ms: 1.04x faster                                                        |
| bench_thread_pool          | 1.00 ms                                                      | 964 us: 1.04x faster                                                         |
| gc_traversal               | 4.15 ms                                                      | 4.00 ms: 1.04x faster                                                        |
| dask                       | 410 ms                                                       | 396 ms: 1.03x faster                                                         |
| pickle_pure_python         | 316 us                                                       | 307 us: 1.03x faster                                                         |
| deepcopy_reduce            | 3.40 us                                                      | 3.30 us: 1.03x faster                                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.62 sec: 1.03x faster                                                       |
| meteor_contest             | 131 ms                                                       | 127 ms: 1.03x faster                                                         |
| deepcopy_memo              | 37.5 us                                                      | 37.0 us: 1.02x faster                                                        |
| pathlib                    | 18.9 ms                                                      | 18.7 ms: 1.02x faster                                                        |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.01 ms: 1.01x faster                                                        |
| pprint_safe_repr           | 805 ms                                                       | 796 ms: 1.01x faster                                                         |
| docutils                   | 2.85 sec                                                     | 2.83 sec: 1.01x faster                                                       |
| sqlglot_optimize           | 59.0 ms                                                      | 58.6 ms: 1.01x faster                                                        |
| dulwich_log                | 67.4 ms                                                      | 67.9 ms: 1.01x slower                                                        |
| 2to3                       | 287 ms                                                       | 293 ms: 1.02x slower                                                         |
| xml_etree_process          | 55.9 ms                                                      | 57.3 ms: 1.03x slower                                                        |
| tomli_loads                | 2.25 sec                                                     | 2.31 sec: 1.03x slower                                                       |
| pidigits                   | 251 ms                                                       | 264 ms: 1.05x slower                                                         |
| pickle                     | 9.89 us                                                      | 10.4 us: 1.05x slower                                                        |
| regex_dna                  | 227 ms                                                       | 239 ms: 1.05x slower                                                         |
| richards                   | 49.7 ms                                                      | 52.2 ms: 1.05x slower                                                        |
| scimark_fft                | 281 ms                                                       | 296 ms: 1.06x slower                                                         |
| unpickle_list              | 4.60 us                                                      | 4.88 us: 1.06x slower                                                        |
| xml_etree_generate         | 79.7 ms                                                      | 84.7 ms: 1.06x slower                                                        |
| float                      | 74.9 ms                                                      | 79.9 ms: 1.07x slower                                                        |
| sqlite_synth               | 2.52 us                                                      | 2.70 us: 1.07x slower                                                        |
| go                         | 158 ms                                                       | 169 ms: 1.07x slower                                                         |
| regex_effbot               | 3.34 ms                                                      | 3.59 ms: 1.07x slower                                                        |
| regex_v8                   | 24.4 ms                                                      | 26.7 ms: 1.09x slower                                                        |
| pickle_list                | 3.94 us                                                      | 4.39 us: 1.11x slower                                                        |
| unpickle                   | 13.3 us                                                      | 14.8 us: 1.12x slower                                                        |
| mypy2                      | 762 ms                                                       | 857 ms: 1.13x slower                                                         |
| async_generators           | 322 ms                                                       | 363 ms: 1.13x slower                                                         |
| unpack_sequence            | 45.7 ns                                                      | 52.1 ns: 1.14x slower                                                        |
| pyflate                    | 449 ms                                                       | 518 ms: 1.15x slower                                                         |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.17x slower                                                        |
| telco                      | 6.81 ms                                                      | 8.05 ms: 1.18x slower                                                        |
| coverage                   | 66.1 ms                                                      | 80.5 ms: 1.22x slower                                                        |
| scimark_sor                | 110 ms                                                       | 141 ms: 1.29x slower                                                         |
| python_startup_no_site     | 7.73 ms                                                      | 11.0 ms: 1.43x slower                                                        |
| Geometric mean             | (ref)                                                        | 1.07x faster                                                                 |

Benchmark hidden because not significant (6): create_gc_cycles, asyncio_websockets, pycparser, xml_etree_iterparse, bench_mp_pool, xml_etree_parse
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.98x