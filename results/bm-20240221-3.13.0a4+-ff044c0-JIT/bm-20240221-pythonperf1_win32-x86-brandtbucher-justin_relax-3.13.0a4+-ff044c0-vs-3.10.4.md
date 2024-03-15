
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_relax
- machine: windows-x86
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.07x faster \*
- HPT reliability: 99.97%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 262 ms: 1.01x faster                                                          |
| chameleon      | 6.42 ms                                                         | 5.99 ms: 1.07x faster                                                         |
| docutils       | 1.95 sec                                                        | 1.85 sec: 1.05x faster                                                        |
| tornado_http   | 118 ms                                                          | 97.8 ms: 1.20x faster                                                         |
| Geometric mean | (ref)                                                           | 1.08x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 511 ms: 1.81x faster                                                          |
| async_tree_none         | 394 ms                                                          | 259 ms: 1.52x faster                                                          |
| async_tree_io           | 940 ms                                                          | 621 ms: 1.51x faster                                                          |
| async_tree_memoization  | 467 ms                                                          | 323 ms: 1.44x faster                                                          |
| Geometric mean          | (ref)                                                           | 1.57x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 199 ms: 2.53x faster                                                          |
| float          | 69.6 ms                                                         | 55.1 ms: 1.26x faster                                                         |
| nbody          | 79.1 ms                                                         | 94.5 ms: 1.19x slower                                                         |
| Geometric mean | (ref)                                                           | 1.39x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 118 ms: 1.11x faster                                                          |
| regex_v8       | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                         |
| regex_effbot   | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                         |
| Geometric mean | (ref)                                                           | 1.01x slower                                                                  |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.90 ms: 1.42x faster                                                         |
| pickle_pure_python   | 280 us                                                          | 228 us: 1.23x faster                                                          |
| xml_etree_process    | 48.1 ms                                                         | 42.7 ms: 1.13x faster                                                         |
| tomli_loads          | 1.91 sec                                                        | 1.71 sec: 1.12x faster                                                        |
| json_loads           | 22.4 us                                                         | 20.1 us: 1.12x faster                                                         |
| xml_etree_parse      | 120 ms                                                          | 108 ms: 1.11x faster                                                          |
| xml_etree_iterparse  | 70.8 ms                                                         | 67.0 ms: 1.06x faster                                                         |
| unpickle_list        | 2.98 us                                                         | 2.85 us: 1.05x faster                                                         |
| unpickle_pure_python | 189 us                                                          | 181 us: 1.04x faster                                                          |
| xml_etree_generate   | 61.6 ms                                                         | 60.5 ms: 1.02x faster                                                         |
| pickle_list          | 3.22 us                                                         | 3.25 us: 1.01x slower                                                         |
| pickle               | 7.83 us                                                         | 7.92 us: 1.01x slower                                                         |
| unpickle             | 9.82 us                                                         | 10.0 us: 1.02x slower                                                         |
| pickle_dict          | 18.2 us                                                         | 19.8 us: 1.09x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.08x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 26.3 ms: 1.15x slower                                                         |
| python_startup_no_site | 18.1 ms                                                         | 23.8 ms: 1.32x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.23x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.25 ms: 1.26x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|--------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 99.3 us: 3.99x faster                                                         |
| pidigits                 | 502 ms                                                          | 199 ms: 2.53x faster                                                          |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 511 ms: 1.81x faster                                                          |
| async_tree_none          | 394 ms                                                          | 259 ms: 1.52x faster                                                          |
| async_tree_io            | 940 ms                                                          | 621 ms: 1.51x faster                                                          |
| deltablue                | 4.04 ms                                                         | 2.74 ms: 1.47x faster                                                         |
| async_tree_memoization   | 467 ms                                                          | 323 ms: 1.44x faster                                                          |
| json_dumps               | 9.82 ms                                                         | 6.90 ms: 1.42x faster                                                         |
| logging_silent           | 97.9 ns                                                         | 69.0 ns: 1.42x faster                                                         |
| crypto_pyaes             | 81.3 ms                                                         | 60.8 ms: 1.34x faster                                                         |
| sqlglot_parse            | 1.33 ms                                                         | 1.01 ms: 1.32x faster                                                         |
| chaos                    | 74.4 ms                                                         | 57.3 ms: 1.30x faster                                                         |
| generators               | 31.6 ms                                                         | 24.6 ms: 1.29x faster                                                         |
| float                    | 69.6 ms                                                         | 55.1 ms: 1.26x faster                                                         |
| mako                     | 9.10 ms                                                         | 7.25 ms: 1.26x faster                                                         |
| sqlglot_transpile        | 1.58 ms                                                         | 1.28 ms: 1.24x faster                                                         |
| pickle_pure_python       | 280 us                                                          | 228 us: 1.23x faster                                                          |
| comprehensions           | 17.7 us                                                         | 14.7 us: 1.21x faster                                                         |
| tornado_http             | 118 ms                                                          | 97.8 ms: 1.20x faster                                                         |
| pycparser                | 1.04 sec                                                        | 869 ms: 1.20x faster                                                          |
| asyncio_tcp              | 744 ms                                                          | 624 ms: 1.19x faster                                                          |
| go                       | 146 ms                                                          | 123 ms: 1.18x faster                                                          |
| coroutines               | 17.9 ms                                                         | 15.3 ms: 1.17x faster                                                         |
| sqlite_synth             | 2.29 us                                                         | 1.97 us: 1.16x faster                                                         |
| raytrace                 | 303 ms                                                          | 263 ms: 1.15x faster                                                          |
| richards_super           | 49.9 ms                                                         | 43.7 ms: 1.14x faster                                                         |
| spectral_norm            | 80.2 ms                                                         | 70.7 ms: 1.13x faster                                                         |
| xml_etree_process        | 48.1 ms                                                         | 42.7 ms: 1.13x faster                                                         |
| sympy_sum                | 122 ms                                                          | 109 ms: 1.12x faster                                                          |
| tomli_loads              | 1.91 sec                                                        | 1.71 sec: 1.12x faster                                                        |
| json_loads               | 22.4 us                                                         | 20.1 us: 1.12x faster                                                         |
| json                     | 4.76 ms                                                         | 4.28 ms: 1.11x faster                                                         |
| regex_dna                | 131 ms                                                          | 118 ms: 1.11x faster                                                          |
| xml_etree_parse          | 120 ms                                                          | 108 ms: 1.11x faster                                                          |
| pyflate                  | 422 ms                                                          | 384 ms: 1.10x faster                                                          |
| deepcopy_memo            | 29.6 us                                                         | 27.4 us: 1.08x faster                                                         |
| scimark_sor              | 115 ms                                                          | 107 ms: 1.08x faster                                                          |
| chameleon                | 6.42 ms                                                         | 5.99 ms: 1.07x faster                                                         |
| bench_thread_pool        | 1.12 ms                                                         | 1.05 ms: 1.06x faster                                                         |
| create_gc_cycles         | 694 us                                                          | 656 us: 1.06x faster                                                          |
| xml_etree_iterparse      | 70.8 ms                                                         | 67.0 ms: 1.06x faster                                                         |
| docutils                 | 1.95 sec                                                        | 1.85 sec: 1.05x faster                                                        |
| sympy_str                | 229 ms                                                          | 218 ms: 1.05x faster                                                          |
| mdp                      | 1.83 sec                                                        | 1.74 sec: 1.05x faster                                                        |
| unpickle_list            | 2.98 us                                                         | 2.85 us: 1.05x faster                                                         |
| scimark_lu               | 89.8 ms                                                         | 85.7 ms: 1.05x faster                                                         |
| unpickle_pure_python     | 189 us                                                          | 181 us: 1.04x faster                                                          |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.11 ms: 1.04x faster                                                         |
| deepcopy                 | 310 us                                                          | 298 us: 1.04x faster                                                          |
| sympy_integrate          | 16.6 ms                                                         | 16.0 ms: 1.04x faster                                                         |
| deepcopy_reduce          | 2.68 us                                                         | 2.59 us: 1.03x faster                                                         |
| richards                 | 40.3 ms                                                         | 39.1 ms: 1.03x faster                                                         |
| xml_etree_generate       | 61.6 ms                                                         | 60.5 ms: 1.02x faster                                                         |
| sympy_expand             | 391 ms                                                          | 384 ms: 1.02x faster                                                          |
| sqlglot_normalize        | 230 ms                                                          | 227 ms: 1.01x faster                                                          |
| 2to3                     | 265 ms                                                          | 262 ms: 1.01x faster                                                          |
| pickle_list              | 3.22 us                                                         | 3.25 us: 1.01x slower                                                         |
| pickle                   | 7.83 us                                                         | 7.92 us: 1.01x slower                                                         |
| regex_v8                 | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                         |
| unpickle                 | 9.82 us                                                         | 10.0 us: 1.02x slower                                                         |
| meteor_contest           | 80.0 ms                                                         | 82.1 ms: 1.03x slower                                                         |
| sqlglot_optimize         | 44.7 ms                                                         | 46.0 ms: 1.03x slower                                                         |
| fannkuch                 | 317 ms                                                          | 330 ms: 1.04x slower                                                          |
| pathlib                  | 81.2 ms                                                         | 84.9 ms: 1.05x slower                                                         |
| nqueens                  | 87.1 ms                                                         | 91.3 ms: 1.05x slower                                                         |
| hexiom                   | 6.13 ms                                                         | 6.47 ms: 1.06x slower                                                         |
| scimark_monte_carlo      | 61.9 ms                                                         | 65.5 ms: 1.06x slower                                                         |
| pprint_pformat           | 1.37 sec                                                        | 1.46 sec: 1.07x slower                                                        |
| gc_traversal             | 1.28 ms                                                         | 1.38 ms: 1.08x slower                                                         |
| pickle_dict              | 18.2 us                                                         | 19.8 us: 1.09x slower                                                         |
| pprint_safe_repr         | 658 ms                                                          | 719 ms: 1.09x slower                                                          |
| scimark_fft              | 216 ms                                                          | 237 ms: 1.10x slower                                                          |
| bench_mp_pool            | 66.4 ms                                                         | 74.8 ms: 1.13x slower                                                         |
| regex_effbot             | 1.66 ms                                                         | 1.90 ms: 1.14x slower                                                         |
| python_startup           | 22.9 ms                                                         | 26.3 ms: 1.15x slower                                                         |
| logging_format           | 7.91 us                                                         | 9.08 us: 1.15x slower                                                         |
| logging_simple           | 7.29 us                                                         | 8.50 us: 1.17x slower                                                         |
| nbody                    | 79.1 ms                                                         | 94.5 ms: 1.19x slower                                                         |
| async_generators         | 241 ms                                                          | 294 ms: 1.22x slower                                                          |
| python_startup_no_site   | 18.1 ms                                                         | 23.8 ms: 1.32x slower                                                         |
| telco                    | 4.83 ms                                                         | 6.46 ms: 1.34x slower                                                         |
| unpack_sequence          | 40.0 ns                                                         | 64.6 ns: 1.61x slower                                                         |
| coverage                 | 46.6 ms                                                         | 478 ms: 10.26x slower                                                         |
| Geometric mean           | (ref)                                                           | 1.07x faster                                                                  |

Benchmark hidden because not significant (2): asyncio_tcp_ssl, regex_compile
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240221-3.13.0a4+-ff044c0-JIT/bm-20240221-pythonperf1_win32-x86-brandtbucher-justin_relax-3.13.0a4+-ff044c0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.97% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown