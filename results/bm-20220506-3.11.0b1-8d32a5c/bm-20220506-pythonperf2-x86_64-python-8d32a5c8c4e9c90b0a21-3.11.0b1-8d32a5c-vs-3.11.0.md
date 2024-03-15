
# Results vs. 3.11.0

- fork: python
- ref: 8d32a5c8c4e9c90b0a21
- machine: linux-x86_64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.67%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 281 ms: 1.02x faster                                                        |
| chameleon      | 7.92 ms                                                      | 7.53 ms: 1.05x faster                                                       |
| docutils       | 2.85 sec                                                     | 2.82 sec: 1.01x faster                                                      |
| html5lib       | 72.2 ms                                                      | 69.0 ms: 1.05x faster                                                       |
| tornado_http   | 124 ms                                                       | 121 ms: 1.03x faster                                                        |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 753 ms                                                       | 748 ms: 1.01x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.00x faster                                                                |

Benchmark hidden because not significant (3): async_tree_memoization, async_tree_none, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 100 ms: 1.08x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                |

Benchmark hidden because not significant (2): float, pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 2.97 ms: 1.13x faster                                                       |
| regex_v8       | 24.4 ms                                                      | 22.8 ms: 1.07x faster                                                       |
| regex_compile  | 156 ms                                                       | 153 ms: 1.02x faster                                                        |
| regex_dna      | 227 ms                                                       | 232 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads           | 28.9 us                                                      | 24.6 us: 1.18x faster                                                       |
| pickle_dict          | 32.3 us                                                      | 29.9 us: 1.08x faster                                                       |
| pickle_list          | 3.94 us                                                      | 3.81 us: 1.03x faster                                                       |
| pickle               | 9.89 us                                                      | 9.62 us: 1.03x faster                                                       |
| unpickle_pure_python | 238 us                                                       | 233 us: 1.02x faster                                                        |
| xml_etree_iterparse  | 107 ms                                                       | 105 ms: 1.02x faster                                                        |
| unpickle_list        | 4.60 us                                                      | 4.56 us: 1.01x faster                                                       |
| xml_etree_process    | 55.9 ms                                                      | 56.1 ms: 1.00x slower                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 80.3 ms: 1.01x slower                                                       |
| pickle_pure_python   | 316 us                                                       | 320 us: 1.01x slower                                                        |
| json_dumps           | 13.3 ms                                                      | 13.5 ms: 1.02x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                                |

Benchmark hidden because not significant (2): unpickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.5 ms: 1.02x faster                                                       |
| python_startup_no_site | 7.73 ms                                                      | 7.68 ms: 1.01x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| django_template | 39.3 ms                                                      | 41.3 ms: 1.05x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.01x slower                                                                |

Benchmark hidden because not significant (3): mako, genshi_xml, genshi_text

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads              | 28.9 us                                                      | 24.6 us: 1.18x faster                                                       |
| regex_effbot            | 3.34 ms                                                      | 2.97 ms: 1.13x faster                                                       |
| json                    | 5.58 ms                                                      | 5.14 ms: 1.09x faster                                                       |
| pickle_dict             | 32.3 us                                                      | 29.9 us: 1.08x faster                                                       |
| gc_traversal            | 4.15 ms                                                      | 3.85 ms: 1.08x faster                                                       |
| regex_v8                | 24.4 ms                                                      | 22.8 ms: 1.07x faster                                                       |
| nqueens                 | 103 ms                                                       | 95.8 ms: 1.07x faster                                                       |
| pprint_safe_repr        | 805 ms                                                       | 755 ms: 1.07x faster                                                        |
| pprint_pformat          | 1.67 sec                                                     | 1.57 sec: 1.06x faster                                                      |
| chameleon               | 7.92 ms                                                      | 7.53 ms: 1.05x faster                                                       |
| logging_simple          | 7.24 us                                                      | 6.90 us: 1.05x faster                                                       |
| html5lib                | 72.2 ms                                                      | 69.0 ms: 1.05x faster                                                       |
| aiohttp                 | 986 us                                                       | 945 us: 1.04x faster                                                        |
| gunicorn                | 966 us                                                       | 928 us: 1.04x faster                                                        |
| sympy_sum               | 186 ms                                                       | 178 ms: 1.04x faster                                                        |
| pycparser               | 1.31 sec                                                     | 1.26 sec: 1.04x faster                                                      |
| pyflate                 | 449 ms                                                       | 433 ms: 1.04x faster                                                        |
| chaos                   | 74.9 ms                                                      | 72.4 ms: 1.03x faster                                                       |
| pickle_list             | 3.94 us                                                      | 3.81 us: 1.03x faster                                                       |
| bench_mp_pool           | 4.70 ms                                                      | 4.56 ms: 1.03x faster                                                       |
| pickle                  | 9.89 us                                                      | 9.62 us: 1.03x faster                                                       |
| tornado_http            | 124 ms                                                       | 121 ms: 1.03x faster                                                        |
| sympy_integrate         | 25.8 ms                                                      | 25.2 ms: 1.03x faster                                                       |
| sympy_expand            | 553 ms                                                       | 540 ms: 1.02x faster                                                        |
| sqlglot_normalize       | 122 ms                                                       | 119 ms: 1.02x faster                                                        |
| sympy_str               | 337 ms                                                       | 329 ms: 1.02x faster                                                        |
| unpickle_pure_python    | 238 us                                                       | 233 us: 1.02x faster                                                        |
| regex_compile           | 156 ms                                                       | 153 ms: 1.02x faster                                                        |
| spectral_norm           | 95.1 ms                                                      | 93.1 ms: 1.02x faster                                                       |
| thrift                  | 931 us                                                       | 913 us: 1.02x faster                                                        |
| xml_etree_iterparse     | 107 ms                                                       | 105 ms: 1.02x faster                                                        |
| 2to3                    | 287 ms                                                       | 281 ms: 1.02x faster                                                        |
| python_startup          | 10.7 ms                                                      | 10.5 ms: 1.02x faster                                                       |
| pylint                  | 514 ms                                                       | 505 ms: 1.02x faster                                                        |
| flaskblogging           | 3.88 ms                                                      | 3.82 ms: 1.02x faster                                                       |
| sqlalchemy_imperative   | 19.8 ms                                                      | 19.5 ms: 1.01x faster                                                       |
| crypto_pyaes            | 83.3 ms                                                      | 82.3 ms: 1.01x faster                                                       |
| async_generators        | 322 ms                                                       | 318 ms: 1.01x faster                                                        |
| hexiom                  | 6.98 ms                                                      | 6.91 ms: 1.01x faster                                                       |
| deltablue               | 3.97 ms                                                      | 3.93 ms: 1.01x faster                                                       |
| scimark_monte_carlo     | 69.8 ms                                                      | 69.2 ms: 1.01x faster                                                       |
| go                      | 158 ms                                                       | 156 ms: 1.01x faster                                                        |
| docutils                | 2.85 sec                                                     | 2.82 sec: 1.01x faster                                                      |
| unpickle_list           | 4.60 us                                                      | 4.56 us: 1.01x faster                                                       |
| python_startup_no_site  | 7.73 ms                                                      | 7.68 ms: 1.01x faster                                                       |
| pathlib                 | 18.9 ms                                                      | 18.8 ms: 1.01x faster                                                       |
| async_tree_cpu_io_mixed | 753 ms                                                       | 748 ms: 1.01x faster                                                        |
| asyncio_tcp             | 747 ms                                                       | 749 ms: 1.00x slower                                                        |
| mdp                     | 2.77 sec                                                     | 2.78 sec: 1.00x slower                                                      |
| xml_etree_process       | 55.9 ms                                                      | 56.1 ms: 1.00x slower                                                       |
| meteor_contest          | 131 ms                                                       | 131 ms: 1.01x slower                                                        |
| deepcopy                | 391 us                                                       | 394 us: 1.01x slower                                                        |
| xml_etree_generate      | 79.7 ms                                                      | 80.3 ms: 1.01x slower                                                       |
| dulwich_log             | 67.4 ms                                                      | 68.0 ms: 1.01x slower                                                       |
| coroutines              | 27.8 ms                                                      | 28.0 ms: 1.01x slower                                                       |
| richards                | 49.7 ms                                                      | 50.1 ms: 1.01x slower                                                       |
| pickle_pure_python      | 316 us                                                       | 320 us: 1.01x slower                                                        |
| generators              | 54.6 ms                                                      | 55.5 ms: 1.02x slower                                                       |
| regex_dna               | 227 ms                                                       | 232 ms: 1.02x slower                                                        |
| json_dumps              | 13.3 ms                                                      | 13.5 ms: 1.02x slower                                                       |
| bench_thread_pool       | 1.00 ms                                                      | 1.02 ms: 1.02x slower                                                       |
| dask                    | 410 ms                                                       | 418 ms: 1.02x slower                                                        |
| telco                   | 6.81 ms                                                      | 6.99 ms: 1.03x slower                                                       |
| create_gc_cycles        | 1.58 ms                                                      | 1.64 ms: 1.04x slower                                                       |
| scimark_fft             | 281 ms                                                       | 294 ms: 1.05x slower                                                        |
| django_template         | 39.3 ms                                                      | 41.3 ms: 1.05x slower                                                       |
| nbody                   | 92.9 ms                                                      | 100 ms: 1.08x slower                                                        |
| comprehensions          | 25.1 us                                                      | 28.2 us: 1.12x slower                                                       |
| sqlglot_transpile       | 1.91 ms                                                      | 2.30 ms: 1.21x slower                                                       |
| sqlglot_parse           | 1.51 ms                                                      | 1.95 ms: 1.29x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.01x faster                                                                |

Benchmark hidden because not significant (23): mako, async_tree_memoization, sqlalchemy_declarative, genshi_xml, logging_format, logging_silent, async_tree_none, sqlite_synth, genshi_text, float, async_tree_io, raytrace, scimark_sparse_mat_mult, sqlglot_optimize, scimark_lu, unpickle, pidigits, deepcopy_memo, scimark_sor, xml_etree_parse, fannkuch, deepcopy_reduce, unpack_sequence
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 99.67% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x