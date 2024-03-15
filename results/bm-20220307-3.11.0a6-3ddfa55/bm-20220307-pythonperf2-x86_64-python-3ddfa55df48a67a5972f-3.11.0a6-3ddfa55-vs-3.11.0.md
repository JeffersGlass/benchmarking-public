
# Results vs. 3.11.0

- fork: python
- ref: 3ddfa55df48a67a5972f
- machine: linux-x86_64
- commit hash: 3ddfa55
- commit date: 2022-03-07
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x slower
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 300 ms: 1.05x slower                                                        |
| chameleon      | 7.92 ms                                                      | 8.43 ms: 1.06x slower                                                       |
| docutils       | 2.85 sec                                                     | 2.98 sec: 1.05x slower                                                      |
| html5lib       | 72.2 ms                                                      | 75.6 ms: 1.05x slower                                                       |
| tornado_http   | 124 ms                                                       | 130 ms: 1.05x slower                                                        |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 753 ms                                                       | 763 ms: 1.01x slower                                                        |
| async_tree_io           | 1.17 sec                                                     | 1.19 sec: 1.02x slower                                                      |
| async_tree_none         | 518 ms                                                       | 532 ms: 1.03x slower                                                        |
| async_tree_memoization  | 629 ms                                                       | 651 ms: 1.03x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.02x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 253 ms: 1.01x slower                                                        |
| nbody          | 92.9 ms                                                      | 98.0 ms: 1.06x slower                                                       |
| float          | 74.9 ms                                                      | 79.1 ms: 1.06x slower                                                       |
| Geometric mean | (ref)                                                        | 1.04x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 161 ms: 1.03x slower                                                        |
| regex_effbot   | 3.34 ms                                                      | 3.49 ms: 1.05x slower                                                       |
| regex_v8       | 24.4 ms                                                      | 26.4 ms: 1.08x slower                                                       |
| regex_dna      | 227 ms                                                       | 257 ms: 1.13x slower                                                        |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads           | 28.9 us                                                      | 23.9 us: 1.21x faster                                                       |
| xml_etree_iterparse  | 107 ms                                                       | 104 ms: 1.02x faster                                                        |
| pickle               | 9.89 us                                                      | 9.96 us: 1.01x slower                                                       |
| unpickle_list        | 4.60 us                                                      | 4.68 us: 1.02x slower                                                       |
| unpickle             | 13.3 us                                                      | 13.5 us: 1.02x slower                                                       |
| json_dumps           | 13.3 ms                                                      | 13.6 ms: 1.03x slower                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 83.5 ms: 1.05x slower                                                       |
| xml_etree_process    | 55.9 ms                                                      | 59.4 ms: 1.06x slower                                                       |
| pickle_list          | 3.94 us                                                      | 4.28 us: 1.09x slower                                                       |
| pickle_pure_python   | 316 us                                                       | 352 us: 1.11x slower                                                        |
| unpickle_pure_python | 238 us                                                       | 273 us: 1.14x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                                |

Benchmark hidden because not significant (2): xml_etree_parse, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.4 ms: 1.03x faster                                                       |
| python_startup_no_site | 7.73 ms                                                      | 7.55 ms: 1.02x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.03x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 11.4 ms: 1.04x slower                                                       |
| genshi_text     | 25.5 ms                                                      | 26.5 ms: 1.04x slower                                                       |
| genshi_xml      | 57.1 ms                                                      | 60.7 ms: 1.06x slower                                                       |
| django_template | 39.3 ms                                                      | 43.8 ms: 1.11x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.06x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads              | 28.9 us                                                      | 23.9 us: 1.21x faster                                                       |
| json                    | 5.58 ms                                                      | 5.04 ms: 1.11x faster                                                       |
| python_startup          | 10.7 ms                                                      | 10.4 ms: 1.03x faster                                                       |
| gc_traversal            | 4.15 ms                                                      | 4.03 ms: 1.03x faster                                                       |
| python_startup_no_site  | 7.73 ms                                                      | 7.55 ms: 1.02x faster                                                       |
| logging_simple          | 7.24 us                                                      | 7.08 us: 1.02x faster                                                       |
| xml_etree_iterparse     | 107 ms                                                       | 104 ms: 1.02x faster                                                        |
| nqueens                 | 103 ms                                                       | 100 ms: 1.02x faster                                                        |
| sympy_sum               | 186 ms                                                       | 184 ms: 1.01x faster                                                        |
| async_generators        | 322 ms                                                       | 320 ms: 1.00x faster                                                        |
| sympy_integrate         | 25.8 ms                                                      | 25.9 ms: 1.01x slower                                                       |
| pidigits                | 251 ms                                                       | 253 ms: 1.01x slower                                                        |
| pickle                  | 9.89 us                                                      | 9.96 us: 1.01x slower                                                       |
| telco                   | 6.81 ms                                                      | 6.90 ms: 1.01x slower                                                       |
| async_tree_cpu_io_mixed | 753 ms                                                       | 763 ms: 1.01x slower                                                        |
| asyncio_tcp             | 747 ms                                                       | 757 ms: 1.01x slower                                                        |
| async_tree_io           | 1.17 sec                                                     | 1.19 sec: 1.02x slower                                                      |
| meteor_contest          | 131 ms                                                       | 133 ms: 1.02x slower                                                        |
| unpickle_list           | 4.60 us                                                      | 4.68 us: 1.02x slower                                                       |
| aiohttp                 | 986 us                                                       | 1.00 ms: 1.02x slower                                                       |
| unpickle                | 13.3 us                                                      | 13.5 us: 1.02x slower                                                       |
| sympy_str               | 337 ms                                                       | 343 ms: 1.02x slower                                                        |
| pathlib                 | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                       |
| async_tree_none         | 518 ms                                                       | 532 ms: 1.03x slower                                                        |
| json_dumps              | 13.3 ms                                                      | 13.6 ms: 1.03x slower                                                       |
| flaskblogging           | 3.88 ms                                                      | 3.99 ms: 1.03x slower                                                       |
| gunicorn                | 966 us                                                       | 994 us: 1.03x slower                                                        |
| regex_compile           | 156 ms                                                       | 161 ms: 1.03x slower                                                        |
| create_gc_cycles        | 1.58 ms                                                      | 1.63 ms: 1.03x slower                                                       |
| chaos                   | 74.9 ms                                                      | 77.5 ms: 1.03x slower                                                       |
| async_tree_memoization  | 629 ms                                                       | 651 ms: 1.03x slower                                                        |
| sympy_expand            | 553 ms                                                       | 573 ms: 1.04x slower                                                        |
| mako                    | 11.0 ms                                                      | 11.4 ms: 1.04x slower                                                       |
| genshi_text             | 25.5 ms                                                      | 26.5 ms: 1.04x slower                                                       |
| bench_thread_pool       | 1.00 ms                                                      | 1.04 ms: 1.04x slower                                                       |
| tornado_http            | 124 ms                                                       | 130 ms: 1.05x slower                                                        |
| regex_effbot            | 3.34 ms                                                      | 3.49 ms: 1.05x slower                                                       |
| html5lib                | 72.2 ms                                                      | 75.6 ms: 1.05x slower                                                       |
| 2to3                    | 287 ms                                                       | 300 ms: 1.05x slower                                                        |
| xml_etree_generate      | 79.7 ms                                                      | 83.5 ms: 1.05x slower                                                       |
| docutils                | 2.85 sec                                                     | 2.98 sec: 1.05x slower                                                      |
| mdp                     | 2.77 sec                                                     | 2.91 sec: 1.05x slower                                                      |
| nbody                   | 92.9 ms                                                      | 98.0 ms: 1.06x slower                                                       |
| deepcopy                | 391 us                                                       | 413 us: 1.06x slower                                                        |
| float                   | 74.9 ms                                                      | 79.1 ms: 1.06x slower                                                       |
| sqlalchemy_declarative  | 154 ms                                                       | 164 ms: 1.06x slower                                                        |
| pprint_safe_repr        | 805 ms                                                       | 853 ms: 1.06x slower                                                        |
| sqlalchemy_imperative   | 19.8 ms                                                      | 21.0 ms: 1.06x slower                                                       |
| xml_etree_process       | 55.9 ms                                                      | 59.4 ms: 1.06x slower                                                       |
| genshi_xml              | 57.1 ms                                                      | 60.7 ms: 1.06x slower                                                       |
| chameleon               | 7.92 ms                                                      | 8.43 ms: 1.06x slower                                                       |
| pprint_pformat          | 1.67 sec                                                     | 1.77 sec: 1.06x slower                                                      |
| thrift                  | 931 us                                                       | 991 us: 1.06x slower                                                        |
| scimark_monte_carlo     | 69.8 ms                                                      | 74.4 ms: 1.07x slower                                                       |
| scimark_lu              | 114 ms                                                       | 122 ms: 1.07x slower                                                        |
| sqlglot_normalize       | 122 ms                                                       | 131 ms: 1.08x slower                                                        |
| dask                    | 410 ms                                                       | 442 ms: 1.08x slower                                                        |
| regex_v8                | 24.4 ms                                                      | 26.4 ms: 1.08x slower                                                       |
| sqlglot_optimize        | 59.0 ms                                                      | 63.7 ms: 1.08x slower                                                       |
| coroutines              | 27.8 ms                                                      | 30.1 ms: 1.08x slower                                                       |
| scimark_fft             | 281 ms                                                       | 305 ms: 1.09x slower                                                        |
| pickle_list             | 3.94 us                                                      | 4.28 us: 1.09x slower                                                       |
| fannkuch                | 416 ms                                                       | 453 ms: 1.09x slower                                                        |
| pycparser               | 1.31 sec                                                     | 1.43 sec: 1.09x slower                                                      |
| dulwich_log             | 67.4 ms                                                      | 73.8 ms: 1.10x slower                                                       |
| deepcopy_reduce         | 3.40 us                                                      | 3.73 us: 1.10x slower                                                       |
| pyflate                 | 449 ms                                                       | 494 ms: 1.10x slower                                                        |
| scimark_sor             | 110 ms                                                       | 121 ms: 1.10x slower                                                        |
| hexiom                  | 6.98 ms                                                      | 7.74 ms: 1.11x slower                                                       |
| deepcopy_memo           | 37.5 us                                                      | 41.7 us: 1.11x slower                                                       |
| raytrace                | 309 ms                                                       | 343 ms: 1.11x slower                                                        |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 4.53 ms: 1.11x slower                                                       |
| pickle_pure_python      | 316 us                                                       | 352 us: 1.11x slower                                                        |
| django_template         | 39.3 ms                                                      | 43.8 ms: 1.11x slower                                                       |
| crypto_pyaes            | 83.3 ms                                                      | 93.5 ms: 1.12x slower                                                       |
| richards                | 49.7 ms                                                      | 55.9 ms: 1.13x slower                                                       |
| go                      | 158 ms                                                       | 178 ms: 1.13x slower                                                        |
| regex_dna               | 227 ms                                                       | 257 ms: 1.13x slower                                                        |
| deltablue               | 3.97 ms                                                      | 4.49 ms: 1.13x slower                                                       |
| unpickle_pure_python    | 238 us                                                       | 273 us: 1.14x slower                                                        |
| logging_silent          | 100 ns                                                       | 115 ns: 1.15x slower                                                        |
| spectral_norm           | 95.1 ms                                                      | 111 ms: 1.16x slower                                                        |
| comprehensions          | 25.1 us                                                      | 29.6 us: 1.18x slower                                                       |
| coverage                | 66.1 ms                                                      | 84.1 ms: 1.27x slower                                                       |
| sqlglot_transpile       | 1.91 ms                                                      | 2.50 ms: 1.31x slower                                                       |
| sqlglot_parse           | 1.51 ms                                                      | 2.13 ms: 1.41x slower                                                       |
| unpack_sequence         | 45.7 ns                                                      | 152 ns: 3.32x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.07x slower                                                                |

Benchmark hidden because not significant (6): xml_etree_parse, pickle_dict, generators, logging_format, sqlite_synth, bench_mp_pool
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.03x


# Memory

- memory change: 1.06x