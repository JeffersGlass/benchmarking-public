
# Results vs. 3.10.4

- fork: python
- ref: 4297d7301b97aba2e0df
- machine: windows-x86
- commit hash: 4297d73
- commit date: 2024-02-12
- overall geometric mean: 1.12x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 246 ms: 1.08x faster                                                            |
| chameleon      | 6.42 ms                                                         | 6.02 ms: 1.07x faster                                                           |
| docutils       | 1.95 sec                                                        | 1.78 sec: 1.09x faster                                                          |
| tornado_http   | 118 ms                                                          | 95.7 ms: 1.23x faster                                                           |
| Geometric mean | (ref)                                                           | 1.12x faster                                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 510 ms: 1.81x faster                                                            |
| async_tree_io           | 940 ms                                                          | 597 ms: 1.58x faster                                                            |
| async_tree_none         | 394 ms                                                          | 250 ms: 1.57x faster                                                            |
| async_tree_memoization  | 467 ms                                                          | 311 ms: 1.50x faster                                                            |
| Geometric mean          | (ref)                                                           | 1.61x faster                                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 203 ms: 2.48x faster                                                            |
| float          | 69.6 ms                                                         | 53.8 ms: 1.29x faster                                                           |
| nbody          | 79.1 ms                                                         | 90.6 ms: 1.15x slower                                                           |
| Geometric mean | (ref)                                                           | 1.41x faster                                                                    |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 117 ms: 1.12x faster                                                            |
| regex_compile  | 117 ms                                                          | 105 ms: 1.11x faster                                                            |
| regex_v8       | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                           |
| regex_effbot   | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                           |
| Geometric mean | (ref)                                                           | 1.02x faster                                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.71 ms: 1.46x faster                                                           |
| pickle_pure_python   | 280 us                                                          | 205 us: 1.37x faster                                                            |
| unpickle_pure_python | 189 us                                                          | 150 us: 1.27x faster                                                            |
| tomli_loads          | 1.91 sec                                                        | 1.59 sec: 1.20x faster                                                          |
| xml_etree_process    | 48.1 ms                                                         | 41.4 ms: 1.16x faster                                                           |
| xml_etree_parse      | 120 ms                                                          | 104 ms: 1.16x faster                                                            |
| json_loads           | 22.4 us                                                         | 20.0 us: 1.12x faster                                                           |
| xml_etree_iterparse  | 70.8 ms                                                         | 65.5 ms: 1.08x faster                                                           |
| xml_etree_generate   | 61.6 ms                                                         | 60.4 ms: 1.02x faster                                                           |
| unpickle             | 9.82 us                                                         | 10.2 us: 1.04x slower                                                           |
| pickle               | 7.83 us                                                         | 8.13 us: 1.04x slower                                                           |
| unpickle_list        | 2.98 us                                                         | 3.10 us: 1.04x slower                                                           |
| pickle_dict          | 18.2 us                                                         | 19.8 us: 1.08x slower                                                           |
| pickle_list          | 3.22 us                                                         | 3.66 us: 1.14x slower                                                           |
| Geometric mean       | (ref)                                                           | 1.10x faster                                                                    |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 22.3 ms: 1.03x faster                                                           |
| python_startup_no_site | 18.1 ms                                                         | 20.1 ms: 1.11x slower                                                           |
| Geometric mean         | (ref)                                                           | 1.04x slower                                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-----------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| mako      | 9.10 ms                                                         | 7.64 ms: 1.19x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|--------------------------|:---------------------------------------------------------------:|:-------------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 93.8 us: 4.22x faster                                                           |
| pidigits                 | 502 ms                                                          | 203 ms: 2.48x faster                                                            |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 510 ms: 1.81x faster                                                            |
| deltablue                | 4.04 ms                                                         | 2.38 ms: 1.70x faster                                                           |
| logging_silent           | 97.9 ns                                                         | 60.5 ns: 1.62x faster                                                           |
| async_tree_io            | 940 ms                                                          | 597 ms: 1.58x faster                                                            |
| async_tree_none          | 394 ms                                                          | 250 ms: 1.57x faster                                                            |
| richards_super           | 49.9 ms                                                         | 32.3 ms: 1.55x faster                                                           |
| async_tree_memoization   | 467 ms                                                          | 311 ms: 1.50x faster                                                            |
| scimark_lu               | 89.8 ms                                                         | 60.1 ms: 1.49x faster                                                           |
| json_dumps               | 9.82 ms                                                         | 6.71 ms: 1.46x faster                                                           |
| scimark_sor              | 115 ms                                                          | 79.9 ms: 1.44x faster                                                           |
| sqlglot_parse            | 1.33 ms                                                         | 932 us: 1.43x faster                                                            |
| richards                 | 40.3 ms                                                         | 28.4 ms: 1.42x faster                                                           |
| generators               | 31.6 ms                                                         | 22.4 ms: 1.41x faster                                                           |
| pickle_pure_python       | 280 us                                                          | 205 us: 1.37x faster                                                            |
| sqlglot_transpile        | 1.58 ms                                                         | 1.18 ms: 1.35x faster                                                           |
| crypto_pyaes             | 81.3 ms                                                         | 60.4 ms: 1.35x faster                                                           |
| raytrace                 | 303 ms                                                          | 228 ms: 1.32x faster                                                            |
| deepcopy_memo            | 29.6 us                                                         | 22.7 us: 1.30x faster                                                           |
| float                    | 69.6 ms                                                         | 53.8 ms: 1.29x faster                                                           |
| unpickle_pure_python     | 189 us                                                          | 150 us: 1.27x faster                                                            |
| go                       | 146 ms                                                          | 116 ms: 1.25x faster                                                            |
| sqlite_synth             | 2.29 us                                                         | 1.84 us: 1.25x faster                                                           |
| coroutines               | 17.9 ms                                                         | 14.4 ms: 1.24x faster                                                           |
| pycparser                | 1.04 sec                                                        | 843 ms: 1.24x faster                                                            |
| tornado_http             | 118 ms                                                          | 95.7 ms: 1.23x faster                                                           |
| asyncio_tcp              | 744 ms                                                          | 609 ms: 1.22x faster                                                            |
| comprehensions           | 17.7 us                                                         | 14.7 us: 1.21x faster                                                           |
| chaos                    | 74.4 ms                                                         | 61.8 ms: 1.20x faster                                                           |
| tomli_loads              | 1.91 sec                                                        | 1.59 sec: 1.20x faster                                                          |
| mako                     | 9.10 ms                                                         | 7.64 ms: 1.19x faster                                                           |
| json                     | 4.76 ms                                                         | 4.08 ms: 1.17x faster                                                           |
| xml_etree_process        | 48.1 ms                                                         | 41.4 ms: 1.16x faster                                                           |
| xml_etree_parse          | 120 ms                                                          | 104 ms: 1.16x faster                                                            |
| dask                     | 341 ms                                                          | 298 ms: 1.14x faster                                                            |
| deepcopy_reduce          | 2.68 us                                                         | 2.37 us: 1.13x faster                                                           |
| deepcopy                 | 310 us                                                          | 276 us: 1.12x faster                                                            |
| regex_dna                | 131 ms                                                          | 117 ms: 1.12x faster                                                            |
| json_loads               | 22.4 us                                                         | 20.0 us: 1.12x faster                                                           |
| regex_compile            | 117 ms                                                          | 105 ms: 1.11x faster                                                            |
| sympy_sum                | 122 ms                                                          | 110 ms: 1.11x faster                                                            |
| pyflate                  | 422 ms                                                          | 383 ms: 1.10x faster                                                            |
| bench_thread_pool        | 1.12 ms                                                         | 1.02 ms: 1.10x faster                                                           |
| docutils                 | 1.95 sec                                                        | 1.78 sec: 1.09x faster                                                          |
| create_gc_cycles         | 694 us                                                          | 640 us: 1.08x faster                                                            |
| fannkuch                 | 317 ms                                                          | 293 ms: 1.08x faster                                                            |
| xml_etree_iterparse      | 70.8 ms                                                         | 65.5 ms: 1.08x faster                                                           |
| 2to3                     | 265 ms                                                          | 246 ms: 1.08x faster                                                            |
| sympy_str                | 229 ms                                                          | 214 ms: 1.07x faster                                                            |
| chameleon                | 6.42 ms                                                         | 6.02 ms: 1.07x faster                                                           |
| sympy_integrate          | 16.6 ms                                                         | 15.6 ms: 1.06x faster                                                           |
| sympy_expand             | 391 ms                                                          | 372 ms: 1.05x faster                                                            |
| sqlglot_normalize        | 230 ms                                                          | 219 ms: 1.05x faster                                                            |
| sqlglot_optimize         | 44.7 ms                                                         | 42.8 ms: 1.04x faster                                                           |
| python_startup           | 22.9 ms                                                         | 22.3 ms: 1.03x faster                                                           |
| spectral_norm            | 80.2 ms                                                         | 78.4 ms: 1.02x faster                                                           |
| xml_etree_generate       | 61.6 ms                                                         | 60.4 ms: 1.02x faster                                                           |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.19 ms: 1.02x faster                                                           |
| nqueens                  | 87.1 ms                                                         | 86.1 ms: 1.01x faster                                                           |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                                          |
| pprint_pformat           | 1.37 sec                                                        | 1.39 sec: 1.01x slower                                                          |
| regex_v8                 | 15.8 ms                                                         | 16.0 ms: 1.02x slower                                                           |
| pprint_safe_repr         | 658 ms                                                          | 674 ms: 1.02x slower                                                            |
| hexiom                   | 6.13 ms                                                         | 6.30 ms: 1.03x slower                                                           |
| unpack_sequence          | 40.0 ns                                                         | 41.2 ns: 1.03x slower                                                           |
| pathlib                  | 81.2 ms                                                         | 83.9 ms: 1.03x slower                                                           |
| meteor_contest           | 80.0 ms                                                         | 82.6 ms: 1.03x slower                                                           |
| mdp                      | 1.83 sec                                                        | 1.89 sec: 1.03x slower                                                          |
| unpickle                 | 9.82 us                                                         | 10.2 us: 1.04x slower                                                           |
| pickle                   | 7.83 us                                                         | 8.13 us: 1.04x slower                                                           |
| unpickle_list            | 2.98 us                                                         | 3.10 us: 1.04x slower                                                           |
| gc_traversal             | 1.28 ms                                                         | 1.38 ms: 1.08x slower                                                           |
| logging_format           | 7.91 us                                                         | 8.57 us: 1.08x slower                                                           |
| pickle_dict              | 18.2 us                                                         | 19.8 us: 1.08x slower                                                           |
| bench_mp_pool            | 66.4 ms                                                         | 72.0 ms: 1.08x slower                                                           |
| logging_simple           | 7.29 us                                                         | 7.97 us: 1.09x slower                                                           |
| scimark_monte_carlo      | 61.9 ms                                                         | 68.8 ms: 1.11x slower                                                           |
| python_startup_no_site   | 18.1 ms                                                         | 20.1 ms: 1.11x slower                                                           |
| regex_effbot             | 1.66 ms                                                         | 1.89 ms: 1.14x slower                                                           |
| pickle_list              | 3.22 us                                                         | 3.66 us: 1.14x slower                                                           |
| nbody                    | 79.1 ms                                                         | 90.6 ms: 1.15x slower                                                           |
| async_generators         | 241 ms                                                          | 277 ms: 1.15x slower                                                            |
| scimark_fft              | 216 ms                                                          | 251 ms: 1.16x slower                                                            |
| telco                    | 4.83 ms                                                         | 6.11 ms: 1.27x slower                                                           |
| coverage                 | 46.6 ms                                                         | 465 ms: 9.98x slower                                                            |
| Geometric mean           | (ref)                                                           | 1.12x faster                                                                    |
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, dulwich_log, flaskblogging, genshi_text, genshi_xml, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240212-3.13.0a3+-4297d73-JIT/bm-20240212-pythonperf1_win32-x86-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown