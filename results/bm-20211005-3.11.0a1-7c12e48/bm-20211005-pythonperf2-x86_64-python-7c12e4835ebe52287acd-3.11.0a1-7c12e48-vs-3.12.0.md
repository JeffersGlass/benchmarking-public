
# Results vs. 3.12.0

- fork: python
- ref: 7c12e4835ebe52287acd
- machine: linux-x86_64
- commit hash: 7c12e48
- commit date: 2021-10-05
- overall geometric mean: 1.16x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x slower
- Memory change: 0.87x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 329 ms: 1.15x slower                                                        |
| chameleon      | 7.23 ms                                                      | 8.97 ms: 1.24x slower                                                       |
| docutils       | 2.87 sec                                                     | 3.22 sec: 1.12x slower                                                      |
| tornado_http   | 121 ms                                                       | 136 ms: 1.12x slower                                                        |
| Geometric mean | (ref)                                                        | 1.16x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 452 ms                                                       | 515 ms: 1.14x slower                                                        |
| async_tree_cpu_io_mixed | 696 ms                                                       | 796 ms: 1.14x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.24 sec: 1.19x slower                                                      |
| async_tree_memoization  | 544 ms                                                       | 660 ms: 1.21x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.17x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 266 ms: 1.00x slower                                                        |
| float          | 76.6 ms                                                      | 86.6 ms: 1.13x slower                                                       |
| nbody          | 88.0 ms                                                      | 132 ms: 1.50x slower                                                        |
| Geometric mean | (ref)                                                        | 1.19x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.05 ms: 1.17x faster                                                       |
| regex_v8       | 23.6 ms                                                      | 25.6 ms: 1.08x slower                                                       |
| regex_dna      | 239 ms                                                       | 262 ms: 1.10x slower                                                        |
| regex_compile  | 144 ms                                                       | 169 ms: 1.17x slower                                                        |
| Geometric mean | (ref)                                                        | 1.05x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle             | 14.8 us                                                      | 13.7 us: 1.08x faster                                                       |
| pickle_list          | 4.43 us                                                      | 4.14 us: 1.07x faster                                                       |
| pickle_dict          | 32.5 us                                                      | 31.5 us: 1.03x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.54 us: 1.03x faster                                                       |
| pickle               | 10.5 us                                                      | 10.4 us: 1.01x faster                                                       |
| xml_etree_generate   | 86.1 ms                                                      | 86.0 ms: 1.00x faster                                                       |
| xml_etree_iterparse  | 103 ms                                                       | 111 ms: 1.08x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 64.1 ms: 1.10x slower                                                       |
| xml_etree_parse      | 144 ms                                                       | 158 ms: 1.10x slower                                                        |
| json_loads           | 24.4 us                                                      | 27.0 us: 1.11x slower                                                       |
| pickle_pure_python   | 318 us                                                       | 394 us: 1.24x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 13.6 ms: 1.33x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 293 us: 1.40x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.08x slower                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.57 ms: 1.14x faster                                                       |
| python_startup         | 11.6 ms                                                      | 11.8 ms: 1.01x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.06x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 47.5 ms: 1.24x slower                                                       |
| mako            | 10.0 ms                                                      | 13.1 ms: 1.31x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.27x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot            | 3.57 ms                                                      | 3.05 ms: 1.17x faster                                                       |
| unpack_sequence         | 53.2 ns                                                      | 46.5 ns: 1.14x faster                                                       |
| python_startup_no_site  | 8.64 ms                                                      | 7.57 ms: 1.14x faster                                                       |
| async_generators        | 390 ms                                                       | 356 ms: 1.09x faster                                                        |
| unpickle                | 14.8 us                                                      | 13.7 us: 1.08x faster                                                       |
| pickle_list             | 4.43 us                                                      | 4.14 us: 1.07x faster                                                       |
| telco                   | 6.96 ms                                                      | 6.66 ms: 1.05x faster                                                       |
| pickle_dict             | 32.5 us                                                      | 31.5 us: 1.03x faster                                                       |
| logging_format          | 7.48 us                                                      | 7.28 us: 1.03x faster                                                       |
| unpickle_list           | 4.66 us                                                      | 4.54 us: 1.03x faster                                                       |
| gunicorn                | 1.00 ms                                                      | 988 us: 1.01x faster                                                        |
| pickle                  | 10.5 us                                                      | 10.4 us: 1.01x faster                                                       |
| sqlite_synth            | 2.77 us                                                      | 2.76 us: 1.01x faster                                                       |
| xml_etree_generate      | 86.1 ms                                                      | 86.0 ms: 1.00x faster                                                       |
| pidigits                | 265 ms                                                       | 266 ms: 1.00x slower                                                        |
| python_startup          | 11.6 ms                                                      | 11.8 ms: 1.01x slower                                                       |
| gc_traversal            | 3.48 ms                                                      | 3.55 ms: 1.02x slower                                                       |
| meteor_contest          | 128 ms                                                       | 133 ms: 1.04x slower                                                        |
| json                    | 5.12 ms                                                      | 5.40 ms: 1.05x slower                                                       |
| bench_mp_pool           | 4.76 ms                                                      | 5.14 ms: 1.08x slower                                                       |
| coverage                | 66.7 ms                                                      | 72.0 ms: 1.08x slower                                                       |
| xml_etree_iterparse     | 103 ms                                                       | 111 ms: 1.08x slower                                                        |
| regex_v8                | 23.6 ms                                                      | 25.6 ms: 1.08x slower                                                       |
| pprint_safe_repr        | 807 ms                                                       | 879 ms: 1.09x slower                                                        |
| xml_etree_process       | 58.4 ms                                                      | 64.1 ms: 1.10x slower                                                       |
| regex_dna               | 239 ms                                                       | 262 ms: 1.10x slower                                                        |
| deepcopy_reduce         | 3.37 us                                                      | 3.70 us: 1.10x slower                                                       |
| xml_etree_parse         | 144 ms                                                       | 158 ms: 1.10x slower                                                        |
| dask                    | 392 ms                                                       | 433 ms: 1.10x slower                                                        |
| scimark_fft             | 301 ms                                                       | 333 ms: 1.11x slower                                                        |
| pprint_pformat          | 1.65 sec                                                     | 1.83 sec: 1.11x slower                                                      |
| mdp                     | 2.57 sec                                                     | 2.84 sec: 1.11x slower                                                      |
| json_loads              | 24.4 us                                                      | 27.0 us: 1.11x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 20.9 ms: 1.11x slower                                                       |
| sympy_integrate         | 23.9 ms                                                      | 26.8 ms: 1.12x slower                                                       |
| docutils                | 2.87 sec                                                     | 3.22 sec: 1.12x slower                                                      |
| tornado_http            | 121 ms                                                       | 136 ms: 1.12x slower                                                        |
| bench_thread_pool       | 950 us                                                       | 1.07 ms: 1.12x slower                                                       |
| float                   | 76.6 ms                                                      | 86.6 ms: 1.13x slower                                                       |
| sympy_str               | 302 ms                                                       | 343 ms: 1.13x slower                                                        |
| dulwich_log             | 65.4 ms                                                      | 74.2 ms: 1.14x slower                                                       |
| sympy_sum               | 162 ms                                                       | 184 ms: 1.14x slower                                                        |
| async_tree_none         | 452 ms                                                       | 515 ms: 1.14x slower                                                        |
| async_tree_cpu_io_mixed | 696 ms                                                       | 796 ms: 1.14x slower                                                        |
| pycparser               | 1.23 sec                                                     | 1.41 sec: 1.14x slower                                                      |
| nqueens                 | 89.9 ms                                                      | 103 ms: 1.14x slower                                                        |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 4.84 ms: 1.15x slower                                                       |
| 2to3                    | 285 ms                                                       | 329 ms: 1.15x slower                                                        |
| sqlglot_optimize        | 57.5 ms                                                      | 66.6 ms: 1.16x slower                                                       |
| deepcopy                | 368 us                                                       | 427 us: 1.16x slower                                                        |
| sqlglot_normalize       | 116 ms                                                       | 135 ms: 1.17x slower                                                        |
| regex_compile           | 144 ms                                                       | 169 ms: 1.17x slower                                                        |
| sympy_expand            | 484 ms                                                       | 573 ms: 1.18x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.24 sec: 1.19x slower                                                      |
| create_gc_cycles        | 1.59 ms                                                      | 1.90 ms: 1.20x slower                                                       |
| async_tree_memoization  | 544 ms                                                       | 660 ms: 1.21x slower                                                        |
| deepcopy_memo           | 36.8 us                                                      | 44.7 us: 1.22x slower                                                       |
| pickle_pure_python      | 318 us                                                       | 394 us: 1.24x slower                                                        |
| coroutines              | 23.0 ms                                                      | 28.5 ms: 1.24x slower                                                       |
| chameleon               | 7.23 ms                                                      | 8.97 ms: 1.24x slower                                                       |
| django_template         | 38.2 ms                                                      | 47.5 ms: 1.24x slower                                                       |
| raytrace                | 298 ms                                                       | 371 ms: 1.24x slower                                                        |
| scimark_monte_carlo     | 69.0 ms                                                      | 87.3 ms: 1.26x slower                                                       |
| crypto_pyaes            | 80.3 ms                                                      | 102 ms: 1.27x slower                                                        |
| mako                    | 10.0 ms                                                      | 13.1 ms: 1.31x slower                                                       |
| spectral_norm           | 91.6 ms                                                      | 120 ms: 1.31x slower                                                        |
| json_dumps              | 10.2 ms                                                      | 13.6 ms: 1.33x slower                                                       |
| comprehensions          | 21.9 us                                                      | 29.5 us: 1.35x slower                                                       |
| scimark_sor             | 109 ms                                                       | 147 ms: 1.35x slower                                                        |
| fannkuch                | 350 ms                                                       | 472 ms: 1.35x slower                                                        |
| chaos                   | 64.0 ms                                                      | 87.5 ms: 1.37x slower                                                       |
| hexiom                  | 5.96 ms                                                      | 8.15 ms: 1.37x slower                                                       |
| unpickle_pure_python    | 210 us                                                       | 293 us: 1.40x slower                                                        |
| generators              | 37.4 ms                                                      | 52.5 ms: 1.40x slower                                                       |
| pyflate                 | 439 ms                                                       | 615 ms: 1.40x slower                                                        |
| go                      | 150 ms                                                       | 211 ms: 1.41x slower                                                        |
| richards                | 45.7 ms                                                      | 64.9 ms: 1.42x slower                                                       |
| logging_silent          | 94.4 ns                                                      | 134 ns: 1.42x slower                                                        |
| scimark_lu              | 98.8 ms                                                      | 145 ms: 1.47x slower                                                        |
| nbody                   | 88.0 ms                                                      | 132 ms: 1.50x slower                                                        |
| sqlglot_transpile       | 1.78 ms                                                      | 2.76 ms: 1.55x slower                                                       |
| sqlglot_parse           | 1.38 ms                                                      | 2.37 ms: 1.72x slower                                                       |
| deltablue               | 3.24 ms                                                      | 5.73 ms: 1.77x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.16x slower                                                                |

Benchmark hidden because not significant (1): logging_simple
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (5) of results/bm-20211005-3.11.0a1-7c12e48/bm-20211005-pythonperf2-x86_64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48.json: flaskblogging, genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.13x
- 95% likely to have a slowdown of 1.12x
- 99% likely to have a slowdown of 1.12x


# Memory

- memory change: 0.87x