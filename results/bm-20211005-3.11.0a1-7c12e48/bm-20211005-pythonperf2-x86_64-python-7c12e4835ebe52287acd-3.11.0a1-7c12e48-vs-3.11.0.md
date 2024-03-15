
# Results vs. 3.11.0

- fork: python
- ref: 7c12e4835ebe52287acd
- machine: linux-x86_64
- commit hash: 7c12e48
- commit date: 2021-10-05
- overall geometric mean: 1.11x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 329 ms: 1.15x slower                                                        |
| chameleon      | 7.92 ms                                                      | 8.97 ms: 1.13x slower                                                       |
| docutils       | 2.85 sec                                                     | 3.22 sec: 1.13x slower                                                      |
| html5lib       | 72.2 ms                                                      | 83.0 ms: 1.15x slower                                                       |
| tornado_http   | 124 ms                                                       | 136 ms: 1.09x slower                                                        |
| Geometric mean | (ref)                                                        | 1.13x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 660 ms: 1.05x slower                                                        |
| async_tree_cpu_io_mixed | 753 ms                                                       | 796 ms: 1.06x slower                                                        |
| async_tree_io           | 1.17 sec                                                     | 1.24 sec: 1.06x slower                                                      |
| Geometric mean          | (ref)                                                        | 1.04x slower                                                                |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 266 ms: 1.06x slower                                                        |
| float          | 74.9 ms                                                      | 86.6 ms: 1.16x slower                                                       |
| nbody          | 92.9 ms                                                      | 132 ms: 1.42x slower                                                        |
| Geometric mean | (ref)                                                        | 1.20x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.05 ms: 1.09x faster                                                       |
| regex_v8       | 24.4 ms                                                      | 25.6 ms: 1.05x slower                                                       |
| regex_compile  | 156 ms                                                       | 169 ms: 1.08x slower                                                        |
| regex_dna      | 227 ms                                                       | 262 ms: 1.15x slower                                                        |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads           | 28.9 us                                                      | 27.0 us: 1.07x faster                                                       |
| pickle_dict          | 32.3 us                                                      | 31.5 us: 1.03x faster                                                       |
| unpickle_list        | 4.60 us                                                      | 4.54 us: 1.01x faster                                                       |
| xml_etree_parse      | 155 ms                                                       | 158 ms: 1.02x slower                                                        |
| json_dumps           | 13.3 ms                                                      | 13.6 ms: 1.03x slower                                                       |
| unpickle             | 13.3 us                                                      | 13.7 us: 1.03x slower                                                       |
| xml_etree_iterparse  | 107 ms                                                       | 111 ms: 1.04x slower                                                        |
| pickle_list          | 3.94 us                                                      | 4.14 us: 1.05x slower                                                       |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 86.0 ms: 1.08x slower                                                       |
| xml_etree_process    | 55.9 ms                                                      | 64.1 ms: 1.15x slower                                                       |
| unpickle_pure_python | 238 us                                                       | 293 us: 1.23x slower                                                        |
| pickle_pure_python   | 316 us                                                       | 394 us: 1.25x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.06x slower                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 7.73 ms                                                      | 7.57 ms: 1.02x faster                                                       |
| python_startup         | 10.7 ms                                                      | 11.8 ms: 1.10x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.04x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| genshi_xml      | 57.1 ms                                                      | 59.9 ms: 1.05x slower                                                       |
| genshi_text     | 25.5 ms                                                      | 28.3 ms: 1.11x slower                                                       |
| mako            | 11.0 ms                                                      | 13.1 ms: 1.19x slower                                                       |
| django_template | 39.3 ms                                                      | 47.5 ms: 1.21x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.14x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| gc_traversal            | 4.15 ms                                                      | 3.55 ms: 1.17x faster                                                       |
| regex_effbot            | 3.34 ms                                                      | 3.05 ms: 1.09x faster                                                       |
| logging_simple          | 7.24 us                                                      | 6.69 us: 1.08x faster                                                       |
| json_loads              | 28.9 us                                                      | 27.0 us: 1.07x faster                                                       |
| logging_format          | 7.71 us                                                      | 7.28 us: 1.06x faster                                                       |
| generators              | 54.6 ms                                                      | 52.5 ms: 1.04x faster                                                       |
| json                    | 5.58 ms                                                      | 5.40 ms: 1.03x faster                                                       |
| pickle_dict             | 32.3 us                                                      | 31.5 us: 1.03x faster                                                       |
| telco                   | 6.81 ms                                                      | 6.66 ms: 1.02x faster                                                       |
| python_startup_no_site  | 7.73 ms                                                      | 7.57 ms: 1.02x faster                                                       |
| unpickle_list           | 4.60 us                                                      | 4.54 us: 1.01x faster                                                       |
| sympy_sum               | 186 ms                                                       | 184 ms: 1.01x faster                                                        |
| sympy_str               | 337 ms                                                       | 343 ms: 1.02x slower                                                        |
| unpack_sequence         | 45.7 ns                                                      | 46.5 ns: 1.02x slower                                                       |
| meteor_contest          | 131 ms                                                       | 133 ms: 1.02x slower                                                        |
| gunicorn                | 966 us                                                       | 988 us: 1.02x slower                                                        |
| xml_etree_parse         | 155 ms                                                       | 158 ms: 1.02x slower                                                        |
| coroutines              | 27.8 ms                                                      | 28.5 ms: 1.03x slower                                                       |
| mdp                     | 2.77 sec                                                     | 2.84 sec: 1.03x slower                                                      |
| json_dumps              | 13.3 ms                                                      | 13.6 ms: 1.03x slower                                                       |
| unpickle                | 13.3 us                                                      | 13.7 us: 1.03x slower                                                       |
| sympy_expand            | 553 ms                                                       | 573 ms: 1.04x slower                                                        |
| sympy_integrate         | 25.8 ms                                                      | 26.8 ms: 1.04x slower                                                       |
| xml_etree_iterparse     | 107 ms                                                       | 111 ms: 1.04x slower                                                        |
| regex_v8                | 24.4 ms                                                      | 25.6 ms: 1.05x slower                                                       |
| pickle_list             | 3.94 us                                                      | 4.14 us: 1.05x slower                                                       |
| async_tree_memoization  | 629 ms                                                       | 660 ms: 1.05x slower                                                        |
| genshi_xml              | 57.1 ms                                                      | 59.9 ms: 1.05x slower                                                       |
| pickle                  | 9.89 us                                                      | 10.4 us: 1.05x slower                                                       |
| dask                    | 410 ms                                                       | 433 ms: 1.06x slower                                                        |
| async_tree_cpu_io_mixed | 753 ms                                                       | 796 ms: 1.06x slower                                                        |
| pidigits                | 251 ms                                                       | 266 ms: 1.06x slower                                                        |
| async_tree_io           | 1.17 sec                                                     | 1.24 sec: 1.06x slower                                                      |
| bench_thread_pool       | 1.00 ms                                                      | 1.07 ms: 1.07x slower                                                       |
| xml_etree_generate      | 79.7 ms                                                      | 86.0 ms: 1.08x slower                                                       |
| pycparser               | 1.31 sec                                                     | 1.41 sec: 1.08x slower                                                      |
| regex_compile           | 156 ms                                                       | 169 ms: 1.08x slower                                                        |
| coverage                | 66.1 ms                                                      | 72.0 ms: 1.09x slower                                                       |
| deepcopy_reduce         | 3.40 us                                                      | 3.70 us: 1.09x slower                                                       |
| thrift                  | 931 us                                                       | 1.02 ms: 1.09x slower                                                       |
| pprint_safe_repr        | 805 ms                                                       | 879 ms: 1.09x slower                                                        |
| sqlite_synth            | 2.52 us                                                      | 2.76 us: 1.09x slower                                                       |
| deepcopy                | 391 us                                                       | 427 us: 1.09x slower                                                        |
| tornado_http            | 124 ms                                                       | 136 ms: 1.09x slower                                                        |
| bench_mp_pool           | 4.70 ms                                                      | 5.14 ms: 1.09x slower                                                       |
| python_startup          | 10.7 ms                                                      | 11.8 ms: 1.10x slower                                                       |
| pprint_pformat          | 1.67 sec                                                     | 1.83 sec: 1.10x slower                                                      |
| dulwich_log             | 67.4 ms                                                      | 74.2 ms: 1.10x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 20.9 ms: 1.10x slower                                                       |
| async_generators        | 322 ms                                                       | 356 ms: 1.11x slower                                                        |
| genshi_text             | 25.5 ms                                                      | 28.3 ms: 1.11x slower                                                       |
| sqlglot_normalize       | 122 ms                                                       | 135 ms: 1.11x slower                                                        |
| sqlglot_optimize        | 59.0 ms                                                      | 66.6 ms: 1.13x slower                                                       |
| docutils                | 2.85 sec                                                     | 3.22 sec: 1.13x slower                                                      |
| chameleon               | 7.92 ms                                                      | 8.97 ms: 1.13x slower                                                       |
| fannkuch                | 416 ms                                                       | 472 ms: 1.14x slower                                                        |
| 2to3                    | 287 ms                                                       | 329 ms: 1.15x slower                                                        |
| xml_etree_process       | 55.9 ms                                                      | 64.1 ms: 1.15x slower                                                       |
| html5lib                | 72.2 ms                                                      | 83.0 ms: 1.15x slower                                                       |
| regex_dna               | 227 ms                                                       | 262 ms: 1.15x slower                                                        |
| float                   | 74.9 ms                                                      | 86.6 ms: 1.16x slower                                                       |
| chaos                   | 74.9 ms                                                      | 87.5 ms: 1.17x slower                                                       |
| hexiom                  | 6.98 ms                                                      | 8.15 ms: 1.17x slower                                                       |
| comprehensions          | 25.1 us                                                      | 29.5 us: 1.18x slower                                                       |
| scimark_fft             | 281 ms                                                       | 333 ms: 1.19x slower                                                        |
| mako                    | 11.0 ms                                                      | 13.1 ms: 1.19x slower                                                       |
| deepcopy_memo           | 37.5 us                                                      | 44.7 us: 1.19x slower                                                       |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 4.84 ms: 1.19x slower                                                       |
| raytrace                | 309 ms                                                       | 371 ms: 1.20x slower                                                        |
| create_gc_cycles        | 1.58 ms                                                      | 1.90 ms: 1.21x slower                                                       |
| django_template         | 39.3 ms                                                      | 47.5 ms: 1.21x slower                                                       |
| crypto_pyaes            | 83.3 ms                                                      | 102 ms: 1.22x slower                                                        |
| unpickle_pure_python    | 238 us                                                       | 293 us: 1.23x slower                                                        |
| pickle_pure_python      | 316 us                                                       | 394 us: 1.25x slower                                                        |
| scimark_monte_carlo     | 69.8 ms                                                      | 87.3 ms: 1.25x slower                                                       |
| flaskblogging           | 3.88 ms                                                      | 4.88 ms: 1.26x slower                                                       |
| spectral_norm           | 95.1 ms                                                      | 120 ms: 1.26x slower                                                        |
| scimark_lu              | 114 ms                                                       | 145 ms: 1.27x slower                                                        |
| richards                | 49.7 ms                                                      | 64.9 ms: 1.31x slower                                                       |
| logging_silent          | 100 ns                                                       | 134 ns: 1.34x slower                                                        |
| scimark_sor             | 110 ms                                                       | 147 ms: 1.34x slower                                                        |
| go                      | 158 ms                                                       | 211 ms: 1.34x slower                                                        |
| pyflate                 | 449 ms                                                       | 615 ms: 1.37x slower                                                        |
| nbody                   | 92.9 ms                                                      | 132 ms: 1.42x slower                                                        |
| sqlglot_transpile       | 1.91 ms                                                      | 2.76 ms: 1.44x slower                                                       |
| deltablue               | 3.97 ms                                                      | 5.73 ms: 1.44x slower                                                       |
| sqlglot_parse           | 1.51 ms                                                      | 2.37 ms: 1.57x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.11x slower                                                                |

Benchmark hidden because not significant (2): async_tree_none, nqueens
Ignored benchmarks (15) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.08x
- 95% likely to have a slowdown of 1.08x
- 99% likely to have a slowdown of 1.07x


# Memory

- memory change: 0.98x