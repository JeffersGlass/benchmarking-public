# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_arena
- machine: windows-x86
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 280 ms                                                          | 260 ms: 1.08x faster                                                          |
| chameleon      | 7.75 ms                                                         | 5.71 ms: 1.36x faster                                                         |
| docutils       | 1.98 sec                                                        | 1.80 sec: 1.10x faster                                                        |
| tornado_http   | 105 ms                                                          | 95.9 ms: 1.09x faster                                                         |
| Geometric mean | (ref)                                                           | 1.15x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_none            | 298 ms                                                          | 257 ms: 1.16x faster                                                          |
| async_tree_memoization_tg  | 350 ms                                                          | 303 ms: 1.16x faster                                                          |
| async_tree_none_tg         | 278 ms                                                          | 242 ms: 1.15x faster                                                          |
| async_tree_memoization     | 364 ms                                                          | 320 ms: 1.14x faster                                                          |
| async_tree_io_tg           | 677 ms                                                          | 605 ms: 1.12x faster                                                          |
| async_tree_io              | 693 ms                                                          | 621 ms: 1.12x faster                                                          |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 518 ms: 1.09x faster                                                          |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 509 ms: 1.07x faster                                                          |
| Geometric mean             | (ref)                                                           | 1.12x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| float          | 76.7 ms                                                         | 55.1 ms: 1.39x faster                                                         |
| nbody          | 127 ms                                                          | 96.5 ms: 1.32x faster                                                         |
| pidigits       | 199 ms                                                          | 198 ms: 1.01x faster                                                          |
| Geometric mean | (ref)                                                           | 1.23x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_compile  | 129 ms                                                          | 107 ms: 1.21x faster                                                          |
| regex_dna      | 127 ms                                                          | 116 ms: 1.09x faster                                                          |
| regex_effbot   | 2.04 ms                                                         | 1.88 ms: 1.08x faster                                                         |
| regex_v8       | 15.0 ms                                                         | 16.1 ms: 1.07x slower                                                         |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pickle_pure_python   | 286 us                                                          | 209 us: 1.37x faster                                                          |
| tomli_loads          | 2.20 sec                                                        | 1.70 sec: 1.29x faster                                                        |
| xml_etree_process    | 53.2 ms                                                         | 42.8 ms: 1.24x faster                                                         |
| unpickle_pure_python | 210 us                                                          | 171 us: 1.23x faster                                                          |
| xml_etree_iterparse  | 77.6 ms                                                         | 66.5 ms: 1.17x faster                                                         |
| xml_etree_generate   | 72.1 ms                                                         | 62.5 ms: 1.15x faster                                                         |
| json_dumps           | 7.40 ms                                                         | 6.87 ms: 1.08x faster                                                         |
| pickle_list          | 3.37 us                                                         | 3.23 us: 1.04x faster                                                         |
| unpickle_list        | 2.95 us                                                         | 2.82 us: 1.04x faster                                                         |
| xml_etree_parse      | 113 ms                                                          | 109 ms: 1.04x faster                                                          |
| json_loads           | 20.4 us                                                         | 19.8 us: 1.03x faster                                                         |
| pickle_dict          | 19.9 us                                                         | 19.9 us: 1.00x faster                                                         |
| pickle               | 7.79 us                                                         | 7.89 us: 1.01x slower                                                         |
| unpickle             | 9.71 us                                                         | 10.0 us: 1.03x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.4 ms                                                         | 25.7 ms: 1.15x slower                                                         |
| python_startup_no_site | 19.1 ms                                                         | 23.6 ms: 1.24x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.19x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako            | 9.96 ms                                                         | 7.12 ms: 1.40x faster                                                         |
| django_template | 36.9 ms                                                         | 29.9 ms: 1.23x faster                                                         |
| Geometric mean  | (ref)                                                           | 1.31x faster                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| generators                 | 38.5 ms                                                         | 22.1 ms: 1.75x faster                                                         |
| logging_silent             | 101 ns                                                          | 59.6 ns: 1.69x faster                                                         |
| deepcopy_memo              | 38.4 us                                                         | 24.4 us: 1.57x faster                                                         |
| unpack_sequence            | 62.5 ns                                                         | 41.7 ns: 1.50x faster                                                         |
| coroutines                 | 20.9 ms                                                         | 14.4 ms: 1.45x faster                                                         |
| deltablue                  | 3.58 ms                                                         | 2.52 ms: 1.42x faster                                                         |
| spectral_norm              | 104 ms                                                          | 74.0 ms: 1.40x faster                                                         |
| mako                       | 9.96 ms                                                         | 7.12 ms: 1.40x faster                                                         |
| float                      | 76.7 ms                                                         | 55.1 ms: 1.39x faster                                                         |
| pickle_pure_python         | 286 us                                                          | 209 us: 1.37x faster                                                          |
| deepcopy_reduce            | 3.23 us                                                         | 2.36 us: 1.36x faster                                                         |
| chameleon                  | 7.75 ms                                                         | 5.71 ms: 1.36x faster                                                         |
| scimark_sor                | 130 ms                                                          | 98.4 ms: 1.32x faster                                                         |
| nbody                      | 127 ms                                                          | 96.5 ms: 1.32x faster                                                         |
| deepcopy                   | 360 us                                                          | 276 us: 1.30x faster                                                          |
| sqlglot_parse              | 1.25 ms                                                         | 965 us: 1.29x faster                                                          |
| typing_runtime_protocols   | 126 us                                                          | 97.7 us: 1.29x faster                                                         |
| tomli_loads                | 2.20 sec                                                        | 1.70 sec: 1.29x faster                                                        |
| comprehensions             | 19.2 us                                                         | 14.9 us: 1.28x faster                                                         |
| sqlglot_transpile          | 1.53 ms                                                         | 1.21 ms: 1.26x faster                                                         |
| xml_etree_process          | 53.2 ms                                                         | 42.8 ms: 1.24x faster                                                         |
| richards_super             | 46.5 ms                                                         | 37.7 ms: 1.23x faster                                                         |
| django_template            | 36.9 ms                                                         | 29.9 ms: 1.23x faster                                                         |
| richards                   | 41.3 ms                                                         | 33.6 ms: 1.23x faster                                                         |
| unpickle_pure_python       | 210 us                                                          | 171 us: 1.23x faster                                                          |
| scimark_sparse_mat_mult    | 3.86 ms                                                         | 3.18 ms: 1.21x faster                                                         |
| regex_compile              | 129 ms                                                          | 107 ms: 1.21x faster                                                          |
| logging_simple             | 9.75 us                                                         | 8.26 us: 1.18x faster                                                         |
| logging_format             | 10.4 us                                                         | 8.87 us: 1.17x faster                                                         |
| xml_etree_iterparse        | 77.6 ms                                                         | 66.5 ms: 1.17x faster                                                         |
| go                         | 137 ms                                                          | 118 ms: 1.17x faster                                                          |
| chaos                      | 69.4 ms                                                         | 59.5 ms: 1.17x faster                                                         |
| pycparser                  | 978 ms                                                          | 842 ms: 1.16x faster                                                          |
| async_tree_none            | 298 ms                                                          | 257 ms: 1.16x faster                                                          |
| async_tree_memoization_tg  | 350 ms                                                          | 303 ms: 1.16x faster                                                          |
| xml_etree_generate         | 72.1 ms                                                         | 62.5 ms: 1.15x faster                                                         |
| sympy_sum                  | 123 ms                                                          | 107 ms: 1.15x faster                                                          |
| sympy_str                  | 240 ms                                                          | 209 ms: 1.15x faster                                                          |
| crypto_pyaes               | 69.2 ms                                                         | 60.3 ms: 1.15x faster                                                         |
| async_tree_none_tg         | 278 ms                                                          | 242 ms: 1.15x faster                                                          |
| sympy_integrate            | 17.5 ms                                                         | 15.4 ms: 1.14x faster                                                         |
| async_tree_memoization     | 364 ms                                                          | 320 ms: 1.14x faster                                                          |
| scimark_fft                | 271 ms                                                          | 240 ms: 1.13x faster                                                          |
| raytrace                   | 308 ms                                                          | 273 ms: 1.13x faster                                                          |
| async_tree_io_tg           | 677 ms                                                          | 605 ms: 1.12x faster                                                          |
| async_tree_io              | 693 ms                                                          | 621 ms: 1.12x faster                                                          |
| pyflate                    | 424 ms                                                          | 380 ms: 1.11x faster                                                          |
| docutils                   | 1.98 sec                                                        | 1.80 sec: 1.10x faster                                                        |
| tornado_http               | 105 ms                                                          | 95.9 ms: 1.09x faster                                                         |
| regex_dna                  | 127 ms                                                          | 116 ms: 1.09x faster                                                          |
| mdp                        | 1.91 sec                                                        | 1.75 sec: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 564 ms                                                          | 518 ms: 1.09x faster                                                          |
| sympy_expand               | 398 ms                                                          | 366 ms: 1.09x faster                                                          |
| hexiom                     | 6.82 ms                                                         | 6.29 ms: 1.08x faster                                                         |
| regex_effbot               | 2.04 ms                                                         | 1.88 ms: 1.08x faster                                                         |
| pathlib                    | 91.4 ms                                                         | 84.5 ms: 1.08x faster                                                         |
| sqlite_synth               | 2.07 us                                                         | 1.92 us: 1.08x faster                                                         |
| json_dumps                 | 7.40 ms                                                         | 6.87 ms: 1.08x faster                                                         |
| 2to3                       | 280 ms                                                          | 260 ms: 1.08x faster                                                          |
| async_tree_cpu_io_mixed_tg | 546 ms                                                          | 509 ms: 1.07x faster                                                          |
| sqlglot_optimize           | 48.5 ms                                                         | 45.3 ms: 1.07x faster                                                         |
| scimark_lu                 | 93.2 ms                                                         | 87.3 ms: 1.07x faster                                                         |
| bench_thread_pool          | 1.10 ms                                                         | 1.05 ms: 1.05x faster                                                         |
| asyncio_tcp_ssl            | 17.7 sec                                                        | 16.8 sec: 1.05x faster                                                        |
| pickle_list                | 3.37 us                                                         | 3.23 us: 1.04x faster                                                         |
| unpickle_list              | 2.95 us                                                         | 2.82 us: 1.04x faster                                                         |
| async_generators           | 313 ms                                                          | 302 ms: 1.04x faster                                                          |
| xml_etree_parse            | 113 ms                                                          | 109 ms: 1.04x faster                                                          |
| bench_mp_pool              | 75.4 ms                                                         | 73.1 ms: 1.03x faster                                                         |
| json_loads                 | 20.4 us                                                         | 19.8 us: 1.03x faster                                                         |
| fannkuch                   | 354 ms                                                          | 345 ms: 1.02x faster                                                          |
| gc_traversal               | 1.44 ms                                                         | 1.41 ms: 1.02x faster                                                         |
| scimark_monte_carlo        | 66.4 ms                                                         | 65.1 ms: 1.02x faster                                                         |
| meteor_contest             | 86.9 ms                                                         | 85.9 ms: 1.01x faster                                                         |
| pidigits                   | 199 ms                                                          | 198 ms: 1.01x faster                                                          |
| pickle_dict                | 19.9 us                                                         | 19.9 us: 1.00x faster                                                         |
| pprint_pformat             | 1.50 sec                                                        | 1.51 sec: 1.01x slower                                                        |
| nqueens                    | 93.7 ms                                                         | 94.5 ms: 1.01x slower                                                         |
| pickle                     | 7.79 us                                                         | 7.89 us: 1.01x slower                                                         |
| json                       | 4.15 ms                                                         | 4.24 ms: 1.02x slower                                                         |
| unpickle                   | 9.71 us                                                         | 10.0 us: 1.03x slower                                                         |
| pprint_safe_repr           | 721 ms                                                          | 744 ms: 1.03x slower                                                          |
| regex_v8                   | 15.0 ms                                                         | 16.1 ms: 1.07x slower                                                         |
| python_startup             | 22.4 ms                                                         | 25.7 ms: 1.15x slower                                                         |
| telco                      | 5.51 ms                                                         | 6.35 ms: 1.15x slower                                                         |
| python_startup_no_site     | 19.1 ms                                                         | 23.6 ms: 1.24x slower                                                         |
| dask                       | 323 ms                                                          | 419 ms: 1.30x slower                                                          |
| sqlglot_normalize          | 100 ms                                                          | 221 ms: 2.20x slower                                                          |
| coverage                   | 48.4 ms                                                         | 484 ms: 10.00x slower                                                         |
| Geometric mean             | (ref)                                                           | 1.10x faster                                                                  |

Benchmark hidden because not significant (2): asyncio_tcp, create_gc_cycles
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1_win32-x86-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dulwich_log, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240229-3.13.0a4+-1a78317-JIT/bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.07x


# Memory

- memory change: unknown