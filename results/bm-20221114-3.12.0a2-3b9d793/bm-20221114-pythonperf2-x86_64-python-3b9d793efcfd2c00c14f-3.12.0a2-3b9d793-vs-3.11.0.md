
# Results vs. 3.11.0

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: linux-x86_64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 282 ms: 1.01x faster                                                        |
| chameleon      | 7.92 ms                                                      | 7.19 ms: 1.10x faster                                                       |
| docutils       | 2.85 sec                                                     | 2.77 sec: 1.03x faster                                                      |
| html5lib       | 72.2 ms                                                      | 66.7 ms: 1.08x faster                                                       |
| tornado_http   | 124 ms                                                       | 115 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                        | 1.06x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_memoization  | 629 ms                                                       | 621 ms: 1.01x faster                                                        |
| async_tree_cpu_io_mixed | 753 ms                                                       | 762 ms: 1.01x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.00x slower                                                                |

Benchmark hidden because not significant (2): async_tree_io, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 74.9 ms                                                      | 73.2 ms: 1.02x faster                                                       |
| nbody          | 92.9 ms                                                      | 90.9 ms: 1.02x faster                                                       |
| pidigits       | 251 ms                                                       | 252 ms: 1.00x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 147 ms: 1.06x faster                                                        |
| regex_v8       | 24.4 ms                                                      | 23.2 ms: 1.05x faster                                                       |
| regex_dna      | 227 ms                                                       | 227 ms: 1.00x faster                                                        |
| regex_effbot   | 3.34 ms                                                      | 3.45 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                                       |
| json_loads           | 28.9 us                                                      | 23.7 us: 1.22x faster                                                       |
| unpickle_pure_python | 238 us                                                       | 209 us: 1.14x faster                                                        |
| xml_etree_parse      | 155 ms                                                       | 143 ms: 1.08x faster                                                        |
| pickle_list          | 3.94 us                                                      | 3.65 us: 1.08x faster                                                       |
| unpickle             | 13.3 us                                                      | 12.6 us: 1.05x faster                                                       |
| xml_etree_process    | 55.9 ms                                                      | 54.8 ms: 1.02x faster                                                       |
| unpickle_list        | 4.60 us                                                      | 4.51 us: 1.02x faster                                                       |
| pickle_pure_python   | 316 us                                                       | 314 us: 1.01x faster                                                        |
| xml_etree_generate   | 79.7 ms                                                      | 79.3 ms: 1.00x faster                                                       |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                       |
| pickle_dict          | 32.3 us                                                      | 33.4 us: 1.03x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.06x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.8 ms: 1.01x slower                                                       |
| python_startup_no_site | 7.73 ms                                                      | 7.87 ms: 1.02x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 10.2 ms: 1.08x faster                                                       |
| genshi_xml      | 57.1 ms                                                      | 54.0 ms: 1.06x faster                                                       |
| genshi_text     | 25.5 ms                                                      | 25.2 ms: 1.01x faster                                                       |
| django_template | 39.3 ms                                                      | 39.7 ms: 1.01x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.03x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps              | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                                       |
| json_loads              | 28.9 us                                                      | 23.7 us: 1.22x faster                                                       |
| unpickle_pure_python    | 238 us                                                       | 209 us: 1.14x faster                                                        |
| json                    | 5.58 ms                                                      | 4.95 ms: 1.13x faster                                                       |
| chameleon               | 7.92 ms                                                      | 7.19 ms: 1.10x faster                                                       |
| richards                | 49.7 ms                                                      | 45.4 ms: 1.10x faster                                                       |
| gunicorn                | 966 us                                                       | 886 us: 1.09x faster                                                        |
| aiohttp                 | 986 us                                                       | 904 us: 1.09x faster                                                        |
| deltablue               | 3.97 ms                                                      | 3.64 ms: 1.09x faster                                                       |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 3.74 ms: 1.09x faster                                                       |
| xml_etree_parse         | 155 ms                                                       | 143 ms: 1.08x faster                                                        |
| html5lib                | 72.2 ms                                                      | 66.7 ms: 1.08x faster                                                       |
| pickle_list             | 3.94 us                                                      | 3.65 us: 1.08x faster                                                       |
| tornado_http            | 124 ms                                                       | 115 ms: 1.08x faster                                                        |
| mako                    | 11.0 ms                                                      | 10.2 ms: 1.08x faster                                                       |
| pprint_pformat          | 1.67 sec                                                     | 1.55 sec: 1.07x faster                                                      |
| pprint_safe_repr        | 805 ms                                                       | 752 ms: 1.07x faster                                                        |
| logging_simple          | 7.24 us                                                      | 6.78 us: 1.07x faster                                                       |
| regex_compile           | 156 ms                                                       | 147 ms: 1.06x faster                                                        |
| fannkuch                | 416 ms                                                       | 391 ms: 1.06x faster                                                        |
| gc_traversal            | 4.15 ms                                                      | 3.92 ms: 1.06x faster                                                       |
| genshi_xml              | 57.1 ms                                                      | 54.0 ms: 1.06x faster                                                       |
| regex_v8                | 24.4 ms                                                      | 23.2 ms: 1.05x faster                                                       |
| pycparser               | 1.31 sec                                                     | 1.24 sec: 1.05x faster                                                      |
| scimark_monte_carlo     | 69.8 ms                                                      | 66.4 ms: 1.05x faster                                                       |
| unpickle                | 13.3 us                                                      | 12.6 us: 1.05x faster                                                       |
| telco                   | 6.81 ms                                                      | 6.58 ms: 1.04x faster                                                       |
| bench_thread_pool       | 1.00 ms                                                      | 969 us: 1.03x faster                                                        |
| crypto_pyaes            | 83.3 ms                                                      | 80.7 ms: 1.03x faster                                                       |
| hexiom                  | 6.98 ms                                                      | 6.76 ms: 1.03x faster                                                       |
| pyflate                 | 449 ms                                                       | 436 ms: 1.03x faster                                                        |
| scimark_sor             | 110 ms                                                       | 106 ms: 1.03x faster                                                        |
| docutils                | 2.85 sec                                                     | 2.77 sec: 1.03x faster                                                      |
| chaos                   | 74.9 ms                                                      | 72.9 ms: 1.03x faster                                                       |
| scimark_fft             | 281 ms                                                       | 273 ms: 1.03x faster                                                        |
| scimark_lu              | 114 ms                                                       | 111 ms: 1.03x faster                                                        |
| deepcopy_memo           | 37.5 us                                                      | 36.7 us: 1.02x faster                                                       |
| float                   | 74.9 ms                                                      | 73.2 ms: 1.02x faster                                                       |
| nbody                   | 92.9 ms                                                      | 90.9 ms: 1.02x faster                                                       |
| sqlglot_transpile       | 1.91 ms                                                      | 1.87 ms: 1.02x faster                                                       |
| xml_etree_process       | 55.9 ms                                                      | 54.8 ms: 1.02x faster                                                       |
| spectral_norm           | 95.1 ms                                                      | 93.2 ms: 1.02x faster                                                       |
| thrift                  | 931 us                                                       | 913 us: 1.02x faster                                                        |
| unpickle_list           | 4.60 us                                                      | 4.51 us: 1.02x faster                                                       |
| meteor_contest          | 131 ms                                                       | 129 ms: 1.02x faster                                                        |
| 2to3                    | 287 ms                                                       | 282 ms: 1.01x faster                                                        |
| mdp                     | 2.77 sec                                                     | 2.73 sec: 1.01x faster                                                      |
| async_tree_memoization  | 629 ms                                                       | 621 ms: 1.01x faster                                                        |
| logging_format          | 7.71 us                                                      | 7.60 us: 1.01x faster                                                       |
| genshi_text             | 25.5 ms                                                      | 25.2 ms: 1.01x faster                                                       |
| raytrace                | 309 ms                                                       | 305 ms: 1.01x faster                                                        |
| sqlglot_optimize        | 59.0 ms                                                      | 58.2 ms: 1.01x faster                                                       |
| sympy_integrate         | 25.8 ms                                                      | 25.5 ms: 1.01x faster                                                       |
| logging_silent          | 100 ns                                                       | 99.2 ns: 1.01x faster                                                       |
| deepcopy                | 391 us                                                       | 387 us: 1.01x faster                                                        |
| sqlglot_parse           | 1.51 ms                                                      | 1.50 ms: 1.01x faster                                                       |
| pickle_pure_python      | 316 us                                                       | 314 us: 1.01x faster                                                        |
| sympy_sum               | 186 ms                                                       | 184 ms: 1.01x faster                                                        |
| sympy_expand            | 553 ms                                                       | 550 ms: 1.01x faster                                                        |
| xml_etree_generate      | 79.7 ms                                                      | 79.3 ms: 1.00x faster                                                       |
| regex_dna               | 227 ms                                                       | 227 ms: 1.00x faster                                                        |
| pidigits                | 251 ms                                                       | 252 ms: 1.00x slower                                                        |
| sqlglot_normalize       | 122 ms                                                       | 122 ms: 1.00x slower                                                        |
| python_startup          | 10.7 ms                                                      | 10.8 ms: 1.01x slower                                                       |
| django_template         | 39.3 ms                                                      | 39.7 ms: 1.01x slower                                                       |
| async_tree_cpu_io_mixed | 753 ms                                                       | 762 ms: 1.01x slower                                                        |
| create_gc_cycles        | 1.58 ms                                                      | 1.60 ms: 1.01x slower                                                       |
| pickle                  | 9.89 us                                                      | 10.1 us: 1.02x slower                                                       |
| go                      | 158 ms                                                       | 160 ms: 1.02x slower                                                        |
| python_startup_no_site  | 7.73 ms                                                      | 7.87 ms: 1.02x slower                                                       |
| sqlite_synth            | 2.52 us                                                      | 2.57 us: 1.02x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                       |
| regex_effbot            | 3.34 ms                                                      | 3.45 ms: 1.03x slower                                                       |
| pickle_dict             | 32.3 us                                                      | 33.4 us: 1.03x slower                                                       |
| comprehensions          | 25.1 us                                                      | 26.9 us: 1.07x slower                                                       |
| generators              | 54.6 ms                                                      | 61.2 ms: 1.12x slower                                                       |
| coverage                | 66.1 ms                                                      | 86.9 ms: 1.32x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.03x faster                                                                |

Benchmark hidden because not significant (13): bench_mp_pool, dulwich_log, deepcopy_reduce, async_generators, nqueens, async_tree_io, sympy_str, dask, asyncio_tcp, unpack_sequence, coroutines, async_tree_none, xml_etree_iterparse
Ignored benchmarks (14) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x