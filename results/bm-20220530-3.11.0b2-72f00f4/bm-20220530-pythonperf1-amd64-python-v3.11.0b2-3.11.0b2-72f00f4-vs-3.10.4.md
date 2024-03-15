
# Results vs. 3.10.4

- fork: python
- ref: v3.11.0b2
- machine: windows-amd64
- commit hash: 72f00f4
- commit date: 2022-05-30
- overall geometric mean: 1.09x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 211 ms: 1.16x faster                                            |
| chameleon      | 5.79 ms                                                     | 5.59 ms: 1.04x faster                                           |
| docutils       | 1.92 sec                                                    | 1.66 sec: 1.16x faster                                          |
| html5lib       | 51.0 ms                                                     | 41.4 ms: 1.23x faster                                           |
| tornado_http   | 108 ms                                                      | 95.3 ms: 1.14x faster                                           |
| Geometric mean | (ref)                                                       | 1.14x faster                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 794 ms: 1.40x faster                                            |
| async_tree_memoization  | 526 ms                                                      | 400 ms: 1.32x faster                                            |
| async_tree_none         | 435 ms                                                      | 336 ms: 1.29x faster                                            |
| async_tree_cpu_io_mixed | 638 ms                                                      | 520 ms: 1.23x faster                                            |
| Geometric mean          | (ref)                                                       | 1.31x faster                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 54.5 ms: 1.13x faster                                           |
| nbody          | 71.3 ms                                                     | 70.1 ms: 1.02x faster                                           |
| pidigits       | 149 ms                                                      | 153 ms: 1.03x slower                                            |
| Geometric mean | (ref)                                                       | 1.04x faster                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_effbot   | 1.66 ms                                                     | 1.39 ms: 1.19x faster                                           |
| regex_dna      | 136 ms                                                      | 120 ms: 1.14x faster                                            |
| regex_compile  | 106 ms                                                      | 97.0 ms: 1.09x faster                                           |
| regex_v8       | 15.4 ms                                                     | 14.4 ms: 1.07x faster                                           |
| Geometric mean | (ref)                                                       | 1.12x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 216 us: 1.25x faster                                            |
| xml_etree_process    | 44.5 ms                                                     | 39.1 ms: 1.14x faster                                           |
| unpickle             | 9.09 us                                                     | 8.07 us: 1.13x faster                                           |
| unpickle_pure_python | 183 us                                                      | 164 us: 1.12x faster                                            |
| json_dumps           | 9.16 ms                                                     | 8.21 ms: 1.12x faster                                           |
| xml_etree_iterparse  | 65.0 ms                                                     | 62.0 ms: 1.05x faster                                           |
| pickle_list          | 2.75 us                                                     | 2.64 us: 1.04x faster                                           |
| xml_etree_generate   | 55.5 ms                                                     | 54.1 ms: 1.03x faster                                           |
| pickle               | 6.85 us                                                     | 6.74 us: 1.02x faster                                           |
| pickle_dict          | 17.2 us                                                     | 17.4 us: 1.01x slower                                           |
| unpickle_list        | 2.71 us                                                     | 2.76 us: 1.02x slower                                           |
| Geometric mean       | (ref)                                                       | 1.06x faster                                                    |

Benchmark hidden because not significant (2): xml_etree_parse, json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.0 ms: 1.08x faster                                           |
| python_startup_no_site | 15.5 ms                                                     | 15.8 ms: 1.02x slower                                           |
| Geometric mean         | (ref)                                                       | 1.03x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.62 ms: 1.19x faster                                           |
| django_template | 28.9 ms                                                     | 25.1 ms: 1.15x faster                                           |
| genshi_text     | 19.8 ms                                                     | 17.9 ms: 1.11x faster                                           |
| genshi_xml      | 41.0 ms                                                     | 40.2 ms: 1.02x faster                                           |
| Geometric mean  | (ref)                                                       | 1.11x faster                                                    |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 2.72 ms: 1.54x faster                                           |
| async_tree_io           | 1.11 sec                                                    | 794 ms: 1.40x faster                                            |
| go                      | 139 ms                                                      | 100 ms: 1.39x faster                                            |
| richards                | 42.4 ms                                                     | 31.6 ms: 1.34x faster                                           |
| scimark_lu              | 85.8 ms                                                     | 64.6 ms: 1.33x faster                                           |
| scimark_sor             | 106 ms                                                      | 80.0 ms: 1.33x faster                                           |
| async_tree_memoization  | 526 ms                                                      | 400 ms: 1.32x faster                                            |
| logging_silent          | 94.6 ns                                                     | 72.2 ns: 1.31x faster                                           |
| pyflate                 | 409 ms                                                      | 314 ms: 1.30x faster                                            |
| async_tree_none         | 435 ms                                                      | 336 ms: 1.29x faster                                            |
| raytrace                | 273 ms                                                      | 213 ms: 1.28x faster                                            |
| pickle_pure_python      | 270 us                                                      | 216 us: 1.25x faster                                            |
| scimark_monte_carlo     | 57.3 ms                                                     | 46.0 ms: 1.24x faster                                           |
| sqlalchemy_declarative  | 103 ms                                                      | 83.2 ms: 1.24x faster                                           |
| pycparser               | 930 ms                                                      | 750 ms: 1.24x faster                                            |
| html5lib                | 51.0 ms                                                     | 41.4 ms: 1.23x faster                                           |
| async_tree_cpu_io_mixed | 638 ms                                                      | 520 ms: 1.23x faster                                            |
| crypto_pyaes            | 62.5 ms                                                     | 51.8 ms: 1.21x faster                                           |
| thrift                  | 617 us                                                      | 516 us: 1.20x faster                                            |
| regex_effbot            | 1.66 ms                                                     | 1.39 ms: 1.19x faster                                           |
| chaos                   | 61.7 ms                                                     | 51.8 ms: 1.19x faster                                           |
| hexiom                  | 5.74 ms                                                     | 4.84 ms: 1.19x faster                                           |
| mako                    | 9.03 ms                                                     | 7.62 ms: 1.19x faster                                           |
| create_gc_cycles        | 800 us                                                      | 675 us: 1.19x faster                                            |
| async_generators        | 222 ms                                                      | 187 ms: 1.18x faster                                            |
| 2to3                    | 246 ms                                                      | 211 ms: 1.16x faster                                            |
| docutils                | 1.92 sec                                                    | 1.66 sec: 1.16x faster                                          |
| django_template         | 28.9 ms                                                     | 25.1 ms: 1.15x faster                                           |
| regex_dna               | 136 ms                                                      | 120 ms: 1.14x faster                                            |
| xml_etree_process       | 44.5 ms                                                     | 39.1 ms: 1.14x faster                                           |
| tornado_http            | 108 ms                                                      | 95.3 ms: 1.14x faster                                           |
| float                   | 61.7 ms                                                     | 54.5 ms: 1.13x faster                                           |
| unpickle                | 9.09 us                                                     | 8.07 us: 1.13x faster                                           |
| sqlite_synth            | 1.91 us                                                     | 1.71 us: 1.12x faster                                           |
| unpickle_pure_python    | 183 us                                                      | 164 us: 1.12x faster                                            |
| dask                    | 313 ms                                                      | 280 ms: 1.12x faster                                            |
| json_dumps              | 9.16 ms                                                     | 8.21 ms: 1.12x faster                                           |
| genshi_text             | 19.8 ms                                                     | 17.9 ms: 1.11x faster                                           |
| deepcopy_memo           | 28.8 us                                                     | 26.1 us: 1.10x faster                                           |
| pprint_pformat          | 1.22 sec                                                    | 1.11 sec: 1.10x faster                                          |
| dulwich_log             | 50.5 ms                                                     | 46.1 ms: 1.09x faster                                           |
| spectral_norm           | 77.3 ms                                                     | 70.6 ms: 1.09x faster                                           |
| regex_compile           | 106 ms                                                      | 97.0 ms: 1.09x faster                                           |
| sqlalchemy_imperative   | 11.4 ms                                                     | 10.5 ms: 1.09x faster                                           |
| python_startup          | 20.6 ms                                                     | 19.0 ms: 1.08x faster                                           |
| pprint_safe_repr        | 592 ms                                                      | 548 ms: 1.08x faster                                            |
| aiohttp                 | 995 us                                                      | 921 us: 1.08x faster                                            |
| bench_thread_pool       | 958 us                                                      | 889 us: 1.08x faster                                            |
| sympy_integrate         | 15.3 ms                                                     | 14.2 ms: 1.07x faster                                           |
| regex_v8                | 15.4 ms                                                     | 14.4 ms: 1.07x faster                                           |
| sqlglot_optimize        | 39.8 ms                                                     | 37.5 ms: 1.06x faster                                           |
| pylint                  | 350 ms                                                      | 331 ms: 1.06x faster                                            |
| logging_format          | 6.76 us                                                     | 6.39 us: 1.06x faster                                           |
| xml_etree_iterparse     | 65.0 ms                                                     | 62.0 ms: 1.05x faster                                           |
| logging_simple          | 6.22 us                                                     | 5.94 us: 1.05x faster                                           |
| sympy_sum               | 107 ms                                                      | 103 ms: 1.04x faster                                            |
| pickle_list             | 2.75 us                                                     | 2.64 us: 1.04x faster                                           |
| sqlglot_transpile       | 1.48 ms                                                     | 1.42 ms: 1.04x faster                                           |
| chameleon               | 5.79 ms                                                     | 5.59 ms: 1.04x faster                                           |
| coroutines              | 16.0 ms                                                     | 15.6 ms: 1.03x faster                                           |
| xml_etree_generate      | 55.5 ms                                                     | 54.1 ms: 1.03x faster                                           |
| sympy_str               | 194 ms                                                      | 190 ms: 1.02x faster                                            |
| genshi_xml              | 41.0 ms                                                     | 40.2 ms: 1.02x faster                                           |
| nbody                   | 71.3 ms                                                     | 70.1 ms: 1.02x faster                                           |
| pickle                  | 6.85 us                                                     | 6.74 us: 1.02x faster                                           |
| mdp                     | 1.78 sec                                                    | 1.75 sec: 1.01x faster                                          |
| sqlglot_normalize       | 205 ms                                                      | 203 ms: 1.01x faster                                            |
| pathlib                 | 75.7 ms                                                     | 74.8 ms: 1.01x faster                                           |
| sqlglot_parse           | 1.22 ms                                                     | 1.21 ms: 1.01x faster                                           |
| sympy_expand            | 314 ms                                                      | 312 ms: 1.01x faster                                            |
| pickle_dict             | 17.2 us                                                     | 17.4 us: 1.01x slower                                           |
| unpickle_list           | 2.71 us                                                     | 2.76 us: 1.02x slower                                           |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.77 ms: 1.02x slower                                           |
| scimark_fft             | 187 ms                                                      | 191 ms: 1.02x slower                                            |
| bench_mp_pool           | 62.0 ms                                                     | 63.3 ms: 1.02x slower                                           |
| python_startup_no_site  | 15.5 ms                                                     | 15.8 ms: 1.02x slower                                           |
| deepcopy                | 255 us                                                      | 261 us: 1.02x slower                                            |
| pidigits                | 149 ms                                                      | 153 ms: 1.03x slower                                            |
| telco                   | 3.94 ms                                                     | 4.05 ms: 1.03x slower                                           |
| gc_traversal            | 1.41 ms                                                     | 1.46 ms: 1.03x slower                                           |
| nqueens                 | 66.6 ms                                                     | 68.9 ms: 1.03x slower                                           |
| meteor_contest          | 75.9 ms                                                     | 78.7 ms: 1.04x slower                                           |
| fannkuch                | 256 ms                                                      | 266 ms: 1.04x slower                                            |
| comprehensions          | 16.5 us                                                     | 18.2 us: 1.10x slower                                           |
| generators              | 32.4 ms                                                     | 35.7 ms: 1.10x slower                                           |
| unpack_sequence         | 39.6 ns                                                     | 44.3 ns: 1.12x slower                                           |
| coverage                | 39.0 ms                                                     | 106 ms: 2.71x slower                                            |
| Geometric mean          | (ref)                                                       | 1.09x faster                                                    |

Benchmark hidden because not significant (5): deepcopy_reduce, xml_etree_parse, json_loads, asyncio_tcp, json
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown