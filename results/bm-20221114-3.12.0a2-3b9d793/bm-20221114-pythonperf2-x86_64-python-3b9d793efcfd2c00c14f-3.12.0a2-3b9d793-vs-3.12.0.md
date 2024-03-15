
# Results vs. 3.12.0

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: linux-x86_64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.02x slower \*
- HPT reliability: 95.28%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 282 ms: 1.01x faster                                                        |
| chameleon      | 7.23 ms                                                      | 7.19 ms: 1.01x faster                                                       |
| docutils       | 2.87 sec                                                     | 2.77 sec: 1.04x faster                                                      |
| tornado_http   | 121 ms                                                       | 115 ms: 1.05x faster                                                        |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 762 ms: 1.10x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                                      |
| async_tree_memoization  | 544 ms                                                       | 621 ms: 1.14x slower                                                        |
| async_tree_none         | 452 ms                                                       | 520 ms: 1.15x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.13x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 252 ms: 1.05x faster                                                        |
| float          | 76.6 ms                                                      | 73.2 ms: 1.05x faster                                                       |
| nbody          | 88.0 ms                                                      | 90.9 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 227 ms: 1.05x faster                                                        |
| regex_effbot   | 3.57 ms                                                      | 3.45 ms: 1.04x faster                                                       |
| regex_v8       | 23.6 ms                                                      | 23.2 ms: 1.02x faster                                                       |
| regex_compile  | 144 ms                                                       | 147 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|---------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_list         | 4.43 us                                                      | 3.65 us: 1.21x faster                                                       |
| unpickle            | 14.8 us                                                      | 12.6 us: 1.17x faster                                                       |
| xml_etree_generate  | 86.1 ms                                                      | 79.3 ms: 1.09x faster                                                       |
| xml_etree_process   | 58.4 ms                                                      | 54.8 ms: 1.07x faster                                                       |
| pickle              | 10.5 us                                                      | 10.1 us: 1.05x faster                                                       |
| unpickle_list       | 4.66 us                                                      | 4.51 us: 1.03x faster                                                       |
| json_loads          | 24.4 us                                                      | 23.7 us: 1.03x faster                                                       |
| pickle_pure_python  | 318 us                                                       | 314 us: 1.01x faster                                                        |
| pickle_dict         | 32.5 us                                                      | 33.4 us: 1.03x slower                                                       |
| xml_etree_iterparse | 103 ms                                                       | 108 ms: 1.05x slower                                                        |
| Geometric mean      | (ref)                                                        | 1.04x faster                                                                |

Benchmark hidden because not significant (3): xml_etree_parse, json_dumps, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.87 ms: 1.10x faster                                                       |
| python_startup         | 11.6 ms                                                      | 10.8 ms: 1.08x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.09x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 10.0 ms                                                      | 10.2 ms: 1.02x slower                                                       |
| django_template | 38.2 ms                                                      | 39.7 ms: 1.04x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.03x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_generators        | 390 ms                                                       | 321 ms: 1.22x faster                                                        |
| pickle_list             | 4.43 us                                                      | 3.65 us: 1.21x faster                                                       |
| unpickle                | 14.8 us                                                      | 12.6 us: 1.17x faster                                                       |
| unpack_sequence         | 53.2 ns                                                      | 45.8 ns: 1.16x faster                                                       |
| gunicorn                | 1.00 ms                                                      | 886 us: 1.13x faster                                                        |
| aiohttp                 | 1.02 ms                                                      | 904 us: 1.13x faster                                                        |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 3.74 ms: 1.13x faster                                                       |
| scimark_fft             | 301 ms                                                       | 273 ms: 1.10x faster                                                        |
| python_startup_no_site  | 8.64 ms                                                      | 7.87 ms: 1.10x faster                                                       |
| xml_etree_generate      | 86.1 ms                                                      | 79.3 ms: 1.09x faster                                                       |
| sqlite_synth            | 2.77 us                                                      | 2.57 us: 1.08x faster                                                       |
| python_startup          | 11.6 ms                                                      | 10.8 ms: 1.08x faster                                                       |
| pprint_safe_repr        | 807 ms                                                       | 752 ms: 1.07x faster                                                        |
| pprint_pformat          | 1.65 sec                                                     | 1.55 sec: 1.07x faster                                                      |
| xml_etree_process       | 58.4 ms                                                      | 54.8 ms: 1.07x faster                                                       |
| telco                   | 6.96 ms                                                      | 6.58 ms: 1.06x faster                                                       |
| regex_dna               | 239 ms                                                       | 227 ms: 1.05x faster                                                        |
| pidigits                | 265 ms                                                       | 252 ms: 1.05x faster                                                        |
| tornado_http            | 121 ms                                                       | 115 ms: 1.05x faster                                                        |
| float                   | 76.6 ms                                                      | 73.2 ms: 1.05x faster                                                       |
| pickle                  | 10.5 us                                                      | 10.1 us: 1.05x faster                                                       |
| scimark_monte_carlo     | 69.0 ms                                                      | 66.4 ms: 1.04x faster                                                       |
| docutils                | 2.87 sec                                                     | 2.77 sec: 1.04x faster                                                      |
| regex_effbot            | 3.57 ms                                                      | 3.45 ms: 1.04x faster                                                       |
| json                    | 5.12 ms                                                      | 4.95 ms: 1.03x faster                                                       |
| unpickle_list           | 4.66 us                                                      | 4.51 us: 1.03x faster                                                       |
| json_loads              | 24.4 us                                                      | 23.7 us: 1.03x faster                                                       |
| scimark_sor             | 109 ms                                                       | 106 ms: 1.02x faster                                                        |
| regex_v8                | 23.6 ms                                                      | 23.2 ms: 1.02x faster                                                       |
| pickle_pure_python      | 318 us                                                       | 314 us: 1.01x faster                                                        |
| 2to3                    | 285 ms                                                       | 282 ms: 1.01x faster                                                        |
| pyflate                 | 439 ms                                                       | 436 ms: 1.01x faster                                                        |
| chameleon               | 7.23 ms                                                      | 7.19 ms: 1.01x faster                                                       |
| meteor_contest          | 128 ms                                                       | 129 ms: 1.00x slower                                                        |
| crypto_pyaes            | 80.3 ms                                                      | 80.7 ms: 1.00x slower                                                       |
| logging_simple          | 6.71 us                                                      | 6.78 us: 1.01x slower                                                       |
| sqlglot_optimize        | 57.5 ms                                                      | 58.2 ms: 1.01x slower                                                       |
| logging_format          | 7.48 us                                                      | 7.60 us: 1.02x slower                                                       |
| spectral_norm           | 91.6 ms                                                      | 93.2 ms: 1.02x slower                                                       |
| regex_compile           | 144 ms                                                       | 147 ms: 1.02x slower                                                        |
| mako                    | 10.0 ms                                                      | 10.2 ms: 1.02x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                       |
| raytrace                | 298 ms                                                       | 305 ms: 1.02x slower                                                        |
| pickle_dict             | 32.5 us                                                      | 33.4 us: 1.03x slower                                                       |
| dulwich_log             | 65.4 ms                                                      | 67.2 ms: 1.03x slower                                                       |
| nbody                   | 88.0 ms                                                      | 90.9 ms: 1.03x slower                                                       |
| django_template         | 38.2 ms                                                      | 39.7 ms: 1.04x slower                                                       |
| dask                    | 392 ms                                                       | 410 ms: 1.05x slower                                                        |
| xml_etree_iterparse     | 103 ms                                                       | 108 ms: 1.05x slower                                                        |
| deepcopy                | 368 us                                                       | 387 us: 1.05x slower                                                        |
| logging_silent          | 94.4 ns                                                      | 99.2 ns: 1.05x slower                                                       |
| sqlglot_transpile       | 1.78 ms                                                      | 1.87 ms: 1.05x slower                                                       |
| sqlglot_normalize       | 116 ms                                                       | 122 ms: 1.06x slower                                                        |
| mdp                     | 2.57 sec                                                     | 2.73 sec: 1.06x slower                                                      |
| sympy_integrate         | 23.9 ms                                                      | 25.5 ms: 1.07x slower                                                       |
| go                      | 150 ms                                                       | 160 ms: 1.07x slower                                                        |
| sqlglot_parse           | 1.38 ms                                                      | 1.50 ms: 1.09x slower                                                       |
| async_tree_cpu_io_mixed | 696 ms                                                       | 762 ms: 1.10x slower                                                        |
| sympy_str               | 302 ms                                                       | 337 ms: 1.12x slower                                                        |
| fannkuch                | 350 ms                                                       | 391 ms: 1.12x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                                      |
| scimark_lu              | 98.8 ms                                                      | 111 ms: 1.13x slower                                                        |
| deltablue               | 3.24 ms                                                      | 3.64 ms: 1.13x slower                                                       |
| gc_traversal            | 3.48 ms                                                      | 3.92 ms: 1.13x slower                                                       |
| hexiom                  | 5.96 ms                                                      | 6.76 ms: 1.14x slower                                                       |
| sympy_expand            | 484 ms                                                       | 550 ms: 1.14x slower                                                        |
| sympy_sum               | 162 ms                                                       | 184 ms: 1.14x slower                                                        |
| chaos                   | 64.0 ms                                                      | 72.9 ms: 1.14x slower                                                       |
| async_tree_memoization  | 544 ms                                                       | 621 ms: 1.14x slower                                                        |
| nqueens                 | 89.9 ms                                                      | 103 ms: 1.14x slower                                                        |
| async_tree_none         | 452 ms                                                       | 520 ms: 1.15x slower                                                        |
| coroutines              | 23.0 ms                                                      | 27.9 ms: 1.21x slower                                                       |
| comprehensions          | 21.9 us                                                      | 26.9 us: 1.23x slower                                                       |
| coverage                | 66.7 ms                                                      | 86.9 ms: 1.30x slower                                                       |
| generators              | 37.4 ms                                                      | 61.2 ms: 1.63x slower                                                       |
| asyncio_tcp             | 378 ms                                                       | 749 ms: 1.98x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.02x slower                                                                |

Benchmark hidden because not significant (10): bench_mp_pool, richards, xml_etree_parse, deepcopy_memo, json_dumps, unpickle_pure_python, deepcopy_reduce, create_gc_cycles, pycparser, bench_thread_pool
Ignored benchmarks (12) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20221114-3.12.0a2-3b9d793/bm-20221114-pythonperf2-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 95.28% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.90x