
# Results vs. 3.12.0

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: linux-x86_64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.28x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x slower
- Memory change: 0.84x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 350 ms: 1.23x slower                                                       |
| chameleon      | 7.23 ms                                                      | 9.41 ms: 1.30x slower                                                      |
| docutils       | 2.87 sec                                                     | 3.42 sec: 1.19x slower                                                     |
| tornado_http   | 121 ms                                                       | 150 ms: 1.24x slower                                                       |
| Geometric mean | (ref)                                                        | 1.24x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 952 ms: 1.37x slower                                                       |
| async_tree_memoization  | 544 ms                                                       | 827 ms: 1.52x slower                                                       |
| async_tree_none         | 452 ms                                                       | 695 ms: 1.54x slower                                                       |
| async_tree_io           | 1.04 sec                                                     | 1.61 sec: 1.54x slower                                                     |
| Geometric mean          | (ref)                                                        | 1.49x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 271 ms: 1.02x slower                                                       |
| float          | 76.6 ms                                                      | 110 ms: 1.44x slower                                                       |
| nbody          | 88.0 ms                                                      | 137 ms: 1.56x slower                                                       |
| Geometric mean | (ref)                                                        | 1.32x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.25 ms: 1.10x faster                                                      |
| regex_dna      | 239 ms                                                       | 259 ms: 1.08x slower                                                       |
| regex_v8       | 23.6 ms                                                      | 27.1 ms: 1.15x slower                                                      |
| regex_compile  | 144 ms                                                       | 191 ms: 1.33x slower                                                       |
| Geometric mean | (ref)                                                        | 1.11x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 4.04 us: 1.10x faster                                                      |
| unpickle             | 14.8 us                                                      | 14.1 us: 1.05x faster                                                      |
| pickle_dict          | 32.5 us                                                      | 31.1 us: 1.05x faster                                                      |
| pickle               | 10.5 us                                                      | 10.1 us: 1.04x faster                                                      |
| unpickle_list        | 4.66 us                                                      | 4.61 us: 1.01x faster                                                      |
| xml_etree_iterparse  | 103 ms                                                       | 109 ms: 1.06x slower                                                       |
| xml_etree_generate   | 86.1 ms                                                      | 92.8 ms: 1.08x slower                                                      |
| xml_etree_parse      | 144 ms                                                       | 160 ms: 1.11x slower                                                       |
| json_loads           | 24.4 us                                                      | 30.2 us: 1.24x slower                                                      |
| xml_etree_process    | 58.4 ms                                                      | 76.5 ms: 1.31x slower                                                      |
| json_dumps           | 10.2 ms                                                      | 14.4 ms: 1.41x slower                                                      |
| pickle_pure_python   | 318 us                                                       | 454 us: 1.43x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 313 us: 1.49x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.13x slower                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.35 ms: 1.17x faster                                                      |
| python_startup         | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                                      |
| Geometric mean         | (ref)                                                        | 1.09x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 53.2 ms: 1.39x slower                                                      |
| mako            | 10.0 ms                                                      | 14.9 ms: 1.49x slower                                                      |
| Geometric mean  | (ref)                                                        | 1.44x slower                                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site  | 8.64 ms                                                      | 7.35 ms: 1.17x faster                                                      |
| regex_effbot            | 3.57 ms                                                      | 3.25 ms: 1.10x faster                                                      |
| pickle_list             | 4.43 us                                                      | 4.04 us: 1.10x faster                                                      |
| unpickle                | 14.8 us                                                      | 14.1 us: 1.05x faster                                                      |
| coverage                | 66.7 ms                                                      | 63.5 ms: 1.05x faster                                                      |
| pickle_dict             | 32.5 us                                                      | 31.1 us: 1.05x faster                                                      |
| pickle                  | 10.5 us                                                      | 10.1 us: 1.04x faster                                                      |
| unpickle_list           | 4.66 us                                                      | 4.61 us: 1.01x faster                                                      |
| python_startup          | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                                      |
| pidigits                | 265 ms                                                       | 271 ms: 1.02x slower                                                       |
| telco                   | 6.96 ms                                                      | 7.16 ms: 1.03x slower                                                      |
| gc_traversal            | 3.48 ms                                                      | 3.68 ms: 1.06x slower                                                      |
| xml_etree_iterparse     | 103 ms                                                       | 109 ms: 1.06x slower                                                       |
| sqlite_synth            | 2.77 us                                                      | 2.97 us: 1.07x slower                                                      |
| async_generators        | 390 ms                                                       | 418 ms: 1.07x slower                                                       |
| xml_etree_generate      | 86.1 ms                                                      | 92.8 ms: 1.08x slower                                                      |
| meteor_contest          | 128 ms                                                       | 139 ms: 1.08x slower                                                       |
| regex_dna               | 239 ms                                                       | 259 ms: 1.08x slower                                                       |
| xml_etree_parse         | 144 ms                                                       | 160 ms: 1.11x slower                                                       |
| pathlib                 | 18.9 ms                                                      | 21.0 ms: 1.11x slower                                                      |
| unpack_sequence         | 53.2 ns                                                      | 59.4 ns: 1.12x slower                                                      |
| gunicorn                | 1.00 ms                                                      | 1.13 ms: 1.13x slower                                                      |
| aiohttp                 | 1.02 ms                                                      | 1.15 ms: 1.13x slower                                                      |
| create_gc_cycles        | 1.59 ms                                                      | 1.82 ms: 1.14x slower                                                      |
| regex_v8                | 23.6 ms                                                      | 27.1 ms: 1.15x slower                                                      |
| bench_thread_pool       | 950 us                                                       | 1.10 ms: 1.16x slower                                                      |
| json                    | 5.12 ms                                                      | 5.97 ms: 1.17x slower                                                      |
| dask                    | 392 ms                                                       | 459 ms: 1.17x slower                                                       |
| sqlalchemy_declarative  | 159 ms                                                       | 188 ms: 1.18x slower                                                       |
| deepcopy_reduce         | 3.37 us                                                      | 3.99 us: 1.18x slower                                                      |
| sympy_integrate         | 23.9 ms                                                      | 28.4 ms: 1.19x slower                                                      |
| docutils                | 2.87 sec                                                     | 3.42 sec: 1.19x slower                                                     |
| scimark_fft             | 301 ms                                                       | 360 ms: 1.19x slower                                                       |
| sqlglot_optimize        | 57.5 ms                                                      | 69.1 ms: 1.20x slower                                                      |
| sympy_str               | 302 ms                                                       | 366 ms: 1.21x slower                                                       |
| mdp                     | 2.57 sec                                                     | 3.12 sec: 1.21x slower                                                     |
| sympy_sum               | 162 ms                                                       | 199 ms: 1.23x slower                                                       |
| 2to3                    | 285 ms                                                       | 350 ms: 1.23x slower                                                       |
| dulwich_log             | 65.4 ms                                                      | 80.1 ms: 1.23x slower                                                      |
| sqlalchemy_imperative   | 18.7 ms                                                      | 23.0 ms: 1.23x slower                                                      |
| comprehensions          | 21.9 us                                                      | 27.1 us: 1.24x slower                                                      |
| json_loads              | 24.4 us                                                      | 30.2 us: 1.24x slower                                                      |
| tornado_http            | 121 ms                                                       | 150 ms: 1.24x slower                                                       |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 5.22 ms: 1.24x slower                                                      |
| sqlglot_normalize       | 116 ms                                                       | 144 ms: 1.25x slower                                                       |
| nqueens                 | 89.9 ms                                                      | 112 ms: 1.25x slower                                                       |
| deepcopy                | 368 us                                                       | 465 us: 1.26x slower                                                       |
| sympy_expand            | 484 ms                                                       | 615 ms: 1.27x slower                                                       |
| logging_format          | 7.48 us                                                      | 9.57 us: 1.28x slower                                                      |
| pprint_safe_repr        | 807 ms                                                       | 1.03 sec: 1.28x slower                                                     |
| pprint_pformat          | 1.65 sec                                                     | 2.14 sec: 1.30x slower                                                     |
| chameleon               | 7.23 ms                                                      | 9.41 ms: 1.30x slower                                                      |
| pycparser               | 1.23 sec                                                     | 1.61 sec: 1.30x slower                                                     |
| xml_etree_process       | 58.4 ms                                                      | 76.5 ms: 1.31x slower                                                      |
| coroutines              | 23.0 ms                                                      | 30.2 ms: 1.31x slower                                                      |
| regex_compile           | 144 ms                                                       | 191 ms: 1.33x slower                                                       |
| logging_simple          | 6.71 us                                                      | 8.94 us: 1.33x slower                                                      |
| fannkuch                | 350 ms                                                       | 477 ms: 1.36x slower                                                       |
| async_tree_cpu_io_mixed | 696 ms                                                       | 952 ms: 1.37x slower                                                       |
| deepcopy_memo           | 36.8 us                                                      | 51.1 us: 1.39x slower                                                      |
| django_template         | 38.2 ms                                                      | 53.2 ms: 1.39x slower                                                      |
| json_dumps              | 10.2 ms                                                      | 14.4 ms: 1.41x slower                                                      |
| pickle_pure_python      | 318 us                                                       | 454 us: 1.43x slower                                                       |
| crypto_pyaes            | 80.3 ms                                                      | 115 ms: 1.43x slower                                                       |
| bench_mp_pool           | 4.76 ms                                                      | 6.82 ms: 1.43x slower                                                      |
| float                   | 76.6 ms                                                      | 110 ms: 1.44x slower                                                       |
| mako                    | 10.0 ms                                                      | 14.9 ms: 1.49x slower                                                      |
| spectral_norm           | 91.6 ms                                                      | 137 ms: 1.49x slower                                                       |
| unpickle_pure_python    | 210 us                                                       | 313 us: 1.49x slower                                                       |
| sqlglot_transpile       | 1.78 ms                                                      | 2.69 ms: 1.52x slower                                                      |
| async_tree_memoization  | 544 ms                                                       | 827 ms: 1.52x slower                                                       |
| async_tree_none         | 452 ms                                                       | 695 ms: 1.54x slower                                                       |
| async_tree_io           | 1.04 sec                                                     | 1.61 sec: 1.54x slower                                                     |
| generators              | 37.4 ms                                                      | 57.8 ms: 1.54x slower                                                      |
| nbody                   | 88.0 ms                                                      | 137 ms: 1.56x slower                                                       |
| pyflate                 | 439 ms                                                       | 693 ms: 1.58x slower                                                       |
| hexiom                  | 5.96 ms                                                      | 9.43 ms: 1.58x slower                                                      |
| scimark_monte_carlo     | 69.0 ms                                                      | 110 ms: 1.60x slower                                                       |
| scimark_sor             | 109 ms                                                       | 176 ms: 1.62x slower                                                       |
| richards                | 45.7 ms                                                      | 74.5 ms: 1.63x slower                                                      |
| scimark_lu              | 98.8 ms                                                      | 161 ms: 1.63x slower                                                       |
| sqlglot_parse           | 1.38 ms                                                      | 2.26 ms: 1.64x slower                                                      |
| chaos                   | 64.0 ms                                                      | 105 ms: 1.64x slower                                                       |
| raytrace                | 298 ms                                                       | 491 ms: 1.65x slower                                                       |
| logging_silent          | 94.4 ns                                                      | 166 ns: 1.76x slower                                                       |
| go                      | 150 ms                                                       | 264 ms: 1.77x slower                                                       |
| asyncio_tcp             | 378 ms                                                       | 781 ms: 2.07x slower                                                       |
| deltablue               | 3.24 ms                                                      | 7.44 ms: 2.30x slower                                                      |
| Geometric mean          | (ref)                                                        | 1.28x slower                                                               |
Ignored benchmarks (10) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20230404-3.10.11-7d4cc5a/bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.24x
- 95% likely to have a slowdown of 1.23x
- 99% likely to have a slowdown of 1.22x


# Memory

- memory change: 0.84x