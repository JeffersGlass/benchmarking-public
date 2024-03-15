# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_jumps
- machine: windows-x86
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.07x faster \*
- HPT reliability: 99.91%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| chameleon      | 6.42 ms                                                         | 5.90 ms: 1.09x faster                                                         |
| docutils       | 1.95 sec                                                        | 1.89 sec: 1.03x faster                                                        |
| tornado_http   | 118 ms                                                          | 99.4 ms: 1.18x faster                                                         |
| Geometric mean | (ref)                                                           | 1.07x faster                                                                  |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 556 ms: 1.66x faster                                                          |
| async_tree_io           | 940 ms                                                          | 637 ms: 1.48x faster                                                          |
| async_tree_none         | 394 ms                                                          | 268 ms: 1.47x faster                                                          |
| async_tree_memoization  | 467 ms                                                          | 332 ms: 1.40x faster                                                          |
| Geometric mean          | (ref)                                                           | 1.50x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 200 ms: 2.51x faster                                                          |
| float          | 69.6 ms                                                         | 55.2 ms: 1.26x faster                                                         |
| nbody          | 79.1 ms                                                         | 97.7 ms: 1.23x slower                                                         |
| Geometric mean | (ref)                                                           | 1.37x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 119 ms: 1.10x faster                                                          |
| regex_compile  | 117 ms                                                          | 114 ms: 1.03x faster                                                          |
| regex_v8       | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                         |
| regex_effbot   | 1.66 ms                                                         | 1.89 ms: 1.13x slower                                                         |
| Geometric mean | (ref)                                                           | 1.01x slower                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 7.16 ms: 1.37x faster                                                         |
| pickle_pure_python   | 280 us                                                          | 227 us: 1.24x faster                                                          |
| xml_etree_parse      | 120 ms                                                          | 108 ms: 1.11x faster                                                          |
| json_loads           | 22.4 us                                                         | 20.4 us: 1.10x faster                                                         |
| tomli_loads          | 1.91 sec                                                        | 1.75 sec: 1.09x faster                                                        |
| unpickle_pure_python | 189 us                                                          | 174 us: 1.09x faster                                                          |
| xml_etree_process    | 48.1 ms                                                         | 44.3 ms: 1.09x faster                                                         |
| unpickle_list        | 2.98 us                                                         | 2.79 us: 1.07x faster                                                         |
| xml_etree_iterparse  | 70.8 ms                                                         | 66.9 ms: 1.06x faster                                                         |
| pickle               | 7.83 us                                                         | 7.91 us: 1.01x slower                                                         |
| unpickle             | 9.82 us                                                         | 10.0 us: 1.02x slower                                                         |
| pickle_list          | 3.22 us                                                         | 3.29 us: 1.02x slower                                                         |
| xml_etree_generate   | 61.6 ms                                                         | 63.8 ms: 1.04x slower                                                         |
| pickle_dict          | 18.2 us                                                         | 20.1 us: 1.10x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.07x faster                                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 26.0 ms: 1.13x slower                                                         |
| python_startup_no_site | 18.1 ms                                                         | 23.7 ms: 1.31x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.22x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.24 ms: 1.26x faster                                                         |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|--------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 97.1 us: 4.07x faster                                                         |
| pidigits                 | 502 ms                                                          | 200 ms: 2.51x faster                                                          |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 556 ms: 1.66x faster                                                          |
| async_tree_io            | 940 ms                                                          | 637 ms: 1.48x faster                                                          |
| deltablue                | 4.04 ms                                                         | 2.74 ms: 1.47x faster                                                         |
| async_tree_none          | 394 ms                                                          | 268 ms: 1.47x faster                                                          |
| async_tree_memoization   | 467 ms                                                          | 332 ms: 1.40x faster                                                          |
| logging_silent           | 97.9 ns                                                         | 70.3 ns: 1.39x faster                                                         |
| json_dumps               | 9.82 ms                                                         | 7.16 ms: 1.37x faster                                                         |
| crypto_pyaes             | 81.3 ms                                                         | 61.1 ms: 1.33x faster                                                         |
| sqlglot_parse            | 1.33 ms                                                         | 1.04 ms: 1.28x faster                                                         |
| chaos                    | 74.4 ms                                                         | 58.9 ms: 1.26x faster                                                         |
| float                    | 69.6 ms                                                         | 55.2 ms: 1.26x faster                                                         |
| generators               | 31.6 ms                                                         | 25.0 ms: 1.26x faster                                                         |
| mako                     | 9.10 ms                                                         | 7.24 ms: 1.26x faster                                                         |
| pickle_pure_python       | 280 us                                                          | 227 us: 1.24x faster                                                          |
| sqlite_synth             | 2.29 us                                                         | 1.86 us: 1.23x faster                                                         |
| sqlglot_transpile        | 1.58 ms                                                         | 1.31 ms: 1.21x faster                                                         |
| richards_super           | 49.9 ms                                                         | 41.7 ms: 1.20x faster                                                         |
| pycparser                | 1.04 sec                                                        | 878 ms: 1.19x faster                                                          |
| coroutines               | 17.9 ms                                                         | 15.1 ms: 1.19x faster                                                         |
| tornado_http             | 118 ms                                                          | 99.4 ms: 1.18x faster                                                         |
| asyncio_tcp              | 744 ms                                                          | 632 ms: 1.18x faster                                                          |
| comprehensions           | 17.7 us                                                         | 15.3 us: 1.16x faster                                                         |
| json                     | 4.76 ms                                                         | 4.13 ms: 1.15x faster                                                         |
| go                       | 146 ms                                                          | 128 ms: 1.14x faster                                                          |
| sympy_sum                | 122 ms                                                          | 109 ms: 1.13x faster                                                          |
| xml_etree_parse          | 120 ms                                                          | 108 ms: 1.11x faster                                                          |
| regex_dna                | 131 ms                                                          | 119 ms: 1.10x faster                                                          |
| json_loads               | 22.4 us                                                         | 20.4 us: 1.10x faster                                                         |
| spectral_norm            | 80.2 ms                                                         | 73.3 ms: 1.09x faster                                                         |
| tomli_loads              | 1.91 sec                                                        | 1.75 sec: 1.09x faster                                                        |
| raytrace                 | 303 ms                                                          | 277 ms: 1.09x faster                                                          |
| chameleon                | 6.42 ms                                                         | 5.90 ms: 1.09x faster                                                         |
| unpickle_pure_python     | 189 us                                                          | 174 us: 1.09x faster                                                          |
| pyflate                  | 422 ms                                                          | 388 ms: 1.09x faster                                                          |
| xml_etree_process        | 48.1 ms                                                         | 44.3 ms: 1.09x faster                                                         |
| richards                 | 40.3 ms                                                         | 37.1 ms: 1.09x faster                                                         |
| sympy_str                | 229 ms                                                          | 213 ms: 1.07x faster                                                          |
| unpickle_list            | 2.98 us                                                         | 2.79 us: 1.07x faster                                                         |
| scimark_sor              | 115 ms                                                          | 108 ms: 1.07x faster                                                          |
| create_gc_cycles         | 694 us                                                          | 653 us: 1.06x faster                                                          |
| deepcopy_memo            | 29.6 us                                                         | 27.9 us: 1.06x faster                                                         |
| xml_etree_iterparse      | 70.8 ms                                                         | 66.9 ms: 1.06x faster                                                         |
| deepcopy                 | 310 us                                                          | 294 us: 1.06x faster                                                          |
| bench_thread_pool        | 1.12 ms                                                         | 1.06 ms: 1.05x faster                                                         |
| sympy_expand             | 391 ms                                                          | 372 ms: 1.05x faster                                                          |
| sympy_integrate          | 16.6 ms                                                         | 15.9 ms: 1.05x faster                                                         |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.11 ms: 1.04x faster                                                         |
| docutils                 | 1.95 sec                                                        | 1.89 sec: 1.03x faster                                                        |
| scimark_lu               | 89.8 ms                                                         | 87.2 ms: 1.03x faster                                                         |
| deepcopy_reduce          | 2.68 us                                                         | 2.61 us: 1.03x faster                                                         |
| regex_compile            | 117 ms                                                          | 114 ms: 1.03x faster                                                          |
| mdp                      | 1.83 sec                                                        | 1.80 sec: 1.02x faster                                                        |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                                        |
| pickle                   | 7.83 us                                                         | 7.91 us: 1.01x slower                                                         |
| regex_v8                 | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                         |
| unpickle                 | 9.82 us                                                         | 10.0 us: 1.02x slower                                                         |
| sqlglot_normalize        | 230 ms                                                          | 235 ms: 1.02x slower                                                          |
| pickle_list              | 3.22 us                                                         | 3.29 us: 1.02x slower                                                         |
| hexiom                   | 6.13 ms                                                         | 6.32 ms: 1.03x slower                                                         |
| xml_etree_generate       | 61.6 ms                                                         | 63.8 ms: 1.04x slower                                                         |
| pathlib                  | 81.2 ms                                                         | 84.6 ms: 1.04x slower                                                         |
| meteor_contest           | 80.0 ms                                                         | 83.5 ms: 1.04x slower                                                         |
| fannkuch                 | 317 ms                                                          | 332 ms: 1.05x slower                                                          |
| nqueens                  | 87.1 ms                                                         | 91.7 ms: 1.05x slower                                                         |
| sqlglot_optimize         | 44.7 ms                                                         | 47.4 ms: 1.06x slower                                                         |
| scimark_monte_carlo      | 61.9 ms                                                         | 65.7 ms: 1.06x slower                                                         |
| unpack_sequence          | 40.0 ns                                                         | 43.7 ns: 1.09x slower                                                         |
| gc_traversal             | 1.28 ms                                                         | 1.40 ms: 1.09x slower                                                         |
| pprint_pformat           | 1.37 sec                                                        | 1.50 sec: 1.10x slower                                                        |
| pickle_dict              | 18.2 us                                                         | 20.1 us: 1.10x slower                                                         |
| scimark_fft              | 216 ms                                                          | 239 ms: 1.10x slower                                                          |
| pprint_safe_repr         | 658 ms                                                          | 735 ms: 1.12x slower                                                          |
| logging_format           | 7.91 us                                                         | 8.87 us: 1.12x slower                                                         |
| bench_mp_pool            | 66.4 ms                                                         | 74.5 ms: 1.12x slower                                                         |
| regex_effbot             | 1.66 ms                                                         | 1.89 ms: 1.13x slower                                                         |
| python_startup           | 22.9 ms                                                         | 26.0 ms: 1.13x slower                                                         |
| logging_simple           | 7.29 us                                                         | 8.33 us: 1.14x slower                                                         |
| nbody                    | 79.1 ms                                                         | 97.7 ms: 1.23x slower                                                         |
| telco                    | 4.83 ms                                                         | 6.18 ms: 1.28x slower                                                         |
| async_generators         | 241 ms                                                          | 316 ms: 1.31x slower                                                          |
| python_startup_no_site   | 18.1 ms                                                         | 23.7 ms: 1.31x slower                                                         |
| coverage                 | 46.6 ms                                                         | 330 ms: 7.08x slower                                                          |
| Geometric mean           | (ref)                                                           | 1.07x faster                                                                  |

Benchmark hidden because not significant (1): 2to3
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-594cca3-JIT/bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_jumps-3.13.0a4+-594cca3.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.91% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown