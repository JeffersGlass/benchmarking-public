
# Results vs. 3.12.0

- fork: faster_cpython
- ref: nogil
- machine: linux-x86_64
- commit hash: 258cab1
- commit date: 2022-12-21
- overall geometric mean: 1.18x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x slower
- Memory change: 1.36x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 382 ms: 1.39x slower                                         |
| chameleon      | 7.41 ms                                                | 8.20 ms: 1.11x slower                                        |
| docutils       | 2.77 sec                                               | 5.20 sec: 1.88x slower                                       |
| tornado_http   | 103 ms                                                 | 124 ms: 1.21x slower                                         |
| Geometric mean | (ref)                                                  | 1.37x slower                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_io           | 1.16 sec                                               | 829 ms: 1.39x faster                                         |
| async_tree_none         | 472 ms                                                 | 372 ms: 1.27x faster                                         |
| async_tree_memoization  | 578 ms                                                 | 460 ms: 1.26x faster                                         |
| async_tree_cpu_io_mixed | 726 ms                                                 | 614 ms: 1.18x faster                                         |
| Geometric mean          | (ref)                                                  | 1.27x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 186 ms: 1.01x faster                                         |
| float          | 84.7 ms                                                | 104 ms: 1.23x slower                                         |
| nbody          | 97.0 ms                                                | 172 ms: 1.77x slower                                         |
| Geometric mean | (ref)                                                  | 1.29x slower                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.35 ms: 1.08x faster                                        |
| regex_dna      | 212 ms                                                 | 218 ms: 1.03x slower                                         |
| regex_v8       | 23.1 ms                                                | 24.1 ms: 1.04x slower                                        |
| regex_compile  | 148 ms                                                 | 186 ms: 1.26x slower                                         |
| Geometric mean | (ref)                                                  | 1.06x slower                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 25.3 us: 1.40x faster                                        |
| pickle_list          | 5.08 us                                                | 4.17 us: 1.22x faster                                        |
| pickle               | 11.6 us                                                | 10.0 us: 1.16x faster                                        |
| xml_etree_iterparse  | 107 ms                                                 | 95.5 ms: 1.12x faster                                        |
| xml_etree_parse      | 159 ms                                                 | 149 ms: 1.07x faster                                         |
| xml_etree_generate   | 89.2 ms                                                | 87.8 ms: 1.01x faster                                        |
| pickle_pure_python   | 324 us                                                 | 346 us: 1.07x slower                                         |
| unpickle_list        | 5.29 us                                                | 5.80 us: 1.10x slower                                        |
| json_loads           | 28.5 us                                                | 32.5 us: 1.14x slower                                        |
| unpickle_pure_python | 230 us                                                 | 262 us: 1.14x slower                                         |
| xml_etree_process    | 61.7 ms                                                | 71.4 ms: 1.16x slower                                        |
| unpickle             | 15.9 us                                                | 18.6 us: 1.17x slower                                        |
| json_dumps           | 10.4 ms                                                | 13.4 ms: 1.29x slower                                        |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.91 ms: 1.17x faster                                        |
| python_startup         | 9.55 ms                                                | 9.41 ms: 1.02x faster                                        |
| Geometric mean         | (ref)                                                  | 1.09x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| django_template | 34.6 ms                                                | 42.6 ms: 1.23x slower                                        |
| mako            | 11.9 ms                                                | 16.4 ms: 1.38x slower                                        |
| Geometric mean  | (ref)                                                  | 1.30x slower                                                 |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_dict             | 35.5 us                                                | 25.3 us: 1.40x faster                                        |
| async_tree_io           | 1.16 sec                                               | 829 ms: 1.39x faster                                         |
| async_tree_none         | 472 ms                                                 | 372 ms: 1.27x faster                                         |
| async_tree_memoization  | 578 ms                                                 | 460 ms: 1.26x faster                                         |
| pickle_list             | 5.08 us                                                | 4.17 us: 1.22x faster                                        |
| async_tree_cpu_io_mixed | 726 ms                                                 | 614 ms: 1.18x faster                                         |
| python_startup_no_site  | 6.94 ms                                                | 5.91 ms: 1.17x faster                                        |
| richards                | 45.8 ms                                                | 39.3 ms: 1.16x faster                                        |
| pickle                  | 11.6 us                                                | 10.0 us: 1.16x faster                                        |
| pprint_pformat          | 1.57 sec                                               | 1.40 sec: 1.12x faster                                       |
| xml_etree_iterparse     | 107 ms                                                 | 95.5 ms: 1.12x faster                                        |
| logging_silent          | 104 ns                                                 | 96.0 ns: 1.09x faster                                        |
| regex_effbot            | 3.61 ms                                                | 3.35 ms: 1.08x faster                                        |
| xml_etree_parse         | 159 ms                                                 | 149 ms: 1.07x faster                                         |
| unpack_sequence         | 54.0 ns                                                | 52.4 ns: 1.03x faster                                        |
| deepcopy_memo           | 40.7 us                                                | 40.1 us: 1.02x faster                                        |
| python_startup          | 9.55 ms                                                | 9.41 ms: 1.02x faster                                        |
| xml_etree_generate      | 89.2 ms                                                | 87.8 ms: 1.01x faster                                        |
| pidigits                | 187 ms                                                 | 186 ms: 1.01x faster                                         |
| bench_mp_pool           | 24.0 ms                                                | 23.8 ms: 1.01x faster                                        |
| json                    | 5.26 ms                                                | 5.37 ms: 1.02x slower                                        |
| regex_dna               | 212 ms                                                 | 218 ms: 1.03x slower                                         |
| regex_v8                | 23.1 ms                                                | 24.1 ms: 1.04x slower                                        |
| deepcopy                | 371 us                                                 | 393 us: 1.06x slower                                         |
| logging_format          | 7.23 us                                                | 7.69 us: 1.06x slower                                        |
| pathlib                 | 19.3 ms                                                | 20.6 ms: 1.07x slower                                        |
| pickle_pure_python      | 324 us                                                 | 346 us: 1.07x slower                                         |
| logging_simple          | 6.46 us                                                | 6.95 us: 1.08x slower                                        |
| deepcopy_reduce         | 3.35 us                                                | 3.63 us: 1.09x slower                                        |
| unpickle_list           | 5.29 us                                                | 5.80 us: 1.10x slower                                        |
| chameleon               | 7.41 ms                                                | 8.20 ms: 1.11x slower                                        |
| sympy_expand            | 478 ms                                                 | 531 ms: 1.11x slower                                         |
| scimark_sor             | 129 ms                                                 | 144 ms: 1.12x slower                                         |
| sympy_str               | 300 ms                                                 | 335 ms: 1.12x slower                                         |
| dulwich_log             | 68.5 ms                                                | 77.0 ms: 1.12x slower                                        |
| scimark_fft             | 382 ms                                                 | 430 ms: 1.13x slower                                         |
| meteor_contest          | 112 ms                                                 | 127 ms: 1.13x slower                                         |
| json_loads              | 28.5 us                                                | 32.5 us: 1.14x slower                                        |
| unpickle_pure_python    | 230 us                                                 | 262 us: 1.14x slower                                         |
| go                      | 139 ms                                                 | 159 ms: 1.14x slower                                         |
| sqlite_synth            | 2.83 us                                                | 3.24 us: 1.14x slower                                        |
| pycparser               | 1.18 sec                                               | 1.35 sec: 1.15x slower                                       |
| xml_etree_process       | 61.7 ms                                                | 71.4 ms: 1.16x slower                                        |
| unpickle                | 15.9 us                                                | 18.6 us: 1.17x slower                                        |
| fannkuch                | 417 ms                                                 | 490 ms: 1.17x slower                                         |
| mdp                     | 2.63 sec                                               | 3.10 sec: 1.18x slower                                       |
| sympy_integrate         | 21.4 ms                                                | 25.4 ms: 1.19x slower                                        |
| scimark_sparse_mat_mult | 5.06 ms                                                | 6.09 ms: 1.20x slower                                        |
| hexiom                  | 6.41 ms                                                | 7.74 ms: 1.21x slower                                        |
| tornado_http            | 103 ms                                                 | 124 ms: 1.21x slower                                         |
| gunicorn                | 1.24 ms                                                | 1.52 ms: 1.23x slower                                        |
| django_template         | 34.6 ms                                                | 42.6 ms: 1.23x slower                                        |
| float                   | 84.7 ms                                                | 104 ms: 1.23x slower                                         |
| spectral_norm           | 115 ms                                                 | 143 ms: 1.24x slower                                         |
| aiohttp                 | 1.15 ms                                                | 1.44 ms: 1.25x slower                                        |
| sympy_sum               | 169 ms                                                 | 212 ms: 1.25x slower                                         |
| regex_compile           | 148 ms                                                 | 186 ms: 1.26x slower                                         |
| sqlglot_optimize        | 54.8 ms                                                | 69.3 ms: 1.26x slower                                        |
| scimark_lu              | 118 ms                                                 | 149 ms: 1.27x slower                                         |
| json_dumps              | 10.4 ms                                                | 13.4 ms: 1.29x slower                                        |
| nqueens                 | 83.3 ms                                                | 109 ms: 1.31x slower                                         |
| sqlglot_normalize       | 110 ms                                                 | 144 ms: 1.31x slower                                         |
| pyflate                 | 482 ms                                                 | 636 ms: 1.32x slower                                         |
| raytrace                | 312 ms                                                 | 416 ms: 1.33x slower                                         |
| scimark_monte_carlo     | 75.1 ms                                                | 101 ms: 1.34x slower                                         |
| async_generators        | 463 ms                                                 | 626 ms: 1.35x slower                                         |
| mako                    | 11.9 ms                                                | 16.4 ms: 1.38x slower                                        |
| 2to3                    | 274 ms                                                 | 382 ms: 1.39x slower                                         |
| bench_thread_pool       | 842 us                                                 | 1.19 ms: 1.41x slower                                        |
| deltablue               | 3.72 ms                                                | 5.41 ms: 1.46x slower                                        |
| crypto_pyaes            | 81.9 ms                                                | 122 ms: 1.49x slower                                         |
| sqlglot_transpile       | 1.68 ms                                                | 2.55 ms: 1.51x slower                                        |
| chaos                   | 67.0 ms                                                | 102 ms: 1.52x slower                                         |
| sqlglot_parse           | 1.36 ms                                                | 2.18 ms: 1.60x slower                                        |
| nbody                   | 97.0 ms                                                | 172 ms: 1.77x slower                                         |
| docutils                | 2.77 sec                                               | 5.20 sec: 1.88x slower                                       |
| generators              | 31.2 ms                                                | 81.6 ms: 2.61x slower                                        |
| coroutines              | 23.2 ms                                                | 72.5 ms: 3.13x slower                                        |
| coverage                | 72.7 ms                                                | 553 ms: 7.60x slower                                         |
| Geometric mean          | (ref)                                                  | 1.18x slower                                                 |

Benchmark hidden because not significant (1): telco
Ignored benchmarks (18) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (8) of results/bm-20221221-3.9.10-258cab1/bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, mypy, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.13x
- 95% likely to have a slowdown of 1.12x
- 99% likely to have a slowdown of 1.11x


# Memory

- memory change: 1.36x