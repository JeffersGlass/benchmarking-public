
# Results vs. 3.12.0

- fork: python
- ref: 3ddfa55df48a67a5972f
- machine: linux-x86_64
- commit hash: 3ddfa55
- commit date: 2022-03-07
- overall geometric mean: 1.12x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x slower
- Memory change: 0.95x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 300 ms: 1.05x slower                                                        |
| chameleon      | 7.23 ms                                                      | 8.43 ms: 1.17x slower                                                       |
| docutils       | 2.87 sec                                                     | 2.98 sec: 1.04x slower                                                      |
| tornado_http   | 121 ms                                                       | 130 ms: 1.07x slower                                                        |
| Geometric mean | (ref)                                                        | 1.08x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 763 ms: 1.10x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.19 sec: 1.14x slower                                                      |
| async_tree_none         | 452 ms                                                       | 532 ms: 1.18x slower                                                        |
| async_tree_memoization  | 544 ms                                                       | 651 ms: 1.20x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.15x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 253 ms: 1.05x faster                                                        |
| float          | 76.6 ms                                                      | 79.1 ms: 1.03x slower                                                       |
| nbody          | 88.0 ms                                                      | 98.0 ms: 1.11x slower                                                       |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.49 ms: 1.02x faster                                                       |
| regex_dna      | 239 ms                                                       | 257 ms: 1.08x slower                                                        |
| regex_v8       | 23.6 ms                                                      | 26.4 ms: 1.12x slower                                                       |
| regex_compile  | 144 ms                                                       | 161 ms: 1.12x slower                                                        |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle             | 14.8 us                                                      | 13.5 us: 1.10x faster                                                       |
| pickle               | 10.5 us                                                      | 9.96 us: 1.06x faster                                                       |
| pickle_list          | 4.43 us                                                      | 4.28 us: 1.03x faster                                                       |
| xml_etree_generate   | 86.1 ms                                                      | 83.5 ms: 1.03x faster                                                       |
| json_loads           | 24.4 us                                                      | 23.9 us: 1.02x faster                                                       |
| pickle_dict          | 32.5 us                                                      | 32.2 us: 1.01x faster                                                       |
| xml_etree_iterparse  | 103 ms                                                       | 104 ms: 1.02x slower                                                        |
| xml_etree_process    | 58.4 ms                                                      | 59.4 ms: 1.02x slower                                                       |
| xml_etree_parse      | 144 ms                                                       | 154 ms: 1.07x slower                                                        |
| pickle_pure_python   | 318 us                                                       | 352 us: 1.11x slower                                                        |
| unpickle_pure_python | 210 us                                                       | 273 us: 1.30x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 13.6 ms: 1.33x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.04x slower                                                                |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.55 ms: 1.14x faster                                                       |
| python_startup         | 11.6 ms                                                      | 10.4 ms: 1.11x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.13x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 10.0 ms                                                      | 11.4 ms: 1.14x slower                                                       |
| django_template | 38.2 ms                                                      | 43.8 ms: 1.15x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.15x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_generators        | 390 ms                                                       | 320 ms: 1.22x faster                                                        |
| python_startup_no_site  | 8.64 ms                                                      | 7.55 ms: 1.14x faster                                                       |
| python_startup          | 11.6 ms                                                      | 10.4 ms: 1.11x faster                                                       |
| unpickle                | 14.8 us                                                      | 13.5 us: 1.10x faster                                                       |
| sqlite_synth            | 2.77 us                                                      | 2.54 us: 1.09x faster                                                       |
| pickle                  | 10.5 us                                                      | 9.96 us: 1.06x faster                                                       |
| pidigits                | 265 ms                                                       | 253 ms: 1.05x faster                                                        |
| pickle_list             | 4.43 us                                                      | 4.28 us: 1.03x faster                                                       |
| xml_etree_generate      | 86.1 ms                                                      | 83.5 ms: 1.03x faster                                                       |
| regex_effbot            | 3.57 ms                                                      | 3.49 ms: 1.02x faster                                                       |
| json_loads              | 24.4 us                                                      | 23.9 us: 1.02x faster                                                       |
| json                    | 5.12 ms                                                      | 5.04 ms: 1.02x faster                                                       |
| aiohttp                 | 1.02 ms                                                      | 1.00 ms: 1.02x faster                                                       |
| pickle_dict             | 32.5 us                                                      | 32.2 us: 1.01x faster                                                       |
| telco                   | 6.96 ms                                                      | 6.90 ms: 1.01x faster                                                       |
| gunicorn                | 1.00 ms                                                      | 994 us: 1.01x faster                                                        |
| scimark_fft             | 301 ms                                                       | 305 ms: 1.01x slower                                                        |
| xml_etree_iterparse     | 103 ms                                                       | 104 ms: 1.02x slower                                                        |
| xml_etree_process       | 58.4 ms                                                      | 59.4 ms: 1.02x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                       |
| create_gc_cycles        | 1.59 ms                                                      | 1.63 ms: 1.03x slower                                                       |
| sqlalchemy_declarative  | 159 ms                                                       | 164 ms: 1.03x slower                                                        |
| float                   | 76.6 ms                                                      | 79.1 ms: 1.03x slower                                                       |
| meteor_contest          | 128 ms                                                       | 133 ms: 1.03x slower                                                        |
| logging_format          | 7.48 us                                                      | 7.75 us: 1.04x slower                                                       |
| docutils                | 2.87 sec                                                     | 2.98 sec: 1.04x slower                                                      |
| 2to3                    | 285 ms                                                       | 300 ms: 1.05x slower                                                        |
| logging_simple          | 6.71 us                                                      | 7.08 us: 1.05x slower                                                       |
| pprint_safe_repr        | 807 ms                                                       | 853 ms: 1.06x slower                                                        |
| xml_etree_parse         | 144 ms                                                       | 154 ms: 1.07x slower                                                        |
| pprint_pformat          | 1.65 sec                                                     | 1.77 sec: 1.07x slower                                                      |
| tornado_http            | 121 ms                                                       | 130 ms: 1.07x slower                                                        |
| regex_dna               | 239 ms                                                       | 257 ms: 1.08x slower                                                        |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 4.53 ms: 1.08x slower                                                       |
| scimark_monte_carlo     | 69.0 ms                                                      | 74.4 ms: 1.08x slower                                                       |
| sympy_integrate         | 23.9 ms                                                      | 25.9 ms: 1.08x slower                                                       |
| async_tree_cpu_io_mixed | 696 ms                                                       | 763 ms: 1.10x slower                                                        |
| bench_thread_pool       | 950 us                                                       | 1.04 ms: 1.10x slower                                                       |
| pickle_pure_python      | 318 us                                                       | 352 us: 1.11x slower                                                        |
| deepcopy_reduce         | 3.37 us                                                      | 3.73 us: 1.11x slower                                                       |
| scimark_sor             | 109 ms                                                       | 121 ms: 1.11x slower                                                        |
| sqlglot_optimize        | 57.5 ms                                                      | 63.7 ms: 1.11x slower                                                       |
| nbody                   | 88.0 ms                                                      | 98.0 ms: 1.11x slower                                                       |
| regex_v8                | 23.6 ms                                                      | 26.4 ms: 1.12x slower                                                       |
| nqueens                 | 89.9 ms                                                      | 100 ms: 1.12x slower                                                        |
| regex_compile           | 144 ms                                                       | 161 ms: 1.12x slower                                                        |
| deepcopy                | 368 us                                                       | 413 us: 1.12x slower                                                        |
| sqlalchemy_imperative   | 18.7 ms                                                      | 21.0 ms: 1.12x slower                                                       |
| pyflate                 | 439 ms                                                       | 494 ms: 1.13x slower                                                        |
| dask                    | 392 ms                                                       | 442 ms: 1.13x slower                                                        |
| dulwich_log             | 65.4 ms                                                      | 73.8 ms: 1.13x slower                                                       |
| mdp                     | 2.57 sec                                                     | 2.91 sec: 1.13x slower                                                      |
| sqlglot_normalize       | 116 ms                                                       | 131 ms: 1.13x slower                                                        |
| deepcopy_memo           | 36.8 us                                                      | 41.7 us: 1.13x slower                                                       |
| sympy_str               | 302 ms                                                       | 343 ms: 1.14x slower                                                        |
| sympy_sum               | 162 ms                                                       | 184 ms: 1.14x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.19 sec: 1.14x slower                                                      |
| mako                    | 10.0 ms                                                      | 11.4 ms: 1.14x slower                                                       |
| django_template         | 38.2 ms                                                      | 43.8 ms: 1.15x slower                                                       |
| raytrace                | 298 ms                                                       | 343 ms: 1.15x slower                                                        |
| pycparser               | 1.23 sec                                                     | 1.43 sec: 1.16x slower                                                      |
| gc_traversal            | 3.48 ms                                                      | 4.03 ms: 1.16x slower                                                       |
| crypto_pyaes            | 80.3 ms                                                      | 93.5 ms: 1.16x slower                                                       |
| chameleon               | 7.23 ms                                                      | 8.43 ms: 1.17x slower                                                       |
| async_tree_none         | 452 ms                                                       | 532 ms: 1.18x slower                                                        |
| sympy_expand            | 484 ms                                                       | 573 ms: 1.18x slower                                                        |
| go                      | 150 ms                                                       | 178 ms: 1.19x slower                                                        |
| async_tree_memoization  | 544 ms                                                       | 651 ms: 1.20x slower                                                        |
| spectral_norm           | 91.6 ms                                                      | 111 ms: 1.21x slower                                                        |
| chaos                   | 64.0 ms                                                      | 77.5 ms: 1.21x slower                                                       |
| logging_silent          | 94.4 ns                                                      | 115 ns: 1.22x slower                                                        |
| richards                | 45.7 ms                                                      | 55.9 ms: 1.22x slower                                                       |
| scimark_lu              | 98.8 ms                                                      | 122 ms: 1.23x slower                                                        |
| coverage                | 66.7 ms                                                      | 84.1 ms: 1.26x slower                                                       |
| fannkuch                | 350 ms                                                       | 453 ms: 1.29x slower                                                        |
| hexiom                  | 5.96 ms                                                      | 7.74 ms: 1.30x slower                                                       |
| unpickle_pure_python    | 210 us                                                       | 273 us: 1.30x slower                                                        |
| coroutines              | 23.0 ms                                                      | 30.1 ms: 1.31x slower                                                       |
| json_dumps              | 10.2 ms                                                      | 13.6 ms: 1.33x slower                                                       |
| comprehensions          | 21.9 us                                                      | 29.6 us: 1.35x slower                                                       |
| deltablue               | 3.24 ms                                                      | 4.49 ms: 1.39x slower                                                       |
| sqlglot_transpile       | 1.78 ms                                                      | 2.50 ms: 1.41x slower                                                       |
| generators              | 37.4 ms                                                      | 54.8 ms: 1.47x slower                                                       |
| sqlglot_parse           | 1.38 ms                                                      | 2.13 ms: 1.55x slower                                                       |
| asyncio_tcp             | 378 ms                                                       | 757 ms: 2.00x slower                                                        |
| unpack_sequence         | 53.2 ns                                                      | 152 ns: 2.85x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.12x slower                                                                |

Benchmark hidden because not significant (2): unpickle_list, bench_mp_pool
Ignored benchmarks (10) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (5) of results/bm-20220307-3.11.0a6-3ddfa55/bm-20220307-pythonperf2-x86_64-python-3ddfa55df48a67a5972f-3.11.0a6-3ddfa55.json: flaskblogging, genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.10x
- 95% likely to have a slowdown of 1.09x
- 99% likely to have a slowdown of 1.07x


# Memory

- memory change: 0.95x