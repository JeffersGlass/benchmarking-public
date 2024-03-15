
# Results vs. 3.11.0

- fork: python
- ref: e2b4e4bab90b69fbd361
- machine: linux-x86_64
- commit hash: e2b4e4b
- commit date: 2021-11-05
- overall geometric mean: 1.08x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 299 ms: 1.04x slower                                                        |
| chameleon      | 7.92 ms                                                      | 9.27 ms: 1.17x slower                                                       |
| docutils       | 2.85 sec                                                     | 3.05 sec: 1.07x slower                                                      |
| html5lib       | 72.2 ms                                                      | 80.0 ms: 1.11x slower                                                       |
| tornado_http   | 124 ms                                                       | 136 ms: 1.09x slower                                                        |
| Geometric mean | (ref)                                                        | 1.09x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 518 ms                                                       | 532 ms: 1.03x slower                                                        |
| async_tree_memoization  | 629 ms                                                       | 668 ms: 1.06x slower                                                        |
| async_tree_io           | 1.17 sec                                                     | 1.27 sec: 1.08x slower                                                      |
| async_tree_cpu_io_mixed | 753 ms                                                       | 818 ms: 1.09x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.06x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 264 ms: 1.05x slower                                                        |
| float          | 74.9 ms                                                      | 86.1 ms: 1.15x slower                                                       |
| nbody          | 92.9 ms                                                      | 113 ms: 1.22x slower                                                        |
| Geometric mean | (ref)                                                        | 1.14x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.34 ms                                                      | 3.06 ms: 1.09x faster                                                       |
| regex_compile  | 156 ms                                                       | 158 ms: 1.01x slower                                                        |
| regex_v8       | 24.4 ms                                                      | 25.8 ms: 1.06x slower                                                       |
| regex_dna      | 227 ms                                                       | 262 ms: 1.15x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads           | 28.9 us                                                      | 24.7 us: 1.17x faster                                                       |
| pickle_dict          | 32.3 us                                                      | 30.2 us: 1.07x faster                                                       |
| unpickle_list        | 4.60 us                                                      | 4.55 us: 1.01x faster                                                       |
| unpickle             | 13.3 us                                                      | 13.4 us: 1.01x slower                                                       |
| json_dumps           | 13.3 ms                                                      | 13.4 ms: 1.01x slower                                                       |
| xml_etree_parse      | 155 ms                                                       | 157 ms: 1.02x slower                                                        |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                                       |
| pickle_list          | 3.94 us                                                      | 4.17 us: 1.06x slower                                                       |
| xml_etree_generate   | 79.7 ms                                                      | 85.8 ms: 1.08x slower                                                       |
| xml_etree_process    | 55.9 ms                                                      | 61.7 ms: 1.10x slower                                                       |
| unpickle_pure_python | 238 us                                                       | 277 us: 1.16x slower                                                        |
| pickle_pure_python   | 316 us                                                       | 386 us: 1.22x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.03x slower                                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 7.73 ms                                                      | 7.43 ms: 1.04x faster                                                       |
| python_startup         | 10.7 ms                                                      | 11.2 ms: 1.04x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.00x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| genshi_xml      | 57.1 ms                                                      | 57.9 ms: 1.01x slower                                                       |
| genshi_text     | 25.5 ms                                                      | 28.2 ms: 1.11x slower                                                       |
| mako            | 11.0 ms                                                      | 12.9 ms: 1.17x slower                                                       |
| django_template | 39.3 ms                                                      | 47.4 ms: 1.21x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.12x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads              | 28.9 us                                                      | 24.7 us: 1.17x faster                                                       |
| gc_traversal            | 4.15 ms                                                      | 3.77 ms: 1.10x faster                                                       |
| regex_effbot            | 3.34 ms                                                      | 3.06 ms: 1.09x faster                                                       |
| json                    | 5.58 ms                                                      | 5.19 ms: 1.08x faster                                                       |
| pickle_dict             | 32.3 us                                                      | 30.2 us: 1.07x faster                                                       |
| python_startup_no_site  | 7.73 ms                                                      | 7.43 ms: 1.04x faster                                                       |
| generators              | 54.6 ms                                                      | 52.7 ms: 1.04x faster                                                       |
| meteor_contest          | 131 ms                                                       | 128 ms: 1.02x faster                                                        |
| sympy_sum               | 186 ms                                                       | 183 ms: 1.01x faster                                                        |
| unpickle_list           | 4.60 us                                                      | 4.55 us: 1.01x faster                                                       |
| nqueens                 | 103 ms                                                       | 102 ms: 1.01x faster                                                        |
| unpickle                | 13.3 us                                                      | 13.4 us: 1.01x slower                                                       |
| sympy_str               | 337 ms                                                       | 340 ms: 1.01x slower                                                        |
| async_generators        | 322 ms                                                       | 325 ms: 1.01x slower                                                        |
| regex_compile           | 156 ms                                                       | 158 ms: 1.01x slower                                                        |
| json_dumps              | 13.3 ms                                                      | 13.4 ms: 1.01x slower                                                       |
| gunicorn                | 966 us                                                       | 980 us: 1.01x slower                                                        |
| logging_simple          | 7.24 us                                                      | 7.35 us: 1.01x slower                                                       |
| genshi_xml              | 57.1 ms                                                      | 57.9 ms: 1.01x slower                                                       |
| xml_etree_parse         | 155 ms                                                       | 157 ms: 1.02x slower                                                        |
| sympy_expand            | 553 ms                                                       | 563 ms: 1.02x slower                                                        |
| async_tree_none         | 518 ms                                                       | 532 ms: 1.03x slower                                                        |
| sympy_integrate         | 25.8 ms                                                      | 26.5 ms: 1.03x slower                                                       |
| thrift                  | 931 us                                                       | 961 us: 1.03x slower                                                        |
| mdp                     | 2.77 sec                                                     | 2.87 sec: 1.04x slower                                                      |
| pickle                  | 9.89 us                                                      | 10.3 us: 1.04x slower                                                       |
| coverage                | 66.1 ms                                                      | 68.7 ms: 1.04x slower                                                       |
| python_startup          | 10.7 ms                                                      | 11.2 ms: 1.04x slower                                                       |
| 2to3                    | 287 ms                                                       | 299 ms: 1.04x slower                                                        |
| logging_format          | 7.71 us                                                      | 8.08 us: 1.05x slower                                                       |
| bench_thread_pool       | 1.00 ms                                                      | 1.05 ms: 1.05x slower                                                       |
| pidigits                | 251 ms                                                       | 264 ms: 1.05x slower                                                        |
| regex_v8                | 24.4 ms                                                      | 25.8 ms: 1.06x slower                                                       |
| chaos                   | 74.9 ms                                                      | 79.2 ms: 1.06x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 20.0 ms: 1.06x slower                                                       |
| create_gc_cycles        | 1.58 ms                                                      | 1.67 ms: 1.06x slower                                                       |
| pickle_list             | 3.94 us                                                      | 4.17 us: 1.06x slower                                                       |
| async_tree_memoization  | 629 ms                                                       | 668 ms: 1.06x slower                                                        |
| coroutines              | 27.8 ms                                                      | 29.5 ms: 1.06x slower                                                       |
| bench_mp_pool           | 4.70 ms                                                      | 5.01 ms: 1.07x slower                                                       |
| docutils                | 2.85 sec                                                     | 3.05 sec: 1.07x slower                                                      |
| dulwich_log             | 67.4 ms                                                      | 72.4 ms: 1.07x slower                                                       |
| xml_etree_generate      | 79.7 ms                                                      | 85.8 ms: 1.08x slower                                                       |
| async_tree_io           | 1.17 sec                                                     | 1.27 sec: 1.08x slower                                                      |
| dask                    | 410 ms                                                       | 445 ms: 1.09x slower                                                        |
| async_tree_cpu_io_mixed | 753 ms                                                       | 818 ms: 1.09x slower                                                        |
| sqlglot_normalize       | 122 ms                                                       | 132 ms: 1.09x slower                                                        |
| tornado_http            | 124 ms                                                       | 136 ms: 1.09x slower                                                        |
| pprint_safe_repr        | 805 ms                                                       | 877 ms: 1.09x slower                                                        |
| sqlite_synth            | 2.52 us                                                      | 2.75 us: 1.09x slower                                                       |
| pprint_pformat          | 1.67 sec                                                     | 1.82 sec: 1.09x slower                                                      |
| deepcopy                | 391 us                                                       | 428 us: 1.09x slower                                                        |
| spectral_norm           | 95.1 ms                                                      | 104 ms: 1.10x slower                                                        |
| sqlglot_optimize        | 59.0 ms                                                      | 64.9 ms: 1.10x slower                                                       |
| fannkuch                | 416 ms                                                       | 458 ms: 1.10x slower                                                        |
| xml_etree_process       | 55.9 ms                                                      | 61.7 ms: 1.10x slower                                                       |
| genshi_text             | 25.5 ms                                                      | 28.2 ms: 1.11x slower                                                       |
| html5lib                | 72.2 ms                                                      | 80.0 ms: 1.11x slower                                                       |
| scimark_fft             | 281 ms                                                       | 311 ms: 1.11x slower                                                        |
| scimark_sparse_mat_mult | 4.06 ms                                                      | 4.56 ms: 1.12x slower                                                       |
| deepcopy_reduce         | 3.40 us                                                      | 3.81 us: 1.12x slower                                                       |
| hexiom                  | 6.98 ms                                                      | 7.87 ms: 1.13x slower                                                       |
| raytrace                | 309 ms                                                       | 349 ms: 1.13x slower                                                        |
| pycparser               | 1.31 sec                                                     | 1.48 sec: 1.13x slower                                                      |
| scimark_monte_carlo     | 69.8 ms                                                      | 79.5 ms: 1.14x slower                                                       |
| crypto_pyaes            | 83.3 ms                                                      | 94.9 ms: 1.14x slower                                                       |
| deepcopy_memo           | 37.5 us                                                      | 42.9 us: 1.14x slower                                                       |
| comprehensions          | 25.1 us                                                      | 28.8 us: 1.15x slower                                                       |
| float                   | 74.9 ms                                                      | 86.1 ms: 1.15x slower                                                       |
| regex_dna               | 227 ms                                                       | 262 ms: 1.15x slower                                                        |
| scimark_lu              | 114 ms                                                       | 132 ms: 1.16x slower                                                        |
| unpickle_pure_python    | 238 us                                                       | 277 us: 1.16x slower                                                        |
| chameleon               | 7.92 ms                                                      | 9.27 ms: 1.17x slower                                                       |
| mako                    | 11.0 ms                                                      | 12.9 ms: 1.17x slower                                                       |
| richards                | 49.7 ms                                                      | 59.0 ms: 1.19x slower                                                       |
| logging_silent          | 100 ns                                                       | 121 ns: 1.20x slower                                                        |
| django_template         | 39.3 ms                                                      | 47.4 ms: 1.21x slower                                                       |
| nbody                   | 92.9 ms                                                      | 113 ms: 1.22x slower                                                        |
| pickle_pure_python      | 316 us                                                       | 386 us: 1.22x slower                                                        |
| go                      | 158 ms                                                       | 194 ms: 1.23x slower                                                        |
| flaskblogging           | 3.88 ms                                                      | 4.84 ms: 1.25x slower                                                       |
| scimark_sor             | 110 ms                                                       | 140 ms: 1.27x slower                                                        |
| deltablue               | 3.97 ms                                                      | 5.07 ms: 1.28x slower                                                       |
| pyflate                 | 449 ms                                                       | 582 ms: 1.29x slower                                                        |
| sqlglot_transpile       | 1.91 ms                                                      | 2.63 ms: 1.38x slower                                                       |
| sqlglot_parse           | 1.51 ms                                                      | 2.24 ms: 1.48x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.08x slower                                                                |

Benchmark hidden because not significant (3): telco, xml_etree_iterparse, unpack_sequence
Ignored benchmarks (15) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.07x
- 95% likely to have a slowdown of 1.06x
- 99% likely to have a slowdown of 1.05x


# Memory

- memory change: 0.99x