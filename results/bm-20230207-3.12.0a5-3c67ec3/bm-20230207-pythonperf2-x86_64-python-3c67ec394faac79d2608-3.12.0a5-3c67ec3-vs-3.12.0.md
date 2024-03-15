
# Results vs. 3.12.0

- fork: python
- ref: 3c67ec394faac79d2608
- machine: linux-x86_64
- commit hash: 3c67ec3
- commit date: 2023-02-07
- overall geometric mean: 1.01x slower \*
- HPT reliability: 97.24%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 282 ms: 1.01x faster                                                        |
| chameleon      | 7.23 ms                                                      | 7.46 ms: 1.03x slower                                                       |
| docutils       | 2.87 sec                                                     | 2.78 sec: 1.03x faster                                                      |
| tornado_http   | 121 ms                                                       | 117 ms: 1.04x faster                                                        |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 737 ms: 1.06x slower                                                        |
| async_tree_memoization  | 544 ms                                                       | 601 ms: 1.10x slower                                                        |
| async_tree_none         | 452 ms                                                       | 503 ms: 1.11x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                                      |
| Geometric mean          | (ref)                                                        | 1.10x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 71.9 ms: 1.07x faster                                                       |
| pidigits       | 265 ms                                                       | 251 ms: 1.06x faster                                                        |
| nbody          | 88.0 ms                                                      | 101 ms: 1.15x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_v8       | 23.6 ms                                                      | 22.7 ms: 1.04x faster                                                       |
| regex_effbot   | 3.57 ms                                                      | 3.50 ms: 1.02x faster                                                       |
| regex_compile  | 144 ms                                                       | 145 ms: 1.01x slower                                                        |
| regex_dna      | 239 ms                                                       | 240 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpickle             | 14.8 us                                                      | 12.8 us: 1.16x faster                                                       |
| pickle_list          | 4.43 us                                                      | 3.84 us: 1.15x faster                                                       |
| xml_etree_generate   | 86.1 ms                                                      | 80.6 ms: 1.07x faster                                                       |
| pickle               | 10.5 us                                                      | 9.88 us: 1.07x faster                                                       |
| xml_etree_process    | 58.4 ms                                                      | 55.6 ms: 1.05x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.50 us: 1.03x faster                                                       |
| pickle_dict          | 32.5 us                                                      | 31.6 us: 1.03x faster                                                       |
| unpickle_pure_python | 210 us                                                       | 204 us: 1.03x faster                                                        |
| json_loads           | 24.4 us                                                      | 23.8 us: 1.02x faster                                                       |
| pickle_pure_python   | 318 us                                                       | 312 us: 1.02x faster                                                        |
| json_dumps           | 10.2 ms                                                      | 10.0 ms: 1.02x faster                                                       |
| Geometric mean       | (ref)                                                        | 1.05x faster                                                                |

Benchmark hidden because not significant (2): xml_etree_parse, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 8.25 ms: 1.05x faster                                                       |
| python_startup         | 11.6 ms                                                      | 11.2 ms: 1.04x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.04x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 10.0 ms                                                      | 10.3 ms: 1.03x slower                                                       |
| django_template | 38.2 ms                                                      | 40.5 ms: 1.06x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.04x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpack_sequence         | 53.2 ns                                                      | 43.3 ns: 1.23x faster                                                       |
| async_generators        | 390 ms                                                       | 325 ms: 1.20x faster                                                        |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 3.61 ms: 1.17x faster                                                       |
| unpickle                | 14.8 us                                                      | 12.8 us: 1.16x faster                                                       |
| pickle_list             | 4.43 us                                                      | 3.84 us: 1.15x faster                                                       |
| pprint_safe_repr        | 807 ms                                                       | 744 ms: 1.09x faster                                                        |
| scimark_fft             | 301 ms                                                       | 278 ms: 1.08x faster                                                        |
| pprint_pformat          | 1.65 sec                                                     | 1.53 sec: 1.08x faster                                                      |
| sqlite_synth            | 2.77 us                                                      | 2.58 us: 1.08x faster                                                       |
| xml_etree_generate      | 86.1 ms                                                      | 80.6 ms: 1.07x faster                                                       |
| float                   | 76.6 ms                                                      | 71.9 ms: 1.07x faster                                                       |
| pickle                  | 10.5 us                                                      | 9.88 us: 1.07x faster                                                       |
| telco                   | 6.96 ms                                                      | 6.59 ms: 1.06x faster                                                       |
| pidigits                | 265 ms                                                       | 251 ms: 1.06x faster                                                        |
| xml_etree_process       | 58.4 ms                                                      | 55.6 ms: 1.05x faster                                                       |
| python_startup_no_site  | 8.64 ms                                                      | 8.25 ms: 1.05x faster                                                       |
| regex_v8                | 23.6 ms                                                      | 22.7 ms: 1.04x faster                                                       |
| python_startup          | 11.6 ms                                                      | 11.2 ms: 1.04x faster                                                       |
| tornado_http            | 121 ms                                                       | 117 ms: 1.04x faster                                                        |
| scimark_sor             | 109 ms                                                       | 105 ms: 1.04x faster                                                        |
| json                    | 5.12 ms                                                      | 4.94 ms: 1.04x faster                                                       |
| unpickle_list           | 4.66 us                                                      | 4.50 us: 1.03x faster                                                       |
| docutils                | 2.87 sec                                                     | 2.78 sec: 1.03x faster                                                      |
| pickle_dict             | 32.5 us                                                      | 31.6 us: 1.03x faster                                                       |
| comprehensions          | 21.9 us                                                      | 21.3 us: 1.03x faster                                                       |
| deepcopy_memo           | 36.8 us                                                      | 35.8 us: 1.03x faster                                                       |
| unpickle_pure_python    | 210 us                                                       | 204 us: 1.03x faster                                                        |
| pyflate                 | 439 ms                                                       | 428 ms: 1.02x faster                                                        |
| json_loads              | 24.4 us                                                      | 23.8 us: 1.02x faster                                                       |
| deepcopy_reduce         | 3.37 us                                                      | 3.30 us: 1.02x faster                                                       |
| pickle_pure_python      | 318 us                                                       | 312 us: 1.02x faster                                                        |
| regex_effbot            | 3.57 ms                                                      | 3.50 ms: 1.02x faster                                                       |
| json_dumps              | 10.2 ms                                                      | 10.0 ms: 1.02x faster                                                       |
| 2to3                    | 285 ms                                                       | 282 ms: 1.01x faster                                                        |
| logging_format          | 7.48 us                                                      | 7.43 us: 1.01x faster                                                       |
| sqlglot_optimize        | 57.5 ms                                                      | 57.7 ms: 1.00x slower                                                       |
| regex_compile           | 144 ms                                                       | 145 ms: 1.01x slower                                                        |
| regex_dna               | 239 ms                                                       | 240 ms: 1.01x slower                                                        |
| raytrace                | 298 ms                                                       | 301 ms: 1.01x slower                                                        |
| richards                | 45.7 ms                                                      | 46.1 ms: 1.01x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                       |
| sympy_integrate         | 23.9 ms                                                      | 24.3 ms: 1.02x slower                                                       |
| go                      | 150 ms                                                       | 152 ms: 1.02x slower                                                        |
| scimark_monte_carlo     | 69.0 ms                                                      | 70.2 ms: 1.02x slower                                                       |
| dulwich_log             | 65.4 ms                                                      | 66.6 ms: 1.02x slower                                                       |
| crypto_pyaes            | 80.3 ms                                                      | 81.8 ms: 1.02x slower                                                       |
| gc_traversal            | 3.48 ms                                                      | 3.55 ms: 1.02x slower                                                       |
| logging_silent          | 94.4 ns                                                      | 96.5 ns: 1.02x slower                                                       |
| mako                    | 10.0 ms                                                      | 10.3 ms: 1.03x slower                                                       |
| asyncio_tcp             | 378 ms                                                       | 388 ms: 1.03x slower                                                        |
| create_gc_cycles        | 1.59 ms                                                      | 1.64 ms: 1.03x slower                                                       |
| chameleon               | 7.23 ms                                                      | 7.46 ms: 1.03x slower                                                       |
| pycparser               | 1.23 sec                                                     | 1.28 sec: 1.03x slower                                                      |
| sympy_str               | 302 ms                                                       | 313 ms: 1.04x slower                                                        |
| mdp                     | 2.57 sec                                                     | 2.66 sec: 1.04x slower                                                      |
| deepcopy                | 368 us                                                       | 383 us: 1.04x slower                                                        |
| sqlglot_normalize       | 116 ms                                                       | 120 ms: 1.04x slower                                                        |
| spectral_norm           | 91.6 ms                                                      | 95.4 ms: 1.04x slower                                                       |
| nqueens                 | 89.9 ms                                                      | 94.2 ms: 1.05x slower                                                       |
| scimark_lu              | 98.8 ms                                                      | 104 ms: 1.05x slower                                                        |
| async_tree_cpu_io_mixed | 696 ms                                                       | 737 ms: 1.06x slower                                                        |
| django_template         | 38.2 ms                                                      | 40.5 ms: 1.06x slower                                                       |
| sympy_sum               | 162 ms                                                       | 172 ms: 1.06x slower                                                        |
| sqlglot_transpile       | 1.78 ms                                                      | 1.93 ms: 1.09x slower                                                       |
| sympy_expand            | 484 ms                                                       | 526 ms: 1.09x slower                                                        |
| chaos                   | 64.0 ms                                                      | 69.6 ms: 1.09x slower                                                       |
| hexiom                  | 5.96 ms                                                      | 6.49 ms: 1.09x slower                                                       |
| async_tree_memoization  | 544 ms                                                       | 601 ms: 1.10x slower                                                        |
| deltablue               | 3.24 ms                                                      | 3.60 ms: 1.11x slower                                                       |
| async_tree_none         | 452 ms                                                       | 503 ms: 1.11x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                                      |
| sqlglot_parse           | 1.38 ms                                                      | 1.56 ms: 1.13x slower                                                       |
| nbody                   | 88.0 ms                                                      | 101 ms: 1.15x slower                                                        |
| fannkuch                | 350 ms                                                       | 409 ms: 1.17x slower                                                        |
| coroutines              | 23.0 ms                                                      | 29.1 ms: 1.26x slower                                                       |
| coverage                | 66.7 ms                                                      | 86.0 ms: 1.29x slower                                                       |
| dask                    | 392 ms                                                       | 562 ms: 1.43x slower                                                        |
| generators              | 37.4 ms                                                      | 60.4 ms: 1.61x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.01x slower                                                                |

Benchmark hidden because not significant (6): bench_mp_pool, xml_etree_parse, logging_simple, xml_etree_iterparse, meteor_contest, bench_thread_pool
Ignored benchmarks (14) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20230207-3.12.0a5-3c67ec3/bm-20230207-pythonperf2-x86_64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 97.24% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.88x