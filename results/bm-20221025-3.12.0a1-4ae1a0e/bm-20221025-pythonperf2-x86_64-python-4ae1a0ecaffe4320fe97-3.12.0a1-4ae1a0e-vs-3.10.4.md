
# Results vs. 3.10.4

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: linux-x86_64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.25x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 278 ms: 1.26x faster                                                        |
| chameleon      | 9.44 ms                                                      | 7.62 ms: 1.24x faster                                                       |
| docutils       | 3.41 sec                                                     | 2.79 sec: 1.22x faster                                                      |
| html5lib       | 94.6 ms                                                      | 66.2 ms: 1.43x faster                                                       |
| tornado_http   | 157 ms                                                       | 114 ms: 1.37x faster                                                        |
| Geometric mean | (ref)                                                        | 1.30x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.16 sec: 1.38x faster                                                      |
| async_tree_none         | 692 ms                                                       | 516 ms: 1.34x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 618 ms: 1.33x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 756 ms: 1.24x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.32x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 73.2 ms: 1.52x faster                                                       |
| nbody          | 134 ms                                                       | 98.1 ms: 1.37x faster                                                       |
| pidigits       | 271 ms                                                       | 251 ms: 1.08x faster                                                        |
| Geometric mean | (ref)                                                        | 1.31x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 146 ms: 1.31x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 22.9 ms: 1.19x faster                                                       |
| regex_dna      | 261 ms                                                       | 232 ms: 1.13x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.34 ms: 1.08x slower                                                       |
| Geometric mean | (ref)                                                        | 1.13x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle_pure_python | 312 us                                                       | 208 us: 1.50x faster                                                        |
| pickle_pure_python   | 455 us                                                       | 313 us: 1.45x faster                                                        |
| xml_etree_process    | 75.9 ms                                                      | 54.1 ms: 1.40x faster                                                       |
| json_dumps           | 14.5 ms                                                      | 10.4 ms: 1.40x faster                                                       |
| json_loads           | 30.3 us                                                      | 24.3 us: 1.25x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 77.6 ms: 1.19x faster                                                       |
| xml_etree_parse      | 160 ms                                                       | 138 ms: 1.16x faster                                                        |
| xml_etree_iterparse  | 110 ms                                                       | 103 ms: 1.08x faster                                                        |
| pickle_list          | 4.12 us                                                      | 3.84 us: 1.07x faster                                                       |
| unpickle_list        | 4.65 us                                                      | 4.47 us: 1.04x faster                                                       |
| unpickle             | 13.5 us                                                      | 13.3 us: 1.01x faster                                                       |
| pickle               | 9.89 us                                                      | 10.1 us: 1.02x slower                                                       |
| pickle_dict          | 29.5 us                                                      | 31.9 us: 1.08x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.17x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 10.6 ms: 1.09x faster                                                       |
| python_startup_no_site | 7.33 ms                                                      | 7.62 ms: 1.04x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.4 ms: 1.41x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 24.7 ms: 1.27x faster                                                       |
| django_template | 50.2 ms                                                      | 40.6 ms: 1.24x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 55.5 ms: 1.14x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.26x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 3.65 ms: 2.05x faster                                                       |
| logging_silent          | 167 ns                                                       | 95.5 ns: 1.75x faster                                                       |
| pyflate                 | 733 ms                                                       | 431 ms: 1.70x faster                                                        |
| go                      | 262 ms                                                       | 155 ms: 1.69x faster                                                        |
| scimark_sor             | 180 ms                                                       | 108 ms: 1.66x faster                                                        |
| raytrace                | 489 ms                                                       | 298 ms: 1.64x faster                                                        |
| scimark_monte_carlo     | 107 ms                                                       | 67.8 ms: 1.58x faster                                                       |
| richards                | 75.1 ms                                                      | 47.6 ms: 1.58x faster                                                       |
| float                   | 111 ms                                                       | 73.2 ms: 1.52x faster                                                       |
| scimark_lu              | 167 ms                                                       | 111 ms: 1.50x faster                                                        |
| unpickle_pure_python    | 312 us                                                       | 208 us: 1.50x faster                                                        |
| sqlglot_parse           | 2.24 ms                                                      | 1.51 ms: 1.48x faster                                                       |
| chaos                   | 109 ms                                                       | 73.4 ms: 1.48x faster                                                       |
| pickle_pure_python      | 455 us                                                       | 313 us: 1.45x faster                                                        |
| spectral_norm           | 139 ms                                                       | 96.1 ms: 1.45x faster                                                       |
| crypto_pyaes            | 119 ms                                                       | 83.2 ms: 1.43x faster                                                       |
| html5lib                | 94.6 ms                                                      | 66.2 ms: 1.43x faster                                                       |
| hexiom                  | 9.42 ms                                                      | 6.61 ms: 1.42x faster                                                       |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 3.58 ms: 1.42x faster                                                       |
| sqlglot_transpile       | 2.68 ms                                                      | 1.90 ms: 1.41x faster                                                       |
| mako                    | 14.7 ms                                                      | 10.4 ms: 1.41x faster                                                       |
| xml_etree_process       | 75.9 ms                                                      | 54.1 ms: 1.40x faster                                                       |
| json_dumps              | 14.5 ms                                                      | 10.4 ms: 1.40x faster                                                       |
| bench_mp_pool           | 6.37 ms                                                      | 4.56 ms: 1.40x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.16 sec: 1.38x faster                                                      |
| pprint_safe_repr        | 1.05 sec                                                     | 761 ms: 1.38x faster                                                        |
| pprint_pformat          | 2.15 sec                                                     | 1.57 sec: 1.37x faster                                                      |
| tornado_http            | 157 ms                                                       | 114 ms: 1.37x faster                                                        |
| deepcopy_memo           | 49.8 us                                                      | 36.4 us: 1.37x faster                                                       |
| nbody                   | 134 ms                                                       | 98.1 ms: 1.37x faster                                                       |
| async_tree_none         | 692 ms                                                       | 516 ms: 1.34x faster                                                        |
| pycparser               | 1.67 sec                                                     | 1.25 sec: 1.34x faster                                                      |
| unpack_sequence         | 59.9 ns                                                      | 45.0 ns: 1.33x faster                                                       |
| aiohttp                 | 1.19 ms                                                      | 894 us: 1.33x faster                                                        |
| async_tree_memoization  | 819 ms                                                       | 618 ms: 1.33x faster                                                        |
| async_generators        | 421 ms                                                       | 321 ms: 1.31x faster                                                        |
| regex_compile           | 190 ms                                                       | 146 ms: 1.31x faster                                                        |
| gunicorn                | 1.16 ms                                                      | 888 us: 1.30x faster                                                        |
| genshi_text             | 31.4 ms                                                      | 24.7 ms: 1.27x faster                                                       |
| 2to3                    | 350 ms                                                       | 278 ms: 1.26x faster                                                        |
| logging_simple          | 8.88 us                                                      | 7.06 us: 1.26x faster                                                       |
| scimark_fft             | 361 ms                                                       | 288 ms: 1.26x faster                                                        |
| json_loads              | 30.3 us                                                      | 24.3 us: 1.25x faster                                                       |
| logging_format          | 9.64 us                                                      | 7.77 us: 1.24x faster                                                       |
| chameleon               | 9.44 ms                                                      | 7.62 ms: 1.24x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 756 ms: 1.24x faster                                                        |
| django_template         | 50.2 ms                                                      | 40.6 ms: 1.24x faster                                                       |
| thrift                  | 1.18 ms                                                      | 953 us: 1.23x faster                                                        |
| dulwich_log             | 81.1 ms                                                      | 65.9 ms: 1.23x faster                                                       |
| docutils                | 3.41 sec                                                     | 2.79 sec: 1.22x faster                                                      |
| sqlglot_optimize        | 70.1 ms                                                      | 58.2 ms: 1.21x faster                                                       |
| sqlglot_normalize       | 144 ms                                                       | 120 ms: 1.20x faster                                                        |
| deepcopy_reduce         | 4.01 us                                                      | 3.35 us: 1.20x faster                                                       |
| fannkuch                | 483 ms                                                       | 405 ms: 1.19x faster                                                        |
| xml_etree_generate      | 92.3 ms                                                      | 77.6 ms: 1.19x faster                                                       |
| deepcopy                | 468 us                                                       | 394 us: 1.19x faster                                                        |
| regex_v8                | 27.2 ms                                                      | 22.9 ms: 1.19x faster                                                       |
| nqueens                 | 115 ms                                                       | 97.1 ms: 1.18x faster                                                       |
| bench_thread_pool       | 1.14 ms                                                      | 966 us: 1.18x faster                                                        |
| sqlite_synth            | 2.99 us                                                      | 2.54 us: 1.18x faster                                                       |
| json                    | 5.86 ms                                                      | 5.05 ms: 1.16x faster                                                       |
| xml_etree_parse         | 160 ms                                                       | 138 ms: 1.16x faster                                                        |
| dask                    | 472 ms                                                       | 409 ms: 1.15x faster                                                        |
| pylint                  | 566 ms                                                       | 496 ms: 1.14x faster                                                        |
| genshi_xml              | 63.3 ms                                                      | 55.5 ms: 1.14x faster                                                       |
| sympy_expand            | 600 ms                                                       | 527 ms: 1.14x faster                                                        |
| regex_dna               | 261 ms                                                       | 232 ms: 1.13x faster                                                        |
| pathlib                 | 21.4 ms                                                      | 19.0 ms: 1.13x faster                                                       |
| mdp                     | 3.01 sec                                                     | 2.71 sec: 1.11x faster                                                      |
| sympy_integrate         | 28.2 ms                                                      | 25.4 ms: 1.11x faster                                                       |
| sympy_str               | 360 ms                                                       | 326 ms: 1.11x faster                                                        |
| coroutines              | 30.3 ms                                                      | 27.4 ms: 1.10x faster                                                       |
| comprehensions          | 26.7 us                                                      | 24.2 us: 1.10x faster                                                       |
| meteor_contest          | 138 ms                                                       | 126 ms: 1.10x faster                                                        |
| create_gc_cycles        | 1.76 ms                                                      | 1.61 ms: 1.10x faster                                                       |
| telco                   | 7.23 ms                                                      | 6.64 ms: 1.09x faster                                                       |
| python_startup          | 11.5 ms                                                      | 10.6 ms: 1.09x faster                                                       |
| pidigits                | 271 ms                                                       | 251 ms: 1.08x faster                                                        |
| xml_etree_iterparse     | 110 ms                                                       | 103 ms: 1.08x faster                                                        |
| pickle_list             | 4.12 us                                                      | 3.84 us: 1.07x faster                                                       |
| sympy_sum               | 193 ms                                                       | 181 ms: 1.06x faster                                                        |
| generators              | 57.3 ms                                                      | 54.6 ms: 1.05x faster                                                       |
| asyncio_tcp             | 779 ms                                                       | 747 ms: 1.04x faster                                                        |
| unpickle_list           | 4.65 us                                                      | 4.47 us: 1.04x faster                                                       |
| unpickle                | 13.5 us                                                      | 13.3 us: 1.01x faster                                                       |
| pickle                  | 9.89 us                                                      | 10.1 us: 1.02x slower                                                       |
| gc_traversal            | 3.42 ms                                                      | 3.54 ms: 1.04x slower                                                       |
| python_startup_no_site  | 7.33 ms                                                      | 7.62 ms: 1.04x slower                                                       |
| pickle_dict             | 29.5 us                                                      | 31.9 us: 1.08x slower                                                       |
| regex_effbot            | 3.09 ms                                                      | 3.34 ms: 1.08x slower                                                       |
| coverage                | 63.3 ms                                                      | 81.5 ms: 1.29x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.25x faster                                                                |
Ignored benchmarks (9) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.09x