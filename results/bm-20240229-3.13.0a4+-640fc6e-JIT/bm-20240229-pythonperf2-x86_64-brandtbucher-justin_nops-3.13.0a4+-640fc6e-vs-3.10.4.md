# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_nops
- machine: linux-x86_64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.36x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 308 ms: 1.14x faster                                                      |
| chameleon      | 9.44 ms                                                      | 7.45 ms: 1.27x faster                                                     |
| docutils       | 3.41 sec                                                     | 2.91 sec: 1.17x faster                                                    |
| html5lib       | 94.6 ms                                                      | 74.4 ms: 1.27x faster                                                     |
| tornado_http   | 157 ms                                                       | 125 ms: 1.25x faster                                                      |
| Geometric mean | (ref)                                                        | 1.22x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 441 ms: 1.57x faster                                                      |
| async_tree_memoization  | 819 ms                                                       | 554 ms: 1.48x faster                                                      |
| async_tree_io           | 1.60 sec                                                     | 1.10 sec: 1.45x faster                                                    |
| async_tree_cpu_io_mixed | 936 ms                                                       | 707 ms: 1.32x faster                                                      |
| Geometric mean          | (ref)                                                        | 1.45x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 79.0 ms: 1.41x faster                                                     |
| nbody          | 134 ms                                                       | 99.1 ms: 1.35x faster                                                     |
| pidigits       | 271 ms                                                       | 262 ms: 1.03x faster                                                      |
| Geometric mean | (ref)                                                        | 1.25x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 147 ms: 1.29x faster                                                      |
| regex_dna      | 261 ms                                                       | 238 ms: 1.10x faster                                                      |
| regex_v8       | 27.2 ms                                                      | 25.0 ms: 1.09x faster                                                     |
| regex_effbot   | 3.09 ms                                                      | 3.56 ms: 1.15x slower                                                     |
| Geometric mean | (ref)                                                        | 1.07x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 319 us: 1.43x faster                                                      |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                     |
| xml_etree_process    | 75.9 ms                                                      | 57.7 ms: 1.32x faster                                                     |
| tomli_loads          | 2.92 sec                                                     | 2.22 sec: 1.31x faster                                                    |
| unpickle_pure_python | 312 us                                                       | 238 us: 1.31x faster                                                      |
| json_loads           | 30.3 us                                                      | 25.1 us: 1.21x faster                                                     |
| xml_etree_parse      | 160 ms                                                       | 143 ms: 1.12x faster                                                      |
| xml_etree_generate   | 92.3 ms                                                      | 83.5 ms: 1.11x faster                                                     |
| xml_etree_iterparse  | 110 ms                                                       | 102 ms: 1.08x faster                                                      |
| pickle_list          | 4.12 us                                                      | 4.38 us: 1.06x slower                                                     |
| pickle               | 9.89 us                                                      | 10.6 us: 1.08x slower                                                     |
| pickle_dict          | 29.5 us                                                      | 32.9 us: 1.12x slower                                                     |
| unpickle             | 13.5 us                                                      | 15.2 us: 1.12x slower                                                     |
| Geometric mean       | (ref)                                                        | 1.12x faster                                                              |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 15.5 ms: 1.35x slower                                                     |
| python_startup_no_site | 7.33 ms                                                      | 14.0 ms: 1.91x slower                                                     |
| Geometric mean         | (ref)                                                        | 1.60x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 10.1 ms: 1.46x faster                                                     |
| django_template | 50.2 ms                                                      | 40.3 ms: 1.25x faster                                                     |
| genshi_text     | 31.4 ms                                                      | 28.8 ms: 1.09x faster                                                     |
| genshi_xml      | 63.3 ms                                                      | 61.8 ms: 1.02x faster                                                     |
| Geometric mean  | (ref)                                                        | 1.19x faster                                                              |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|--------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 123 us: 4.36x faster                                                      |
| asyncio_tcp              | 779 ms                                                       | 372 ms: 2.09x faster                                                      |
| deltablue                | 7.50 ms                                                      | 3.77 ms: 1.99x faster                                                     |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.97x faster                                                    |
| logging_silent           | 167 ns                                                       | 97.4 ns: 1.72x faster                                                     |
| generators               | 57.3 ms                                                      | 34.0 ms: 1.69x faster                                                     |
| richards_super           | 90.6 ms                                                      | 56.2 ms: 1.61x faster                                                     |
| chaos                    | 109 ms                                                       | 68.3 ms: 1.59x faster                                                     |
| raytrace                 | 489 ms                                                       | 310 ms: 1.58x faster                                                      |
| pylint                   | 566 ms                                                       | 361 ms: 1.57x faster                                                      |
| async_tree_none          | 692 ms                                                       | 441 ms: 1.57x faster                                                      |
| sqlglot_parse            | 2.24 ms                                                      | 1.43 ms: 1.56x faster                                                     |
| crypto_pyaes             | 119 ms                                                       | 77.5 ms: 1.54x faster                                                     |
| go                       | 262 ms                                                       | 173 ms: 1.51x faster                                                      |
| richards                 | 75.1 ms                                                      | 50.2 ms: 1.49x faster                                                     |
| async_tree_memoization   | 819 ms                                                       | 554 ms: 1.48x faster                                                      |
| spectral_norm            | 139 ms                                                       | 94.7 ms: 1.47x faster                                                     |
| mako                     | 14.7 ms                                                      | 10.1 ms: 1.46x faster                                                     |
| async_tree_io            | 1.60 sec                                                     | 1.10 sec: 1.45x faster                                                    |
| sqlglot_transpile        | 2.68 ms                                                      | 1.86 ms: 1.44x faster                                                     |
| pickle_pure_python       | 455 us                                                       | 319 us: 1.43x faster                                                      |
| scimark_lu               | 167 ms                                                       | 118 ms: 1.41x faster                                                      |
| float                    | 111 ms                                                       | 79.0 ms: 1.41x faster                                                     |
| comprehensions           | 26.7 us                                                      | 19.2 us: 1.39x faster                                                     |
| pyflate                  | 733 ms                                                       | 528 ms: 1.39x faster                                                      |
| scimark_monte_carlo      | 107 ms                                                       | 77.9 ms: 1.38x faster                                                     |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.37x faster                                                     |
| nbody                    | 134 ms                                                       | 99.1 ms: 1.35x faster                                                     |
| coroutines               | 30.3 ms                                                      | 22.6 ms: 1.34x faster                                                     |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 707 ms: 1.32x faster                                                      |
| deepcopy_memo            | 49.8 us                                                      | 37.7 us: 1.32x faster                                                     |
| thrift                   | 1.18 ms                                                      | 891 us: 1.32x faster                                                      |
| logging_simple           | 8.88 us                                                      | 6.74 us: 1.32x faster                                                     |
| xml_etree_process        | 75.9 ms                                                      | 57.7 ms: 1.32x faster                                                     |
| tomli_loads              | 2.92 sec                                                     | 2.22 sec: 1.31x faster                                                    |
| unpickle_pure_python     | 312 us                                                       | 238 us: 1.31x faster                                                      |
| logging_format           | 9.64 us                                                      | 7.39 us: 1.30x faster                                                     |
| regex_compile            | 190 ms                                                       | 147 ms: 1.29x faster                                                      |
| pycparser                | 1.67 sec                                                     | 1.30 sec: 1.29x faster                                                    |
| html5lib                 | 94.6 ms                                                      | 74.4 ms: 1.27x faster                                                     |
| hexiom                   | 9.42 ms                                                      | 7.43 ms: 1.27x faster                                                     |
| chameleon                | 9.44 ms                                                      | 7.45 ms: 1.27x faster                                                     |
| tornado_http             | 157 ms                                                       | 125 ms: 1.25x faster                                                      |
| django_template          | 50.2 ms                                                      | 40.3 ms: 1.25x faster                                                     |
| pprint_safe_repr         | 1.05 sec                                                     | 846 ms: 1.24x faster                                                      |
| deepcopy                 | 468 us                                                       | 378 us: 1.24x faster                                                      |
| pprint_pformat           | 2.15 sec                                                     | 1.74 sec: 1.24x faster                                                    |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.18 ms: 1.22x faster                                                     |
| json_loads               | 30.3 us                                                      | 25.1 us: 1.21x faster                                                     |
| sqlglot_normalize        | 144 ms                                                       | 119 ms: 1.21x faster                                                      |
| sympy_sum                | 193 ms                                                       | 160 ms: 1.20x faster                                                      |
| fannkuch                 | 483 ms                                                       | 402 ms: 1.20x faster                                                      |
| deepcopy_reduce          | 4.01 us                                                      | 3.37 us: 1.19x faster                                                     |
| sympy_str                | 360 ms                                                       | 303 ms: 1.19x faster                                                      |
| scimark_sor              | 180 ms                                                       | 153 ms: 1.18x faster                                                      |
| docutils                 | 3.41 sec                                                     | 2.91 sec: 1.17x faster                                                    |
| sympy_expand             | 600 ms                                                       | 513 ms: 1.17x faster                                                      |
| dulwich_log              | 81.1 ms                                                      | 69.4 ms: 1.17x faster                                                     |
| mdp                      | 3.01 sec                                                     | 2.58 sec: 1.17x faster                                                    |
| bench_thread_pool        | 1.14 ms                                                      | 986 us: 1.16x faster                                                      |
| sympy_integrate          | 28.2 ms                                                      | 24.5 ms: 1.15x faster                                                     |
| create_gc_cycles         | 1.76 ms                                                      | 1.55 ms: 1.14x faster                                                     |
| 2to3                     | 350 ms                                                       | 308 ms: 1.14x faster                                                      |
| xml_etree_parse          | 160 ms                                                       | 143 ms: 1.12x faster                                                      |
| nqueens                  | 115 ms                                                       | 103 ms: 1.12x faster                                                      |
| async_generators         | 421 ms                                                       | 377 ms: 1.12x faster                                                      |
| sqlglot_optimize         | 70.1 ms                                                      | 63.3 ms: 1.11x faster                                                     |
| xml_etree_generate       | 92.3 ms                                                      | 83.5 ms: 1.11x faster                                                     |
| scimark_fft              | 361 ms                                                       | 327 ms: 1.10x faster                                                      |
| sqlite_synth             | 2.99 us                                                      | 2.71 us: 1.10x faster                                                     |
| json                     | 5.86 ms                                                      | 5.34 ms: 1.10x faster                                                     |
| regex_dna                | 261 ms                                                       | 238 ms: 1.10x faster                                                      |
| genshi_text              | 31.4 ms                                                      | 28.8 ms: 1.09x faster                                                     |
| regex_v8                 | 27.2 ms                                                      | 25.0 ms: 1.09x faster                                                     |
| pathlib                  | 21.4 ms                                                      | 19.6 ms: 1.09x faster                                                     |
| xml_etree_iterparse      | 110 ms                                                       | 102 ms: 1.08x faster                                                      |
| gunicorn                 | 1.16 ms                                                      | 1.07 ms: 1.08x faster                                                     |
| aiohttp                  | 1.19 ms                                                      | 1.11 ms: 1.07x faster                                                     |
| meteor_contest           | 138 ms                                                       | 133 ms: 1.04x faster                                                      |
| pidigits                 | 271 ms                                                       | 262 ms: 1.03x faster                                                      |
| genshi_xml               | 63.3 ms                                                      | 61.8 ms: 1.02x faster                                                     |
| unpack_sequence          | 59.9 ns                                                      | 61.0 ns: 1.02x slower                                                     |
| pickle_list              | 4.12 us                                                      | 4.38 us: 1.06x slower                                                     |
| pickle                   | 9.89 us                                                      | 10.6 us: 1.08x slower                                                     |
| gc_traversal             | 3.42 ms                                                      | 3.68 ms: 1.08x slower                                                     |
| bench_mp_pool            | 6.37 ms                                                      | 6.96 ms: 1.09x slower                                                     |
| pickle_dict              | 29.5 us                                                      | 32.9 us: 1.12x slower                                                     |
| unpickle                 | 13.5 us                                                      | 15.2 us: 1.12x slower                                                     |
| telco                    | 7.23 ms                                                      | 8.24 ms: 1.14x slower                                                     |
| regex_effbot             | 3.09 ms                                                      | 3.56 ms: 1.15x slower                                                     |
| dask                     | 472 ms                                                       | 589 ms: 1.25x slower                                                      |
| coverage                 | 63.3 ms                                                      | 80.4 ms: 1.27x slower                                                     |
| python_startup           | 11.5 ms                                                      | 15.5 ms: 1.35x slower                                                     |
| python_startup_no_site   | 7.33 ms                                                      | 14.0 ms: 1.91x slower                                                     |
| Geometric mean           | (ref)                                                        | 1.23x faster                                                              |

Benchmark hidden because not significant (3): mypy2, unpickle_list, asyncio_websockets
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-640fc6e-JIT/bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.36x