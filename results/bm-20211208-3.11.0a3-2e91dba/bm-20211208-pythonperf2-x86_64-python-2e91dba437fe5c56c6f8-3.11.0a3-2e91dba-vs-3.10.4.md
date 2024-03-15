
# Results vs. 3.10.4

- fork: python
- ref: 2e91dba437fe5c56c6f8
- machine: linux-x86_64
- commit hash: 2e91dba
- commit date: 2021-12-08
- overall geometric mean: 1.15x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: 1.13x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 293 ms: 1.19x faster                                                        |
| chameleon      | 9.44 ms                                                      | 8.85 ms: 1.07x faster                                                       |
| docutils       | 3.41 sec                                                     | 3.02 sec: 1.13x faster                                                      |
| html5lib       | 94.6 ms                                                      | 75.1 ms: 1.26x faster                                                       |
| tornado_http   | 157 ms                                                       | 135 ms: 1.17x faster                                                        |
| Geometric mean | (ref)                                                        | 1.16x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 545 ms: 1.27x faster                                                        |
| async_tree_io           | 1.60 sec                                                     | 1.32 sec: 1.21x faster                                                      |
| async_tree_memoization  | 819 ms                                                       | 686 ms: 1.19x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 811 ms: 1.15x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.21x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 80.9 ms: 1.37x faster                                                       |
| nbody          | 134 ms                                                       | 109 ms: 1.24x faster                                                        |
| pidigits       | 271 ms                                                       | 253 ms: 1.07x faster                                                        |
| Geometric mean | (ref)                                                        | 1.22x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 153 ms: 1.24x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 25.7 ms: 1.05x faster                                                       |
| regex_dna      | 261 ms                                                       | 261 ms: 1.00x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.10 ms: 1.00x slower                                                       |
| Geometric mean | (ref)                                                        | 1.07x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| xml_etree_process    | 75.9 ms                                                      | 60.9 ms: 1.25x faster                                                       |
| pickle_pure_python   | 455 us                                                       | 366 us: 1.24x faster                                                        |
| json_loads           | 30.3 us                                                      | 25.3 us: 1.20x faster                                                       |
| unpickle_pure_python | 312 us                                                       | 265 us: 1.18x faster                                                        |
| xml_etree_generate   | 92.3 ms                                                      | 82.8 ms: 1.11x faster                                                       |
| json_dumps           | 14.5 ms                                                      | 14.1 ms: 1.04x faster                                                       |
| xml_etree_parse      | 160 ms                                                       | 155 ms: 1.03x faster                                                        |
| unpickle_list        | 4.65 us                                                      | 4.53 us: 1.02x faster                                                       |
| unpickle             | 13.5 us                                                      | 13.2 us: 1.02x faster                                                       |
| pickle               | 9.89 us                                                      | 10.2 us: 1.04x slower                                                       |
| pickle_list          | 4.12 us                                                      | 4.32 us: 1.05x slower                                                       |
| pickle_dict          | 29.5 us                                                      | 33.0 us: 1.12x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.06x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.1 ms: 1.14x faster                                                       |
| python_startup_no_site | 7.33 ms                                                      | 7.14 ms: 1.03x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.08x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 12.9 ms: 1.14x faster                                                       |
| django_template | 50.2 ms                                                      | 44.9 ms: 1.12x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 28.2 ms: 1.11x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 59.7 ms: 1.06x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.11x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211208-pythonperf2-x86_64-python-2e91dba437fe5c56c6f8-3.11.0a3-2e91dba |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 4.78 ms: 1.57x faster                                                       |
| scimark_sor             | 180 ms                                                       | 115 ms: 1.56x faster                                                        |
| scimark_lu              | 167 ms                                                       | 110 ms: 1.52x faster                                                        |
| go                      | 262 ms                                                       | 173 ms: 1.52x faster                                                        |
| logging_silent          | 167 ns                                                       | 116 ns: 1.44x faster                                                        |
| raytrace                | 489 ms                                                       | 347 ms: 1.41x faster                                                        |
| scimark_monte_carlo     | 107 ms                                                       | 76.7 ms: 1.40x faster                                                       |
| pyflate                 | 733 ms                                                       | 525 ms: 1.40x faster                                                        |
| spectral_norm           | 139 ms                                                       | 99.9 ms: 1.39x faster                                                       |
| chaos                   | 109 ms                                                       | 78.3 ms: 1.39x faster                                                       |
| float                   | 111 ms                                                       | 80.9 ms: 1.37x faster                                                       |
| richards                | 75.1 ms                                                      | 56.7 ms: 1.32x faster                                                       |
| async_generators        | 421 ms                                                       | 319 ms: 1.32x faster                                                        |
| bench_mp_pool           | 6.37 ms                                                      | 4.90 ms: 1.30x faster                                                       |
| unpack_sequence         | 59.9 ns                                                      | 46.3 ns: 1.29x faster                                                       |
| hexiom                  | 9.42 ms                                                      | 7.41 ms: 1.27x faster                                                       |
| async_tree_none         | 692 ms                                                       | 545 ms: 1.27x faster                                                        |
| pprint_safe_repr        | 1.05 sec                                                     | 832 ms: 1.26x faster                                                        |
| logging_simple          | 8.88 us                                                      | 7.04 us: 1.26x faster                                                       |
| html5lib                | 94.6 ms                                                      | 75.1 ms: 1.26x faster                                                       |
| crypto_pyaes            | 119 ms                                                       | 94.7 ms: 1.26x faster                                                       |
| logging_format          | 9.64 us                                                      | 7.70 us: 1.25x faster                                                       |
| xml_etree_process       | 75.9 ms                                                      | 60.9 ms: 1.25x faster                                                       |
| regex_compile           | 190 ms                                                       | 153 ms: 1.24x faster                                                        |
| pickle_pure_python      | 455 us                                                       | 366 us: 1.24x faster                                                        |
| pycparser               | 1.67 sec                                                     | 1.35 sec: 1.24x faster                                                      |
| pprint_pformat          | 2.15 sec                                                     | 1.74 sec: 1.24x faster                                                      |
| nbody                   | 134 ms                                                       | 109 ms: 1.24x faster                                                        |
| async_tree_io           | 1.60 sec                                                     | 1.32 sec: 1.21x faster                                                      |
| deepcopy_memo           | 49.8 us                                                      | 41.5 us: 1.20x faster                                                       |
| json_loads              | 30.3 us                                                      | 25.3 us: 1.20x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 686 ms: 1.19x faster                                                        |
| 2to3                    | 350 ms                                                       | 293 ms: 1.19x faster                                                        |
| thrift                  | 1.18 ms                                                      | 995 us: 1.18x faster                                                        |
| unpickle_pure_python    | 312 us                                                       | 265 us: 1.18x faster                                                        |
| tornado_http            | 157 ms                                                       | 135 ms: 1.17x faster                                                        |
| gunicorn                | 1.16 ms                                                      | 1.00 ms: 1.16x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 811 ms: 1.15x faster                                                        |
| scimark_fft             | 361 ms                                                       | 314 ms: 1.15x faster                                                        |
| generators              | 57.3 ms                                                      | 50.1 ms: 1.14x faster                                                       |
| mako                    | 14.7 ms                                                      | 12.9 ms: 1.14x faster                                                       |
| python_startup          | 11.5 ms                                                      | 10.1 ms: 1.14x faster                                                       |
| docutils                | 3.41 sec                                                     | 3.02 sec: 1.13x faster                                                      |
| deepcopy_reduce         | 4.01 us                                                      | 3.55 us: 1.13x faster                                                       |
| fannkuch                | 483 ms                                                       | 428 ms: 1.13x faster                                                        |
| coroutines              | 30.3 ms                                                      | 27.0 ms: 1.12x faster                                                       |
| deepcopy                | 468 us                                                       | 418 us: 1.12x faster                                                        |
| json                    | 5.86 ms                                                      | 5.24 ms: 1.12x faster                                                       |
| django_template         | 50.2 ms                                                      | 44.9 ms: 1.12x faster                                                       |
| nqueens                 | 115 ms                                                       | 103 ms: 1.12x faster                                                        |
| xml_etree_generate      | 92.3 ms                                                      | 82.8 ms: 1.11x faster                                                       |
| genshi_text             | 31.4 ms                                                      | 28.2 ms: 1.11x faster                                                       |
| dulwich_log             | 81.1 ms                                                      | 73.0 ms: 1.11x faster                                                       |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 4.58 ms: 1.11x faster                                                       |
| sqlite_synth            | 2.99 us                                                      | 2.70 us: 1.11x faster                                                       |
| mdp                     | 3.01 sec                                                     | 2.76 sec: 1.09x faster                                                      |
| dask                    | 472 ms                                                       | 435 ms: 1.09x faster                                                        |
| sqlglot_optimize        | 70.1 ms                                                      | 64.7 ms: 1.08x faster                                                       |
| sqlglot_normalize       | 144 ms                                                       | 133 ms: 1.08x faster                                                        |
| bench_thread_pool       | 1.14 ms                                                      | 1.06 ms: 1.08x faster                                                       |
| meteor_contest          | 138 ms                                                       | 129 ms: 1.07x faster                                                        |
| pathlib                 | 21.4 ms                                                      | 19.9 ms: 1.07x faster                                                       |
| pidigits                | 271 ms                                                       | 253 ms: 1.07x faster                                                        |
| chameleon               | 9.44 ms                                                      | 8.85 ms: 1.07x faster                                                       |
| create_gc_cycles        | 1.76 ms                                                      | 1.66 ms: 1.06x faster                                                       |
| sympy_integrate         | 28.2 ms                                                      | 26.5 ms: 1.06x faster                                                       |
| genshi_xml              | 63.3 ms                                                      | 59.7 ms: 1.06x faster                                                       |
| regex_v8                | 27.2 ms                                                      | 25.7 ms: 1.05x faster                                                       |
| sympy_expand            | 600 ms                                                       | 579 ms: 1.04x faster                                                        |
| json_dumps              | 14.5 ms                                                      | 14.1 ms: 1.04x faster                                                       |
| sqlglot_transpile       | 2.68 ms                                                      | 2.60 ms: 1.03x faster                                                       |
| xml_etree_parse         | 160 ms                                                       | 155 ms: 1.03x faster                                                        |
| sympy_str               | 360 ms                                                       | 350 ms: 1.03x faster                                                        |
| python_startup_no_site  | 7.33 ms                                                      | 7.14 ms: 1.03x faster                                                       |
| unpickle_list           | 4.65 us                                                      | 4.53 us: 1.02x faster                                                       |
| unpickle                | 13.5 us                                                      | 13.2 us: 1.02x faster                                                       |
| sympy_sum               | 193 ms                                                       | 189 ms: 1.02x faster                                                        |
| telco                   | 7.23 ms                                                      | 7.11 ms: 1.02x faster                                                       |
| sqlglot_parse           | 2.24 ms                                                      | 2.21 ms: 1.01x faster                                                       |
| regex_dna               | 261 ms                                                       | 261 ms: 1.00x faster                                                        |
| regex_effbot            | 3.09 ms                                                      | 3.10 ms: 1.00x slower                                                       |
| pickle                  | 9.89 us                                                      | 10.2 us: 1.04x slower                                                       |
| pickle_list             | 4.12 us                                                      | 4.32 us: 1.05x slower                                                       |
| pickle_dict             | 29.5 us                                                      | 33.0 us: 1.12x slower                                                       |
| flaskblogging           | 4.39 ms                                                      | 4.95 ms: 1.13x slower                                                       |
| gc_traversal            | 3.42 ms                                                      | 3.89 ms: 1.14x slower                                                       |
| coverage                | 63.3 ms                                                      | 72.1 ms: 1.14x slower                                                       |
| comprehensions          | 26.7 us                                                      | 30.6 us: 1.15x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.15x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: 1.13x