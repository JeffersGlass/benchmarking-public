
# Results vs. 3.10.4

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: linux-x86_64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.24x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 281 ms: 1.25x faster                                                        |
| chameleon      | 9.44 ms                                                      | 7.51 ms: 1.26x faster                                                       |
| docutils       | 3.41 sec                                                     | 2.76 sec: 1.24x faster                                                      |
| html5lib       | 94.6 ms                                                      | 66.2 ms: 1.43x faster                                                       |
| Geometric mean | (ref)                                                        | 1.29x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.18 sec: 1.36x faster                                                      |
| async_tree_memoization  | 819 ms                                                       | 623 ms: 1.31x faster                                                        |
| async_tree_none         | 692 ms                                                       | 531 ms: 1.30x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 767 ms: 1.22x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.30x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 73.2 ms: 1.52x faster                                                       |
| nbody          | 134 ms                                                       | 94.3 ms: 1.42x faster                                                       |
| pidigits       | 271 ms                                                       | 250 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                        | 1.33x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 150 ms: 1.27x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 22.3 ms: 1.22x faster                                                       |
| regex_dna      | 261 ms                                                       | 233 ms: 1.12x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.44 ms: 1.11x slower                                                       |
| Geometric mean | (ref)                                                        | 1.12x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 212 us: 1.47x faster                                                        |
| pickle_pure_python   | 455 us                                                       | 316 us: 1.44x faster                                                        |
| json_dumps           | 14.5 ms                                                      | 10.3 ms: 1.41x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 55.6 ms: 1.36x faster                                                       |
| json_loads           | 30.3 us                                                      | 24.2 us: 1.25x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 78.9 ms: 1.17x faster                                                       |
| xml_etree_parse      | 160 ms                                                       | 141 ms: 1.14x faster                                                        |
| pickle_list          | 4.12 us                                                      | 3.90 us: 1.06x faster                                                       |
| unpickle_list        | 4.65 us                                                      | 4.47 us: 1.04x faster                                                       |
| unpickle             | 13.5 us                                                      | 13.1 us: 1.03x faster                                                       |
| xml_etree_iterparse  | 110 ms                                                       | 108 ms: 1.03x faster                                                        |
| pickle               | 9.89 us                                                      | 9.84 us: 1.01x faster                                                       |
| pickle_dict          | 29.5 us                                                      | 31.9 us: 1.08x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.17x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.8 ms: 1.07x faster                                                       |
| python_startup_no_site | 7.33 ms                                                      | 7.86 ms: 1.07x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.00x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.4 ms: 1.42x faster                                                       |
| django_template | 50.2 ms                                                      | 39.6 ms: 1.27x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 25.8 ms: 1.22x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 53.5 ms: 1.18x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.27x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 3.67 ms: 2.04x faster                                                       |
| logging_silent          | 167 ns                                                       | 99.7 ns: 1.68x faster                                                       |
| scimark_lu              | 167 ms                                                       | 100 ms: 1.67x faster                                                        |
| pyflate                 | 733 ms                                                       | 440 ms: 1.67x faster                                                        |
| scimark_sor             | 180 ms                                                       | 109 ms: 1.65x faster                                                        |
| go                      | 262 ms                                                       | 159 ms: 1.64x faster                                                        |
| richards                | 75.1 ms                                                      | 46.1 ms: 1.63x faster                                                       |
| float                   | 111 ms                                                       | 73.2 ms: 1.52x faster                                                       |
| raytrace                | 489 ms                                                       | 327 ms: 1.50x faster                                                        |
| scimark_monte_carlo     | 107 ms                                                       | 72.7 ms: 1.48x faster                                                       |
| sqlglot_parse           | 2.24 ms                                                      | 1.52 ms: 1.48x faster                                                       |
| unpickle_pure_python    | 312 us                                                       | 212 us: 1.47x faster                                                        |
| crypto_pyaes            | 119 ms                                                       | 81.8 ms: 1.46x faster                                                       |
| spectral_norm           | 139 ms                                                       | 96.2 ms: 1.45x faster                                                       |
| pickle_pure_python      | 455 us                                                       | 316 us: 1.44x faster                                                        |
| sqlglot_transpile       | 2.68 ms                                                      | 1.87 ms: 1.43x faster                                                       |
| html5lib                | 94.6 ms                                                      | 66.2 ms: 1.43x faster                                                       |
| bench_mp_pool           | 6.37 ms                                                      | 4.46 ms: 1.43x faster                                                       |
| nbody                   | 134 ms                                                       | 94.3 ms: 1.42x faster                                                       |
| mako                    | 14.7 ms                                                      | 10.4 ms: 1.42x faster                                                       |
| json_dumps              | 14.5 ms                                                      | 10.3 ms: 1.41x faster                                                       |
| hexiom                  | 9.42 ms                                                      | 6.73 ms: 1.40x faster                                                       |
| chaos                   | 109 ms                                                       | 78.3 ms: 1.39x faster                                                       |
| pprint_safe_repr        | 1.05 sec                                                     | 758 ms: 1.38x faster                                                        |
| pprint_pformat          | 2.15 sec                                                     | 1.56 sec: 1.38x faster                                                      |
| deepcopy_memo           | 49.8 us                                                      | 36.2 us: 1.37x faster                                                       |
| xml_etree_process       | 75.9 ms                                                      | 55.6 ms: 1.36x faster                                                       |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 3.73 ms: 1.36x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.18 sec: 1.36x faster                                                      |
| pycparser               | 1.67 sec                                                     | 1.26 sec: 1.33x faster                                                      |
| unpack_sequence         | 59.9 ns                                                      | 45.5 ns: 1.32x faster                                                       |
| thrift                  | 1.18 ms                                                      | 894 us: 1.32x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 623 ms: 1.31x faster                                                        |
| async_tree_none         | 692 ms                                                       | 531 ms: 1.30x faster                                                        |
| scimark_fft             | 361 ms                                                       | 282 ms: 1.28x faster                                                        |
| regex_compile           | 190 ms                                                       | 150 ms: 1.27x faster                                                        |
| django_template         | 50.2 ms                                                      | 39.6 ms: 1.27x faster                                                       |
| logging_simple          | 8.88 us                                                      | 7.03 us: 1.26x faster                                                       |
| chameleon               | 9.44 ms                                                      | 7.51 ms: 1.26x faster                                                       |
| async_generators        | 421 ms                                                       | 335 ms: 1.25x faster                                                        |
| json_loads              | 30.3 us                                                      | 24.2 us: 1.25x faster                                                       |
| logging_format          | 9.64 us                                                      | 7.72 us: 1.25x faster                                                       |
| 2to3                    | 350 ms                                                       | 281 ms: 1.25x faster                                                        |
| docutils                | 3.41 sec                                                     | 2.76 sec: 1.24x faster                                                      |
| deepcopy                | 468 us                                                       | 380 us: 1.23x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 767 ms: 1.22x faster                                                        |
| genshi_text             | 31.4 ms                                                      | 25.8 ms: 1.22x faster                                                       |
| regex_v8                | 27.2 ms                                                      | 22.3 ms: 1.22x faster                                                       |
| dulwich_log             | 81.1 ms                                                      | 66.7 ms: 1.22x faster                                                       |
| fannkuch                | 483 ms                                                       | 398 ms: 1.21x faster                                                        |
| sqlglot_optimize        | 70.1 ms                                                      | 58.5 ms: 1.20x faster                                                       |
| deepcopy_reduce         | 4.01 us                                                      | 3.37 us: 1.19x faster                                                       |
| sqlglot_normalize       | 144 ms                                                       | 121 ms: 1.19x faster                                                        |
| genshi_xml              | 63.3 ms                                                      | 53.5 ms: 1.18x faster                                                       |
| xml_etree_generate      | 92.3 ms                                                      | 78.9 ms: 1.17x faster                                                       |
| dask                    | 472 ms                                                       | 409 ms: 1.15x faster                                                        |
| json                    | 5.86 ms                                                      | 5.11 ms: 1.15x faster                                                       |
| sqlite_synth            | 2.99 us                                                      | 2.60 us: 1.15x faster                                                       |
| bench_thread_pool       | 1.14 ms                                                      | 994 us: 1.15x faster                                                        |
| xml_etree_parse         | 160 ms                                                       | 141 ms: 1.14x faster                                                        |
| nqueens                 | 115 ms                                                       | 102 ms: 1.13x faster                                                        |
| pathlib                 | 21.4 ms                                                      | 19.0 ms: 1.12x faster                                                       |
| regex_dna               | 261 ms                                                       | 233 ms: 1.12x faster                                                        |
| sympy_expand            | 600 ms                                                       | 539 ms: 1.11x faster                                                        |
| create_gc_cycles        | 1.76 ms                                                      | 1.60 ms: 1.10x faster                                                       |
| sympy_integrate         | 28.2 ms                                                      | 25.6 ms: 1.10x faster                                                       |
| mdp                     | 3.01 sec                                                     | 2.73 sec: 1.10x faster                                                      |
| telco                   | 7.23 ms                                                      | 6.60 ms: 1.09x faster                                                       |
| sympy_str               | 360 ms                                                       | 331 ms: 1.09x faster                                                        |
| coroutines              | 30.3 ms                                                      | 28.0 ms: 1.08x faster                                                       |
| pidigits                | 271 ms                                                       | 250 ms: 1.08x faster                                                        |
| meteor_contest          | 138 ms                                                       | 129 ms: 1.07x faster                                                        |
| python_startup          | 11.5 ms                                                      | 10.8 ms: 1.07x faster                                                       |
| pickle_list             | 4.12 us                                                      | 3.90 us: 1.06x faster                                                       |
| sympy_sum               | 193 ms                                                       | 183 ms: 1.05x faster                                                        |
| asyncio_tcp             | 779 ms                                                       | 743 ms: 1.05x faster                                                        |
| unpickle_list           | 4.65 us                                                      | 4.47 us: 1.04x faster                                                       |
| unpickle                | 13.5 us                                                      | 13.1 us: 1.03x faster                                                       |
| xml_etree_iterparse     | 110 ms                                                       | 108 ms: 1.03x faster                                                        |
| pickle                  | 9.89 us                                                      | 9.84 us: 1.01x faster                                                       |
| comprehensions          | 26.7 us                                                      | 27.3 us: 1.02x slower                                                       |
| generators              | 57.3 ms                                                      | 60.8 ms: 1.06x slower                                                       |
| python_startup_no_site  | 7.33 ms                                                      | 7.86 ms: 1.07x slower                                                       |
| pickle_dict             | 29.5 us                                                      | 31.9 us: 1.08x slower                                                       |
| gc_traversal            | 3.42 ms                                                      | 3.79 ms: 1.11x slower                                                       |
| regex_effbot            | 3.09 ms                                                      | 3.44 ms: 1.11x slower                                                       |
| coverage                | 63.3 ms                                                      | 85.0 ms: 1.34x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.24x faster                                                                |
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.21x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: 1.10x