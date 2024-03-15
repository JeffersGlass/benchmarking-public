
# Results vs. 3.12.0

- fork: python
- ref: 3d5d3f7af6498effbc60
- machine: linux-x86_64
- commit hash: 3d5d3f7
- commit date: 2023-01-10
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.56%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.89x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 286 ms: 1.00x slower                                                        |
| chameleon      | 7.23 ms                                                      | 7.31 ms: 1.01x slower                                                       |
| docutils       | 2.87 sec                                                     | 2.78 sec: 1.03x faster                                                      |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 742 ms: 1.07x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.15 sec: 1.11x slower                                                      |
| async_tree_memoization  | 544 ms                                                       | 608 ms: 1.12x slower                                                        |
| async_tree_none         | 452 ms                                                       | 505 ms: 1.12x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.10x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 72.4 ms: 1.06x faster                                                       |
| pidigits       | 265 ms                                                       | 252 ms: 1.05x faster                                                        |
| nbody          | 88.0 ms                                                      | 98.1 ms: 1.12x slower                                                       |
| Geometric mean | (ref)                                                        | 1.00x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 229 ms: 1.04x faster                                                        |
| regex_effbot   | 3.57 ms                                                      | 3.43 ms: 1.04x faster                                                       |
| regex_v8       | 23.6 ms                                                      | 23.0 ms: 1.03x faster                                                       |
| regex_compile  | 144 ms                                                       | 149 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.70 us: 1.20x faster                                                       |
| unpickle             | 14.8 us                                                      | 13.3 us: 1.11x faster                                                       |
| pickle               | 10.5 us                                                      | 9.71 us: 1.08x faster                                                       |
| xml_etree_generate   | 86.1 ms                                                      | 80.3 ms: 1.07x faster                                                       |
| xml_etree_process    | 58.4 ms                                                      | 55.4 ms: 1.05x faster                                                       |
| pickle_dict          | 32.5 us                                                      | 31.1 us: 1.05x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.48 us: 1.04x faster                                                       |
| pickle_pure_python   | 318 us                                                       | 313 us: 1.02x faster                                                        |
| json_loads           | 24.4 us                                                      | 24.0 us: 1.01x faster                                                       |
| json_dumps           | 10.2 ms                                                      | 10.1 ms: 1.01x faster                                                       |
| xml_etree_iterparse  | 103 ms                                                       | 104 ms: 1.02x slower                                                        |
| unpickle_pure_python | 210 us                                                       | 214 us: 1.02x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.05x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.87 ms: 1.10x faster                                                       |
| python_startup         | 11.6 ms                                                      | 10.8 ms: 1.08x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.09x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 10.0 ms                                                      | 10.2 ms: 1.02x slower                                                       |
| django_template | 38.2 ms                                                      | 39.2 ms: 1.03x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.03x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_generators        | 390 ms                                                       | 322 ms: 1.21x faster                                                        |
| unpack_sequence         | 53.2 ns                                                      | 44.0 ns: 1.21x faster                                                       |
| pickle_list             | 4.43 us                                                      | 3.70 us: 1.20x faster                                                       |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 3.70 ms: 1.14x faster                                                       |
| unpickle                | 14.8 us                                                      | 13.3 us: 1.11x faster                                                       |
| python_startup_no_site  | 8.64 ms                                                      | 7.87 ms: 1.10x faster                                                       |
| pickle                  | 10.5 us                                                      | 9.71 us: 1.08x faster                                                       |
| sqlite_synth            | 2.77 us                                                      | 2.56 us: 1.08x faster                                                       |
| python_startup          | 11.6 ms                                                      | 10.8 ms: 1.08x faster                                                       |
| xml_etree_generate      | 86.1 ms                                                      | 80.3 ms: 1.07x faster                                                       |
| scimark_fft             | 301 ms                                                       | 283 ms: 1.07x faster                                                        |
| float                   | 76.6 ms                                                      | 72.4 ms: 1.06x faster                                                       |
| xml_etree_process       | 58.4 ms                                                      | 55.4 ms: 1.05x faster                                                       |
| pidigits                | 265 ms                                                       | 252 ms: 1.05x faster                                                        |
| pickle_dict             | 32.5 us                                                      | 31.1 us: 1.05x faster                                                       |
| regex_dna               | 239 ms                                                       | 229 ms: 1.04x faster                                                        |
| regex_effbot            | 3.57 ms                                                      | 3.43 ms: 1.04x faster                                                       |
| telco                   | 6.96 ms                                                      | 6.70 ms: 1.04x faster                                                       |
| unpickle_list           | 4.66 us                                                      | 4.48 us: 1.04x faster                                                       |
| scimark_monte_carlo     | 69.0 ms                                                      | 66.6 ms: 1.04x faster                                                       |
| docutils                | 2.87 sec                                                     | 2.78 sec: 1.03x faster                                                      |
| regex_v8                | 23.6 ms                                                      | 23.0 ms: 1.03x faster                                                       |
| pprint_pformat          | 1.65 sec                                                     | 1.63 sec: 1.02x faster                                                      |
| pickle_pure_python      | 318 us                                                       | 313 us: 1.02x faster                                                        |
| pprint_safe_repr        | 807 ms                                                       | 794 ms: 1.02x faster                                                        |
| json_loads              | 24.4 us                                                      | 24.0 us: 1.01x faster                                                       |
| pyflate                 | 439 ms                                                       | 433 ms: 1.01x faster                                                        |
| json_dumps              | 10.2 ms                                                      | 10.1 ms: 1.01x faster                                                       |
| deepcopy_reduce         | 3.37 us                                                      | 3.33 us: 1.01x faster                                                       |
| scimark_sor             | 109 ms                                                       | 108 ms: 1.01x faster                                                        |
| 2to3                    | 285 ms                                                       | 286 ms: 1.00x slower                                                        |
| crypto_pyaes            | 80.3 ms                                                      | 81.1 ms: 1.01x slower                                                       |
| chameleon               | 7.23 ms                                                      | 7.31 ms: 1.01x slower                                                       |
| xml_etree_iterparse     | 103 ms                                                       | 104 ms: 1.02x slower                                                        |
| gc_traversal            | 3.48 ms                                                      | 3.54 ms: 1.02x slower                                                       |
| asyncio_tcp             | 378 ms                                                       | 386 ms: 1.02x slower                                                        |
| pycparser               | 1.23 sec                                                     | 1.26 sec: 1.02x slower                                                      |
| scimark_lu              | 98.8 ms                                                      | 101 ms: 1.02x slower                                                        |
| unpickle_pure_python    | 210 us                                                       | 214 us: 1.02x slower                                                        |
| mako                    | 10.0 ms                                                      | 10.2 ms: 1.02x slower                                                       |
| json                    | 5.12 ms                                                      | 5.24 ms: 1.02x slower                                                       |
| meteor_contest          | 128 ms                                                       | 131 ms: 1.02x slower                                                        |
| logging_format          | 7.48 us                                                      | 7.66 us: 1.02x slower                                                       |
| go                      | 150 ms                                                       | 153 ms: 1.02x slower                                                        |
| richards                | 45.7 ms                                                      | 46.9 ms: 1.02x slower                                                       |
| deepcopy                | 368 us                                                       | 379 us: 1.03x slower                                                        |
| django_template         | 38.2 ms                                                      | 39.2 ms: 1.03x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 19.4 ms: 1.03x slower                                                       |
| sqlglot_optimize        | 57.5 ms                                                      | 59.3 ms: 1.03x slower                                                       |
| dulwich_log             | 65.4 ms                                                      | 67.5 ms: 1.03x slower                                                       |
| regex_compile           | 144 ms                                                       | 149 ms: 1.04x slower                                                        |
| logging_simple          | 6.71 us                                                      | 6.95 us: 1.04x slower                                                       |
| bench_thread_pool       | 950 us                                                       | 987 us: 1.04x slower                                                        |
| dask                    | 392 ms                                                       | 408 ms: 1.04x slower                                                        |
| nqueens                 | 89.9 ms                                                      | 94.0 ms: 1.05x slower                                                       |
| sqlglot_normalize       | 116 ms                                                       | 123 ms: 1.06x slower                                                        |
| async_tree_cpu_io_mixed | 696 ms                                                       | 742 ms: 1.07x slower                                                        |
| sympy_integrate         | 23.9 ms                                                      | 25.6 ms: 1.07x slower                                                       |
| mdp                     | 2.57 sec                                                     | 2.75 sec: 1.07x slower                                                      |
| logging_silent          | 94.4 ns                                                      | 102 ns: 1.08x slower                                                        |
| fannkuch                | 350 ms                                                       | 380 ms: 1.09x slower                                                        |
| sqlglot_transpile       | 1.78 ms                                                      | 1.95 ms: 1.10x slower                                                       |
| spectral_norm           | 91.6 ms                                                      | 101 ms: 1.10x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.15 sec: 1.11x slower                                                      |
| sympy_str               | 302 ms                                                       | 335 ms: 1.11x slower                                                        |
| chaos                   | 64.0 ms                                                      | 70.9 ms: 1.11x slower                                                       |
| sympy_expand            | 484 ms                                                       | 537 ms: 1.11x slower                                                        |
| nbody                   | 88.0 ms                                                      | 98.1 ms: 1.12x slower                                                       |
| async_tree_memoization  | 544 ms                                                       | 608 ms: 1.12x slower                                                        |
| async_tree_none         | 452 ms                                                       | 505 ms: 1.12x slower                                                        |
| hexiom                  | 5.96 ms                                                      | 6.77 ms: 1.14x slower                                                       |
| deltablue               | 3.24 ms                                                      | 3.69 ms: 1.14x slower                                                       |
| sympy_sum               | 162 ms                                                       | 186 ms: 1.15x slower                                                        |
| sqlglot_parse           | 1.38 ms                                                      | 1.59 ms: 1.15x slower                                                       |
| coroutines              | 23.0 ms                                                      | 27.9 ms: 1.21x slower                                                       |
| comprehensions          | 21.9 us                                                      | 27.1 us: 1.23x slower                                                       |
| coverage                | 66.7 ms                                                      | 89.3 ms: 1.34x slower                                                       |
| generators              | 37.4 ms                                                      | 60.5 ms: 1.62x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.02x slower                                                                |

Benchmark hidden because not significant (5): create_gc_cycles, deepcopy_memo, xml_etree_parse, raytrace, bench_mp_pool
Ignored benchmarks (15) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20230110-3.12.0a4-3d5d3f7/bm-20230110-pythonperf2-x86_64-python-3d5d3f7af6498effbc60-3.12.0a4-3d5d3f7.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 99.56% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.89x