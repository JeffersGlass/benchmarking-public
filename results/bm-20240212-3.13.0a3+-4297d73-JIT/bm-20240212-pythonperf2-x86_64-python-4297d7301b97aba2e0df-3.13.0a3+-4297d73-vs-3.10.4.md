
# Results vs. 3.10.4

- fork: python
- ref: 4297d7301b97aba2e0df
- machine: linux-x86_64
- commit hash: 4297d73
- commit date: 2024-02-12
- overall geometric mean: 1.25x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 298 ms: 1.17x faster                                                         |
| chameleon      | 9.44 ms                                                      | 7.54 ms: 1.25x faster                                                        |
| docutils       | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                                       |
| tornado_http   | 157 ms                                                       | 124 ms: 1.26x faster                                                         |
| Geometric mean | (ref)                                                        | 1.22x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 431 ms: 1.61x faster                                                         |
| async_tree_memoization  | 819 ms                                                       | 547 ms: 1.50x faster                                                         |
| async_tree_io           | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 699 ms: 1.34x faster                                                         |
| Geometric mean          | (ref)                                                        | 1.48x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 81.7 ms: 1.36x faster                                                        |
| nbody          | 134 ms                                                       | 107 ms: 1.26x faster                                                         |
| pidigits       | 271 ms                                                       | 263 ms: 1.03x faster                                                         |
| Geometric mean | (ref)                                                        | 1.21x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 146 ms: 1.30x faster                                                         |
| regex_dna      | 261 ms                                                       | 240 ms: 1.09x faster                                                         |
| regex_v8       | 27.2 ms                                                      | 26.3 ms: 1.03x faster                                                        |
| regex_effbot   | 3.09 ms                                                      | 3.69 ms: 1.20x slower                                                        |
| Geometric mean | (ref)                                                        | 1.05x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 301 us: 1.51x faster                                                         |
| json_dumps           | 14.5 ms                                                      | 10.5 ms: 1.39x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 228 us: 1.37x faster                                                         |
| xml_etree_process    | 75.9 ms                                                      | 58.2 ms: 1.30x faster                                                        |
| tomli_loads          | 2.92 sec                                                     | 2.31 sec: 1.26x faster                                                       |
| json_loads           | 30.3 us                                                      | 25.2 us: 1.20x faster                                                        |
| xml_etree_generate   | 92.3 ms                                                      | 84.5 ms: 1.09x faster                                                        |
| xml_etree_parse      | 160 ms                                                       | 148 ms: 1.08x faster                                                         |
| xml_etree_iterparse  | 110 ms                                                       | 107 ms: 1.04x faster                                                         |
| pickle               | 9.89 us                                                      | 10.5 us: 1.06x slower                                                        |
| pickle_list          | 4.12 us                                                      | 4.44 us: 1.08x slower                                                        |
| unpickle             | 13.5 us                                                      | 14.8 us: 1.10x slower                                                        |
| pickle_dict          | 29.5 us                                                      | 32.7 us: 1.11x slower                                                        |
| Geometric mean       | (ref)                                                        | 1.12x faster                                                                 |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| python_startup_no_site | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.29x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 11.8 ms: 1.24x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|--------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 119 us: 4.49x faster                                                         |
| asyncio_tcp              | 779 ms                                                       | 369 ms: 2.11x faster                                                         |
| deltablue                | 7.50 ms                                                      | 3.68 ms: 2.04x faster                                                        |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.57 sec: 1.97x faster                                                       |
| raytrace                 | 489 ms                                                       | 275 ms: 1.78x faster                                                         |
| logging_silent           | 167 ns                                                       | 95.1 ns: 1.76x faster                                                        |
| scimark_lu               | 167 ms                                                       | 97.6 ms: 1.71x faster                                                        |
| generators               | 57.3 ms                                                      | 33.6 ms: 1.71x faster                                                        |
| sqlglot_parse            | 2.24 ms                                                      | 1.37 ms: 1.63x faster                                                        |
| async_tree_none          | 692 ms                                                       | 431 ms: 1.61x faster                                                         |
| richards_super           | 90.6 ms                                                      | 56.9 ms: 1.59x faster                                                        |
| go                       | 262 ms                                                       | 169 ms: 1.55x faster                                                         |
| chaos                    | 109 ms                                                       | 70.3 ms: 1.54x faster                                                        |
| pickle_pure_python       | 455 us                                                       | 301 us: 1.51x faster                                                         |
| async_tree_memoization   | 819 ms                                                       | 547 ms: 1.50x faster                                                         |
| async_tree_io            | 1.60 sec                                                     | 1.07 sec: 1.49x faster                                                       |
| sqlglot_transpile        | 2.68 ms                                                      | 1.80 ms: 1.49x faster                                                        |
| richards                 | 75.1 ms                                                      | 51.0 ms: 1.47x faster                                                        |
| crypto_pyaes             | 119 ms                                                       | 81.5 ms: 1.46x faster                                                        |
| pyflate                  | 733 ms                                                       | 521 ms: 1.41x faster                                                         |
| json_dumps               | 14.5 ms                                                      | 10.5 ms: 1.39x faster                                                        |
| scimark_monte_carlo      | 107 ms                                                       | 78.5 ms: 1.37x faster                                                        |
| unpickle_pure_python     | 312 us                                                       | 228 us: 1.37x faster                                                         |
| float                    | 111 ms                                                       | 81.7 ms: 1.36x faster                                                        |
| coroutines               | 30.3 ms                                                      | 22.4 ms: 1.35x faster                                                        |
| deepcopy_memo            | 49.8 us                                                      | 37.0 us: 1.35x faster                                                        |
| logging_simple           | 8.88 us                                                      | 6.60 us: 1.34x faster                                                        |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 699 ms: 1.34x faster                                                         |
| bench_mp_pool            | 6.37 ms                                                      | 4.77 ms: 1.34x faster                                                        |
| unpack_sequence          | 59.9 ns                                                      | 45.1 ns: 1.33x faster                                                        |
| logging_format           | 9.64 us                                                      | 7.33 us: 1.31x faster                                                        |
| xml_etree_process        | 75.9 ms                                                      | 58.2 ms: 1.30x faster                                                        |
| regex_compile            | 190 ms                                                       | 146 ms: 1.30x faster                                                         |
| comprehensions           | 26.7 us                                                      | 20.7 us: 1.29x faster                                                        |
| pycparser                | 1.67 sec                                                     | 1.31 sec: 1.28x faster                                                       |
| scimark_sor              | 180 ms                                                       | 142 ms: 1.27x faster                                                         |
| deepcopy                 | 468 us                                                       | 369 us: 1.27x faster                                                         |
| tornado_http             | 157 ms                                                       | 124 ms: 1.26x faster                                                         |
| tomli_loads              | 2.92 sec                                                     | 2.31 sec: 1.26x faster                                                       |
| nbody                    | 134 ms                                                       | 107 ms: 1.26x faster                                                         |
| chameleon                | 9.44 ms                                                      | 7.54 ms: 1.25x faster                                                        |
| pprint_pformat           | 2.15 sec                                                     | 1.72 sec: 1.25x faster                                                       |
| mako                     | 14.7 ms                                                      | 11.8 ms: 1.24x faster                                                        |
| pprint_safe_repr         | 1.05 sec                                                     | 847 ms: 1.24x faster                                                         |
| hexiom                   | 9.42 ms                                                      | 7.70 ms: 1.22x faster                                                        |
| sqlglot_normalize        | 144 ms                                                       | 119 ms: 1.21x faster                                                         |
| sympy_sum                | 193 ms                                                       | 159 ms: 1.21x faster                                                         |
| sympy_str                | 360 ms                                                       | 299 ms: 1.20x faster                                                         |
| json_loads               | 30.3 us                                                      | 25.2 us: 1.20x faster                                                        |
| deepcopy_reduce          | 4.01 us                                                      | 3.34 us: 1.20x faster                                                        |
| sympy_expand             | 600 ms                                                       | 501 ms: 1.20x faster                                                         |
| fannkuch                 | 483 ms                                                       | 406 ms: 1.19x faster                                                         |
| docutils                 | 3.41 sec                                                     | 2.88 sec: 1.19x faster                                                       |
| bench_thread_pool        | 1.14 ms                                                      | 966 us: 1.18x faster                                                         |
| nqueens                  | 115 ms                                                       | 97.4 ms: 1.18x faster                                                        |
| mdp                      | 3.01 sec                                                     | 2.56 sec: 1.18x faster                                                       |
| spectral_norm            | 139 ms                                                       | 118 ms: 1.18x faster                                                         |
| 2to3                     | 350 ms                                                       | 298 ms: 1.17x faster                                                         |
| dask                     | 472 ms                                                       | 403 ms: 1.17x faster                                                         |
| dulwich_log              | 81.1 ms                                                      | 69.3 ms: 1.17x faster                                                        |
| sympy_integrate          | 28.2 ms                                                      | 24.3 ms: 1.16x faster                                                        |
| create_gc_cycles         | 1.76 ms                                                      | 1.53 ms: 1.15x faster                                                        |
| sqlglot_optimize         | 70.1 ms                                                      | 61.1 ms: 1.15x faster                                                        |
| async_generators         | 421 ms                                                       | 370 ms: 1.14x faster                                                         |
| pathlib                  | 21.4 ms                                                      | 19.0 ms: 1.12x faster                                                        |
| json                     | 5.86 ms                                                      | 5.33 ms: 1.10x faster                                                        |
| xml_etree_generate       | 92.3 ms                                                      | 84.5 ms: 1.09x faster                                                        |
| sqlite_synth             | 2.99 us                                                      | 2.74 us: 1.09x faster                                                        |
| regex_dna                | 261 ms                                                       | 240 ms: 1.09x faster                                                         |
| xml_etree_parse          | 160 ms                                                       | 148 ms: 1.08x faster                                                         |
| meteor_contest           | 138 ms                                                       | 130 ms: 1.07x faster                                                         |
| xml_etree_iterparse      | 110 ms                                                       | 107 ms: 1.04x faster                                                         |
| regex_v8                 | 27.2 ms                                                      | 26.3 ms: 1.03x faster                                                        |
| pidigits                 | 271 ms                                                       | 263 ms: 1.03x faster                                                         |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 5.01 ms: 1.01x faster                                                        |
| pickle                   | 9.89 us                                                      | 10.5 us: 1.06x slower                                                        |
| gc_traversal             | 3.42 ms                                                      | 3.64 ms: 1.07x slower                                                        |
| pickle_list              | 4.12 us                                                      | 4.44 us: 1.08x slower                                                        |
| python_startup           | 11.5 ms                                                      | 12.6 ms: 1.10x slower                                                        |
| unpickle                 | 13.5 us                                                      | 14.8 us: 1.10x slower                                                        |
| pickle_dict              | 29.5 us                                                      | 32.7 us: 1.11x slower                                                        |
| telco                    | 7.23 ms                                                      | 8.15 ms: 1.13x slower                                                        |
| regex_effbot             | 3.09 ms                                                      | 3.69 ms: 1.20x slower                                                        |
| coverage                 | 63.3 ms                                                      | 81.8 ms: 1.29x slower                                                        |
| python_startup_no_site   | 7.33 ms                                                      | 11.1 ms: 1.51x slower                                                        |
| Geometric mean           | (ref)                                                        | 1.25x faster                                                                 |

Benchmark hidden because not significant (4): mypy2, asyncio_websockets, scimark_fft, unpickle_list
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240212-3.13.0a3+-4297d73-JIT/bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: 1.10x