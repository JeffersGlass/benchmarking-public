
# Results vs. 3.10.4

- fork: python
- ref: f428c4dafbfa2425ea05
- machine: windows-x86
- commit hash: f428c4d
- commit date: 2023-12-18
- overall geometric mean: 1.14x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 239 ms: 1.11x faster                                                            |
| chameleon      | 6.42 ms                                                         | 5.78 ms: 1.11x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.76 sec: 1.11x faster                                                          |
| tornado_http   | 118 ms                                                          | 99.1 ms: 1.19x faster                                                           |
| Geometric mean | (ref)                                                           | 1.13x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 496 ms: 1.86x faster                                                            |
| async_tree_none         | 394 ms                                                          | 247 ms: 1.59x faster                                                            |
| async_tree_io           | 940 ms                                                          | 595 ms: 1.58x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 306 ms: 1.53x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.63x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.54x faster                                                            |
| float          | 69.6 ms                                                         | 59.4 ms: 1.17x faster                                                           |
| nbody          | 79.1 ms                                                         | 84.9 ms: 1.07x slower                                                           |
| Geometric mean | (ref)                                                           | 1.41x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_compile  | 117 ms                                                          | 105 ms: 1.11x faster                                                            |
| regex_dna      | 131 ms                                                          | 121 ms: 1.08x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.3 ms: 1.04x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                           |
| Geometric mean | (ref)                                                           | 1.00x slower                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.62 ms: 1.48x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 209 us: 1.34x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 153 us: 1.24x faster                                                            |
| xml_etree_process    | 48.1 ms                                                         | 41.6 ms: 1.16x faster                                                           |
| tomli_loads          | 1.91 sec                                                        | 1.67 sec: 1.14x faster                                                          |
| json_loads           | 22.4 us                                                         | 20.0 us: 1.12x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                                            |
| unpickle             | 9.82 us                                                         | 9.46 us: 1.04x faster                                                           |
| xml_etree_iterparse  | 70.8 ms                                                         | 68.5 ms: 1.03x faster                                                           |
| pickle               | 7.83 us                                                         | 7.65 us: 1.02x faster                                                           |
| unpickle_list        | 2.98 us                                                         | 2.94 us: 1.02x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 60.7 ms: 1.02x faster                                                           |
| pickle_list          | 3.22 us                                                         | 3.25 us: 1.01x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 19.9 us: 1.09x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.11x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 22.7 ms: 1.01x faster                                                           |
| python_startup_no_site | 18.1 ms                                                         | 20.2 ms: 1.12x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.05x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 8.06 ms: 1.13x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 89.7 us: 4.41x faster                                                           |
| pidigits                 | 502 ms                                                          | 198 ms: 2.54x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 496 ms: 1.86x faster                                                            |
| logging_silent           | 97.9 ns                                                         | 59.7 ns: 1.64x faster                                                           |
| async_tree_none          | 394 ms                                                          | 247 ms: 1.59x faster                                                            |
| async_tree_io            | 940 ms                                                          | 595 ms: 1.58x faster                                                            |
| async_tree_memoization   | 467 ms                                                          | 306 ms: 1.53x faster                                                            |
| richards_super           | 49.9 ms                                                         | 32.9 ms: 1.52x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.62 ms: 1.48x faster                                                           |
| scimark_lu               | 89.8 ms                                                         | 60.6 ms: 1.48x faster                                                           |
| raytrace                 | 303 ms                                                          | 206 ms: 1.47x faster                                                            |
| sqlglot_parse            | 1.33 ms                                                         | 919 us: 1.45x faster                                                            |
| crypto_pyaes             | 81.3 ms                                                         | 56.7 ms: 1.43x faster                                                           |
| generators               | 31.6 ms                                                         | 22.0 ms: 1.43x faster                                                           |
| deltablue                | 4.04 ms                                                         | 2.83 ms: 1.42x faster                                                           |
| chaos                    | 74.4 ms                                                         | 52.5 ms: 1.42x faster                                                           |
| go                       | 146 ms                                                          | 104 ms: 1.40x faster                                                            |
| scimark_sor              | 115 ms                                                          | 82.9 ms: 1.39x faster                                                           |
| richards                 | 40.3 ms                                                         | 29.2 ms: 1.38x faster                                                           |
| sqlglot_transpile        | 1.58 ms                                                         | 1.15 ms: 1.37x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 209 us: 1.34x faster                                                            |
| comprehensions           | 17.7 us                                                         | 13.7 us: 1.29x faster                                                           |
| sqlite_synth             | 2.29 us                                                         | 1.79 us: 1.28x faster                                                           |
| pycparser                | 1.04 sec                                                        | 821 ms: 1.27x faster                                                            |
| pyflate                  | 422 ms                                                          | 338 ms: 1.25x faster                                                            |
| unpickle_pure_python     | 189 us                                                          | 153 us: 1.24x faster                                                            |
| coroutines               | 17.9 ms                                                         | 14.8 ms: 1.21x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 619 ms: 1.20x faster                                                            |
| deepcopy_memo            | 29.6 us                                                         | 24.7 us: 1.20x faster                                                           |
| tornado_http             | 118 ms                                                          | 99.1 ms: 1.19x faster                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 52.8 ms: 1.17x faster                                                           |
| float                    | 69.6 ms                                                         | 59.4 ms: 1.17x faster                                                           |
| sympy_sum                | 122 ms                                                          | 105 ms: 1.17x faster                                                            |
| xml_etree_process        | 48.1 ms                                                         | 41.6 ms: 1.16x faster                                                           |
| json                     | 4.76 ms                                                         | 4.17 ms: 1.14x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.67 sec: 1.14x faster                                                          |
| deepcopy                 | 310 us                                                          | 272 us: 1.14x faster                                                            |
| dask                     | 341 ms                                                          | 300 ms: 1.14x faster                                                            |
| hexiom                   | 6.13 ms                                                         | 5.41 ms: 1.13x faster                                                           |
| mako                     | 9.10 ms                                                         | 8.06 ms: 1.13x faster                                                           |
| json_loads               | 22.4 us                                                         | 20.0 us: 1.12x faster                                                           |
| sqlglot_normalize        | 230 ms                                                          | 206 ms: 1.12x faster                                                            |
| deepcopy_reduce          | 2.68 us                                                         | 2.40 us: 1.12x faster                                                           |
| sympy_str                | 229 ms                                                          | 206 ms: 1.11x faster                                                            |
| chameleon                | 6.42 ms                                                         | 5.78 ms: 1.11x faster                                                           |
| 2to3                     | 265 ms                                                          | 239 ms: 1.11x faster                                                            |
| docutils                 | 1.95 sec                                                        | 1.76 sec: 1.11x faster                                                          |
| regex_compile            | 117 ms                                                          | 105 ms: 1.11x faster                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 40.5 ms: 1.10x faster                                                           |
| sympy_expand             | 391 ms                                                          | 355 ms: 1.10x faster                                                            |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                                            |
| sympy_integrate          | 16.6 ms                                                         | 15.2 ms: 1.10x faster                                                           |
| pprint_pformat           | 1.37 sec                                                        | 1.26 sec: 1.09x faster                                                          |
| regex_dna                | 131 ms                                                          | 121 ms: 1.08x faster                                                            |
| pprint_safe_repr         | 658 ms                                                          | 611 ms: 1.08x faster                                                            |
| mdp                      | 1.83 sec                                                        | 1.70 sec: 1.08x faster                                                          |
| nqueens                  | 87.1 ms                                                         | 81.1 ms: 1.07x faster                                                           |
| create_gc_cycles         | 694 us                                                          | 646 us: 1.07x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.07 ms: 1.05x faster                                                           |
| unpickle                 | 9.82 us                                                         | 9.46 us: 1.04x faster                                                           |
| fannkuch                 | 317 ms                                                          | 307 ms: 1.03x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 68.5 ms: 1.03x faster                                                           |
| pickle                   | 7.83 us                                                         | 7.65 us: 1.02x faster                                                           |
| unpickle_list            | 2.98 us                                                         | 2.94 us: 1.02x faster                                                           |
| xml_etree_generate       | 61.6 ms                                                         | 60.7 ms: 1.02x faster                                                           |
| python_startup           | 22.9 ms                                                         | 22.7 ms: 1.01x faster                                                           |
| pickle_list              | 3.22 us                                                         | 3.25 us: 1.01x slower                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 17.3 sec: 1.02x slower                                                          |
| unpack_sequence          | 40.0 ns                                                         | 41.1 ns: 1.03x slower                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.33 ms: 1.03x slower                                                           |
| scimark_fft              | 216 ms                                                          | 223 ms: 1.03x slower                                                            |
| regex_v8                 | 15.8 ms                                                         | 16.3 ms: 1.04x slower                                                           |
| nbody                    | 79.1 ms                                                         | 84.9 ms: 1.07x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 87.6 ms: 1.08x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.54 us: 1.08x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 71.9 ms: 1.08x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 19.9 us: 1.09x slower                                                           |
| logging_simple           | 7.29 us                                                         | 7.95 us: 1.09x slower                                                           |
| async_generators         | 241 ms                                                          | 265 ms: 1.10x slower                                                            |
| gc_traversal             | 1.28 ms                                                         | 1.42 ms: 1.11x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 20.2 ms: 1.12x slower                                                           |
| spectral_norm            | 80.2 ms                                                         | 90.0 ms: 1.12x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.91 ms: 1.15x slower                                                           |
| telco                    | 4.83 ms                                                         | 5.98 ms: 1.24x slower                                                           |
| coverage                 | 46.6 ms                                                         | 479 ms: 10.30x slower                                                           |
| Geometric mean           | (ref)                                                           | 1.14x faster                                                                    |

Benchmark hidden because not significant (1): meteor_contest
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231218-3.13.0a2+-f428c4d-PYTHON_UOPS/bm-20231218-pythonperf1_win32-x86-python-f428c4dafbfa2425ea05-3.13.0a2+-f428c4d.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.10x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown