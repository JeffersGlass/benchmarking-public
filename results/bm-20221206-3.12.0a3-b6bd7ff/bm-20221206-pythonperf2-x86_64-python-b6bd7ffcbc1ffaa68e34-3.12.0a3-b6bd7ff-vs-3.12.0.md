
# Results vs. 3.12.0

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: linux-x86_64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.04x slower \*
- HPT reliability: 99.88%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.90x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 281 ms: 1.02x faster                                                        |
| chameleon      | 7.23 ms                                                      | 7.51 ms: 1.04x slower                                                       |
| docutils       | 2.87 sec                                                     | 2.76 sec: 1.04x faster                                                      |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 767 ms: 1.10x slower                                                        |
| async_tree_io           | 1.04 sec                                                     | 1.18 sec: 1.13x slower                                                      |
| async_tree_memoization  | 544 ms                                                       | 623 ms: 1.15x slower                                                        |
| async_tree_none         | 452 ms                                                       | 531 ms: 1.18x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.14x slower                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 250 ms: 1.06x faster                                                        |
| float          | 76.6 ms                                                      | 73.2 ms: 1.05x faster                                                       |
| nbody          | 88.0 ms                                                      | 94.3 ms: 1.07x slower                                                       |
| Geometric mean | (ref)                                                        | 1.01x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_v8       | 23.6 ms                                                      | 22.3 ms: 1.06x faster                                                       |
| regex_effbot   | 3.57 ms                                                      | 3.44 ms: 1.04x faster                                                       |
| regex_dna      | 239 ms                                                       | 233 ms: 1.02x faster                                                        |
| regex_compile  | 144 ms                                                       | 150 ms: 1.04x slower                                                        |
| Geometric mean | (ref)                                                        | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.90 us: 1.14x faster                                                       |
| unpickle             | 14.8 us                                                      | 13.1 us: 1.13x faster                                                       |
| xml_etree_generate   | 86.1 ms                                                      | 78.9 ms: 1.09x faster                                                       |
| pickle               | 10.5 us                                                      | 9.84 us: 1.07x faster                                                       |
| xml_etree_process    | 58.4 ms                                                      | 55.6 ms: 1.05x faster                                                       |
| unpickle_list        | 4.66 us                                                      | 4.47 us: 1.04x faster                                                       |
| pickle_dict          | 32.5 us                                                      | 31.9 us: 1.02x faster                                                       |
| xml_etree_parse      | 144 ms                                                       | 141 ms: 1.02x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 316 us: 1.01x faster                                                        |
| json_loads           | 24.4 us                                                      | 24.2 us: 1.01x faster                                                       |
| json_dumps           | 10.2 ms                                                      | 10.3 ms: 1.01x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 212 us: 1.01x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 108 ms: 1.05x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.04x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.86 ms: 1.10x faster                                                       |
| python_startup         | 11.6 ms                                                      | 10.8 ms: 1.08x faster                                                       |
| Geometric mean         | (ref)                                                        | 1.09x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 10.0 ms                                                      | 10.4 ms: 1.03x slower                                                       |
| django_template | 38.2 ms                                                      | 39.6 ms: 1.04x slower                                                       |
| Geometric mean  | (ref)                                                        | 1.04x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpack_sequence         | 53.2 ns                                                      | 45.5 ns: 1.17x faster                                                       |
| async_generators        | 390 ms                                                       | 335 ms: 1.16x faster                                                        |
| pickle_list             | 4.43 us                                                      | 3.90 us: 1.14x faster                                                       |
| unpickle                | 14.8 us                                                      | 13.1 us: 1.13x faster                                                       |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 3.73 ms: 1.13x faster                                                       |
| python_startup_no_site  | 8.64 ms                                                      | 7.86 ms: 1.10x faster                                                       |
| xml_etree_generate      | 86.1 ms                                                      | 78.9 ms: 1.09x faster                                                       |
| python_startup          | 11.6 ms                                                      | 10.8 ms: 1.08x faster                                                       |
| pickle                  | 10.5 us                                                      | 9.84 us: 1.07x faster                                                       |
| scimark_fft             | 301 ms                                                       | 282 ms: 1.07x faster                                                        |
| bench_mp_pool           | 4.76 ms                                                      | 4.46 ms: 1.07x faster                                                       |
| sqlite_synth            | 2.77 us                                                      | 2.60 us: 1.07x faster                                                       |
| pprint_safe_repr        | 807 ms                                                       | 758 ms: 1.06x faster                                                        |
| pprint_pformat          | 1.65 sec                                                     | 1.56 sec: 1.06x faster                                                      |
| pidigits                | 265 ms                                                       | 250 ms: 1.06x faster                                                        |
| regex_v8                | 23.6 ms                                                      | 22.3 ms: 1.06x faster                                                       |
| telco                   | 6.96 ms                                                      | 6.60 ms: 1.05x faster                                                       |
| xml_etree_process       | 58.4 ms                                                      | 55.6 ms: 1.05x faster                                                       |
| float                   | 76.6 ms                                                      | 73.2 ms: 1.05x faster                                                       |
| unpickle_list           | 4.66 us                                                      | 4.47 us: 1.04x faster                                                       |
| docutils                | 2.87 sec                                                     | 2.76 sec: 1.04x faster                                                      |
| regex_effbot            | 3.57 ms                                                      | 3.44 ms: 1.04x faster                                                       |
| regex_dna               | 239 ms                                                       | 233 ms: 1.02x faster                                                        |
| pickle_dict             | 32.5 us                                                      | 31.9 us: 1.02x faster                                                       |
| xml_etree_parse         | 144 ms                                                       | 141 ms: 1.02x faster                                                        |
| 2to3                    | 285 ms                                                       | 281 ms: 1.02x faster                                                        |
| deepcopy_memo           | 36.8 us                                                      | 36.2 us: 1.01x faster                                                       |
| pickle_pure_python      | 318 us                                                       | 316 us: 1.01x faster                                                        |
| json_loads              | 24.4 us                                                      | 24.2 us: 1.01x faster                                                       |
| pyflate                 | 439 ms                                                       | 440 ms: 1.00x slower                                                        |
| meteor_contest          | 128 ms                                                       | 129 ms: 1.01x slower                                                        |
| pathlib                 | 18.9 ms                                                      | 19.0 ms: 1.01x slower                                                       |
| richards                | 45.7 ms                                                      | 46.1 ms: 1.01x slower                                                       |
| json_dumps              | 10.2 ms                                                      | 10.3 ms: 1.01x slower                                                       |
| unpickle_pure_python    | 210 us                                                       | 212 us: 1.01x slower                                                        |
| scimark_lu              | 98.8 ms                                                      | 100 ms: 1.01x slower                                                        |
| pycparser               | 1.23 sec                                                     | 1.26 sec: 1.02x slower                                                      |
| sqlglot_optimize        | 57.5 ms                                                      | 58.5 ms: 1.02x slower                                                       |
| crypto_pyaes            | 80.3 ms                                                      | 81.8 ms: 1.02x slower                                                       |
| dulwich_log             | 65.4 ms                                                      | 66.7 ms: 1.02x slower                                                       |
| deepcopy                | 368 us                                                       | 380 us: 1.03x slower                                                        |
| logging_format          | 7.48 us                                                      | 7.72 us: 1.03x slower                                                       |
| mako                    | 10.0 ms                                                      | 10.4 ms: 1.03x slower                                                       |
| django_template         | 38.2 ms                                                      | 39.6 ms: 1.04x slower                                                       |
| chameleon               | 7.23 ms                                                      | 7.51 ms: 1.04x slower                                                       |
| regex_compile           | 144 ms                                                       | 150 ms: 1.04x slower                                                        |
| dask                    | 392 ms                                                       | 409 ms: 1.04x slower                                                        |
| xml_etree_iterparse     | 103 ms                                                       | 108 ms: 1.05x slower                                                        |
| bench_thread_pool       | 950 us                                                       | 994 us: 1.05x slower                                                        |
| sqlglot_normalize       | 116 ms                                                       | 121 ms: 1.05x slower                                                        |
| logging_simple          | 6.71 us                                                      | 7.03 us: 1.05x slower                                                       |
| spectral_norm           | 91.6 ms                                                      | 96.2 ms: 1.05x slower                                                       |
| scimark_monte_carlo     | 69.0 ms                                                      | 72.7 ms: 1.05x slower                                                       |
| sqlglot_transpile       | 1.78 ms                                                      | 1.87 ms: 1.06x slower                                                       |
| logging_silent          | 94.4 ns                                                      | 99.7 ns: 1.06x slower                                                       |
| mdp                     | 2.57 sec                                                     | 2.73 sec: 1.06x slower                                                      |
| go                      | 150 ms                                                       | 159 ms: 1.06x slower                                                        |
| sympy_integrate         | 23.9 ms                                                      | 25.6 ms: 1.07x slower                                                       |
| nbody                   | 88.0 ms                                                      | 94.3 ms: 1.07x slower                                                       |
| gc_traversal            | 3.48 ms                                                      | 3.79 ms: 1.09x slower                                                       |
| sympy_str               | 302 ms                                                       | 331 ms: 1.10x slower                                                        |
| raytrace                | 298 ms                                                       | 327 ms: 1.10x slower                                                        |
| sqlglot_parse           | 1.38 ms                                                      | 1.52 ms: 1.10x slower                                                       |
| async_tree_cpu_io_mixed | 696 ms                                                       | 767 ms: 1.10x slower                                                        |
| sympy_expand            | 484 ms                                                       | 539 ms: 1.11x slower                                                        |
| hexiom                  | 5.96 ms                                                      | 6.73 ms: 1.13x slower                                                       |
| async_tree_io           | 1.04 sec                                                     | 1.18 sec: 1.13x slower                                                      |
| sympy_sum               | 162 ms                                                       | 183 ms: 1.13x slower                                                        |
| deltablue               | 3.24 ms                                                      | 3.67 ms: 1.13x slower                                                       |
| nqueens                 | 89.9 ms                                                      | 102 ms: 1.14x slower                                                        |
| fannkuch                | 350 ms                                                       | 398 ms: 1.14x slower                                                        |
| async_tree_memoization  | 544 ms                                                       | 623 ms: 1.15x slower                                                        |
| async_tree_none         | 452 ms                                                       | 531 ms: 1.18x slower                                                        |
| coroutines              | 23.0 ms                                                      | 28.0 ms: 1.22x slower                                                       |
| chaos                   | 64.0 ms                                                      | 78.3 ms: 1.22x slower                                                       |
| comprehensions          | 21.9 us                                                      | 27.3 us: 1.24x slower                                                       |
| coverage                | 66.7 ms                                                      | 85.0 ms: 1.28x slower                                                       |
| generators              | 37.4 ms                                                      | 60.8 ms: 1.63x slower                                                       |
| asyncio_tcp             | 378 ms                                                       | 743 ms: 1.96x slower                                                        |
| Geometric mean          | (ref)                                                        | 1.04x slower                                                                |

Benchmark hidden because not significant (4): json, deepcopy_reduce, create_gc_cycles, scimark_sor
Ignored benchmarks (15) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, gunicorn, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20221206-3.12.0a3-b6bd7ff/bm-20221206-pythonperf2-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 99.88% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.90x