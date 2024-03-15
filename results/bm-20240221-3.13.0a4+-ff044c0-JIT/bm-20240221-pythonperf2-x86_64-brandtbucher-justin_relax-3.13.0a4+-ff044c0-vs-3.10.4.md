
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.21x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: 1.36x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 310 ms: 1.13x faster                                                       |
| chameleon      | 9.44 ms                                                      | 7.65 ms: 1.23x faster                                                      |
| docutils       | 3.41 sec                                                     | 2.94 sec: 1.16x faster                                                     |
| tornado_http   | 157 ms                                                       | 124 ms: 1.26x faster                                                       |
| Geometric mean | (ref)                                                        | 1.20x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 443 ms: 1.56x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 555 ms: 1.48x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.09 sec: 1.46x faster                                                     |
| async_tree_cpu_io_mixed | 936 ms                                                       | 707 ms: 1.32x faster                                                       |
| Geometric mean          | (ref)                                                        | 1.45x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 80.2 ms: 1.39x faster                                                      |
| nbody          | 134 ms                                                       | 102 ms: 1.32x faster                                                       |
| pidigits       | 271 ms                                                       | 262 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                        | 1.24x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 152 ms: 1.25x faster                                                       |
| regex_dna      | 261 ms                                                       | 237 ms: 1.10x faster                                                       |
| regex_v8       | 27.2 ms                                                      | 25.5 ms: 1.07x faster                                                      |
| regex_effbot   | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                                      |
| Geometric mean | (ref)                                                        | 1.07x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 315 us: 1.45x faster                                                       |
| json_dumps           | 14.5 ms                                                      | 10.6 ms: 1.38x faster                                                      |
| unpickle_pure_python | 312 us                                                       | 240 us: 1.30x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 59.4 ms: 1.28x faster                                                      |
| tomli_loads          | 2.92 sec                                                     | 2.37 sec: 1.23x faster                                                     |
| json_loads           | 30.3 us                                                      | 24.7 us: 1.23x faster                                                      |
| xml_etree_generate   | 92.3 ms                                                      | 86.3 ms: 1.07x faster                                                      |
| xml_etree_parse      | 160 ms                                                       | 151 ms: 1.06x faster                                                       |
| xml_etree_iterparse  | 110 ms                                                       | 105 ms: 1.05x faster                                                       |
| unpickle_list        | 4.65 us                                                      | 4.68 us: 1.01x slower                                                      |
| pickle_list          | 4.12 us                                                      | 4.27 us: 1.04x slower                                                      |
| pickle               | 9.89 us                                                      | 10.3 us: 1.05x slower                                                      |
| pickle_dict          | 29.5 us                                                      | 32.2 us: 1.09x slower                                                      |
| unpickle             | 13.5 us                                                      | 14.8 us: 1.10x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.11x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 15.6 ms: 1.35x slower                                                      |
| python_startup_no_site | 7.33 ms                                                      | 14.1 ms: 1.92x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.61x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.7 ms: 1.37x faster                                                      |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 118 us: 4.55x faster                                                       |
| asyncio_tcp              | 779 ms                                                       | 372 ms: 2.10x faster                                                       |
| deltablue                | 7.50 ms                                                      | 3.75 ms: 2.00x faster                                                      |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.96x faster                                                     |
| logging_silent           | 167 ns                                                       | 100 ns: 1.67x faster                                                       |
| generators               | 57.3 ms                                                      | 34.8 ms: 1.65x faster                                                      |
| raytrace                 | 489 ms                                                       | 310 ms: 1.58x faster                                                       |
| chaos                    | 109 ms                                                       | 69.3 ms: 1.57x faster                                                      |
| async_tree_none          | 692 ms                                                       | 443 ms: 1.56x faster                                                       |
| sqlglot_parse            | 2.24 ms                                                      | 1.44 ms: 1.55x faster                                                      |
| richards_super           | 90.6 ms                                                      | 60.5 ms: 1.50x faster                                                      |
| crypto_pyaes             | 119 ms                                                       | 79.7 ms: 1.49x faster                                                      |
| async_tree_memoization   | 819 ms                                                       | 555 ms: 1.48x faster                                                       |
| async_tree_io            | 1.60 sec                                                     | 1.09 sec: 1.46x faster                                                     |
| spectral_norm            | 139 ms                                                       | 96.2 ms: 1.45x faster                                                      |
| pickle_pure_python       | 455 us                                                       | 315 us: 1.45x faster                                                       |
| go                       | 262 ms                                                       | 182 ms: 1.44x faster                                                       |
| sqlglot_transpile        | 2.68 ms                                                      | 1.87 ms: 1.43x faster                                                      |
| comprehensions           | 26.7 us                                                      | 19.1 us: 1.40x faster                                                      |
| float                    | 111 ms                                                       | 80.2 ms: 1.39x faster                                                      |
| richards                 | 75.1 ms                                                      | 54.4 ms: 1.38x faster                                                      |
| json_dumps               | 14.5 ms                                                      | 10.6 ms: 1.38x faster                                                      |
| mako                     | 14.7 ms                                                      | 10.7 ms: 1.37x faster                                                      |
| coroutines               | 30.3 ms                                                      | 22.4 ms: 1.35x faster                                                      |
| pyflate                  | 733 ms                                                       | 547 ms: 1.34x faster                                                       |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 707 ms: 1.32x faster                                                       |
| nbody                    | 134 ms                                                       | 102 ms: 1.32x faster                                                       |
| logging_simple           | 8.88 us                                                      | 6.75 us: 1.32x faster                                                      |
| unpickle_pure_python     | 312 us                                                       | 240 us: 1.30x faster                                                       |
| deepcopy_memo            | 49.8 us                                                      | 38.4 us: 1.30x faster                                                      |
| logging_format           | 9.64 us                                                      | 7.48 us: 1.29x faster                                                      |
| scimark_monte_carlo      | 107 ms                                                       | 83.6 ms: 1.29x faster                                                      |
| xml_etree_process        | 75.9 ms                                                      | 59.4 ms: 1.28x faster                                                      |
| scimark_lu               | 167 ms                                                       | 131 ms: 1.28x faster                                                       |
| tornado_http             | 157 ms                                                       | 124 ms: 1.26x faster                                                       |
| pycparser                | 1.67 sec                                                     | 1.33 sec: 1.26x faster                                                     |
| regex_compile            | 190 ms                                                       | 152 ms: 1.25x faster                                                       |
| chameleon                | 9.44 ms                                                      | 7.65 ms: 1.23x faster                                                      |
| tomli_loads              | 2.92 sec                                                     | 2.37 sec: 1.23x faster                                                     |
| json_loads               | 30.3 us                                                      | 24.7 us: 1.23x faster                                                      |
| deepcopy                 | 468 us                                                       | 386 us: 1.21x faster                                                       |
| sympy_sum                | 193 ms                                                       | 161 ms: 1.19x faster                                                       |
| hexiom                   | 9.42 ms                                                      | 7.90 ms: 1.19x faster                                                      |
| sqlglot_normalize        | 144 ms                                                       | 121 ms: 1.19x faster                                                       |
| sympy_str                | 360 ms                                                       | 303 ms: 1.19x faster                                                       |
| pprint_safe_repr         | 1.05 sec                                                     | 888 ms: 1.18x faster                                                       |
| pprint_pformat           | 2.15 sec                                                     | 1.83 sec: 1.18x faster                                                     |
| deepcopy_reduce          | 4.01 us                                                      | 3.41 us: 1.18x faster                                                      |
| dulwich_log              | 81.1 ms                                                      | 69.2 ms: 1.17x faster                                                      |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.36 ms: 1.16x faster                                                      |
| scimark_sor              | 180 ms                                                       | 155 ms: 1.16x faster                                                       |
| sympy_expand             | 600 ms                                                       | 516 ms: 1.16x faster                                                       |
| docutils                 | 3.41 sec                                                     | 2.94 sec: 1.16x faster                                                     |
| bench_thread_pool        | 1.14 ms                                                      | 994 us: 1.15x faster                                                       |
| mdp                      | 3.01 sec                                                     | 2.62 sec: 1.15x faster                                                     |
| sympy_integrate          | 28.2 ms                                                      | 24.9 ms: 1.13x faster                                                      |
| 2to3                     | 350 ms                                                       | 310 ms: 1.13x faster                                                       |
| fannkuch                 | 483 ms                                                       | 431 ms: 1.12x faster                                                       |
| pathlib                  | 21.4 ms                                                      | 19.2 ms: 1.11x faster                                                      |
| create_gc_cycles         | 1.76 ms                                                      | 1.59 ms: 1.11x faster                                                      |
| json                     | 5.86 ms                                                      | 5.30 ms: 1.11x faster                                                      |
| nqueens                  | 115 ms                                                       | 104 ms: 1.10x faster                                                       |
| regex_dna                | 261 ms                                                       | 237 ms: 1.10x faster                                                       |
| sqlglot_optimize         | 70.1 ms                                                      | 64.0 ms: 1.10x faster                                                      |
| sqlite_synth             | 2.99 us                                                      | 2.76 us: 1.09x faster                                                      |
| async_generators         | 421 ms                                                       | 390 ms: 1.08x faster                                                       |
| xml_etree_generate       | 92.3 ms                                                      | 86.3 ms: 1.07x faster                                                      |
| regex_v8                 | 27.2 ms                                                      | 25.5 ms: 1.07x faster                                                      |
| scimark_fft              | 361 ms                                                       | 339 ms: 1.07x faster                                                       |
| xml_etree_parse          | 160 ms                                                       | 151 ms: 1.06x faster                                                       |
| xml_etree_iterparse      | 110 ms                                                       | 105 ms: 1.05x faster                                                       |
| meteor_contest           | 138 ms                                                       | 133 ms: 1.04x faster                                                       |
| pidigits                 | 271 ms                                                       | 262 ms: 1.03x faster                                                       |
| unpickle_list            | 4.65 us                                                      | 4.68 us: 1.01x slower                                                      |
| pickle_list              | 4.12 us                                                      | 4.27 us: 1.04x slower                                                      |
| pickle                   | 9.89 us                                                      | 10.3 us: 1.05x slower                                                      |
| bench_mp_pool            | 6.37 ms                                                      | 6.83 ms: 1.07x slower                                                      |
| pickle_dict              | 29.5 us                                                      | 32.2 us: 1.09x slower                                                      |
| unpickle                 | 13.5 us                                                      | 14.8 us: 1.10x slower                                                      |
| regex_effbot             | 3.09 ms                                                      | 3.50 ms: 1.13x slower                                                      |
| telco                    | 7.23 ms                                                      | 8.23 ms: 1.14x slower                                                      |
| gc_traversal             | 3.42 ms                                                      | 3.95 ms: 1.16x slower                                                      |
| coverage                 | 63.3 ms                                                      | 83.7 ms: 1.32x slower                                                      |
| unpack_sequence          | 59.9 ns                                                      | 79.7 ns: 1.33x slower                                                      |
| python_startup           | 11.5 ms                                                      | 15.6 ms: 1.35x slower                                                      |
| python_startup_no_site   | 7.33 ms                                                      | 14.1 ms: 1.92x slower                                                      |
| Geometric mean           | (ref)                                                        | 1.21x faster                                                               |

Benchmark hidden because not significant (2): mypy2, asyncio_websockets
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240221-3.13.0a4+-ff044c0-JIT/bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: 1.36x