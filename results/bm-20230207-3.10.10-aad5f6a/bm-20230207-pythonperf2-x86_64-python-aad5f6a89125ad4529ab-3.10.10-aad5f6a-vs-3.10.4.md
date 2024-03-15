
# Results vs. 3.10.4

- fork: python
- ref: aad5f6a89125ad4529ab
- machine: linux-x86_64
- commit hash: aad5f6a
- commit date: 2023-02-07
- overall geometric mean: 1.01x slower \*
- HPT reliability: 99.49%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| chameleon      | 9.44 ms                                                      | 9.41 ms: 1.00x faster                                                      |
| docutils       | 3.41 sec                                                     | 3.45 sec: 1.01x slower                                                     |
| tornado_http   | 157 ms                                                       | 159 ms: 1.01x slower                                                       |
| Geometric mean | (ref)                                                        | 1.00x slower                                                               |

Benchmark hidden because not significant (2): 2to3, html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.62 sec: 1.02x slower                                                     |
| async_tree_memoization  | 819 ms                                                       | 832 ms: 1.02x slower                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 955 ms: 1.02x slower                                                       |
| async_tree_none         | 692 ms                                                       | 711 ms: 1.03x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.02x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 134 ms                                                       | 138 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (2): float, pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_dna      | 261 ms                                                       | 260 ms: 1.01x faster                                                       |
| regex_v8       | 27.2 ms                                                      | 27.2 ms: 1.00x slower                                                      |
| regex_compile  | 190 ms                                                       | 192 ms: 1.01x slower                                                       |
| regex_effbot   | 3.09 ms                                                      | 3.49 ms: 1.13x slower                                                      |
| Geometric mean | (ref)                                                        | 1.03x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_loads           | 30.3 us                                                      | 30.0 us: 1.01x faster                                                      |
| json_dumps           | 14.5 ms                                                      | 14.4 ms: 1.01x faster                                                      |
| pickle_list          | 4.12 us                                                      | 4.17 us: 1.01x slower                                                      |
| pickle_pure_python   | 455 us                                                       | 461 us: 1.01x slower                                                       |
| unpickle_list        | 4.65 us                                                      | 4.71 us: 1.01x slower                                                      |
| unpickle             | 13.5 us                                                      | 13.7 us: 1.01x slower                                                      |
| xml_etree_generate   | 92.3 ms                                                      | 94.0 ms: 1.02x slower                                                      |
| xml_etree_process    | 75.9 ms                                                      | 77.5 ms: 1.02x slower                                                      |
| xml_etree_parse      | 160 ms                                                       | 164 ms: 1.02x slower                                                       |
| xml_etree_iterparse  | 110 ms                                                       | 113 ms: 1.02x slower                                                       |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                      |
| unpickle_pure_python | 312 us                                                       | 320 us: 1.03x slower                                                       |
| pickle_dict          | 29.5 us                                                      | 32.1 us: 1.09x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 7.33 ms                                                      | 7.34 ms: 1.00x slower                                                      |
| python_startup         | 11.5 ms                                                      | 11.5 ms: 1.00x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.00x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_xml      | 63.3 ms                                                      | 62.5 ms: 1.01x faster                                                      |
| genshi_text     | 31.4 ms                                                      | 32.0 ms: 1.02x slower                                                      |
| django_template | 50.2 ms                                                      | 53.6 ms: 1.07x slower                                                      |
| Geometric mean  | (ref)                                                        | 1.02x slower                                                               |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pyflate                 | 733 ms                                                       | 696 ms: 1.05x faster                                                       |
| aiohttp                 | 1.19 ms                                                      | 1.15 ms: 1.04x faster                                                      |
| bench_thread_pool       | 1.14 ms                                                      | 1.11 ms: 1.03x faster                                                      |
| richards                | 75.1 ms                                                      | 72.9 ms: 1.03x faster                                                      |
| gunicorn                | 1.16 ms                                                      | 1.13 ms: 1.03x faster                                                      |
| fannkuch                | 483 ms                                                       | 470 ms: 1.03x faster                                                       |
| pprint_pformat          | 2.15 sec                                                     | 2.11 sec: 1.02x faster                                                     |
| pprint_safe_repr        | 1.05 sec                                                     | 1.03 sec: 1.02x faster                                                     |
| nqueens                 | 115 ms                                                       | 113 ms: 1.02x faster                                                       |
| scimark_sor             | 180 ms                                                       | 177 ms: 1.02x faster                                                       |
| coroutines              | 30.3 ms                                                      | 29.9 ms: 1.01x faster                                                      |
| genshi_xml              | 63.3 ms                                                      | 62.5 ms: 1.01x faster                                                      |
| sqlalchemy_declarative  | 190 ms                                                       | 187 ms: 1.01x faster                                                       |
| json_loads              | 30.3 us                                                      | 30.0 us: 1.01x faster                                                      |
| unpack_sequence         | 59.9 ns                                                      | 59.3 ns: 1.01x faster                                                      |
| logging_silent          | 167 ns                                                       | 165 ns: 1.01x faster                                                       |
| spectral_norm           | 139 ms                                                       | 138 ms: 1.01x faster                                                       |
| async_generators        | 421 ms                                                       | 417 ms: 1.01x faster                                                       |
| crypto_pyaes            | 119 ms                                                       | 118 ms: 1.01x faster                                                       |
| sqlglot_optimize        | 70.1 ms                                                      | 69.6 ms: 1.01x faster                                                      |
| json_dumps              | 14.5 ms                                                      | 14.4 ms: 1.01x faster                                                      |
| deltablue               | 7.50 ms                                                      | 7.45 ms: 1.01x faster                                                      |
| go                      | 262 ms                                                       | 260 ms: 1.01x faster                                                       |
| regex_dna               | 261 ms                                                       | 260 ms: 1.01x faster                                                       |
| generators              | 57.3 ms                                                      | 57.0 ms: 1.01x faster                                                      |
| chameleon               | 9.44 ms                                                      | 9.41 ms: 1.00x faster                                                      |
| regex_v8                | 27.2 ms                                                      | 27.2 ms: 1.00x slower                                                      |
| python_startup_no_site  | 7.33 ms                                                      | 7.34 ms: 1.00x slower                                                      |
| python_startup          | 11.5 ms                                                      | 11.5 ms: 1.00x slower                                                      |
| deepcopy_memo           | 49.8 us                                                      | 50.0 us: 1.00x slower                                                      |
| meteor_contest          | 138 ms                                                       | 139 ms: 1.00x slower                                                       |
| json                    | 5.86 ms                                                      | 5.91 ms: 1.01x slower                                                      |
| hexiom                  | 9.42 ms                                                      | 9.49 ms: 1.01x slower                                                      |
| sqlglot_transpile       | 2.68 ms                                                      | 2.70 ms: 1.01x slower                                                      |
| sqlalchemy_imperative   | 22.7 ms                                                      | 22.9 ms: 1.01x slower                                                      |
| sympy_str               | 360 ms                                                       | 364 ms: 1.01x slower                                                       |
| logging_simple          | 8.88 us                                                      | 8.96 us: 1.01x slower                                                      |
| docutils                | 3.41 sec                                                     | 3.45 sec: 1.01x slower                                                     |
| pylint                  | 566 ms                                                       | 572 ms: 1.01x slower                                                       |
| deepcopy_reduce         | 4.01 us                                                      | 4.05 us: 1.01x slower                                                      |
| sympy_integrate         | 28.2 ms                                                      | 28.5 ms: 1.01x slower                                                      |
| regex_compile           | 190 ms                                                       | 192 ms: 1.01x slower                                                       |
| pickle_list             | 4.12 us                                                      | 4.17 us: 1.01x slower                                                      |
| sqlglot_normalize       | 144 ms                                                       | 146 ms: 1.01x slower                                                       |
| comprehensions          | 26.7 us                                                      | 27.0 us: 1.01x slower                                                      |
| raytrace                | 489 ms                                                       | 495 ms: 1.01x slower                                                       |
| sympy_expand            | 600 ms                                                       | 608 ms: 1.01x slower                                                       |
| pickle_pure_python      | 455 us                                                       | 461 us: 1.01x slower                                                       |
| unpickle_list           | 4.65 us                                                      | 4.71 us: 1.01x slower                                                      |
| tornado_http            | 157 ms                                                       | 159 ms: 1.01x slower                                                       |
| unpickle                | 13.5 us                                                      | 13.7 us: 1.01x slower                                                      |
| mdp                     | 3.01 sec                                                     | 3.05 sec: 1.02x slower                                                     |
| async_tree_io           | 1.60 sec                                                     | 1.62 sec: 1.02x slower                                                     |
| async_tree_memoization  | 819 ms                                                       | 832 ms: 1.02x slower                                                       |
| genshi_text             | 31.4 ms                                                      | 32.0 ms: 1.02x slower                                                      |
| xml_etree_generate      | 92.3 ms                                                      | 94.0 ms: 1.02x slower                                                      |
| scimark_lu              | 167 ms                                                       | 170 ms: 1.02x slower                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 955 ms: 1.02x slower                                                       |
| xml_etree_process       | 75.9 ms                                                      | 77.5 ms: 1.02x slower                                                      |
| xml_etree_parse         | 160 ms                                                       | 164 ms: 1.02x slower                                                       |
| scimark_monte_carlo     | 107 ms                                                       | 110 ms: 1.02x slower                                                       |
| xml_etree_iterparse     | 110 ms                                                       | 113 ms: 1.02x slower                                                       |
| pickle                  | 9.89 us                                                      | 10.1 us: 1.02x slower                                                      |
| unpickle_pure_python    | 312 us                                                       | 320 us: 1.03x slower                                                       |
| dask                    | 472 ms                                                       | 484 ms: 1.03x slower                                                       |
| nbody                   | 134 ms                                                       | 138 ms: 1.03x slower                                                       |
| async_tree_none         | 692 ms                                                       | 711 ms: 1.03x slower                                                       |
| thrift                  | 1.18 ms                                                      | 1.21 ms: 1.03x slower                                                      |
| create_gc_cycles        | 1.76 ms                                                      | 1.81 ms: 1.03x slower                                                      |
| sympy_sum               | 193 ms                                                       | 199 ms: 1.03x slower                                                       |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 5.28 ms: 1.04x slower                                                      |
| scimark_fft             | 361 ms                                                       | 383 ms: 1.06x slower                                                       |
| django_template         | 50.2 ms                                                      | 53.6 ms: 1.07x slower                                                      |
| pickle_dict             | 29.5 us                                                      | 32.1 us: 1.09x slower                                                      |
| regex_effbot            | 3.09 ms                                                      | 3.49 ms: 1.13x slower                                                      |
| bench_mp_pool           | 6.37 ms                                                      | 7.26 ms: 1.14x slower                                                      |
| gc_traversal            | 3.42 ms                                                      | 4.12 ms: 1.21x slower                                                      |
| Geometric mean          | (ref)                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (17): deepcopy, pycparser, sqlite_synth, html5lib, float, mako, pathlib, dulwich_log, asyncio_tcp, coverage, pidigits, 2to3, flaskblogging, telco, chaos, logging_format, sqlglot_parse
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 99.49% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.02x