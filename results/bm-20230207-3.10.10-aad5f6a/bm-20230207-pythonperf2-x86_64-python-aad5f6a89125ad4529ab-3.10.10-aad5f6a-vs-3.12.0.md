
# Results vs. 3.12.0

- fork: python
- ref: aad5f6a89125ad4529ab
- machine: linux-x86_64
- commit hash: aad5f6a
- commit date: 2023-02-07
- overall geometric mean: 1.29x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x slower
- Memory change: 0.84x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 351 ms: 1.23x slower                                                       |
| chameleon      | 7.23 ms                                                      | 9.41 ms: 1.30x slower                                                      |
| docutils       | 2.87 sec                                                     | 3.45 sec: 1.20x slower                                                     |
| tornado_http   | 121 ms                                                       | 159 ms: 1.31x slower                                                       |
| Geometric mean | (ref)                                                        | 1.26x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 955 ms: 1.37x slower                                                       |
| async_tree_memoization  | 544 ms                                                       | 832 ms: 1.53x slower                                                       |
| async_tree_io           | 1.04 sec                                                     | 1.62 sec: 1.56x slower                                                     |
| async_tree_none         | 452 ms                                                       | 711 ms: 1.57x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.51x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 271 ms: 1.02x slower                                                       |
| float          | 76.6 ms                                                      | 111 ms: 1.45x slower                                                       |
| nbody          | 88.0 ms                                                      | 138 ms: 1.56x slower                                                       |
| Geometric mean | (ref)                                                        | 1.32x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.49 ms: 1.02x faster                                                      |
| regex_dna      | 239 ms                                                       | 260 ms: 1.09x slower                                                       |
| regex_v8       | 23.6 ms                                                      | 27.2 ms: 1.15x slower                                                      |
| regex_compile  | 144 ms                                                       | 192 ms: 1.33x slower                                                       |
| Geometric mean | (ref)                                                        | 1.13x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpickle             | 14.8 us                                                      | 13.7 us: 1.08x faster                                                      |
| pickle_list          | 4.43 us                                                      | 4.17 us: 1.06x faster                                                      |
| pickle               | 10.5 us                                                      | 10.1 us: 1.04x faster                                                      |
| pickle_dict          | 32.5 us                                                      | 32.1 us: 1.01x faster                                                      |
| unpickle_list        | 4.66 us                                                      | 4.71 us: 1.01x slower                                                      |
| xml_etree_generate   | 86.1 ms                                                      | 94.0 ms: 1.09x slower                                                      |
| xml_etree_iterparse  | 103 ms                                                       | 113 ms: 1.10x slower                                                       |
| xml_etree_parse      | 144 ms                                                       | 164 ms: 1.14x slower                                                       |
| json_loads           | 24.4 us                                                      | 30.0 us: 1.23x slower                                                      |
| xml_etree_process    | 58.4 ms                                                      | 77.5 ms: 1.33x slower                                                      |
| json_dumps           | 10.2 ms                                                      | 14.4 ms: 1.41x slower                                                      |
| pickle_pure_python   | 318 us                                                       | 461 us: 1.45x slower                                                       |
| unpickle_pure_python | 210 us                                                       | 320 us: 1.53x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.14x slower                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.34 ms: 1.18x faster                                                      |
| python_startup         | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                                      |
| Geometric mean         | (ref)                                                        | 1.09x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 53.6 ms: 1.41x slower                                                      |
| mako            | 10.0 ms                                                      | 14.7 ms: 1.47x slower                                                      |
| Geometric mean  | (ref)                                                        | 1.44x slower                                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site  | 8.64 ms                                                      | 7.34 ms: 1.18x faster                                                      |
| unpickle                | 14.8 us                                                      | 13.7 us: 1.08x faster                                                      |
| pickle_list             | 4.43 us                                                      | 4.17 us: 1.06x faster                                                      |
| coverage                | 66.7 ms                                                      | 63.3 ms: 1.05x faster                                                      |
| pickle                  | 10.5 us                                                      | 10.1 us: 1.04x faster                                                      |
| regex_effbot            | 3.57 ms                                                      | 3.49 ms: 1.02x faster                                                      |
| pickle_dict             | 32.5 us                                                      | 32.1 us: 1.01x faster                                                      |
| python_startup          | 11.6 ms                                                      | 11.5 ms: 1.01x faster                                                      |
| unpickle_list           | 4.66 us                                                      | 4.71 us: 1.01x slower                                                      |
| pidigits                | 265 ms                                                       | 271 ms: 1.02x slower                                                       |
| telco                   | 6.96 ms                                                      | 7.25 ms: 1.04x slower                                                      |
| async_generators        | 390 ms                                                       | 417 ms: 1.07x slower                                                       |
| sqlite_synth            | 2.77 us                                                      | 2.98 us: 1.07x slower                                                      |
| meteor_contest          | 128 ms                                                       | 139 ms: 1.08x slower                                                       |
| regex_dna               | 239 ms                                                       | 260 ms: 1.09x slower                                                       |
| xml_etree_generate      | 86.1 ms                                                      | 94.0 ms: 1.09x slower                                                      |
| xml_etree_iterparse     | 103 ms                                                       | 113 ms: 1.10x slower                                                       |
| unpack_sequence         | 53.2 ns                                                      | 59.3 ns: 1.11x slower                                                      |
| gunicorn                | 1.00 ms                                                      | 1.13 ms: 1.12x slower                                                      |
| aiohttp                 | 1.02 ms                                                      | 1.15 ms: 1.13x slower                                                      |
| pathlib                 | 18.9 ms                                                      | 21.3 ms: 1.13x slower                                                      |
| xml_etree_parse         | 144 ms                                                       | 164 ms: 1.14x slower                                                       |
| create_gc_cycles        | 1.59 ms                                                      | 1.81 ms: 1.14x slower                                                      |
| regex_v8                | 23.6 ms                                                      | 27.2 ms: 1.15x slower                                                      |
| json                    | 5.12 ms                                                      | 5.91 ms: 1.15x slower                                                      |
| bench_thread_pool       | 950 us                                                       | 1.11 ms: 1.16x slower                                                      |
| sqlalchemy_declarative  | 159 ms                                                       | 187 ms: 1.17x slower                                                       |
| gc_traversal            | 3.48 ms                                                      | 4.12 ms: 1.19x slower                                                      |
| mdp                     | 2.57 sec                                                     | 3.05 sec: 1.19x slower                                                     |
| sympy_integrate         | 23.9 ms                                                      | 28.5 ms: 1.19x slower                                                      |
| deepcopy_reduce         | 3.37 us                                                      | 4.05 us: 1.20x slower                                                      |
| docutils                | 2.87 sec                                                     | 3.45 sec: 1.20x slower                                                     |
| sympy_str               | 302 ms                                                       | 364 ms: 1.20x slower                                                       |
| sqlglot_optimize        | 57.5 ms                                                      | 69.6 ms: 1.21x slower                                                      |
| sqlalchemy_imperative   | 18.7 ms                                                      | 22.9 ms: 1.22x slower                                                      |
| sympy_sum               | 162 ms                                                       | 199 ms: 1.23x slower                                                       |
| 2to3                    | 285 ms                                                       | 351 ms: 1.23x slower                                                       |
| json_loads              | 24.4 us                                                      | 30.0 us: 1.23x slower                                                      |
| comprehensions          | 21.9 us                                                      | 27.0 us: 1.23x slower                                                      |
| dask                    | 392 ms                                                       | 484 ms: 1.23x slower                                                       |
| dulwich_log             | 65.4 ms                                                      | 81.1 ms: 1.24x slower                                                      |
| nqueens                 | 89.9 ms                                                      | 113 ms: 1.25x slower                                                       |
| sympy_expand            | 484 ms                                                       | 608 ms: 1.26x slower                                                       |
| scimark_sparse_mat_mult | 4.21 ms                                                      | 5.28 ms: 1.26x slower                                                      |
| sqlglot_normalize       | 116 ms                                                       | 146 ms: 1.26x slower                                                       |
| deepcopy                | 368 us                                                       | 466 us: 1.27x slower                                                       |
| scimark_fft             | 301 ms                                                       | 383 ms: 1.27x slower                                                       |
| pprint_pformat          | 1.65 sec                                                     | 2.11 sec: 1.27x slower                                                     |
| pprint_safe_repr        | 807 ms                                                       | 1.03 sec: 1.27x slower                                                     |
| logging_format          | 7.48 us                                                      | 9.67 us: 1.29x slower                                                      |
| coroutines              | 23.0 ms                                                      | 29.9 ms: 1.30x slower                                                      |
| chameleon               | 7.23 ms                                                      | 9.41 ms: 1.30x slower                                                      |
| tornado_http            | 121 ms                                                       | 159 ms: 1.31x slower                                                       |
| xml_etree_process       | 58.4 ms                                                      | 77.5 ms: 1.33x slower                                                      |
| regex_compile           | 144 ms                                                       | 192 ms: 1.33x slower                                                       |
| logging_simple          | 6.71 us                                                      | 8.96 us: 1.34x slower                                                      |
| fannkuch                | 350 ms                                                       | 470 ms: 1.34x slower                                                       |
| pycparser               | 1.23 sec                                                     | 1.67 sec: 1.35x slower                                                     |
| deepcopy_memo           | 36.8 us                                                      | 50.0 us: 1.36x slower                                                      |
| async_tree_cpu_io_mixed | 696 ms                                                       | 955 ms: 1.37x slower                                                       |
| django_template         | 38.2 ms                                                      | 53.6 ms: 1.41x slower                                                      |
| json_dumps              | 10.2 ms                                                      | 14.4 ms: 1.41x slower                                                      |
| float                   | 76.6 ms                                                      | 111 ms: 1.45x slower                                                       |
| pickle_pure_python      | 318 us                                                       | 461 us: 1.45x slower                                                       |
| mako                    | 10.0 ms                                                      | 14.7 ms: 1.47x slower                                                      |
| crypto_pyaes            | 80.3 ms                                                      | 118 ms: 1.47x slower                                                       |
| spectral_norm           | 91.6 ms                                                      | 138 ms: 1.50x slower                                                       |
| sqlglot_transpile       | 1.78 ms                                                      | 2.70 ms: 1.52x slower                                                      |
| bench_mp_pool           | 4.76 ms                                                      | 7.26 ms: 1.52x slower                                                      |
| generators              | 37.4 ms                                                      | 57.0 ms: 1.52x slower                                                      |
| unpickle_pure_python    | 210 us                                                       | 320 us: 1.53x slower                                                       |
| async_tree_memoization  | 544 ms                                                       | 832 ms: 1.53x slower                                                       |
| async_tree_io           | 1.04 sec                                                     | 1.62 sec: 1.56x slower                                                     |
| nbody                   | 88.0 ms                                                      | 138 ms: 1.56x slower                                                       |
| async_tree_none         | 452 ms                                                       | 711 ms: 1.57x slower                                                       |
| pyflate                 | 439 ms                                                       | 696 ms: 1.59x slower                                                       |
| scimark_monte_carlo     | 69.0 ms                                                      | 110 ms: 1.59x slower                                                       |
| richards                | 45.7 ms                                                      | 72.9 ms: 1.59x slower                                                      |
| hexiom                  | 5.96 ms                                                      | 9.49 ms: 1.59x slower                                                      |
| scimark_sor             | 109 ms                                                       | 177 ms: 1.62x slower                                                       |
| sqlglot_parse           | 1.38 ms                                                      | 2.25 ms: 1.63x slower                                                      |
| raytrace                | 298 ms                                                       | 495 ms: 1.66x slower                                                       |
| chaos                   | 64.0 ms                                                      | 109 ms: 1.70x slower                                                       |
| scimark_lu              | 98.8 ms                                                      | 170 ms: 1.72x slower                                                       |
| go                      | 150 ms                                                       | 260 ms: 1.74x slower                                                       |
| logging_silent          | 94.4 ns                                                      | 165 ns: 1.75x slower                                                       |
| asyncio_tcp             | 378 ms                                                       | 779 ms: 2.06x slower                                                       |
| deltablue               | 3.24 ms                                                      | 7.45 ms: 2.30x slower                                                      |
| Geometric mean          | (ref)                                                        | 1.29x slower                                                               |
Ignored benchmarks (10) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20230207-3.10.10-aad5f6a/bm-20230207-pythonperf2-x86_64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.25x
- 95% likely to have a slowdown of 1.24x
- 99% likely to have a slowdown of 1.23x


# Memory

- memory change: 0.84x