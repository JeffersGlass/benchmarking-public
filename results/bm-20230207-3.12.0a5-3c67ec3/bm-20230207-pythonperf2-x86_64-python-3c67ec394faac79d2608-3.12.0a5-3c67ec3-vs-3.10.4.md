
# Results vs. 3.10.4

- fork: python
- ref: 3c67ec394faac79d2608
- machine: linux-x86_64
- commit hash: 3c67ec3
- commit date: 2023-02-07
- overall geometric mean: 1.26x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 282 ms: 1.24x faster                                                        |
| chameleon      | 9.44 ms                                                      | 7.46 ms: 1.27x faster                                                       |
| docutils       | 3.41 sec                                                     | 2.78 sec: 1.23x faster                                                      |
| html5lib       | 94.6 ms                                                      | 65.3 ms: 1.45x faster                                                       |
| tornado_http   | 157 ms                                                       | 117 ms: 1.34x faster                                                        |
| Geometric mean | (ref)                                                        | 1.30x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 503 ms: 1.37x faster                                                        |
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.37x faster                                                      |
| async_tree_memoization  | 819 ms                                                       | 601 ms: 1.36x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 737 ms: 1.27x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.34x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 71.9 ms: 1.55x faster                                                       |
| nbody          | 134 ms                                                       | 101 ms: 1.32x faster                                                        |
| pidigits       | 271 ms                                                       | 251 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                        | 1.30x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 145 ms: 1.31x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 22.7 ms: 1.20x faster                                                       |
| regex_dna      | 261 ms                                                       | 240 ms: 1.09x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                                       |
| Geometric mean | (ref)                                                        | 1.11x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 204 us: 1.53x faster                                                        |
| pickle_pure_python   | 455 us                                                       | 312 us: 1.46x faster                                                        |
| json_dumps           | 14.5 ms                                                      | 10.0 ms: 1.45x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 55.6 ms: 1.36x faster                                                       |
| json_loads           | 30.3 us                                                      | 23.8 us: 1.27x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 80.6 ms: 1.14x faster                                                       |
| xml_etree_parse      | 160 ms                                                       | 142 ms: 1.13x faster                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 103 ms: 1.08x faster                                                        |
| pickle_list          | 4.12 us                                                      | 3.84 us: 1.07x faster                                                       |
| unpickle             | 13.5 us                                                      | 12.8 us: 1.05x faster                                                       |
| unpickle_list        | 4.65 us                                                      | 4.50 us: 1.03x faster                                                       |
| pickle_dict          | 29.5 us                                                      | 31.6 us: 1.07x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.18x faster                                                                |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 11.2 ms: 1.03x faster                                                       |
| python_startup_no_site | 7.33 ms                                                      | 8.25 ms: 1.13x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.05x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.3 ms: 1.43x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 24.6 ms: 1.28x faster                                                       |
| django_template | 50.2 ms                                                      | 40.5 ms: 1.24x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 53.4 ms: 1.19x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.28x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 3.60 ms: 2.09x faster                                                       |
| asyncio_tcp             | 779 ms                                                       | 388 ms: 2.01x faster                                                        |
| logging_silent          | 167 ns                                                       | 96.5 ns: 1.73x faster                                                       |
| go                      | 262 ms                                                       | 152 ms: 1.72x faster                                                        |
| scimark_sor             | 180 ms                                                       | 105 ms: 1.72x faster                                                        |
| pyflate                 | 733 ms                                                       | 428 ms: 1.71x faster                                                        |
| richards                | 75.1 ms                                                      | 46.1 ms: 1.63x faster                                                       |
| raytrace                | 489 ms                                                       | 301 ms: 1.63x faster                                                        |
| scimark_lu              | 167 ms                                                       | 104 ms: 1.61x faster                                                        |
| chaos                   | 109 ms                                                       | 69.6 ms: 1.56x faster                                                       |
| float                   | 111 ms                                                       | 71.9 ms: 1.55x faster                                                       |
| scimark_monte_carlo     | 107 ms                                                       | 70.2 ms: 1.53x faster                                                       |
| unpickle_pure_python    | 312 us                                                       | 204 us: 1.53x faster                                                        |
| pickle_pure_python      | 455 us                                                       | 312 us: 1.46x faster                                                        |
| spectral_norm           | 139 ms                                                       | 95.4 ms: 1.46x faster                                                       |
| crypto_pyaes            | 119 ms                                                       | 81.8 ms: 1.46x faster                                                       |
| hexiom                  | 9.42 ms                                                      | 6.49 ms: 1.45x faster                                                       |
| json_dumps              | 14.5 ms                                                      | 10.0 ms: 1.45x faster                                                       |
| html5lib                | 94.6 ms                                                      | 65.3 ms: 1.45x faster                                                       |
| sqlglot_parse           | 2.24 ms                                                      | 1.56 ms: 1.44x faster                                                       |
| mako                    | 14.7 ms                                                      | 10.3 ms: 1.43x faster                                                       |
| pprint_safe_repr        | 1.05 sec                                                     | 744 ms: 1.41x faster                                                        |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 3.61 ms: 1.41x faster                                                       |
| pprint_pformat          | 2.15 sec                                                     | 1.53 sec: 1.41x faster                                                      |
| sqlglot_transpile       | 2.68 ms                                                      | 1.93 ms: 1.39x faster                                                       |
| deepcopy_memo           | 49.8 us                                                      | 35.8 us: 1.39x faster                                                       |
| unpack_sequence         | 59.9 ns                                                      | 43.3 ns: 1.38x faster                                                       |
| async_tree_none         | 692 ms                                                       | 503 ms: 1.37x faster                                                        |
| async_tree_io           | 1.60 sec                                                     | 1.17 sec: 1.37x faster                                                      |
| xml_etree_process       | 75.9 ms                                                      | 55.6 ms: 1.36x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 601 ms: 1.36x faster                                                        |
| bench_mp_pool           | 6.37 ms                                                      | 4.71 ms: 1.35x faster                                                       |
| tornado_http            | 157 ms                                                       | 117 ms: 1.34x faster                                                        |
| logging_simple          | 8.88 us                                                      | 6.67 us: 1.33x faster                                                       |
| nbody                   | 134 ms                                                       | 101 ms: 1.32x faster                                                        |
| regex_compile           | 190 ms                                                       | 145 ms: 1.31x faster                                                        |
| pycparser               | 1.67 sec                                                     | 1.28 sec: 1.31x faster                                                      |
| scimark_fft             | 361 ms                                                       | 278 ms: 1.30x faster                                                        |
| logging_format          | 9.64 us                                                      | 7.43 us: 1.30x faster                                                       |
| async_generators        | 421 ms                                                       | 325 ms: 1.30x faster                                                        |
| genshi_text             | 31.4 ms                                                      | 24.6 ms: 1.28x faster                                                       |
| json_loads              | 30.3 us                                                      | 23.8 us: 1.27x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 737 ms: 1.27x faster                                                        |
| chameleon               | 9.44 ms                                                      | 7.46 ms: 1.27x faster                                                       |
| thrift                  | 1.18 ms                                                      | 935 us: 1.26x faster                                                        |
| comprehensions          | 26.7 us                                                      | 21.3 us: 1.25x faster                                                       |
| 2to3                    | 350 ms                                                       | 282 ms: 1.24x faster                                                        |
| django_template         | 50.2 ms                                                      | 40.5 ms: 1.24x faster                                                       |
| docutils                | 3.41 sec                                                     | 2.78 sec: 1.23x faster                                                      |
| deepcopy                | 468 us                                                       | 383 us: 1.22x faster                                                        |
| nqueens                 | 115 ms                                                       | 94.2 ms: 1.22x faster                                                       |
| dulwich_log             | 81.1 ms                                                      | 66.6 ms: 1.22x faster                                                       |
| sqlglot_optimize        | 70.1 ms                                                      | 57.7 ms: 1.21x faster                                                       |
| deepcopy_reduce         | 4.01 us                                                      | 3.30 us: 1.21x faster                                                       |
| regex_v8                | 27.2 ms                                                      | 22.7 ms: 1.20x faster                                                       |
| sqlglot_normalize       | 144 ms                                                       | 120 ms: 1.19x faster                                                        |
| json                    | 5.86 ms                                                      | 4.94 ms: 1.19x faster                                                       |
| genshi_xml              | 63.3 ms                                                      | 53.4 ms: 1.19x faster                                                       |
| fannkuch                | 483 ms                                                       | 409 ms: 1.18x faster                                                        |
| bench_thread_pool       | 1.14 ms                                                      | 971 us: 1.18x faster                                                        |
| sqlite_synth            | 2.99 us                                                      | 2.58 us: 1.16x faster                                                       |
| sympy_integrate         | 28.2 ms                                                      | 24.3 ms: 1.16x faster                                                       |
| sympy_str               | 360 ms                                                       | 313 ms: 1.15x faster                                                        |
| xml_etree_generate      | 92.3 ms                                                      | 80.6 ms: 1.14x faster                                                       |
| sympy_expand            | 600 ms                                                       | 526 ms: 1.14x faster                                                        |
| mdp                     | 3.01 sec                                                     | 2.66 sec: 1.13x faster                                                      |
| xml_etree_parse         | 160 ms                                                       | 142 ms: 1.13x faster                                                        |
| sympy_sum               | 193 ms                                                       | 172 ms: 1.12x faster                                                        |
| pathlib                 | 21.4 ms                                                      | 19.1 ms: 1.12x faster                                                       |
| telco                   | 7.23 ms                                                      | 6.59 ms: 1.10x faster                                                       |
| regex_dna               | 261 ms                                                       | 240 ms: 1.09x faster                                                        |
| pidigits                | 271 ms                                                       | 251 ms: 1.08x faster                                                        |
| meteor_contest          | 138 ms                                                       | 128 ms: 1.08x faster                                                        |
| xml_etree_iterparse     | 110 ms                                                       | 103 ms: 1.08x faster                                                        |
| create_gc_cycles        | 1.76 ms                                                      | 1.64 ms: 1.07x faster                                                       |
| pickle_list             | 4.12 us                                                      | 3.84 us: 1.07x faster                                                       |
| unpickle                | 13.5 us                                                      | 12.8 us: 1.05x faster                                                       |
| coroutines              | 30.3 ms                                                      | 29.1 ms: 1.04x faster                                                       |
| unpickle_list           | 4.65 us                                                      | 4.50 us: 1.03x faster                                                       |
| python_startup          | 11.5 ms                                                      | 11.2 ms: 1.03x faster                                                       |
| gc_traversal            | 3.42 ms                                                      | 3.55 ms: 1.04x slower                                                       |
| generators              | 57.3 ms                                                      | 60.4 ms: 1.05x slower                                                       |
| pickle_dict             | 29.5 us                                                      | 31.6 us: 1.07x slower                                                       |
| python_startup_no_site  | 7.33 ms                                                      | 8.25 ms: 1.13x slower                                                       |
| regex_effbot            | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                                       |
| dask                    | 472 ms                                                       | 562 ms: 1.19x slower                                                        |
| coverage                | 63.3 ms                                                      | 86.0 ms: 1.36x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.26x faster                                                                |

Benchmark hidden because not significant (1): pickle
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.08x