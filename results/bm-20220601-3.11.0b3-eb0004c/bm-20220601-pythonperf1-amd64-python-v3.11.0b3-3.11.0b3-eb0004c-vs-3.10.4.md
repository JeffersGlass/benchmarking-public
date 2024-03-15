
# Results vs. 3.10.4

- fork: python
- ref: v3.11.0b3
- machine: windows-amd64
- commit hash: eb0004c
- commit date: 2022-06-01
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 212 ms: 1.16x faster                                            |
| chameleon      | 5.79 ms                                                     | 5.63 ms: 1.03x faster                                           |
| docutils       | 1.92 sec                                                    | 1.66 sec: 1.15x faster                                          |
| html5lib       | 51.0 ms                                                     | 41.2 ms: 1.24x faster                                           |
| tornado_http   | 108 ms                                                      | 94.8 ms: 1.14x faster                                           |
| Geometric mean | (ref)                                                       | 1.14x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 781 ms: 1.42x faster                                            |
| async_tree_memoization  | 526 ms                                                      | 402 ms: 1.31x faster                                            |
| async_tree_none         | 435 ms                                                      | 339 ms: 1.28x faster                                            |
| async_tree_cpu_io_mixed | 638 ms                                                      | 519 ms: 1.23x faster                                            |
| Geometric mean          | (ref)                                                       | 1.31x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 57.2 ms: 1.08x faster                                           |
| pidigits       | 149 ms                                                      | 154 ms: 1.03x slower                                            |
| Geometric mean | (ref)                                                       | 1.01x faster                                                    |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 94.2 ms: 1.13x faster                                           |
| regex_dna      | 136 ms                                                      | 127 ms: 1.07x faster                                            |
| regex_effbot   | 1.66 ms                                                     | 1.62 ms: 1.03x faster                                           |
| regex_v8       | 15.4 ms                                                     | 15.2 ms: 1.02x faster                                           |
| Geometric mean | (ref)                                                       | 1.06x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 212 us: 1.27x faster                                            |
| unpickle_pure_python | 183 us                                                      | 158 us: 1.16x faster                                            |
| json_dumps           | 9.16 ms                                                     | 7.98 ms: 1.15x faster                                           |
| xml_etree_process    | 44.5 ms                                                     | 38.9 ms: 1.14x faster                                           |
| unpickle             | 9.09 us                                                     | 8.33 us: 1.09x faster                                           |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.3 ms: 1.03x faster                                           |
| json_loads           | 14.0 us                                                     | 14.2 us: 1.01x slower                                           |
| pickle_list          | 2.75 us                                                     | 2.81 us: 1.02x slower                                           |
| pickle_dict          | 17.2 us                                                     | 17.7 us: 1.03x slower                                           |
| Geometric mean       | (ref)                                                       | 1.06x faster                                                    |

Benchmark hidden because not significant (4): pickle, unpickle_list, xml_etree_generate, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.4 ms: 1.06x faster                                           |
| python_startup_no_site | 15.5 ms                                                     | 16.4 ms: 1.06x slower                                           |
| Geometric mean         | (ref)                                                       | 1.00x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.38 ms: 1.22x faster                                           |
| django_template | 28.9 ms                                                     | 25.4 ms: 1.14x faster                                           |
| genshi_text     | 19.8 ms                                                     | 18.6 ms: 1.07x faster                                           |
| Geometric mean  | (ref)                                                       | 1.10x faster                                                    |

Benchmark hidden because not significant (1): genshi_xml

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220601-pythonperf1-amd64-python-v3.11.0b3-3.11.0b3-eb0004c |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 2.78 ms: 1.51x faster                                           |
| async_tree_io           | 1.11 sec                                                    | 781 ms: 1.42x faster                                            |
| richards                | 42.4 ms                                                     | 30.7 ms: 1.38x faster                                           |
| scimark_sor             | 106 ms                                                      | 77.7 ms: 1.37x faster                                           |
| scimark_lu              | 85.8 ms                                                     | 63.6 ms: 1.35x faster                                           |
| go                      | 139 ms                                                      | 104 ms: 1.33x faster                                            |
| async_tree_memoization  | 526 ms                                                      | 402 ms: 1.31x faster                                            |
| logging_silent          | 94.6 ns                                                     | 72.7 ns: 1.30x faster                                           |
| pyflate                 | 409 ms                                                      | 318 ms: 1.29x faster                                            |
| async_tree_none         | 435 ms                                                      | 339 ms: 1.28x faster                                            |
| raytrace                | 273 ms                                                      | 215 ms: 1.27x faster                                            |
| pickle_pure_python      | 270 us                                                      | 212 us: 1.27x faster                                            |
| pycparser               | 930 ms                                                      | 735 ms: 1.27x faster                                            |
| scimark_monte_carlo     | 57.3 ms                                                     | 45.4 ms: 1.26x faster                                           |
| html5lib                | 51.0 ms                                                     | 41.2 ms: 1.24x faster                                           |
| crypto_pyaes            | 62.5 ms                                                     | 50.9 ms: 1.23x faster                                           |
| async_tree_cpu_io_mixed | 638 ms                                                      | 519 ms: 1.23x faster                                            |
| mako                    | 9.03 ms                                                     | 7.38 ms: 1.22x faster                                           |
| sqlalchemy_declarative  | 103 ms                                                      | 86.0 ms: 1.20x faster                                           |
| thrift                  | 617 us                                                      | 514 us: 1.20x faster                                            |
| chaos                   | 61.7 ms                                                     | 51.8 ms: 1.19x faster                                           |
| hexiom                  | 5.74 ms                                                     | 4.82 ms: 1.19x faster                                           |
| create_gc_cycles        | 800 us                                                      | 686 us: 1.17x faster                                            |
| unpickle_pure_python    | 183 us                                                      | 158 us: 1.16x faster                                            |
| 2to3                    | 246 ms                                                      | 212 ms: 1.16x faster                                            |
| async_generators        | 222 ms                                                      | 192 ms: 1.16x faster                                            |
| docutils                | 1.92 sec                                                    | 1.66 sec: 1.15x faster                                          |
| json_dumps              | 9.16 ms                                                     | 7.98 ms: 1.15x faster                                           |
| xml_etree_process       | 44.5 ms                                                     | 38.9 ms: 1.14x faster                                           |
| tornado_http            | 108 ms                                                      | 94.8 ms: 1.14x faster                                           |
| django_template         | 28.9 ms                                                     | 25.4 ms: 1.14x faster                                           |
| regex_compile           | 106 ms                                                      | 94.2 ms: 1.13x faster                                           |
| dask                    | 313 ms                                                      | 281 ms: 1.11x faster                                            |
| sqlglot_optimize        | 39.8 ms                                                     | 35.9 ms: 1.11x faster                                           |
| dulwich_log             | 50.5 ms                                                     | 45.5 ms: 1.11x faster                                           |
| aiohttp                 | 995 us                                                      | 897 us: 1.11x faster                                            |
| deepcopy_memo           | 28.8 us                                                     | 26.0 us: 1.11x faster                                           |
| sqlalchemy_imperative   | 11.4 ms                                                     | 10.3 ms: 1.10x faster                                           |
| sqlite_synth            | 1.91 us                                                     | 1.74 us: 1.10x faster                                           |
| pprint_safe_repr        | 592 ms                                                      | 541 ms: 1.09x faster                                            |
| unpickle                | 9.09 us                                                     | 8.33 us: 1.09x faster                                           |
| pprint_pformat          | 1.22 sec                                                    | 1.12 sec: 1.08x faster                                          |
| spectral_norm           | 77.3 ms                                                     | 71.4 ms: 1.08x faster                                           |
| float                   | 61.7 ms                                                     | 57.2 ms: 1.08x faster                                           |
| unpack_sequence         | 39.6 ns                                                     | 36.8 ns: 1.08x faster                                           |
| bench_thread_pool       | 958 us                                                      | 890 us: 1.08x faster                                            |
| sympy_integrate         | 15.3 ms                                                     | 14.2 ms: 1.07x faster                                           |
| regex_dna               | 136 ms                                                      | 127 ms: 1.07x faster                                            |
| mdp                     | 1.78 sec                                                    | 1.66 sec: 1.07x faster                                          |
| genshi_text             | 19.8 ms                                                     | 18.6 ms: 1.07x faster                                           |
| sympy_sum               | 107 ms                                                      | 100 ms: 1.07x faster                                            |
| python_startup          | 20.6 ms                                                     | 19.4 ms: 1.06x faster                                           |
| pylint                  | 350 ms                                                      | 331 ms: 1.06x faster                                            |
| logging_format          | 6.76 us                                                     | 6.43 us: 1.05x faster                                           |
| sqlglot_transpile       | 1.48 ms                                                     | 1.41 ms: 1.05x faster                                           |
| logging_simple          | 6.22 us                                                     | 5.96 us: 1.04x faster                                           |
| sqlglot_normalize       | 205 ms                                                      | 198 ms: 1.04x faster                                            |
| sympy_expand            | 314 ms                                                      | 306 ms: 1.03x faster                                            |
| pathlib                 | 75.7 ms                                                     | 73.6 ms: 1.03x faster                                           |
| chameleon               | 5.79 ms                                                     | 5.63 ms: 1.03x faster                                           |
| xml_etree_iterparse     | 65.0 ms                                                     | 63.3 ms: 1.03x faster                                           |
| sympy_str               | 194 ms                                                      | 190 ms: 1.03x faster                                            |
| regex_effbot            | 1.66 ms                                                     | 1.62 ms: 1.03x faster                                           |
| coroutines              | 16.0 ms                                                     | 15.7 ms: 1.02x faster                                           |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.68 ms: 1.02x faster                                           |
| regex_v8                | 15.4 ms                                                     | 15.2 ms: 1.02x faster                                           |
| sqlglot_parse           | 1.22 ms                                                     | 1.21 ms: 1.01x faster                                           |
| scimark_fft             | 187 ms                                                      | 188 ms: 1.01x slower                                            |
| json_loads              | 14.0 us                                                     | 14.2 us: 1.01x slower                                           |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                          |
| meteor_contest          | 75.9 ms                                                     | 77.1 ms: 1.02x slower                                           |
| pickle_list             | 2.75 us                                                     | 2.81 us: 1.02x slower                                           |
| pidigits                | 149 ms                                                      | 154 ms: 1.03x slower                                            |
| pickle_dict             | 17.2 us                                                     | 17.7 us: 1.03x slower                                           |
| deepcopy                | 255 us                                                      | 265 us: 1.04x slower                                            |
| asyncio_tcp             | 732 ms                                                      | 762 ms: 1.04x slower                                            |
| telco                   | 3.94 ms                                                     | 4.13 ms: 1.05x slower                                           |
| gc_traversal            | 1.41 ms                                                     | 1.49 ms: 1.05x slower                                           |
| python_startup_no_site  | 15.5 ms                                                     | 16.4 ms: 1.06x slower                                           |
| nqueens                 | 66.6 ms                                                     | 71.0 ms: 1.07x slower                                           |
| bench_mp_pool           | 62.0 ms                                                     | 67.0 ms: 1.08x slower                                           |
| fannkuch                | 256 ms                                                      | 278 ms: 1.09x slower                                            |
| generators              | 32.4 ms                                                     | 35.4 ms: 1.09x slower                                           |
| comprehensions          | 16.5 us                                                     | 18.7 us: 1.14x slower                                           |
| coverage                | 39.0 ms                                                     | 108 ms: 2.76x slower                                            |
| Geometric mean          | (ref)                                                       | 1.08x faster                                                    |

Benchmark hidden because not significant (8): pickle, genshi_xml, unpickle_list, xml_etree_generate, xml_etree_parse, deepcopy_reduce, nbody, json
Ignored benchmarks (5) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: unknown