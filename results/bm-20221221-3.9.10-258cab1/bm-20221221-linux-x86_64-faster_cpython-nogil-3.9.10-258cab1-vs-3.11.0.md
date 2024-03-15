
# Results vs. 3.11.0

- fork: faster_cpython
- ref: nogil
- machine: linux-x86_64
- commit hash: 258cab1
- commit date: 2022-12-21
- overall geometric mean: 1.20x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x slower
- Memory change: 1.42x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 382 ms: 1.44x slower                                         |
| chameleon      | 6.70 ms                                                | 8.20 ms: 1.22x slower                                        |
| docutils       | 2.66 sec                                               | 5.20 sec: 1.95x slower                                       |
| html5lib       | 64.8 ms                                                | 81.7 ms: 1.26x slower                                        |
| tornado_http   | 98.1 ms                                                | 124 ms: 1.26x slower                                         |
| Geometric mean | (ref)                                                  | 1.41x slower                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_io           | 1.29 sec                                               | 829 ms: 1.55x faster                                         |
| async_tree_none         | 528 ms                                                 | 372 ms: 1.42x faster                                         |
| async_tree_memoization  | 639 ms                                                 | 460 ms: 1.39x faster                                         |
| async_tree_cpu_io_mixed | 749 ms                                                 | 614 ms: 1.22x faster                                         |
| Geometric mean          | (ref)                                                  | 1.39x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 186 ms: 1.05x faster                                         |
| float          | 78.9 ms                                                | 104 ms: 1.32x slower                                         |
| nbody          | 96.0 ms                                                | 172 ms: 1.79x slower                                         |
| Geometric mean | (ref)                                                  | 1.31x slower                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.35 ms: 1.05x faster                                        |
| regex_v8       | 22.9 ms                                                | 24.1 ms: 1.05x slower                                        |
| regex_dna      | 205 ms                                                 | 218 ms: 1.06x slower                                         |
| regex_compile  | 141 ms                                                 | 186 ms: 1.32x slower                                         |
| Geometric mean | (ref)                                                  | 1.09x slower                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 25.3 us: 1.37x faster                                        |
| xml_etree_iterparse  | 108 ms                                                 | 95.5 ms: 1.13x faster                                        |
| xml_etree_parse      | 164 ms                                                 | 149 ms: 1.10x faster                                         |
| pickle_list          | 4.59 us                                                | 4.17 us: 1.10x faster                                        |
| pickle               | 11.0 us                                                | 10.0 us: 1.10x faster                                        |
| pickle_pure_python   | 320 us                                                 | 346 us: 1.08x slower                                         |
| xml_etree_generate   | 81.1 ms                                                | 87.8 ms: 1.08x slower                                        |
| unpickle_pure_python | 242 us                                                 | 262 us: 1.09x slower                                         |
| unpickle_list        | 5.21 us                                                | 5.80 us: 1.11x slower                                        |
| json_loads           | 29.2 us                                                | 32.5 us: 1.11x slower                                        |
| xml_etree_process    | 56.9 ms                                                | 71.4 ms: 1.26x slower                                        |
| unpickle             | 13.8 us                                                | 18.6 us: 1.34x slower                                        |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                 |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 6.01 ms                                                | 5.91 ms: 1.02x faster                                        |
| python_startup         | 8.56 ms                                                | 9.41 ms: 1.10x slower                                        |
| Geometric mean         | (ref)                                                  | 1.04x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| django_template | 33.5 ms                                                | 42.6 ms: 1.27x slower                                        |
| genshi_xml      | 53.4 ms                                                | 73.6 ms: 1.38x slower                                        |
| mako            | 10.7 ms                                                | 16.4 ms: 1.54x slower                                        |
| genshi_text     | 22.5 ms                                                | 52.1 ms: 2.31x slower                                        |
| Geometric mean  | (ref)                                                  | 1.58x slower                                                 |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_io           | 1.29 sec                                               | 829 ms: 1.55x faster                                         |
| async_tree_none         | 528 ms                                                 | 372 ms: 1.42x faster                                         |
| async_tree_memoization  | 639 ms                                                 | 460 ms: 1.39x faster                                         |
| pickle_dict             | 34.6 us                                                | 25.3 us: 1.37x faster                                        |
| richards                | 49.8 ms                                                | 39.3 ms: 1.27x faster                                        |
| async_tree_cpu_io_mixed | 749 ms                                                 | 614 ms: 1.22x faster                                         |
| logging_silent          | 111 ns                                                 | 96.0 ns: 1.16x faster                                        |
| xml_etree_iterparse     | 108 ms                                                 | 95.5 ms: 1.13x faster                                        |
| pprint_pformat          | 1.55 sec                                               | 1.40 sec: 1.11x faster                                       |
| xml_etree_parse         | 164 ms                                                 | 149 ms: 1.10x faster                                         |
| pickle_list             | 4.59 us                                                | 4.17 us: 1.10x faster                                        |
| pickle                  | 11.0 us                                                | 10.0 us: 1.10x faster                                        |
| regex_effbot            | 3.51 ms                                                | 3.35 ms: 1.05x faster                                        |
| pidigits                | 194 ms                                                 | 186 ms: 1.05x faster                                         |
| python_startup_no_site  | 6.01 ms                                                | 5.91 ms: 1.02x faster                                        |
| bench_mp_pool           | 24.0 ms                                                | 23.8 ms: 1.01x faster                                        |
| json                    | 5.24 ms                                                | 5.37 ms: 1.02x slower                                        |
| telco                   | 6.86 ms                                                | 7.15 ms: 1.04x slower                                        |
| regex_v8                | 22.9 ms                                                | 24.1 ms: 1.05x slower                                        |
| regex_dna               | 205 ms                                                 | 218 ms: 1.06x slower                                         |
| go                      | 149 ms                                                 | 159 ms: 1.07x slower                                         |
| deepcopy                | 365 us                                                 | 393 us: 1.08x slower                                         |
| pickle_pure_python      | 320 us                                                 | 346 us: 1.08x slower                                         |
| xml_etree_generate      | 81.1 ms                                                | 87.8 ms: 1.08x slower                                        |
| unpickle_pure_python    | 242 us                                                 | 262 us: 1.09x slower                                         |
| generators              | 74.9 ms                                                | 81.6 ms: 1.09x slower                                        |
| sympy_expand            | 484 ms                                                 | 531 ms: 1.10x slower                                         |
| python_startup          | 8.56 ms                                                | 9.41 ms: 1.10x slower                                        |
| unpickle_list           | 5.21 us                                                | 5.80 us: 1.11x slower                                        |
| json_loads              | 29.2 us                                                | 32.5 us: 1.11x slower                                        |
| pathlib                 | 18.5 ms                                                | 20.6 ms: 1.11x slower                                        |
| mdp                     | 2.77 sec                                               | 3.10 sec: 1.12x slower                                       |
| logging_simple          | 6.22 us                                                | 6.95 us: 1.12x slower                                        |
| hexiom                  | 6.89 ms                                                | 7.74 ms: 1.12x slower                                        |
| sympy_str               | 297 ms                                                 | 335 ms: 1.13x slower                                         |
| logging_format          | 6.81 us                                                | 7.69 us: 1.13x slower                                        |
| deepcopy_reduce         | 3.22 us                                                | 3.63 us: 1.13x slower                                        |
| pycparser               | 1.19 sec                                               | 1.35 sec: 1.14x slower                                       |
| meteor_contest          | 109 ms                                                 | 127 ms: 1.17x slower                                         |
| sympy_integrate         | 21.5 ms                                                | 25.4 ms: 1.18x slower                                        |
| scimark_sor             | 121 ms                                                 | 144 ms: 1.19x slower                                         |
| dulwich_log             | 64.6 ms                                                | 77.0 ms: 1.19x slower                                        |
| unpack_sequence         | 43.5 ns                                                | 52.4 ns: 1.21x slower                                        |
| djangocms               | 33.5 us                                                | 40.5 us: 1.21x slower                                        |
| fannkuch                | 405 ms                                                 | 490 ms: 1.21x slower                                         |
| scimark_sparse_mat_mult | 5.03 ms                                                | 6.09 ms: 1.21x slower                                        |
| chameleon               | 6.70 ms                                                | 8.20 ms: 1.22x slower                                        |
| nqueens                 | 87.9 ms                                                | 109 ms: 1.24x slower                                         |
| scimark_fft             | 345 ms                                                 | 430 ms: 1.25x slower                                         |
| sqlglot_optimize        | 55.3 ms                                                | 69.3 ms: 1.25x slower                                        |
| sympy_sum               | 169 ms                                                 | 212 ms: 1.25x slower                                         |
| xml_etree_process       | 56.9 ms                                                | 71.4 ms: 1.26x slower                                        |
| sqlite_synth            | 2.57 us                                                | 3.24 us: 1.26x slower                                        |
| html5lib                | 64.8 ms                                                | 81.7 ms: 1.26x slower                                        |
| tornado_http            | 98.1 ms                                                | 124 ms: 1.26x slower                                         |
| thrift                  | 784 us                                                 | 992 us: 1.27x slower                                         |
| django_template         | 33.5 ms                                                | 42.6 ms: 1.27x slower                                        |
| gunicorn                | 1.20 ms                                                | 1.52 ms: 1.27x slower                                        |
| sqlglot_normalize       | 113 ms                                                 | 144 ms: 1.28x slower                                         |
| scimark_lu              | 116 ms                                                 | 149 ms: 1.28x slower                                         |
| aiohttp                 | 1.12 ms                                                | 1.44 ms: 1.29x slower                                        |
| pylint                  | 476 ms                                                 | 626 ms: 1.32x slower                                         |
| spectral_norm           | 108 ms                                                 | 143 ms: 1.32x slower                                         |
| regex_compile           | 141 ms                                                 | 186 ms: 1.32x slower                                         |
| float                   | 78.9 ms                                                | 104 ms: 1.32x slower                                         |
| unpickle                | 13.8 us                                                | 18.6 us: 1.34x slower                                        |
| raytrace                | 309 ms                                                 | 416 ms: 1.35x slower                                         |
| genshi_xml              | 53.4 ms                                                | 73.6 ms: 1.38x slower                                        |
| deltablue               | 3.92 ms                                                | 5.41 ms: 1.38x slower                                        |
| chaos                   | 71.9 ms                                                | 102 ms: 1.42x slower                                         |
| bench_thread_pool       | 834 us                                                 | 1.19 ms: 1.42x slower                                        |
| scimark_monte_carlo     | 70.7 ms                                                | 101 ms: 1.42x slower                                         |
| 2to3                    | 264 ms                                                 | 382 ms: 1.44x slower                                         |
| sqlglot_transpile       | 1.75 ms                                                | 2.55 ms: 1.46x slower                                        |
| pyflate                 | 434 ms                                                 | 636 ms: 1.47x slower                                         |
| sqlglot_parse           | 1.43 ms                                                | 2.18 ms: 1.52x slower                                        |
| mako                    | 10.7 ms                                                | 16.4 ms: 1.54x slower                                        |
| crypto_pyaes            | 76.7 ms                                                | 122 ms: 1.59x slower                                         |
| flaskblogging           | 7.28 ms                                                | 12.1 ms: 1.67x slower                                        |
| async_generators        | 374 ms                                                 | 626 ms: 1.68x slower                                         |
| nbody                   | 96.0 ms                                                | 172 ms: 1.79x slower                                         |
| docutils                | 2.66 sec                                               | 5.20 sec: 1.95x slower                                       |
| genshi_text             | 22.5 ms                                                | 52.1 ms: 2.31x slower                                        |
| coroutines              | 27.0 ms                                                | 72.5 ms: 2.68x slower                                        |
| coverage                | 78.8 ms                                                | 553 ms: 7.02x slower                                         |
| Geometric mean          | (ref)                                                  | 1.20x slower                                                 |

Benchmark hidden because not significant (2): deepcopy_memo, json_dumps
Ignored benchmarks (18) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (1) of results/bm-20221221-3.9.10-258cab1/bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1.json: mypy


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.16x
- 95% likely to have a slowdown of 1.15x
- 99% likely to have a slowdown of 1.11x


# Memory

- memory change: 1.42x