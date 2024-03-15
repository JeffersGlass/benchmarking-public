
# Results vs. 3.11.0

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: linux-x86_64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.22x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x slower
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 350 ms: 1.22x slower                                                       |
| chameleon      | 7.92 ms                                                      | 9.41 ms: 1.19x slower                                                      |
| docutils       | 2.85 sec                                                     | 3.42 sec: 1.20x slower                                                     |
| html5lib       | 72.2 ms                                                      | 93.6 ms: 1.30x slower                                                      |
| tornado_http   | 124 ms                                                       | 150 ms: 1.21x slower                                                       |
| Geometric mean | (ref)                                                        | 1.22x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 753 ms                                                       | 952 ms: 1.26x slower                                                       |
| async_tree_memoization  | 629 ms                                                       | 827 ms: 1.32x slower                                                       |
| async_tree_none         | 518 ms                                                       | 695 ms: 1.34x slower                                                       |
| async_tree_io           | 1.17 sec                                                     | 1.61 sec: 1.37x slower                                                     |
| Geometric mean          | (ref)                                                        | 1.32x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 271 ms: 1.08x slower                                                       |
| float          | 74.9 ms                                                      | 110 ms: 1.47x slower                                                       |
| nbody          | 92.9 ms                                                      | 137 ms: 1.47x slower                                                       |
| Geometric mean | (ref)                                                        | 1.33x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.25 ms: 1.03x faster                                                      |
| regex_v8       | 24.4 ms                                                      | 27.1 ms: 1.11x slower                                                      |
| regex_dna      | 227 ms                                                       | 259 ms: 1.14x slower                                                       |
| regex_compile  | 156 ms                                                       | 191 ms: 1.23x slower                                                       |
| Geometric mean | (ref)                                                        | 1.11x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_dict          | 32.3 us                                                      | 31.1 us: 1.04x faster                                                      |
| xml_etree_iterparse  | 107 ms                                                       | 109 ms: 1.02x slower                                                       |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                      |
| pickle_list          | 3.94 us                                                      | 4.04 us: 1.02x slower                                                      |
| xml_etree_parse      | 155 ms                                                       | 160 ms: 1.03x slower                                                       |
| json_loads           | 28.9 us                                                      | 30.2 us: 1.04x slower                                                      |
| unpickle             | 13.3 us                                                      | 14.1 us: 1.06x slower                                                      |
| json_dumps           | 13.3 ms                                                      | 14.4 ms: 1.09x slower                                                      |
| xml_etree_generate   | 79.7 ms                                                      | 92.8 ms: 1.16x slower                                                      |
| unpickle_pure_python | 238 us                                                       | 313 us: 1.31x slower                                                       |
| xml_etree_process    | 55.9 ms                                                      | 76.5 ms: 1.37x slower                                                      |
| pickle_pure_python   | 316 us                                                       | 454 us: 1.44x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.11x slower                                                               |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 7.73 ms                                                      | 7.35 ms: 1.05x faster                                                      |
| python_startup         | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_xml      | 57.1 ms                                                      | 63.7 ms: 1.12x slower                                                      |
| genshi_text     | 25.5 ms                                                      | 31.7 ms: 1.24x slower                                                      |
| django_template | 39.3 ms                                                      | 53.2 ms: 1.35x slower                                                      |
| mako            | 11.0 ms                                                      | 14.9 ms: 1.35x slower                                                      |
| Geometric mean  | (ref)                                                        | 1.26x slower                                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| gc_traversal            | 4.15 ms                                                      | 3.68 ms: 1.13x faster                                                      |
| python_startup_no_site  | 7.73 ms                                                      | 7.35 ms: 1.05x faster                                                      |
| coverage                | 66.1 ms                                                      | 63.5 ms: 1.04x faster                                                      |
| pickle_dict             | 32.3 us                                                      | 31.1 us: 1.04x faster                                                      |
| regex_effbot            | 3.34 ms                                                      | 3.25 ms: 1.03x faster                                                      |
| xml_etree_iterparse     | 107 ms                                                       | 109 ms: 1.02x slower                                                       |
| pickle                  | 9.89 us                                                      | 10.1 us: 1.02x slower                                                      |
| pickle_list             | 3.94 us                                                      | 4.04 us: 1.02x slower                                                      |
| xml_etree_parse         | 155 ms                                                       | 160 ms: 1.03x slower                                                       |
| json_loads              | 28.9 us                                                      | 30.2 us: 1.04x slower                                                      |
| asyncio_tcp             | 747 ms                                                       | 781 ms: 1.05x slower                                                       |
| telco                   | 6.81 ms                                                      | 7.16 ms: 1.05x slower                                                      |
| generators              | 54.6 ms                                                      | 57.8 ms: 1.06x slower                                                      |
| unpickle                | 13.3 us                                                      | 14.1 us: 1.06x slower                                                      |
| meteor_contest          | 131 ms                                                       | 139 ms: 1.06x slower                                                       |
| json                    | 5.58 ms                                                      | 5.97 ms: 1.07x slower                                                      |
| sympy_sum               | 186 ms                                                       | 199 ms: 1.07x slower                                                       |
| python_startup          | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                                      |
| pidigits                | 251 ms                                                       | 271 ms: 1.08x slower                                                       |
| comprehensions          | 25.1 us                                                      | 27.1 us: 1.08x slower                                                      |
| coroutines              | 27.8 ms                                                      | 30.2 ms: 1.09x slower                                                      |
| sympy_str               | 337 ms                                                       | 366 ms: 1.09x slower                                                       |
| json_dumps              | 13.3 ms                                                      | 14.4 ms: 1.09x slower                                                      |
| nqueens                 | 103 ms                                                       | 112 ms: 1.10x slower                                                       |
| sympy_integrate         | 25.8 ms                                                      | 28.4 ms: 1.10x slower                                                      |
| bench_thread_pool       | 1.00 ms                                                      | 1.10 ms: 1.10x slower                                                      |
| regex_v8                | 24.4 ms                                                      | 27.1 ms: 1.11x slower                                                      |
| pathlib                 | 18.9 ms                                                      | 21.0 ms: 1.11x slower                                                      |
| sympy_expand            | 553 ms                                                       | 615 ms: 1.11x slower                                                       |
| pylint                  | 514 ms                                                       | 572 ms: 1.11x slower                                                       |
| genshi_xml              | 57.1 ms                                                      | 63.7 ms: 1.12x slower                                                      |
| flaskblogging           | 3.88 ms                                                      | 4.33 ms: 1.12x slower                                                      |
| dask                    | 410 ms                                                       | 459 ms: 1.12x slower                                                       |
| mdp                     | 2.77 sec                                                     | 3.12 sec: 1.12x slower                                                     |
| regex_dna               | 227 ms                                                       | 259 ms: 1.14x slower                                                       |
| fannkuch                | 416 ms                                                       | 477 ms: 1.15x slower                                                       |
| create_gc_cycles        | 1.58 ms                                                      | 1.82 ms: 1.15x slower                                                      |
| sqlalchemy_imperative   | 19.8 ms                                                      | 23.0 ms: 1.16x slower                                                      |
| xml_etree_generate      | 79.7 ms                                                      | 92.8 ms: 1.16x slower                                                      |
| gunicorn                | 966 us                                                       | 1.13 ms: 1.17x slower                                                      |
| aiohttp                 | 986 us                                                       | 1.15 ms: 1.17x slower                                                      |
| sqlglot_optimize        | 59.0 ms                                                      | 69.1 ms: 1.17x slower                                                      |
| deepcopy_reduce         | 3.40 us                                                      | 3.99 us: 1.17x slower                                                      |
| sqlite_synth            | 2.52 us                                                      | 2.97 us: 1.18x slower                                                      |
| sqlglot_normalize       | 122 ms                                                       | 144 ms: 1.19x slower                                                       |
| chameleon               | 7.92 ms                                                      | 9.41 ms: 1.19x slower                                                      |
| deepcopy                | 391 us                                                       | 465 us: 1.19x slower                                                       |
| dulwich_log             | 67.4 ms                                                      | 80.1 ms: 1.19x slower                                                      |
| docutils                | 2.85 sec                                                     | 3.42 sec: 1.20x slower                                                     |
| tornado_http            | 124 ms                                                       | 150 ms: 1.21x slower                                                       |
| sqlalchemy_declarative  | 154 ms                                                       | 188 ms: 1.22x slower                                                       |
| 2to3                    | 287 ms                                                       | 350 ms: 1.22x slower                                                       |
| regex_compile           | 156 ms                                                       | 191 ms: 1.23x slower                                                       |
| pycparser               | 1.31 sec                                                     | 1.61 sec: 1.23x slower                                                     |
| logging_simple          | 7.24 us                                                      | 8.94 us: 1.23x slower                                                      |
| logging_format          | 7.71 us                                                      | 9.57 us: 1.24x slower                                                      |
| genshi_text             | 25.5 ms                                                      | 31.7 ms: 1.24x slower                                                      |
| thrift                  | 931 us                                                       | 1.17 ms: 1.25x slower                                                      |
| async_tree_cpu_io_mixed | 753 ms                                                       | 952 ms: 1.26x slower                                                       |
| scimark_fft             | 281 ms                                                       | 360 ms: 1.28x slower                                                       |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 5.22 ms: 1.28x slower                                                      |
| pprint_safe_repr        | 805 ms                                                       | 1.03 sec: 1.29x slower                                                     |
| pprint_pformat          | 1.67 sec                                                     | 2.14 sec: 1.29x slower                                                     |
| html5lib                | 72.2 ms                                                      | 93.6 ms: 1.30x slower                                                      |
| async_generators        | 322 ms                                                       | 418 ms: 1.30x slower                                                       |
| unpack_sequence         | 45.7 ns                                                      | 59.4 ns: 1.30x slower                                                      |
| unpickle_pure_python    | 238 us                                                       | 313 us: 1.31x slower                                                       |
| async_tree_memoization  | 629 ms                                                       | 827 ms: 1.32x slower                                                       |
| async_tree_none         | 518 ms                                                       | 695 ms: 1.34x slower                                                       |
| hexiom                  | 6.98 ms                                                      | 9.43 ms: 1.35x slower                                                      |
| django_template         | 39.3 ms                                                      | 53.2 ms: 1.35x slower                                                      |
| mako                    | 11.0 ms                                                      | 14.9 ms: 1.35x slower                                                      |
| deepcopy_memo           | 37.5 us                                                      | 51.1 us: 1.36x slower                                                      |
| xml_etree_process       | 55.9 ms                                                      | 76.5 ms: 1.37x slower                                                      |
| async_tree_io           | 1.17 sec                                                     | 1.61 sec: 1.37x slower                                                     |
| crypto_pyaes            | 83.3 ms                                                      | 115 ms: 1.38x slower                                                       |
| chaos                   | 74.9 ms                                                      | 105 ms: 1.40x slower                                                       |
| sqlglot_transpile       | 1.91 ms                                                      | 2.69 ms: 1.41x slower                                                      |
| scimark_lu              | 114 ms                                                       | 161 ms: 1.41x slower                                                       |
| pickle_pure_python      | 316 us                                                       | 454 us: 1.44x slower                                                       |
| spectral_norm           | 95.1 ms                                                      | 137 ms: 1.44x slower                                                       |
| bench_mp_pool           | 4.70 ms                                                      | 6.82 ms: 1.45x slower                                                      |
| float                   | 74.9 ms                                                      | 110 ms: 1.47x slower                                                       |
| nbody                   | 92.9 ms                                                      | 137 ms: 1.47x slower                                                       |
| sqlglot_parse           | 1.51 ms                                                      | 2.26 ms: 1.49x slower                                                      |
| richards                | 49.7 ms                                                      | 74.5 ms: 1.50x slower                                                      |
| pyflate                 | 449 ms                                                       | 693 ms: 1.54x slower                                                       |
| scimark_monte_carlo     | 69.8 ms                                                      | 110 ms: 1.58x slower                                                       |
| raytrace                | 309 ms                                                       | 491 ms: 1.59x slower                                                       |
| scimark_sor             | 110 ms                                                       | 176 ms: 1.61x slower                                                       |
| logging_silent          | 100 ns                                                       | 166 ns: 1.65x slower                                                       |
| go                      | 158 ms                                                       | 264 ms: 1.68x slower                                                       |
| deltablue               | 3.97 ms                                                      | 7.44 ms: 1.88x slower                                                      |
| Geometric mean          | (ref)                                                        | 1.22x slower                                                               |

Benchmark hidden because not significant (1): unpickle_list
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.18x
- 95% likely to have a slowdown of 1.17x
- 99% likely to have a slowdown of 1.16x


# Memory

- memory change: 0.95x