# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_arena
- machine: windows-x86
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.06x faster \*
- HPT reliability: 99.93%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| 2to3           | 265 ms                                                          | 260 ms: 1.02x faster                                                          |
| chameleon      | 6.42 ms                                                         | 5.71 ms: 1.12x faster                                                         |
| docutils       | 1.95 sec                                                        | 1.80 sec: 1.08x faster                                                        |
| html5lib       | 52.1 ms                                                         | 45.3 ms: 1.15x faster                                                         |
| tornado_http   | 118 ms                                                          | 95.9 ms: 1.23x faster                                                         |
| Geometric mean | (ref)                                                           | 1.12x faster                                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 922 ms                                                          | 518 ms: 1.78x faster                                                          |
| async_tree_none         | 394 ms                                                          | 257 ms: 1.53x faster                                                          |
| async_tree_io           | 940 ms                                                          | 621 ms: 1.52x faster                                                          |
| async_tree_memoization  | 467 ms                                                          | 320 ms: 1.46x faster                                                          |
| Geometric mean          | (ref)                                                           | 1.57x faster                                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| pidigits       | 502 ms                                                          | 198 ms: 2.54x faster                                                          |
| float          | 69.6 ms                                                         | 55.1 ms: 1.26x faster                                                         |
| nbody          | 79.1 ms                                                         | 96.5 ms: 1.22x slower                                                         |
| Geometric mean | (ref)                                                           | 1.38x faster                                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| regex_dna      | 131 ms                                                          | 116 ms: 1.12x faster                                                          |
| regex_compile  | 117 ms                                                          | 107 ms: 1.09x faster                                                          |
| regex_v8       | 15.8 ms                                                         | 16.1 ms: 1.02x slower                                                         |
| regex_effbot   | 1.66 ms                                                         | 1.88 ms: 1.13x slower                                                         |
| Geometric mean | (ref)                                                           | 1.01x faster                                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| json_dumps           | 9.82 ms                                                         | 6.87 ms: 1.43x faster                                                         |
| pickle_pure_python   | 280 us                                                          | 209 us: 1.34x faster                                                          |
| json_loads           | 22.4 us                                                         | 19.8 us: 1.13x faster                                                         |
| xml_etree_process    | 48.1 ms                                                         | 42.8 ms: 1.13x faster                                                         |
| tomli_loads          | 1.91 sec                                                        | 1.70 sec: 1.12x faster                                                        |
| unpickle_pure_python | 189 us                                                          | 171 us: 1.11x faster                                                          |
| xml_etree_parse      | 120 ms                                                          | 109 ms: 1.10x faster                                                          |
| xml_etree_iterparse  | 70.8 ms                                                         | 66.5 ms: 1.07x faster                                                         |
| unpickle_list        | 2.98 us                                                         | 2.82 us: 1.06x faster                                                         |
| pickle               | 7.83 us                                                         | 7.89 us: 1.01x slower                                                         |
| xml_etree_generate   | 61.6 ms                                                         | 62.5 ms: 1.01x slower                                                         |
| unpickle             | 9.82 us                                                         | 10.0 us: 1.02x slower                                                         |
| pickle_dict          | 18.2 us                                                         | 19.9 us: 1.09x slower                                                         |
| Geometric mean       | (ref)                                                           | 1.09x faster                                                                  |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| python_startup         | 22.9 ms                                                         | 25.7 ms: 1.12x slower                                                         |
| python_startup_no_site | 18.1 ms                                                         | 23.6 ms: 1.31x slower                                                         |
| Geometric mean         | (ref)                                                           | 1.21x slower                                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| mako            | 9.10 ms                                                         | 7.12 ms: 1.28x faster                                                         |
| django_template | 36.0 ms                                                         | 29.9 ms: 1.20x faster                                                         |
| genshi_text     | 21.0 ms                                                         | 22.5 ms: 1.07x slower                                                         |
| genshi_xml      | 46.6 ms                                                         | 50.1 ms: 1.08x slower                                                         |
| Geometric mean  | (ref)                                                           | 1.07x faster                                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|--------------------------|:---------------------------------------------------------------:|:-----------------------------------------------------------------------------:|
| typing_runtime_protocols | 396 us                                                          | 97.7 us: 4.05x faster                                                         |
| pidigits                 | 502 ms                                                          | 198 ms: 2.54x faster                                                          |
| async_tree_cpu_io_mixed  | 922 ms                                                          | 518 ms: 1.78x faster                                                          |
| pylint                   | 384 ms                                                          | 226 ms: 1.70x faster                                                          |
| logging_silent           | 97.9 ns                                                         | 59.6 ns: 1.64x faster                                                         |
| deltablue                | 4.04 ms                                                         | 2.52 ms: 1.60x faster                                                         |
| async_tree_none          | 394 ms                                                          | 257 ms: 1.53x faster                                                          |
| async_tree_io            | 940 ms                                                          | 621 ms: 1.52x faster                                                          |
| async_tree_memoization   | 467 ms                                                          | 320 ms: 1.46x faster                                                          |
| generators               | 31.6 ms                                                         | 22.1 ms: 1.43x faster                                                         |
| json_dumps               | 9.82 ms                                                         | 6.87 ms: 1.43x faster                                                         |
| sqlglot_parse            | 1.33 ms                                                         | 965 us: 1.38x faster                                                          |
| crypto_pyaes             | 81.3 ms                                                         | 60.3 ms: 1.35x faster                                                         |
| pickle_pure_python       | 280 us                                                          | 209 us: 1.34x faster                                                          |
| richards_super           | 49.9 ms                                                         | 37.7 ms: 1.32x faster                                                         |
| sqlglot_transpile        | 1.58 ms                                                         | 1.21 ms: 1.31x faster                                                         |
| mako                     | 9.10 ms                                                         | 7.12 ms: 1.28x faster                                                         |
| float                    | 69.6 ms                                                         | 55.1 ms: 1.26x faster                                                         |
| chaos                    | 74.4 ms                                                         | 59.5 ms: 1.25x faster                                                         |
| coroutines               | 17.9 ms                                                         | 14.4 ms: 1.25x faster                                                         |
| go                       | 146 ms                                                          | 118 ms: 1.24x faster                                                          |
| pycparser                | 1.04 sec                                                        | 842 ms: 1.24x faster                                                          |
| tornado_http             | 118 ms                                                          | 95.9 ms: 1.23x faster                                                         |
| deepcopy_memo            | 29.6 us                                                         | 24.4 us: 1.21x faster                                                         |
| django_template          | 36.0 ms                                                         | 29.9 ms: 1.20x faster                                                         |
| richards                 | 40.3 ms                                                         | 33.6 ms: 1.20x faster                                                         |
| sqlite_synth             | 2.29 us                                                         | 1.92 us: 1.19x faster                                                         |
| comprehensions           | 17.7 us                                                         | 14.9 us: 1.19x faster                                                         |
| scimark_sor              | 115 ms                                                          | 98.4 ms: 1.17x faster                                                         |
| html5lib                 | 52.1 ms                                                         | 45.3 ms: 1.15x faster                                                         |
| sympy_sum                | 122 ms                                                          | 107 ms: 1.15x faster                                                          |
| asyncio_tcp              | 744 ms                                                          | 649 ms: 1.15x faster                                                          |
| deepcopy_reduce          | 2.68 us                                                         | 2.36 us: 1.13x faster                                                         |
| json_loads               | 22.4 us                                                         | 19.8 us: 1.13x faster                                                         |
| xml_etree_process        | 48.1 ms                                                         | 42.8 ms: 1.13x faster                                                         |
| chameleon                | 6.42 ms                                                         | 5.71 ms: 1.12x faster                                                         |
| json                     | 4.76 ms                                                         | 4.24 ms: 1.12x faster                                                         |
| tomli_loads              | 1.91 sec                                                        | 1.70 sec: 1.12x faster                                                        |
| deepcopy                 | 310 us                                                          | 276 us: 1.12x faster                                                          |
| regex_dna                | 131 ms                                                          | 116 ms: 1.12x faster                                                          |
| pyflate                  | 422 ms                                                          | 380 ms: 1.11x faster                                                          |
| raytrace                 | 303 ms                                                          | 273 ms: 1.11x faster                                                          |
| unpickle_pure_python     | 189 us                                                          | 171 us: 1.11x faster                                                          |
| sympy_str                | 229 ms                                                          | 209 ms: 1.10x faster                                                          |
| xml_etree_parse          | 120 ms                                                          | 109 ms: 1.10x faster                                                          |
| regex_compile            | 117 ms                                                          | 107 ms: 1.09x faster                                                          |
| spectral_norm            | 80.2 ms                                                         | 74.0 ms: 1.08x faster                                                         |
| docutils                 | 1.95 sec                                                        | 1.80 sec: 1.08x faster                                                        |
| sympy_integrate          | 16.6 ms                                                         | 15.4 ms: 1.08x faster                                                         |
| bench_thread_pool        | 1.12 ms                                                         | 1.05 ms: 1.07x faster                                                         |
| sympy_expand             | 391 ms                                                          | 366 ms: 1.07x faster                                                          |
| xml_etree_iterparse      | 70.8 ms                                                         | 66.5 ms: 1.07x faster                                                         |
| unpickle_list            | 2.98 us                                                         | 2.82 us: 1.06x faster                                                         |
| create_gc_cycles         | 694 us                                                          | 658 us: 1.05x faster                                                          |
| sqlglot_normalize        | 230 ms                                                          | 221 ms: 1.04x faster                                                          |
| mdp                      | 1.83 sec                                                        | 1.75 sec: 1.04x faster                                                        |
| scimark_lu               | 89.8 ms                                                         | 87.3 ms: 1.03x faster                                                         |
| 2to3                     | 265 ms                                                          | 260 ms: 1.02x faster                                                          |
| scimark_sparse_mat_mult  | 3.24 ms                                                         | 3.18 ms: 1.02x faster                                                         |
| asyncio_tcp_ssl          | 17.0 sec                                                        | 16.8 sec: 1.01x faster                                                        |
| pickle                   | 7.83 us                                                         | 7.89 us: 1.01x slower                                                         |
| sqlglot_optimize         | 44.7 ms                                                         | 45.3 ms: 1.01x slower                                                         |
| xml_etree_generate       | 61.6 ms                                                         | 62.5 ms: 1.01x slower                                                         |
| unpickle                 | 9.82 us                                                         | 10.0 us: 1.02x slower                                                         |
| regex_v8                 | 15.8 ms                                                         | 16.1 ms: 1.02x slower                                                         |
| hexiom                   | 6.13 ms                                                         | 6.29 ms: 1.03x slower                                                         |
| pathlib                  | 81.2 ms                                                         | 84.5 ms: 1.04x slower                                                         |
| unpack_sequence          | 40.0 ns                                                         | 41.7 ns: 1.04x slower                                                         |
| scimark_monte_carlo      | 61.9 ms                                                         | 65.1 ms: 1.05x slower                                                         |
| genshi_text              | 21.0 ms                                                         | 22.5 ms: 1.07x slower                                                         |
| meteor_contest           | 80.0 ms                                                         | 85.9 ms: 1.07x slower                                                         |
| genshi_xml               | 46.6 ms                                                         | 50.1 ms: 1.08x slower                                                         |
| nqueens                  | 87.1 ms                                                         | 94.5 ms: 1.09x slower                                                         |
| fannkuch                 | 317 ms                                                          | 345 ms: 1.09x slower                                                          |
| pickle_dict              | 18.2 us                                                         | 19.9 us: 1.09x slower                                                         |
| pprint_pformat           | 1.37 sec                                                        | 1.51 sec: 1.10x slower                                                        |
| bench_mp_pool            | 66.4 ms                                                         | 73.1 ms: 1.10x slower                                                         |
| gc_traversal             | 1.28 ms                                                         | 1.41 ms: 1.10x slower                                                         |
| scimark_fft              | 216 ms                                                          | 240 ms: 1.11x slower                                                          |
| python_startup           | 22.9 ms                                                         | 25.7 ms: 1.12x slower                                                         |
| logging_format           | 7.91 us                                                         | 8.87 us: 1.12x slower                                                         |
| pprint_safe_repr         | 658 ms                                                          | 744 ms: 1.13x slower                                                          |
| regex_effbot             | 1.66 ms                                                         | 1.88 ms: 1.13x slower                                                         |
| logging_simple           | 7.29 us                                                         | 8.26 us: 1.13x slower                                                         |
| nbody                    | 79.1 ms                                                         | 96.5 ms: 1.22x slower                                                         |
| dask                     | 341 ms                                                          | 419 ms: 1.23x slower                                                          |
| async_generators         | 241 ms                                                          | 302 ms: 1.25x slower                                                          |
| python_startup_no_site   | 18.1 ms                                                         | 23.6 ms: 1.31x slower                                                         |
| telco                    | 4.83 ms                                                         | 6.35 ms: 1.32x slower                                                         |
| coverage                 | 46.6 ms                                                         | 484 ms: 10.40x slower                                                         |
| thrift                   | 902 us                                                          | 10.7 ms: 11.85x slower                                                        |
| Geometric mean           | (ref)                                                           | 1.06x faster                                                                  |

Benchmark hidden because not significant (1): pickle_list
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1_win32-x86-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dulwich_log, flaskblogging, mypy2, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-1a78317-JIT/bm-20240229-pythonperf1_win32-x86-brandtbucher-justin_arena-3.13.0a4+-1a78317.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 99.93% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown