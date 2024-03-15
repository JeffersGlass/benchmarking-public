
# Results vs. 3.11.0

- fork: python
- ref: aad5f6a89125ad4529ab
- machine: linux-x86_64
- commit hash: aad5f6a
- commit date: 2023-02-07
- overall geometric mean: 1.23x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x slower
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 351 ms: 1.22x slower                                                       |
| chameleon      | 7.92 ms                                                      | 9.41 ms: 1.19x slower                                                      |
| docutils       | 2.85 sec                                                     | 3.45 sec: 1.21x slower                                                     |
| html5lib       | 72.2 ms                                                      | 94.4 ms: 1.31x slower                                                      |
| tornado_http   | 124 ms                                                       | 159 ms: 1.28x slower                                                       |
| Geometric mean | (ref)                                                        | 1.24x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 753 ms                                                       | 955 ms: 1.27x slower                                                       |
| async_tree_memoization  | 629 ms                                                       | 832 ms: 1.32x slower                                                       |
| async_tree_none         | 518 ms                                                       | 711 ms: 1.37x slower                                                       |
| async_tree_io           | 1.17 sec                                                     | 1.62 sec: 1.39x slower                                                     |
| Geometric mean          | (ref)                                                        | 1.34x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 271 ms: 1.08x slower                                                       |
| float          | 74.9 ms                                                      | 111 ms: 1.48x slower                                                       |
| nbody          | 92.9 ms                                                      | 138 ms: 1.48x slower                                                       |
| Geometric mean | (ref)                                                        | 1.33x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.49 ms: 1.05x slower                                                      |
| regex_v8       | 24.4 ms                                                      | 27.2 ms: 1.11x slower                                                      |
| regex_dna      | 227 ms                                                       | 260 ms: 1.14x slower                                                       |
| regex_compile  | 156 ms                                                       | 192 ms: 1.23x slower                                                       |
| Geometric mean | (ref)                                                        | 1.13x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_dict          | 32.3 us                                                      | 32.1 us: 1.01x faster                                                      |
| unpickle_list        | 4.60 us                                                      | 4.71 us: 1.02x slower                                                      |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                      |
| unpickle             | 13.3 us                                                      | 13.7 us: 1.03x slower                                                      |
| json_loads           | 28.9 us                                                      | 30.0 us: 1.04x slower                                                      |
| pickle_list          | 3.94 us                                                      | 4.17 us: 1.06x slower                                                      |
| xml_etree_parse      | 155 ms                                                       | 164 ms: 1.06x slower                                                       |
| xml_etree_iterparse  | 107 ms                                                       | 113 ms: 1.06x slower                                                       |
| json_dumps           | 13.3 ms                                                      | 14.4 ms: 1.09x slower                                                      |
| xml_etree_generate   | 79.7 ms                                                      | 94.0 ms: 1.18x slower                                                      |
| unpickle_pure_python | 238 us                                                       | 320 us: 1.34x slower                                                       |
| xml_etree_process    | 55.9 ms                                                      | 77.5 ms: 1.39x slower                                                      |
| pickle_pure_python   | 316 us                                                       | 461 us: 1.46x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.12x slower                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 7.73 ms                                                      | 7.34 ms: 1.05x faster                                                      |
| python_startup         | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.01x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_xml      | 57.1 ms                                                      | 62.5 ms: 1.09x slower                                                      |
| genshi_text     | 25.5 ms                                                      | 32.0 ms: 1.26x slower                                                      |
| mako            | 11.0 ms                                                      | 14.7 ms: 1.33x slower                                                      |
| django_template | 39.3 ms                                                      | 53.6 ms: 1.36x slower                                                      |
| Geometric mean  | (ref)                                                        | 1.26x slower                                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site  | 7.73 ms                                                      | 7.34 ms: 1.05x faster                                                      |
| coverage                | 66.1 ms                                                      | 63.3 ms: 1.04x faster                                                      |
| pickle_dict             | 32.3 us                                                      | 32.1 us: 1.01x faster                                                      |
| unpickle_list           | 4.60 us                                                      | 4.71 us: 1.02x slower                                                      |
| pickle                  | 9.89 us                                                      | 10.1 us: 1.02x slower                                                      |
| unpickle                | 13.3 us                                                      | 13.7 us: 1.03x slower                                                      |
| json_loads              | 28.9 us                                                      | 30.0 us: 1.04x slower                                                      |
| asyncio_tcp             | 747 ms                                                       | 779 ms: 1.04x slower                                                       |
| generators              | 54.6 ms                                                      | 57.0 ms: 1.04x slower                                                      |
| regex_effbot            | 3.34 ms                                                      | 3.49 ms: 1.05x slower                                                      |
| pickle_list             | 3.94 us                                                      | 4.17 us: 1.06x slower                                                      |
| xml_etree_parse         | 155 ms                                                       | 164 ms: 1.06x slower                                                       |
| json                    | 5.58 ms                                                      | 5.91 ms: 1.06x slower                                                      |
| xml_etree_iterparse     | 107 ms                                                       | 113 ms: 1.06x slower                                                       |
| telco                   | 6.81 ms                                                      | 7.25 ms: 1.06x slower                                                      |
| meteor_contest          | 131 ms                                                       | 139 ms: 1.07x slower                                                       |
| sympy_sum               | 186 ms                                                       | 199 ms: 1.07x slower                                                       |
| python_startup          | 10.7 ms                                                      | 11.5 ms: 1.07x slower                                                      |
| coroutines              | 27.8 ms                                                      | 29.9 ms: 1.08x slower                                                      |
| comprehensions          | 25.1 us                                                      | 27.0 us: 1.08x slower                                                      |
| pidigits                | 251 ms                                                       | 271 ms: 1.08x slower                                                       |
| sympy_str               | 337 ms                                                       | 364 ms: 1.08x slower                                                       |
| json_dumps              | 13.3 ms                                                      | 14.4 ms: 1.09x slower                                                      |
| genshi_xml              | 57.1 ms                                                      | 62.5 ms: 1.09x slower                                                      |
| nqueens                 | 103 ms                                                       | 113 ms: 1.10x slower                                                       |
| sympy_expand            | 553 ms                                                       | 608 ms: 1.10x slower                                                       |
| mdp                     | 2.77 sec                                                     | 3.05 sec: 1.10x slower                                                     |
| sympy_integrate         | 25.8 ms                                                      | 28.5 ms: 1.10x slower                                                      |
| bench_thread_pool       | 1.00 ms                                                      | 1.11 ms: 1.11x slower                                                      |
| pylint                  | 514 ms                                                       | 572 ms: 1.11x slower                                                       |
| regex_v8                | 24.4 ms                                                      | 27.2 ms: 1.11x slower                                                      |
| pathlib                 | 18.9 ms                                                      | 21.3 ms: 1.13x slower                                                      |
| fannkuch                | 416 ms                                                       | 470 ms: 1.13x slower                                                       |
| flaskblogging           | 3.88 ms                                                      | 4.40 ms: 1.13x slower                                                      |
| regex_dna               | 227 ms                                                       | 260 ms: 1.14x slower                                                       |
| create_gc_cycles        | 1.58 ms                                                      | 1.81 ms: 1.15x slower                                                      |
| sqlalchemy_imperative   | 19.8 ms                                                      | 22.9 ms: 1.16x slower                                                      |
| aiohttp                 | 986 us                                                       | 1.15 ms: 1.16x slower                                                      |
| gunicorn                | 966 us                                                       | 1.13 ms: 1.16x slower                                                      |
| xml_etree_generate      | 79.7 ms                                                      | 94.0 ms: 1.18x slower                                                      |
| sqlglot_optimize        | 59.0 ms                                                      | 69.6 ms: 1.18x slower                                                      |
| sqlite_synth            | 2.52 us                                                      | 2.98 us: 1.18x slower                                                      |
| dask                    | 410 ms                                                       | 484 ms: 1.18x slower                                                       |
| chameleon               | 7.92 ms                                                      | 9.41 ms: 1.19x slower                                                      |
| deepcopy                | 391 us                                                       | 466 us: 1.19x slower                                                       |
| deepcopy_reduce         | 3.40 us                                                      | 4.05 us: 1.19x slower                                                      |
| sqlglot_normalize       | 122 ms                                                       | 146 ms: 1.20x slower                                                       |
| dulwich_log             | 67.4 ms                                                      | 81.1 ms: 1.20x slower                                                      |
| docutils                | 2.85 sec                                                     | 3.45 sec: 1.21x slower                                                     |
| sqlalchemy_declarative  | 154 ms                                                       | 187 ms: 1.21x slower                                                       |
| 2to3                    | 287 ms                                                       | 351 ms: 1.22x slower                                                       |
| regex_compile           | 156 ms                                                       | 192 ms: 1.23x slower                                                       |
| logging_simple          | 7.24 us                                                      | 8.96 us: 1.24x slower                                                      |
| logging_format          | 7.71 us                                                      | 9.67 us: 1.25x slower                                                      |
| genshi_text             | 25.5 ms                                                      | 32.0 ms: 1.26x slower                                                      |
| pprint_pformat          | 1.67 sec                                                     | 2.11 sec: 1.26x slower                                                     |
| async_tree_cpu_io_mixed | 753 ms                                                       | 955 ms: 1.27x slower                                                       |
| pycparser               | 1.31 sec                                                     | 1.67 sec: 1.27x slower                                                     |
| tornado_http            | 124 ms                                                       | 159 ms: 1.28x slower                                                       |
| pprint_safe_repr        | 805 ms                                                       | 1.03 sec: 1.28x slower                                                     |
| async_generators        | 322 ms                                                       | 417 ms: 1.30x slower                                                       |
| unpack_sequence         | 45.7 ns                                                      | 59.3 ns: 1.30x slower                                                      |
| thrift                  | 931 us                                                       | 1.21 ms: 1.30x slower                                                      |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 5.28 ms: 1.30x slower                                                      |
| html5lib                | 72.2 ms                                                      | 94.4 ms: 1.31x slower                                                      |
| async_tree_memoization  | 629 ms                                                       | 832 ms: 1.32x slower                                                       |
| deepcopy_memo           | 37.5 us                                                      | 50.0 us: 1.33x slower                                                      |
| mako                    | 11.0 ms                                                      | 14.7 ms: 1.33x slower                                                      |
| unpickle_pure_python    | 238 us                                                       | 320 us: 1.34x slower                                                       |
| hexiom                  | 6.98 ms                                                      | 9.49 ms: 1.36x slower                                                      |
| scimark_fft             | 281 ms                                                       | 383 ms: 1.36x slower                                                       |
| django_template         | 39.3 ms                                                      | 53.6 ms: 1.36x slower                                                      |
| async_tree_none         | 518 ms                                                       | 711 ms: 1.37x slower                                                       |
| async_tree_io           | 1.17 sec                                                     | 1.62 sec: 1.39x slower                                                     |
| xml_etree_process       | 55.9 ms                                                      | 77.5 ms: 1.39x slower                                                      |
| sqlglot_transpile       | 1.91 ms                                                      | 2.70 ms: 1.41x slower                                                      |
| crypto_pyaes            | 83.3 ms                                                      | 118 ms: 1.42x slower                                                       |
| spectral_norm           | 95.1 ms                                                      | 138 ms: 1.45x slower                                                       |
| chaos                   | 74.9 ms                                                      | 109 ms: 1.45x slower                                                       |
| pickle_pure_python      | 316 us                                                       | 461 us: 1.46x slower                                                       |
| richards                | 49.7 ms                                                      | 72.9 ms: 1.47x slower                                                      |
| float                   | 74.9 ms                                                      | 111 ms: 1.48x slower                                                       |
| nbody                   | 92.9 ms                                                      | 138 ms: 1.48x slower                                                       |
| sqlglot_parse           | 1.51 ms                                                      | 2.25 ms: 1.49x slower                                                      |
| scimark_lu              | 114 ms                                                       | 170 ms: 1.49x slower                                                       |
| bench_mp_pool           | 4.70 ms                                                      | 7.26 ms: 1.54x slower                                                      |
| pyflate                 | 449 ms                                                       | 696 ms: 1.55x slower                                                       |
| scimark_monte_carlo     | 69.8 ms                                                      | 110 ms: 1.57x slower                                                       |
| raytrace                | 309 ms                                                       | 495 ms: 1.60x slower                                                       |
| scimark_sor             | 110 ms                                                       | 177 ms: 1.61x slower                                                       |
| go                      | 158 ms                                                       | 260 ms: 1.65x slower                                                       |
| logging_silent          | 100 ns                                                       | 165 ns: 1.65x slower                                                       |
| deltablue               | 3.97 ms                                                      | 7.45 ms: 1.88x slower                                                      |
| Geometric mean          | (ref)                                                        | 1.23x slower                                                               |

Benchmark hidden because not significant (1): gc_traversal
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.19x
- 95% likely to have a slowdown of 1.18x
- 99% likely to have a slowdown of 1.16x


# Memory

- memory change: 0.95x