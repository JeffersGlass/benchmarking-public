
# Results vs. 3.12.0

- fork: python
- ref: 8d32a5c8c4e9c90b0a21
- machine: linux-x86_64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.04x slower \*
- HPT reliability: 99.91%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 281 ms: 1.01x faster                                                        |
| chameleon      | 7.23 ms                                                      | 7.53 ms: 1.04x slower                                                       |
| docutils       | 2.87 sec                                                     | 2.82 sec: 1.02x faster                                                      |
| Geometric mean | (ref)                                                        | 1.00x slower                                                                |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 748 ms: 1.07x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                                      |
| async_tree_none         | 452 ms                                                       | 516 ms: 1.14x slower                                                        |
| async_tree_memoization  | 544 ms                                                       | 624 ms: 1.15x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.12x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 251 ms: 1.05x faster                                                        |
| float          | 76.6 ms                                                      | 74.7 ms: 1.03x faster                                                       |
| nbody          | 88.0 ms                                                      | 100 ms: 1.14x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 2.97 ms: 1.20x faster                                                       |
| regex_v8       | 23.6 ms                                                      | 22.8 ms: 1.04x faster                                                       |
| regex_dna      | 239 ms                                                       | 232 ms: 1.03x faster                                                        |
| regex_compile  | 144 ms                                                       | 153 ms: 1.06x slower                                                        |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.81 us: 1.16x faster                                                       |
| unpickle             | 14.8 us                                                      | 13.3 us: 1.11x faster                                                       |
| pickle               | 10.5 us                                                      | 9.62 us: 1.09x faster                                                       |
| pickle_dict          | 32.5 us                                                      | 29.9 us: 1.09x faster                                                       |
| xml_etree_generate   | 86.1 ms                                                      | 80.3 ms: 1.07x faster                                                       |
| xml_etree_process    | 58.4 ms                                                      | 56.1 ms: 1.04x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.56 us: 1.02x faster                                                       |
| pickle_pure_python   | 318 us                                                       | 320 us: 1.01x slower                                                        |
| json_loads           | 24.4 us                                                      | 24.6 us: 1.01x slower                                                       |
| xml_etree_iterparse  | 103 ms                                                       | 105 ms: 1.02x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 155 ms: 1.08x slower                                                        |
| unpickle_pure_python | 210 us                                                       | 233 us: 1.11x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 13.5 ms: 1.32x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.68 ms: 1.13x faster                                                       |
| python_startup         | 11.6 ms                                                      | 10.5 ms: 1.10x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.11x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 41.3 ms: 1.08x slower                                                       |
| mako            | 10.0 ms                                                      | 10.9 ms: 1.09x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.09x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_generators        | 390 ms                                                       | 318 ms: 1.23x faster                                                        |
| regex_effbot            | 3.57 ms                                                      | 2.97 ms: 1.20x faster                                                       |
| pickle_list             | 4.43 us                                                      | 3.81 us: 1.16x faster                                                       |
| unpack_sequence         | 53.2 ns                                                      | 46.2 ns: 1.15x faster                                                       |
| python_startup_no_site  | 8.64 ms                                                      | 7.68 ms: 1.13x faster                                                       |
| unpickle                | 14.8 us                                                      | 13.3 us: 1.11x faster                                                       |
| sqlite_synth            | 2.77 us                                                      | 2.51 us: 1.10x faster                                                       |
| python_startup          | 11.6 ms                                                      | 10.5 ms: 1.10x faster                                                       |
| pickle                  | 10.5 us                                                      | 9.62 us: 1.09x faster                                                       |
| pickle_dict             | 32.5 us                                                      | 29.9 us: 1.09x faster                                                       |
| gunicorn                | 1.00 ms                                                      | 928 us: 1.08x faster                                                        |
| aiohttp                 | 1.02 ms                                                      | 945 us: 1.08x faster                                                        |
| xml_etree_generate      | 86.1 ms                                                      | 80.3 ms: 1.07x faster                                                       |
| pprint_safe_repr        | 807 ms                                                       | 755 ms: 1.07x faster                                                        |
| pprint_pformat          | 1.65 sec                                                     | 1.57 sec: 1.06x faster                                                      |
| pidigits                | 265 ms                                                       | 251 ms: 1.05x faster                                                        |
| bench_mp_pool           | 4.76 ms                                                      | 4.56 ms: 1.05x faster                                                       |
| xml_etree_process       | 58.4 ms                                                      | 56.1 ms: 1.04x faster                                                       |
| sqlalchemy_declarative  | 159 ms                                                       | 153 ms: 1.04x faster                                                        |
| regex_v8                | 23.6 ms                                                      | 22.8 ms: 1.04x faster                                                       |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 4.06 ms: 1.04x faster                                                       |
| regex_dna               | 239 ms                                                       | 232 ms: 1.03x faster                                                        |
| float                   | 76.6 ms                                                      | 74.7 ms: 1.03x faster                                                       |
| scimark_fft             | 301 ms                                                       | 294 ms: 1.02x faster                                                        |
| unpickle_list           | 4.66 us                                                      | 4.56 us: 1.02x faster                                                       |
| docutils                | 2.87 sec                                                     | 2.82 sec: 1.02x faster                                                      |
| 2to3                    | 285 ms                                                       | 281 ms: 1.01x faster                                                        |
| pyflate                 | 439 ms                                                       | 433 ms: 1.01x faster                                                        |
| pathlib                 | 18.9 ms                                                      | 18.8 ms: 1.00x faster                                                       |
| scimark_monte_carlo     | 69.0 ms                                                      | 69.2 ms: 1.00x slower                                                       |
| pickle_pure_python      | 318 us                                                       | 320 us: 1.01x slower                                                        |
| scimark_sor             | 109 ms                                                       | 110 ms: 1.01x slower                                                        |
| json_loads              | 24.4 us                                                      | 24.6 us: 1.01x slower                                                       |
| deepcopy_reduce         | 3.37 us                                                      | 3.42 us: 1.02x slower                                                       |
| spectral_norm           | 91.6 ms                                                      | 93.1 ms: 1.02x slower                                                       |
| xml_etree_iterparse     | 103 ms                                                       | 105 ms: 1.02x slower                                                        |
| pycparser               | 1.23 sec                                                     | 1.26 sec: 1.02x slower                                                      |
| deepcopy_memo           | 36.8 us                                                      | 37.6 us: 1.02x slower                                                       |
| logging_format          | 7.48 us                                                      | 7.67 us: 1.02x slower                                                       |
| crypto_pyaes            | 80.3 ms                                                      | 82.3 ms: 1.02x slower                                                       |
| meteor_contest          | 128 ms                                                       | 131 ms: 1.02x slower                                                        |
| sqlglot_optimize        | 57.5 ms                                                      | 58.9 ms: 1.03x slower                                                       |
| sqlglot_normalize       | 116 ms                                                       | 119 ms: 1.03x slower                                                        |
| logging_simple          | 6.71 us                                                      | 6.90 us: 1.03x slower                                                       |
| create_gc_cycles        | 1.59 ms                                                      | 1.64 ms: 1.03x slower                                                       |
| raytrace                | 298 ms                                                       | 309 ms: 1.04x slower                                                        |
| dulwich_log             | 65.4 ms                                                      | 68.0 ms: 1.04x slower                                                       |
| sqlalchemy_imperative   | 18.7 ms                                                      | 19.5 ms: 1.04x slower                                                       |
| chameleon               | 7.23 ms                                                      | 7.53 ms: 1.04x slower                                                       |
| go                      | 150 ms                                                       | 156 ms: 1.04x slower                                                        |
| sympy_integrate         | 23.9 ms                                                      | 25.2 ms: 1.05x slower                                                       |
| logging_silent          | 94.4 ns                                                      | 99.8 ns: 1.06x slower                                                       |
| regex_compile           | 144 ms                                                       | 153 ms: 1.06x slower                                                        |
| nqueens                 | 89.9 ms                                                      | 95.8 ms: 1.07x slower                                                       |
| dask                    | 392 ms                                                       | 418 ms: 1.07x slower                                                        |
| deepcopy                | 368 us                                                       | 394 us: 1.07x slower                                                        |
| bench_thread_pool       | 950 us                                                       | 1.02 ms: 1.07x slower                                                       |
| async_tree_cpu_io_mixed | 696 ms                                                       | 748 ms: 1.07x slower                                                        |
| xml_etree_parse         | 144 ms                                                       | 155 ms: 1.08x slower                                                        |
| django_template         | 38.2 ms                                                      | 41.3 ms: 1.08x slower                                                       |
| mdp                     | 2.57 sec                                                     | 2.78 sec: 1.08x slower                                                      |
| sympy_str               | 302 ms                                                       | 329 ms: 1.09x slower                                                        |
| mako                    | 10.0 ms                                                      | 10.9 ms: 1.09x slower                                                       |
| richards                | 45.7 ms                                                      | 50.1 ms: 1.10x slower                                                       |
| sympy_sum               | 162 ms                                                       | 178 ms: 1.10x slower                                                        |
| gc_traversal            | 3.48 ms                                                      | 3.85 ms: 1.11x slower                                                       |
| unpickle_pure_python    | 210 us                                                       | 233 us: 1.11x slower                                                        |
| sympy_expand            | 484 ms                                                       | 540 ms: 1.12x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                                      |
| chaos                   | 64.0 ms                                                      | 72.4 ms: 1.13x slower                                                       |
| nbody                   | 88.0 ms                                                      | 100 ms: 1.14x slower                                                        |
| async_tree_none         | 452 ms                                                       | 516 ms: 1.14x slower                                                        |
| async_tree_memoization  | 544 ms                                                       | 624 ms: 1.15x slower                                                        |
| scimark_lu              | 98.8 ms                                                      | 114 ms: 1.15x slower                                                        |
| hexiom                  | 5.96 ms                                                      | 6.91 ms: 1.16x slower                                                       |
| fannkuch                | 350 ms                                                       | 418 ms: 1.19x slower                                                        |
| deltablue               | 3.24 ms                                                      | 3.93 ms: 1.21x slower                                                       |
| coroutines              | 23.0 ms                                                      | 28.0 ms: 1.22x slower                                                       |
| comprehensions          | 21.9 us                                                      | 28.2 us: 1.29x slower                                                       |
| sqlglot_transpile       | 1.78 ms                                                      | 2.30 ms: 1.30x slower                                                       |
| json_dumps              | 10.2 ms                                                      | 13.5 ms: 1.32x slower                                                       |
| sqlglot_parse           | 1.38 ms                                                      | 1.95 ms: 1.41x slower                                                       |
| generators              | 37.4 ms                                                      | 55.5 ms: 1.48x slower                                                       |
| asyncio_tcp             | 378 ms                                                       | 749 ms: 1.98x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.04x slower                                                                |

Benchmark hidden because not significant (3): tornado_http, telco, json
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, coverage, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20220506-3.11.0b1-8d32a5c/bm-20220506-pythonperf2-x86_64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.91% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.90x