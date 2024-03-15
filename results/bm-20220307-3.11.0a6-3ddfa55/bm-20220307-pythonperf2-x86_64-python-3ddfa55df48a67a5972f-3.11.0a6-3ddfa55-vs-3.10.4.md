
# Results vs. 3.10.4

- fork: python
- ref: 3ddfa55df48a67a5972f
- machine: linux-x86_64
- commit hash: 3ddfa55
- commit date: 2022-03-07
- overall geometric mean: 1.14x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: 1.15x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 300 ms: 1.17x faster                                                        |
| chameleon      | 9.44 ms                                                      | 8.43 ms: 1.12x faster                                                       |
| docutils       | 3.41 sec                                                     | 2.98 sec: 1.14x faster                                                      |
| html5lib       | 94.6 ms                                                      | 75.6 ms: 1.25x faster                                                       |
| tornado_http   | 157 ms                                                       | 130 ms: 1.21x faster                                                        |
| Geometric mean | (ref)                                                        | 1.18x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.19 sec: 1.34x faster                                                      |
| async_tree_none         | 692 ms                                                       | 532 ms: 1.30x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 651 ms: 1.26x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 763 ms: 1.23x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.28x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 79.1 ms: 1.40x faster                                                       |
| nbody          | 134 ms                                                       | 98.0 ms: 1.37x faster                                                       |
| pidigits       | 271 ms                                                       | 253 ms: 1.07x faster                                                        |
| Geometric mean | (ref)                                                        | 1.27x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 161 ms: 1.18x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 26.4 ms: 1.03x faster                                                       |
| regex_dna      | 261 ms                                                       | 257 ms: 1.02x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.49 ms: 1.13x slower                                                       |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 352 us: 1.29x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 59.4 ms: 1.28x faster                                                       |
| json_loads           | 30.3 us                                                      | 23.9 us: 1.27x faster                                                       |
| unpickle_pure_python | 312 us                                                       | 273 us: 1.14x faster                                                        |
| xml_etree_generate   | 92.3 ms                                                      | 83.5 ms: 1.10x faster                                                       |
| json_dumps           | 14.5 ms                                                      | 13.6 ms: 1.07x faster                                                       |
| xml_etree_iterparse  | 110 ms                                                       | 104 ms: 1.06x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 154 ms: 1.04x faster                                                        |
| pickle               | 9.89 us                                                      | 9.96 us: 1.01x slower                                                       |
| pickle_list          | 4.12 us                                                      | 4.28 us: 1.04x slower                                                       |
| pickle_dict          | 29.5 us                                                      | 32.2 us: 1.09x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.08x faster                                                                |

Benchmark hidden because not significant (2): unpickle, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.4 ms: 1.10x faster                                                       |
| python_startup_no_site | 7.33 ms                                                      | 7.55 ms: 1.03x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.03x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 11.4 ms: 1.28x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 26.5 ms: 1.19x faster                                                       |
| django_template | 50.2 ms                                                      | 43.8 ms: 1.15x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 60.7 ms: 1.04x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.16x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 4.49 ms: 1.67x faster                                                       |
| scimark_sor             | 180 ms                                                       | 121 ms: 1.49x faster                                                        |
| pyflate                 | 733 ms                                                       | 494 ms: 1.48x faster                                                        |
| go                      | 262 ms                                                       | 178 ms: 1.47x faster                                                        |
| logging_silent          | 167 ns                                                       | 115 ns: 1.45x faster                                                        |
| scimark_monte_carlo     | 107 ms                                                       | 74.4 ms: 1.44x faster                                                       |
| raytrace                | 489 ms                                                       | 343 ms: 1.42x faster                                                        |
| float                   | 111 ms                                                       | 79.1 ms: 1.40x faster                                                       |
| chaos                   | 109 ms                                                       | 77.5 ms: 1.40x faster                                                       |
| scimark_lu              | 167 ms                                                       | 122 ms: 1.37x faster                                                        |
| nbody                   | 134 ms                                                       | 98.0 ms: 1.37x faster                                                       |
| richards                | 75.1 ms                                                      | 55.9 ms: 1.34x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.19 sec: 1.34x faster                                                      |
| bench_mp_pool           | 6.37 ms                                                      | 4.80 ms: 1.33x faster                                                       |
| async_generators        | 421 ms                                                       | 320 ms: 1.31x faster                                                        |
| async_tree_none         | 692 ms                                                       | 532 ms: 1.30x faster                                                        |
| pickle_pure_python      | 455 us                                                       | 352 us: 1.29x faster                                                        |
| mako                    | 14.7 ms                                                      | 11.4 ms: 1.28x faster                                                       |
| xml_etree_process       | 75.9 ms                                                      | 59.4 ms: 1.28x faster                                                       |
| crypto_pyaes            | 119 ms                                                       | 93.5 ms: 1.27x faster                                                       |
| json_loads              | 30.3 us                                                      | 23.9 us: 1.27x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 651 ms: 1.26x faster                                                        |
| spectral_norm           | 139 ms                                                       | 111 ms: 1.26x faster                                                        |
| logging_simple          | 8.88 us                                                      | 7.08 us: 1.25x faster                                                       |
| html5lib                | 94.6 ms                                                      | 75.6 ms: 1.25x faster                                                       |
| logging_format          | 9.64 us                                                      | 7.75 us: 1.24x faster                                                       |
| pprint_safe_repr        | 1.05 sec                                                     | 853 ms: 1.23x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 763 ms: 1.23x faster                                                        |
| hexiom                  | 9.42 ms                                                      | 7.74 ms: 1.22x faster                                                       |
| pprint_pformat          | 2.15 sec                                                     | 1.77 sec: 1.21x faster                                                      |
| tornado_http            | 157 ms                                                       | 130 ms: 1.21x faster                                                        |
| deepcopy_memo           | 49.8 us                                                      | 41.7 us: 1.19x faster                                                       |
| scimark_fft             | 361 ms                                                       | 305 ms: 1.19x faster                                                        |
| thrift                  | 1.18 ms                                                      | 991 us: 1.19x faster                                                        |
| genshi_text             | 31.4 ms                                                      | 26.5 ms: 1.19x faster                                                       |
| aiohttp                 | 1.19 ms                                                      | 1.00 ms: 1.19x faster                                                       |
| regex_compile           | 190 ms                                                       | 161 ms: 1.18x faster                                                        |
| sqlite_synth            | 2.99 us                                                      | 2.54 us: 1.18x faster                                                       |
| pycparser               | 1.67 sec                                                     | 1.43 sec: 1.17x faster                                                      |
| 2to3                    | 350 ms                                                       | 300 ms: 1.17x faster                                                        |
| gunicorn                | 1.16 ms                                                      | 994 us: 1.17x faster                                                        |
| json                    | 5.86 ms                                                      | 5.04 ms: 1.16x faster                                                       |
| sqlalchemy_declarative  | 190 ms                                                       | 164 ms: 1.16x faster                                                        |
| django_template         | 50.2 ms                                                      | 43.8 ms: 1.15x faster                                                       |
| nqueens                 | 115 ms                                                       | 100 ms: 1.15x faster                                                        |
| docutils                | 3.41 sec                                                     | 2.98 sec: 1.14x faster                                                      |
| unpickle_pure_python    | 312 us                                                       | 273 us: 1.14x faster                                                        |
| deepcopy                | 468 us                                                       | 413 us: 1.13x faster                                                        |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 4.53 ms: 1.12x faster                                                       |
| chameleon               | 9.44 ms                                                      | 8.43 ms: 1.12x faster                                                       |
| xml_etree_generate      | 92.3 ms                                                      | 83.5 ms: 1.10x faster                                                       |
| pathlib                 | 21.4 ms                                                      | 19.3 ms: 1.10x faster                                                       |
| python_startup          | 11.5 ms                                                      | 10.4 ms: 1.10x faster                                                       |
| sqlglot_optimize        | 70.1 ms                                                      | 63.7 ms: 1.10x faster                                                       |
| flaskblogging           | 4.39 ms                                                      | 3.99 ms: 1.10x faster                                                       |
| dulwich_log             | 81.1 ms                                                      | 73.8 ms: 1.10x faster                                                       |
| sqlglot_normalize       | 144 ms                                                       | 131 ms: 1.10x faster                                                        |
| bench_thread_pool       | 1.14 ms                                                      | 1.04 ms: 1.10x faster                                                       |
| sympy_integrate         | 28.2 ms                                                      | 25.9 ms: 1.09x faster                                                       |
| sqlalchemy_imperative   | 22.7 ms                                                      | 21.0 ms: 1.08x faster                                                       |
| create_gc_cycles        | 1.76 ms                                                      | 1.63 ms: 1.08x faster                                                       |
| deepcopy_reduce         | 4.01 us                                                      | 3.73 us: 1.07x faster                                                       |
| sqlglot_transpile       | 2.68 ms                                                      | 2.50 ms: 1.07x faster                                                       |
| pidigits                | 271 ms                                                       | 253 ms: 1.07x faster                                                        |
| json_dumps              | 14.5 ms                                                      | 13.6 ms: 1.07x faster                                                       |
| dask                    | 472 ms                                                       | 442 ms: 1.07x faster                                                        |
| fannkuch                | 483 ms                                                       | 453 ms: 1.07x faster                                                        |
| xml_etree_iterparse     | 110 ms                                                       | 104 ms: 1.06x faster                                                        |
| sqlglot_parse           | 2.24 ms                                                      | 2.13 ms: 1.05x faster                                                       |
| sympy_str               | 360 ms                                                       | 343 ms: 1.05x faster                                                        |
| telco                   | 7.23 ms                                                      | 6.90 ms: 1.05x faster                                                       |
| sympy_sum               | 193 ms                                                       | 184 ms: 1.05x faster                                                        |
| sympy_expand            | 600 ms                                                       | 573 ms: 1.05x faster                                                        |
| generators              | 57.3 ms                                                      | 54.8 ms: 1.05x faster                                                       |
| meteor_contest          | 138 ms                                                       | 133 ms: 1.04x faster                                                        |
| genshi_xml              | 63.3 ms                                                      | 60.7 ms: 1.04x faster                                                       |
| xml_etree_parse         | 160 ms                                                       | 154 ms: 1.04x faster                                                        |
| mdp                     | 3.01 sec                                                     | 2.91 sec: 1.03x faster                                                      |
| regex_v8                | 27.2 ms                                                      | 26.4 ms: 1.03x faster                                                       |
| asyncio_tcp             | 779 ms                                                       | 757 ms: 1.03x faster                                                        |
| regex_dna               | 261 ms                                                       | 257 ms: 1.02x faster                                                        |
| coroutines              | 30.3 ms                                                      | 30.1 ms: 1.01x faster                                                       |
| pickle                  | 9.89 us                                                      | 9.96 us: 1.01x slower                                                       |
| python_startup_no_site  | 7.33 ms                                                      | 7.55 ms: 1.03x slower                                                       |
| pickle_list             | 4.12 us                                                      | 4.28 us: 1.04x slower                                                       |
| pickle_dict             | 29.5 us                                                      | 32.2 us: 1.09x slower                                                       |
| comprehensions          | 26.7 us                                                      | 29.6 us: 1.11x slower                                                       |
| regex_effbot            | 3.09 ms                                                      | 3.49 ms: 1.13x slower                                                       |
| gc_traversal            | 3.42 ms                                                      | 4.03 ms: 1.18x slower                                                       |
| coverage                | 63.3 ms                                                      | 84.1 ms: 1.33x slower                                                       |
| unpack_sequence         | 59.9 ns                                                      | 152 ns: 2.53x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.14x faster                                                                |

Benchmark hidden because not significant (2): unpickle, unpickle_list
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: 1.15x