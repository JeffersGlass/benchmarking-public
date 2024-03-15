
# Results vs. 3.12.0

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: linux-x86_64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.02x slower \*
- HPT reliability: 94.17%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 278 ms: 1.03x faster                                                        |
| chameleon      | 7.23 ms                                                      | 7.62 ms: 1.05x slower                                                       |
| docutils       | 2.87 sec                                                     | 2.79 sec: 1.03x faster                                                      |
| tornado_http   | 121 ms                                                       | 114 ms: 1.06x faster                                                        |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 756 ms: 1.09x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.16 sec: 1.11x slower                                                      |
| async_tree_memoization  | 544 ms                                                       | 618 ms: 1.14x slower                                                        |
| async_tree_none         | 452 ms                                                       | 516 ms: 1.14x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.12x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 251 ms: 1.05x faster                                                        |
| float          | 76.6 ms                                                      | 73.2 ms: 1.05x faster                                                       |
| nbody          | 88.0 ms                                                      | 98.1 ms: 1.11x slower                                                       |
| Geometric mean | (ref)                                                        | 1.00x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.34 ms: 1.07x faster                                                       |
| regex_v8       | 23.6 ms                                                      | 22.9 ms: 1.03x faster                                                       |
| regex_dna      | 239 ms                                                       | 232 ms: 1.03x faster                                                        |
| regex_compile  | 144 ms                                                       | 146 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                        | 1.03x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.84 us: 1.15x faster                                                       |
| unpickle             | 14.8 us                                                      | 13.3 us: 1.11x faster                                                       |
| xml_etree_generate   | 86.1 ms                                                      | 77.6 ms: 1.11x faster                                                       |
| xml_etree_process    | 58.4 ms                                                      | 54.1 ms: 1.08x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.47 us: 1.04x faster                                                       |
| pickle               | 10.5 us                                                      | 10.1 us: 1.04x faster                                                       |
| xml_etree_parse      | 144 ms                                                       | 138 ms: 1.04x faster                                                        |
| pickle_dict          | 32.5 us                                                      | 31.9 us: 1.02x faster                                                       |
| pickle_pure_python   | 318 us                                                       | 313 us: 1.02x faster                                                        |
| unpickle_pure_python | 210 us                                                       | 208 us: 1.01x faster                                                        |
| json_loads           | 24.4 us                                                      | 24.3 us: 1.00x faster                                                       |
| json_dumps           | 10.2 ms                                                      | 10.4 ms: 1.01x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.05x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.62 ms: 1.13x faster                                                       |
| python_startup         | 11.6 ms                                                      | 10.6 ms: 1.10x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.12x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 10.0 ms                                                      | 10.4 ms: 1.04x slower                                                       |
| django_template | 38.2 ms                                                      | 40.6 ms: 1.06x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.05x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_generators        | 390 ms                                                       | 321 ms: 1.22x faster                                                        |
| unpack_sequence         | 53.2 ns                                                      | 45.0 ns: 1.18x faster                                                       |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 3.58 ms: 1.17x faster                                                       |
| pickle_list             | 4.43 us                                                      | 3.84 us: 1.15x faster                                                       |
| aiohttp                 | 1.02 ms                                                      | 894 us: 1.14x faster                                                        |
| python_startup_no_site  | 8.64 ms                                                      | 7.62 ms: 1.13x faster                                                       |
| gunicorn                | 1.00 ms                                                      | 888 us: 1.13x faster                                                        |
| unpickle                | 14.8 us                                                      | 13.3 us: 1.11x faster                                                       |
| xml_etree_generate      | 86.1 ms                                                      | 77.6 ms: 1.11x faster                                                       |
| python_startup          | 11.6 ms                                                      | 10.6 ms: 1.10x faster                                                       |
| sqlite_synth            | 2.77 us                                                      | 2.54 us: 1.09x faster                                                       |
| xml_etree_process       | 58.4 ms                                                      | 54.1 ms: 1.08x faster                                                       |
| regex_effbot            | 3.57 ms                                                      | 3.34 ms: 1.07x faster                                                       |
| pprint_safe_repr        | 807 ms                                                       | 761 ms: 1.06x faster                                                        |
| tornado_http            | 121 ms                                                       | 114 ms: 1.06x faster                                                        |
| pprint_pformat          | 1.65 sec                                                     | 1.57 sec: 1.06x faster                                                      |
| pidigits                | 265 ms                                                       | 251 ms: 1.05x faster                                                        |
| telco                   | 6.96 ms                                                      | 6.64 ms: 1.05x faster                                                       |
| float                   | 76.6 ms                                                      | 73.2 ms: 1.05x faster                                                       |
| scimark_fft             | 301 ms                                                       | 288 ms: 1.05x faster                                                        |
| bench_mp_pool           | 4.76 ms                                                      | 4.56 ms: 1.05x faster                                                       |
| unpickle_list           | 4.66 us                                                      | 4.47 us: 1.04x faster                                                       |
| pickle                  | 10.5 us                                                      | 10.1 us: 1.04x faster                                                       |
| xml_etree_parse         | 144 ms                                                       | 138 ms: 1.04x faster                                                        |
| regex_v8                | 23.6 ms                                                      | 22.9 ms: 1.03x faster                                                       |
| regex_dna               | 239 ms                                                       | 232 ms: 1.03x faster                                                        |
| 2to3                    | 285 ms                                                       | 278 ms: 1.03x faster                                                        |
| docutils                | 2.87 sec                                                     | 2.79 sec: 1.03x faster                                                      |
| pickle_dict             | 32.5 us                                                      | 31.9 us: 1.02x faster                                                       |
| meteor_contest          | 128 ms                                                       | 126 ms: 1.02x faster                                                        |
| pyflate                 | 439 ms                                                       | 431 ms: 1.02x faster                                                        |
| scimark_monte_carlo     | 69.0 ms                                                      | 67.8 ms: 1.02x faster                                                       |
| pickle_pure_python      | 318 us                                                       | 313 us: 1.02x faster                                                        |
| json                    | 5.12 ms                                                      | 5.05 ms: 1.01x faster                                                       |
| deepcopy_memo           | 36.8 us                                                      | 36.4 us: 1.01x faster                                                       |
| unpickle_pure_python    | 210 us                                                       | 208 us: 1.01x faster                                                        |
| deepcopy_reduce         | 3.37 us                                                      | 3.35 us: 1.01x faster                                                       |
| scimark_sor             | 109 ms                                                       | 108 ms: 1.01x faster                                                        |
| json_loads              | 24.4 us                                                      | 24.3 us: 1.00x faster                                                       |
| pathlib                 | 18.9 ms                                                      | 19.0 ms: 1.00x slower                                                       |
| dulwich_log             | 65.4 ms                                                      | 65.9 ms: 1.01x slower                                                       |
| regex_compile           | 144 ms                                                       | 146 ms: 1.01x slower                                                        |
| sqlglot_optimize        | 57.5 ms                                                      | 58.2 ms: 1.01x slower                                                       |
| logging_silent          | 94.4 ns                                                      | 95.5 ns: 1.01x slower                                                       |
| pycparser               | 1.23 sec                                                     | 1.25 sec: 1.01x slower                                                      |
| json_dumps              | 10.2 ms                                                      | 10.4 ms: 1.01x slower                                                       |
| gc_traversal            | 3.48 ms                                                      | 3.54 ms: 1.02x slower                                                       |
| go                      | 150 ms                                                       | 155 ms: 1.03x slower                                                        |
| crypto_pyaes            | 80.3 ms                                                      | 83.2 ms: 1.04x slower                                                       |
| sqlglot_normalize       | 116 ms                                                       | 120 ms: 1.04x slower                                                        |
| logging_format          | 7.48 us                                                      | 7.77 us: 1.04x slower                                                       |
| richards                | 45.7 ms                                                      | 47.6 ms: 1.04x slower                                                       |
| mako                    | 10.0 ms                                                      | 10.4 ms: 1.04x slower                                                       |
| dask                    | 392 ms                                                       | 409 ms: 1.04x slower                                                        |
| spectral_norm           | 91.6 ms                                                      | 96.1 ms: 1.05x slower                                                       |
| logging_simple          | 6.71 us                                                      | 7.06 us: 1.05x slower                                                       |
| mdp                     | 2.57 sec                                                     | 2.71 sec: 1.05x slower                                                      |
| chameleon               | 7.23 ms                                                      | 7.62 ms: 1.05x slower                                                       |
| sympy_integrate         | 23.9 ms                                                      | 25.4 ms: 1.06x slower                                                       |
| django_template         | 38.2 ms                                                      | 40.6 ms: 1.06x slower                                                       |
| sqlglot_transpile       | 1.78 ms                                                      | 1.90 ms: 1.07x slower                                                       |
| deepcopy                | 368 us                                                       | 394 us: 1.07x slower                                                        |
| sympy_str               | 302 ms                                                       | 326 ms: 1.08x slower                                                        |
| nqueens                 | 89.9 ms                                                      | 97.1 ms: 1.08x slower                                                       |
| async_tree_cpu_io_mixed | 696 ms                                                       | 756 ms: 1.09x slower                                                        |
| sympy_expand            | 484 ms                                                       | 527 ms: 1.09x slower                                                        |
| sqlglot_parse           | 1.38 ms                                                      | 1.51 ms: 1.10x slower                                                       |
| comprehensions          | 21.9 us                                                      | 24.2 us: 1.11x slower                                                       |
| hexiom                  | 5.96 ms                                                      | 6.61 ms: 1.11x slower                                                       |
| async_tree_io           | 1.04 sec                                                     | 1.16 sec: 1.11x slower                                                      |
| nbody                   | 88.0 ms                                                      | 98.1 ms: 1.11x slower                                                       |
| sympy_sum               | 162 ms                                                       | 181 ms: 1.12x slower                                                        |
| scimark_lu              | 98.8 ms                                                      | 111 ms: 1.12x slower                                                        |
| deltablue               | 3.24 ms                                                      | 3.65 ms: 1.13x slower                                                       |
| async_tree_memoization  | 544 ms                                                       | 618 ms: 1.14x slower                                                        |
| async_tree_none         | 452 ms                                                       | 516 ms: 1.14x slower                                                        |
| chaos                   | 64.0 ms                                                      | 73.4 ms: 1.15x slower                                                       |
| fannkuch                | 350 ms                                                       | 405 ms: 1.16x slower                                                        |
| coroutines              | 23.0 ms                                                      | 27.4 ms: 1.19x slower                                                       |
| coverage                | 66.7 ms                                                      | 81.5 ms: 1.22x slower                                                       |
| generators              | 37.4 ms                                                      | 54.6 ms: 1.46x slower                                                       |
| asyncio_tcp             | 378 ms                                                       | 747 ms: 1.98x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.02x slower                                                                |

Benchmark hidden because not significant (4): xml_etree_iterparse, raytrace, create_gc_cycles, bench_thread_pool
Ignored benchmarks (12) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (5) of results/bm-20221025-3.12.0a1-4ae1a0e/bm-20221025-pythonperf2-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 94.17% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.90x