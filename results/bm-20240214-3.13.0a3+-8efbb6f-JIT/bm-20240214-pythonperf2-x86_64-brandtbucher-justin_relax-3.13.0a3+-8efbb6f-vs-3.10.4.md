
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: 8efbb6f
- commit date: 2024-02-14
- overall geometric mean: 1.27x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: 1.12x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 300 ms: 1.17x faster                                                       |
| chameleon      | 9.44 ms                                                      | 7.20 ms: 1.31x faster                                                      |
| docutils       | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                                     |
| tornado_http   | 157 ms                                                       | 123 ms: 1.27x faster                                                       |
| Geometric mean | (ref)                                                        | 1.23x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 434 ms: 1.59x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 548 ms: 1.50x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                     |
| async_tree_cpu_io_mixed | 936 ms                                                       | 709 ms: 1.32x faster                                                       |
| Geometric mean          | (ref)                                                        | 1.47x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 78.3 ms: 1.42x faster                                                      |
| nbody          | 134 ms                                                       | 102 ms: 1.32x faster                                                       |
| pidigits       | 271 ms                                                       | 261 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                        | 1.25x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 146 ms: 1.31x faster                                                       |
| regex_dna      | 261 ms                                                       | 241 ms: 1.08x faster                                                       |
| regex_v8       | 27.2 ms                                                      | 25.7 ms: 1.05x faster                                                      |
| regex_effbot   | 3.09 ms                                                      | 3.69 ms: 1.19x slower                                                      |
| Geometric mean | (ref)                                                        | 1.06x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 306 us: 1.49x faster                                                       |
| unpickle_pure_python | 312 us                                                       | 218 us: 1.43x faster                                                       |
| json_dumps           | 14.5 ms                                                      | 10.5 ms: 1.39x faster                                                      |
| tomli_loads          | 2.92 sec                                                     | 2.22 sec: 1.31x faster                                                     |
| xml_etree_process    | 75.9 ms                                                      | 58.1 ms: 1.31x faster                                                      |
| json_loads           | 30.3 us                                                      | 25.2 us: 1.21x faster                                                      |
| xml_etree_parse      | 160 ms                                                       | 146 ms: 1.10x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 85.0 ms: 1.09x faster                                                      |
| xml_etree_iterparse  | 110 ms                                                       | 105 ms: 1.05x faster                                                       |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                      |
| pickle_list          | 4.12 us                                                      | 4.41 us: 1.07x slower                                                      |
| unpickle             | 13.5 us                                                      | 14.9 us: 1.11x slower                                                      |
| pickle_dict          | 29.5 us                                                      | 33.0 us: 1.12x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                               |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.7 ms: 1.10x slower                                                      |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.2 ms: 1.44x faster                                                      |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 116 us: 4.62x faster                                                       |
| asyncio_tcp              | 779 ms                                                       | 370 ms: 2.11x faster                                                       |
| deltablue                | 7.50 ms                                                      | 3.63 ms: 2.07x faster                                                      |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                                     |
| logging_silent           | 167 ns                                                       | 94.3 ns: 1.77x faster                                                      |
| raytrace                 | 489 ms                                                       | 278 ms: 1.76x faster                                                       |
| chaos                    | 109 ms                                                       | 62.8 ms: 1.73x faster                                                      |
| scimark_lu               | 167 ms                                                       | 97.6 ms: 1.71x faster                                                      |
| generators               | 57.3 ms                                                      | 34.0 ms: 1.69x faster                                                      |
| sqlglot_parse            | 2.24 ms                                                      | 1.39 ms: 1.60x faster                                                      |
| async_tree_none          | 692 ms                                                       | 434 ms: 1.59x faster                                                       |
| go                       | 262 ms                                                       | 167 ms: 1.57x faster                                                       |
| crypto_pyaes             | 119 ms                                                       | 77.0 ms: 1.55x faster                                                      |
| richards_super           | 90.6 ms                                                      | 59.6 ms: 1.52x faster                                                      |
| scimark_monte_carlo      | 107 ms                                                       | 71.1 ms: 1.51x faster                                                      |
| async_tree_memoization   | 819 ms                                                       | 548 ms: 1.50x faster                                                       |
| pickle_pure_python       | 455 us                                                       | 306 us: 1.49x faster                                                       |
| async_tree_io            | 1.60 sec                                                     | 1.08 sec: 1.48x faster                                                     |
| sqlglot_transpile        | 2.68 ms                                                      | 1.82 ms: 1.47x faster                                                      |
| spectral_norm            | 139 ms                                                       | 95.3 ms: 1.46x faster                                                      |
| pyflate                  | 733 ms                                                       | 508 ms: 1.44x faster                                                       |
| mako                     | 14.7 ms                                                      | 10.2 ms: 1.44x faster                                                      |
| unpickle_pure_python     | 312 us                                                       | 218 us: 1.43x faster                                                       |
| float                    | 111 ms                                                       | 78.3 ms: 1.42x faster                                                      |
| richards                 | 75.1 ms                                                      | 53.6 ms: 1.40x faster                                                      |
| comprehensions           | 26.7 us                                                      | 19.1 us: 1.40x faster                                                      |
| json_dumps               | 14.5 ms                                                      | 10.5 ms: 1.39x faster                                                      |
| logging_simple           | 8.88 us                                                      | 6.44 us: 1.38x faster                                                      |
| deepcopy_memo            | 49.8 us                                                      | 36.4 us: 1.37x faster                                                      |
| hexiom                   | 9.42 ms                                                      | 6.93 ms: 1.36x faster                                                      |
| coroutines               | 30.3 ms                                                      | 22.3 ms: 1.36x faster                                                      |
| logging_format           | 9.64 us                                                      | 7.14 us: 1.35x faster                                                      |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 709 ms: 1.32x faster                                                       |
| pprint_pformat           | 2.15 sec                                                     | 1.63 sec: 1.32x faster                                                     |
| nbody                    | 134 ms                                                       | 102 ms: 1.32x faster                                                       |
| tomli_loads              | 2.92 sec                                                     | 2.22 sec: 1.31x faster                                                     |
| chameleon                | 9.44 ms                                                      | 7.20 ms: 1.31x faster                                                      |
| pprint_safe_repr         | 1.05 sec                                                     | 801 ms: 1.31x faster                                                       |
| xml_etree_process        | 75.9 ms                                                      | 58.1 ms: 1.31x faster                                                      |
| regex_compile            | 190 ms                                                       | 146 ms: 1.31x faster                                                       |
| bench_mp_pool            | 6.37 ms                                                      | 4.92 ms: 1.29x faster                                                      |
| pycparser                | 1.67 sec                                                     | 1.31 sec: 1.28x faster                                                     |
| deepcopy                 | 468 us                                                       | 367 us: 1.27x faster                                                       |
| tornado_http             | 157 ms                                                       | 123 ms: 1.27x faster                                                       |
| scimark_sor              | 180 ms                                                       | 143 ms: 1.26x faster                                                       |
| sqlglot_normalize        | 144 ms                                                       | 116 ms: 1.24x faster                                                       |
| nqueens                  | 115 ms                                                       | 93.6 ms: 1.23x faster                                                      |
| sympy_sum                | 193 ms                                                       | 157 ms: 1.22x faster                                                       |
| deepcopy_reduce          | 4.01 us                                                      | 3.30 us: 1.22x faster                                                      |
| sympy_str                | 360 ms                                                       | 298 ms: 1.21x faster                                                       |
| json_loads               | 30.3 us                                                      | 25.2 us: 1.21x faster                                                      |
| fannkuch                 | 483 ms                                                       | 401 ms: 1.20x faster                                                       |
| sympy_expand             | 600 ms                                                       | 503 ms: 1.19x faster                                                       |
| mdp                      | 3.01 sec                                                     | 2.54 sec: 1.19x faster                                                     |
| docutils                 | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                                     |
| unpack_sequence          | 59.9 ns                                                      | 50.7 ns: 1.18x faster                                                      |
| sqlglot_optimize         | 70.1 ms                                                      | 59.7 ms: 1.18x faster                                                      |
| dulwich_log              | 81.1 ms                                                      | 69.1 ms: 1.17x faster                                                      |
| bench_thread_pool        | 1.14 ms                                                      | 972 us: 1.17x faster                                                       |
| sympy_integrate          | 28.2 ms                                                      | 24.0 ms: 1.17x faster                                                      |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.34 ms: 1.17x faster                                                      |
| dask                     | 472 ms                                                       | 404 ms: 1.17x faster                                                       |
| 2to3                     | 350 ms                                                       | 300 ms: 1.17x faster                                                       |
| async_generators         | 421 ms                                                       | 365 ms: 1.15x faster                                                       |
| create_gc_cycles         | 1.76 ms                                                      | 1.57 ms: 1.13x faster                                                      |
| pathlib                  | 21.4 ms                                                      | 19.1 ms: 1.12x faster                                                      |
| xml_etree_parse          | 160 ms                                                       | 146 ms: 1.10x faster                                                       |
| json                     | 5.86 ms                                                      | 5.36 ms: 1.09x faster                                                      |
| xml_etree_generate       | 92.3 ms                                                      | 85.0 ms: 1.09x faster                                                      |
| regex_dna                | 261 ms                                                       | 241 ms: 1.08x faster                                                       |
| sqlite_synth             | 2.99 us                                                      | 2.76 us: 1.08x faster                                                      |
| scimark_fft              | 361 ms                                                       | 335 ms: 1.08x faster                                                       |
| meteor_contest           | 138 ms                                                       | 129 ms: 1.07x faster                                                       |
| mypy2                    | 933 ms                                                       | 883 ms: 1.06x faster                                                       |
| xml_etree_iterparse      | 110 ms                                                       | 105 ms: 1.05x faster                                                       |
| regex_v8                 | 27.2 ms                                                      | 25.7 ms: 1.05x faster                                                      |
| pidigits                 | 271 ms                                                       | 261 ms: 1.04x faster                                                       |
| asyncio_websockets       | 390 ms                                                       | 386 ms: 1.01x faster                                                       |
| pickle                   | 9.89 us                                                      | 10.4 us: 1.05x slower                                                      |
| pickle_list              | 4.12 us                                                      | 4.41 us: 1.07x slower                                                      |
| python_startup           | 11.5 ms                                                      | 12.7 ms: 1.10x slower                                                      |
| unpickle                 | 13.5 us                                                      | 14.9 us: 1.11x slower                                                      |
| telco                    | 7.23 ms                                                      | 8.03 ms: 1.11x slower                                                      |
| pickle_dict              | 29.5 us                                                      | 33.0 us: 1.12x slower                                                      |
| gc_traversal             | 3.42 ms                                                      | 3.94 ms: 1.15x slower                                                      |
| regex_effbot             | 3.09 ms                                                      | 3.69 ms: 1.19x slower                                                      |
| coverage                 | 63.3 ms                                                      | 84.2 ms: 1.33x slower                                                      |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.52x slower                                                      |
| Geometric mean           | (ref)                                                        | 1.27x faster                                                               |

Benchmark hidden because not significant (1): unpickle_list
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240214-3.13.0a3+-8efbb6f-JIT/bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: 1.12x