
# Results vs. 3.11.0

- fork: python
- ref: ed7c3ff15680c1939fad
- machine: linux-x86_64
- commit hash: ed7c3ff
- commit date: 2022-09-11
- overall geometric mean: 1.00x slower \*
- HPT reliability: 96.75%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| chameleon      | 7.92 ms                                                      | 7.50 ms: 1.06x faster                                                        |
| docutils       | 2.85 sec                                                     | 2.86 sec: 1.00x slower                                                       |
| html5lib       | 72.2 ms                                                      | 73.2 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                 |

Benchmark hidden because not significant (2): 2to3, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 753 ms                                                       | 746 ms: 1.01x faster                                                         |
| async_tree_memoization  | 629 ms                                                       | 636 ms: 1.01x slower                                                         |
| Geometric mean          | (ref)                                                        | 1.00x slower                                                                 |

Benchmark hidden because not significant (2): async_tree_none, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 89.6 ms: 1.04x faster                                                        |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                 |

Benchmark hidden because not significant (2): pidigits, float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.29 ms: 1.01x faster                                                        |
| regex_dna      | 227 ms                                                       | 225 ms: 1.01x faster                                                         |
| regex_v8       | 24.4 ms                                                      | 24.3 ms: 1.00x faster                                                        |
| regex_compile  | 156 ms                                                       | 157 ms: 1.01x slower                                                         |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.3 us                                                      | 30.7 us: 1.05x faster                                                        |
| pickle_list          | 3.94 us                                                      | 3.77 us: 1.05x faster                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 104 ms: 1.03x faster                                                         |
| pickle               | 9.89 us                                                      | 9.61 us: 1.03x faster                                                        |
| unpickle             | 13.3 us                                                      | 13.0 us: 1.02x faster                                                        |
| json_loads           | 28.9 us                                                      | 28.4 us: 1.02x faster                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 80.8 ms: 1.01x slower                                                        |
| json_dumps           | 13.3 ms                                                      | 13.5 ms: 1.02x slower                                                        |
| xml_etree_process    | 55.9 ms                                                      | 57.0 ms: 1.02x slower                                                        |
| pickle_pure_python   | 316 us                                                       | 324 us: 1.03x slower                                                         |
| unpickle_list        | 4.60 us                                                      | 4.72 us: 1.03x slower                                                        |
| xml_etree_parse      | 155 ms                                                       | 160 ms: 1.04x slower                                                         |
| unpickle_pure_python | 238 us                                                       | 250 us: 1.05x slower                                                         |
| Geometric mean       | (ref)                                                        | 1.00x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.7 ms: 1.00x faster                                                        |
| python_startup_no_site | 7.73 ms                                                      | 7.72 ms: 1.00x faster                                                        |
| Geometric mean         | (ref)                                                        | 1.00x faster                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| django_template | 39.3 ms                                                      | 39.7 ms: 1.01x slower                                                        |
| genshi_text     | 25.5 ms                                                      | 26.1 ms: 1.02x slower                                                        |
| genshi_xml      | 57.1 ms                                                      | 59.2 ms: 1.04x slower                                                        |
| Geometric mean  | (ref)                                                        | 1.01x slower                                                                 |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf2-x86_64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| gc_traversal            | 4.15 ms                                                      | 3.63 ms: 1.14x faster                                                        |
| chameleon               | 7.92 ms                                                      | 7.50 ms: 1.06x faster                                                        |
| pickle_dict             | 32.3 us                                                      | 30.7 us: 1.05x faster                                                        |
| pickle_list             | 3.94 us                                                      | 3.77 us: 1.05x faster                                                        |
| nbody                   | 92.9 ms                                                      | 89.6 ms: 1.04x faster                                                        |
| bench_mp_pool           | 4.70 ms                                                      | 4.54 ms: 1.04x faster                                                        |
| xml_etree_iterparse     | 107 ms                                                       | 104 ms: 1.03x faster                                                         |
| pickle                  | 9.89 us                                                      | 9.61 us: 1.03x faster                                                        |
| thrift                  | 931 us                                                       | 906 us: 1.03x faster                                                         |
| gunicorn                | 966 us                                                       | 941 us: 1.03x faster                                                         |
| flaskblogging           | 3.88 ms                                                      | 3.80 ms: 1.02x faster                                                        |
| mdp                     | 2.77 sec                                                     | 2.72 sec: 1.02x faster                                                       |
| aiohttp                 | 986 us                                                       | 966 us: 1.02x faster                                                         |
| unpickle                | 13.3 us                                                      | 13.0 us: 1.02x faster                                                        |
| json_loads              | 28.9 us                                                      | 28.4 us: 1.02x faster                                                        |
| pprint_safe_repr        | 805 ms                                                       | 791 ms: 1.02x faster                                                         |
| scimark_monte_carlo     | 69.8 ms                                                      | 68.7 ms: 1.02x faster                                                        |
| sqlite_synth            | 2.52 us                                                      | 2.48 us: 1.02x faster                                                        |
| regex_effbot            | 3.34 ms                                                      | 3.29 ms: 1.01x faster                                                        |
| nqueens                 | 103 ms                                                       | 101 ms: 1.01x faster                                                         |
| sympy_sum               | 186 ms                                                       | 183 ms: 1.01x faster                                                         |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 4.01 ms: 1.01x faster                                                        |
| pprint_pformat          | 1.67 sec                                                     | 1.65 sec: 1.01x faster                                                       |
| regex_dna               | 227 ms                                                       | 225 ms: 1.01x faster                                                         |
| scimark_fft             | 281 ms                                                       | 277 ms: 1.01x faster                                                         |
| async_tree_cpu_io_mixed | 753 ms                                                       | 746 ms: 1.01x faster                                                         |
| generators              | 54.6 ms                                                      | 54.2 ms: 1.01x faster                                                        |
| raytrace                | 309 ms                                                       | 307 ms: 1.01x faster                                                         |
| regex_v8                | 24.4 ms                                                      | 24.3 ms: 1.00x faster                                                        |
| sqlglot_normalize       | 122 ms                                                       | 121 ms: 1.00x faster                                                         |
| python_startup          | 10.7 ms                                                      | 10.7 ms: 1.00x faster                                                        |
| python_startup_no_site  | 7.73 ms                                                      | 7.72 ms: 1.00x faster                                                        |
| docutils                | 2.85 sec                                                     | 2.86 sec: 1.00x slower                                                       |
| coroutines              | 27.8 ms                                                      | 27.9 ms: 1.00x slower                                                        |
| spectral_norm           | 95.1 ms                                                      | 95.5 ms: 1.00x slower                                                        |
| sympy_integrate         | 25.8 ms                                                      | 25.9 ms: 1.00x slower                                                        |
| asyncio_tcp             | 747 ms                                                       | 752 ms: 1.01x slower                                                         |
| sqlalchemy_imperative   | 19.8 ms                                                      | 19.9 ms: 1.01x slower                                                        |
| regex_compile           | 156 ms                                                       | 157 ms: 1.01x slower                                                         |
| django_template         | 39.3 ms                                                      | 39.7 ms: 1.01x slower                                                        |
| pathlib                 | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                        |
| async_tree_memoization  | 629 ms                                                       | 636 ms: 1.01x slower                                                         |
| crypto_pyaes            | 83.3 ms                                                      | 84.3 ms: 1.01x slower                                                        |
| html5lib                | 72.2 ms                                                      | 73.2 ms: 1.01x slower                                                        |
| meteor_contest          | 131 ms                                                       | 132 ms: 1.01x slower                                                         |
| xml_etree_generate      | 79.7 ms                                                      | 80.8 ms: 1.01x slower                                                        |
| json_dumps              | 13.3 ms                                                      | 13.5 ms: 1.02x slower                                                        |
| comprehensions          | 25.1 us                                                      | 25.5 us: 1.02x slower                                                        |
| async_generators        | 322 ms                                                       | 328 ms: 1.02x slower                                                         |
| hexiom                  | 6.98 ms                                                      | 7.12 ms: 1.02x slower                                                        |
| xml_etree_process       | 55.9 ms                                                      | 57.0 ms: 1.02x slower                                                        |
| pycparser               | 1.31 sec                                                     | 1.34 sec: 1.02x slower                                                       |
| genshi_text             | 25.5 ms                                                      | 26.1 ms: 1.02x slower                                                        |
| dask                    | 410 ms                                                       | 420 ms: 1.02x slower                                                         |
| pickle_pure_python      | 316 us                                                       | 324 us: 1.03x slower                                                         |
| unpickle_list           | 4.60 us                                                      | 4.72 us: 1.03x slower                                                        |
| logging_simple          | 7.24 us                                                      | 7.43 us: 1.03x slower                                                        |
| deltablue               | 3.97 ms                                                      | 4.09 ms: 1.03x slower                                                        |
| dulwich_log             | 67.4 ms                                                      | 69.6 ms: 1.03x slower                                                        |
| sqlglot_parse           | 1.51 ms                                                      | 1.56 ms: 1.03x slower                                                        |
| deepcopy_reduce         | 3.40 us                                                      | 3.51 us: 1.03x slower                                                        |
| xml_etree_parse         | 155 ms                                                       | 160 ms: 1.04x slower                                                         |
| genshi_xml              | 57.1 ms                                                      | 59.2 ms: 1.04x slower                                                        |
| logging_format          | 7.71 us                                                      | 8.03 us: 1.04x slower                                                        |
| deepcopy                | 391 us                                                       | 407 us: 1.04x slower                                                         |
| unpickle_pure_python    | 238 us                                                       | 250 us: 1.05x slower                                                         |
| create_gc_cycles        | 1.58 ms                                                      | 1.66 ms: 1.05x slower                                                        |
| fannkuch                | 416 ms                                                       | 441 ms: 1.06x slower                                                         |
| richards                | 49.7 ms                                                      | 53.5 ms: 1.08x slower                                                        |
| chaos                   | 74.9 ms                                                      | 81.4 ms: 1.09x slower                                                        |
| go                      | 158 ms                                                       | 172 ms: 1.09x slower                                                         |
| deepcopy_memo           | 37.5 us                                                      | 41.0 us: 1.09x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.00x slower                                                                 |

Benchmark hidden because not significant (21): mako, sqlglot_optimize, async_tree_none, json, scimark_lu, sympy_expand, pidigits, unpack_sequence, pyflate, sympy_str, scimark_sor, 2to3, float, async_tree_io, bench_thread_pool, sqlglot_transpile, sqlalchemy_declarative, logging_silent, tornado_http, telco, pylint
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 96.75% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.02x