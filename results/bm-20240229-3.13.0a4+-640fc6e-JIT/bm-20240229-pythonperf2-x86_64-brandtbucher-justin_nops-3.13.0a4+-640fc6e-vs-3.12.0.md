# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_nops
- machine: linux-x86_64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.06x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 308 ms: 1.08x slower                                                      |
| chameleon      | 7.23 ms                                                      | 7.45 ms: 1.03x slower                                                     |
| docutils       | 2.87 sec                                                     | 2.91 sec: 1.01x slower                                                    |
| tornado_http   | 121 ms                                                       | 125 ms: 1.03x slower                                                      |
| Geometric mean | (ref)                                                        | 1.04x slower                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 441 ms: 1.02x faster                                                      |
| async_tree_none_tg         | 431 ms                                                       | 435 ms: 1.01x slower                                                      |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 708 ms: 1.02x slower                                                      |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 707 ms: 1.02x slower                                                      |
| async_tree_memoization     | 544 ms                                                       | 554 ms: 1.02x slower                                                      |
| async_tree_memoization_tg  | 540 ms                                                       | 554 ms: 1.02x slower                                                      |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                    |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                                    |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 262 ms: 1.01x faster                                                      |
| float          | 76.6 ms                                                      | 79.0 ms: 1.03x slower                                                     |
| nbody          | 88.0 ms                                                      | 99.1 ms: 1.13x slower                                                     |
| Geometric mean | (ref)                                                        | 1.05x slower                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_dna      | 239 ms                                                       | 238 ms: 1.00x faster                                                      |
| regex_compile  | 144 ms                                                       | 147 ms: 1.02x slower                                                      |
| regex_v8       | 23.6 ms                                                      | 25.0 ms: 1.06x slower                                                     |
| Geometric mean | (ref)                                                        | 1.02x slower                                                              |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| xml_etree_generate   | 86.1 ms                                                      | 83.5 ms: 1.03x faster                                                     |
| xml_etree_process    | 58.4 ms                                                      | 57.7 ms: 1.01x faster                                                     |
| pickle_list          | 4.43 us                                                      | 4.38 us: 1.01x faster                                                     |
| unpickle_list        | 4.66 us                                                      | 4.63 us: 1.01x faster                                                     |
| xml_etree_parse      | 144 ms                                                       | 143 ms: 1.00x faster                                                      |
| pickle               | 10.5 us                                                      | 10.6 us: 1.01x slower                                                     |
| pickle_dict          | 32.5 us                                                      | 32.9 us: 1.01x slower                                                     |
| unpickle             | 14.8 us                                                      | 15.2 us: 1.02x slower                                                     |
| tomli_loads          | 2.16 sec                                                     | 2.22 sec: 1.03x slower                                                    |
| json_loads           | 24.4 us                                                      | 25.1 us: 1.03x slower                                                     |
| json_dumps           | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                     |
| unpickle_pure_python | 210 us                                                       | 238 us: 1.13x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                              |

Benchmark hidden because not significant (2): xml_etree_iterparse, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 15.5 ms: 1.33x slower                                                     |
| python_startup_no_site | 8.64 ms                                                      | 14.0 ms: 1.62x slower                                                     |
| Geometric mean         | (ref)                                                        | 1.47x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 40.3 ms: 1.06x slower                                                     |
| Geometric mean  | (ref)                                                        | 1.03x slower                                                              |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 123 us: 1.23x faster                                                      |
| comprehensions             | 21.9 us                                                      | 19.2 us: 1.14x faster                                                     |
| generators                 | 37.4 ms                                                      | 34.0 ms: 1.10x faster                                                     |
| crypto_pyaes               | 80.3 ms                                                      | 77.5 ms: 1.04x faster                                                     |
| async_generators           | 390 ms                                                       | 377 ms: 1.04x faster                                                      |
| xml_etree_generate         | 86.1 ms                                                      | 83.5 ms: 1.03x faster                                                     |
| create_gc_cycles           | 1.59 ms                                                      | 1.55 ms: 1.03x faster                                                     |
| sqlite_synth               | 2.77 us                                                      | 2.71 us: 1.02x faster                                                     |
| async_tree_none            | 452 ms                                                       | 441 ms: 1.02x faster                                                      |
| coroutines                 | 23.0 ms                                                      | 22.6 ms: 1.02x faster                                                     |
| asyncio_tcp                | 378 ms                                                       | 372 ms: 1.02x faster                                                      |
| logging_format             | 7.48 us                                                      | 7.39 us: 1.01x faster                                                     |
| sympy_sum                  | 162 ms                                                       | 160 ms: 1.01x faster                                                      |
| pidigits                   | 265 ms                                                       | 262 ms: 1.01x faster                                                      |
| xml_etree_process          | 58.4 ms                                                      | 57.7 ms: 1.01x faster                                                     |
| pickle_list                | 4.43 us                                                      | 4.38 us: 1.01x faster                                                     |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 4.18 ms: 1.01x faster                                                     |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.58 sec: 1.01x faster                                                    |
| unpickle_list              | 4.66 us                                                      | 4.63 us: 1.01x faster                                                     |
| xml_etree_parse            | 144 ms                                                       | 143 ms: 1.00x faster                                                      |
| regex_dna                  | 239 ms                                                       | 238 ms: 1.00x faster                                                      |
| sympy_str                  | 302 ms                                                       | 303 ms: 1.00x slower                                                      |
| asyncio_websockets         | 387 ms                                                       | 391 ms: 1.01x slower                                                      |
| async_tree_none_tg         | 431 ms                                                       | 435 ms: 1.01x slower                                                      |
| pickle                     | 10.5 us                                                      | 10.6 us: 1.01x slower                                                     |
| pickle_dict                | 32.5 us                                                      | 32.9 us: 1.01x slower                                                     |
| docutils                   | 2.87 sec                                                     | 2.91 sec: 1.01x slower                                                    |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 708 ms: 1.02x slower                                                      |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 707 ms: 1.02x slower                                                      |
| async_tree_memoization     | 544 ms                                                       | 554 ms: 1.02x slower                                                      |
| regex_compile              | 144 ms                                                       | 147 ms: 1.02x slower                                                      |
| unpickle                   | 14.8 us                                                      | 15.2 us: 1.02x slower                                                     |
| async_tree_memoization_tg  | 540 ms                                                       | 554 ms: 1.02x slower                                                      |
| deepcopy                   | 368 us                                                       | 378 us: 1.02x slower                                                      |
| deepcopy_memo              | 36.8 us                                                      | 37.7 us: 1.02x slower                                                     |
| sympy_integrate            | 23.9 ms                                                      | 24.5 ms: 1.03x slower                                                     |
| tomli_loads                | 2.16 sec                                                     | 2.22 sec: 1.03x slower                                                    |
| async_tree_io_tg           | 1.05 sec                                                     | 1.08 sec: 1.03x slower                                                    |
| json_loads                 | 24.4 us                                                      | 25.1 us: 1.03x slower                                                     |
| float                      | 76.6 ms                                                      | 79.0 ms: 1.03x slower                                                     |
| chameleon                  | 7.23 ms                                                      | 7.45 ms: 1.03x slower                                                     |
| sqlglot_normalize          | 116 ms                                                       | 119 ms: 1.03x slower                                                      |
| logging_silent             | 94.4 ns                                                      | 97.4 ns: 1.03x slower                                                     |
| spectral_norm              | 91.6 ms                                                      | 94.7 ms: 1.03x slower                                                     |
| tornado_http               | 121 ms                                                       | 125 ms: 1.03x slower                                                      |
| bench_thread_pool          | 950 us                                                       | 986 us: 1.04x slower                                                      |
| json_dumps                 | 10.2 ms                                                      | 10.6 ms: 1.04x slower                                                     |
| meteor_contest             | 128 ms                                                       | 133 ms: 1.04x slower                                                      |
| raytrace                   | 298 ms                                                       | 310 ms: 1.04x slower                                                      |
| sqlglot_parse              | 1.38 ms                                                      | 1.43 ms: 1.04x slower                                                     |
| pathlib                    | 18.9 ms                                                      | 19.6 ms: 1.04x slower                                                     |
| json                       | 5.12 ms                                                      | 5.34 ms: 1.04x slower                                                     |
| sqlglot_transpile          | 1.78 ms                                                      | 1.86 ms: 1.05x slower                                                     |
| pprint_safe_repr           | 807 ms                                                       | 846 ms: 1.05x slower                                                      |
| pprint_pformat             | 1.65 sec                                                     | 1.74 sec: 1.05x slower                                                    |
| pycparser                  | 1.23 sec                                                     | 1.30 sec: 1.05x slower                                                    |
| async_tree_io              | 1.04 sec                                                     | 1.10 sec: 1.05x slower                                                    |
| django_template            | 38.2 ms                                                      | 40.3 ms: 1.06x slower                                                     |
| gc_traversal               | 3.48 ms                                                      | 3.68 ms: 1.06x slower                                                     |
| regex_v8                   | 23.6 ms                                                      | 25.0 ms: 1.06x slower                                                     |
| sympy_expand               | 484 ms                                                       | 513 ms: 1.06x slower                                                      |
| dulwich_log                | 65.4 ms                                                      | 69.4 ms: 1.06x slower                                                     |
| chaos                      | 64.0 ms                                                      | 68.3 ms: 1.07x slower                                                     |
| gunicorn                   | 1.00 ms                                                      | 1.07 ms: 1.07x slower                                                     |
| 2to3                       | 285 ms                                                       | 308 ms: 1.08x slower                                                      |
| scimark_fft                | 301 ms                                                       | 327 ms: 1.09x slower                                                      |
| aiohttp                    | 1.02 ms                                                      | 1.11 ms: 1.09x slower                                                     |
| richards_super             | 51.3 ms                                                      | 56.2 ms: 1.10x slower                                                     |
| richards                   | 45.7 ms                                                      | 50.2 ms: 1.10x slower                                                     |
| sqlglot_optimize           | 57.5 ms                                                      | 63.3 ms: 1.10x slower                                                     |
| mypy2                      | 830 ms                                                       | 915 ms: 1.10x slower                                                      |
| nbody                      | 88.0 ms                                                      | 99.1 ms: 1.13x slower                                                     |
| scimark_monte_carlo        | 69.0 ms                                                      | 77.9 ms: 1.13x slower                                                     |
| unpickle_pure_python       | 210 us                                                       | 238 us: 1.13x slower                                                      |
| nqueens                    | 89.9 ms                                                      | 103 ms: 1.14x slower                                                      |
| unpack_sequence            | 53.2 ns                                                      | 61.0 ns: 1.15x slower                                                     |
| fannkuch                   | 350 ms                                                       | 402 ms: 1.15x slower                                                      |
| go                         | 150 ms                                                       | 173 ms: 1.15x slower                                                      |
| deltablue                  | 3.24 ms                                                      | 3.77 ms: 1.17x slower                                                     |
| telco                      | 6.96 ms                                                      | 8.24 ms: 1.18x slower                                                     |
| scimark_lu                 | 98.8 ms                                                      | 118 ms: 1.19x slower                                                      |
| pyflate                    | 439 ms                                                       | 528 ms: 1.20x slower                                                      |
| coverage                   | 66.7 ms                                                      | 80.4 ms: 1.21x slower                                                     |
| hexiom                     | 5.96 ms                                                      | 7.43 ms: 1.25x slower                                                     |
| python_startup             | 11.6 ms                                                      | 15.5 ms: 1.33x slower                                                     |
| scimark_sor                | 109 ms                                                       | 153 ms: 1.40x slower                                                      |
| bench_mp_pool              | 4.76 ms                                                      | 6.96 ms: 1.46x slower                                                     |
| dask                       | 392 ms                                                       | 589 ms: 1.50x slower                                                      |
| python_startup_no_site     | 8.64 ms                                                      | 14.0 ms: 1.62x slower                                                     |
| Geometric mean             | (ref)                                                        | 1.06x slower                                                              |

Benchmark hidden because not significant (7): xml_etree_iterparse, regex_effbot, deepcopy_reduce, pickle_pure_python, mdp, logging_simple, mako
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240229-3.13.0a4+-640fc6e-JIT/bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.11x