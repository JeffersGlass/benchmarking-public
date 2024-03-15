
# Results vs. 3.10.4

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: linux-x86_64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.00x slower \*
- HPT reliability: 64.62%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 350 ms: 1.00x faster                                                       |
| chameleon      | 9.44 ms                                                      | 9.41 ms: 1.00x faster                                                      |
| docutils       | 3.41 sec                                                     | 3.42 sec: 1.00x slower                                                     |
| tornado_http   | 157 ms                                                       | 150 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                        | 1.01x faster                                                               |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 1.60 sec                                                     | 1.61 sec: 1.01x slower                                                     |
| async_tree_memoization  | 819 ms                                                       | 827 ms: 1.01x slower                                                       |
| async_tree_cpu_io_mixed | 936 ms                                                       | 952 ms: 1.02x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 110 ms: 1.01x faster                                                       |
| pidigits       | 271 ms                                                       | 271 ms: 1.00x slower                                                       |
| nbody          | 134 ms                                                       | 137 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                        | 1.00x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_dna      | 261 ms                                                       | 259 ms: 1.01x faster                                                       |
| regex_v8       | 27.2 ms                                                      | 27.1 ms: 1.00x faster                                                      |
| regex_compile  | 190 ms                                                       | 191 ms: 1.01x slower                                                       |
| regex_effbot   | 3.09 ms                                                      | 3.25 ms: 1.05x slower                                                      |
| Geometric mean | (ref)                                                        | 1.01x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|---------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_list         | 4.12 us                                                      | 4.04 us: 1.02x faster                                                      |
| xml_etree_iterparse | 110 ms                                                       | 109 ms: 1.01x faster                                                       |
| unpickle_list       | 4.65 us                                                      | 4.61 us: 1.01x faster                                                      |
| json_loads          | 30.3 us                                                      | 30.2 us: 1.00x faster                                                      |
| xml_etree_generate  | 92.3 ms                                                      | 92.8 ms: 1.01x slower                                                      |
| xml_etree_process   | 75.9 ms                                                      | 76.5 ms: 1.01x slower                                                      |
| pickle              | 9.89 us                                                      | 10.1 us: 1.02x slower                                                      |
| unpickle            | 13.5 us                                                      | 14.1 us: 1.04x slower                                                      |
| pickle_dict         | 29.5 us                                                      | 31.1 us: 1.05x slower                                                      |
| Geometric mean      | (ref)                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (4): json_dumps, xml_etree_parse, pickle_pure_python, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 7.33 ms                                                      | 7.35 ms: 1.00x slower                                                      |
| python_startup         | 11.5 ms                                                      | 11.5 ms: 1.00x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.00x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_text     | 31.4 ms                                                      | 31.7 ms: 1.01x slower                                                      |
| mako            | 14.7 ms                                                      | 14.9 ms: 1.01x slower                                                      |
| django_template | 50.2 ms                                                      | 53.2 ms: 1.06x slower                                                      |
| Geometric mean  | (ref)                                                        | 1.02x slower                                                               |

Benchmark hidden because not significant (1): genshi_xml

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf2-x86_64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pyflate                 | 733 ms                                                       | 693 ms: 1.06x faster                                                       |
| tornado_http            | 157 ms                                                       | 150 ms: 1.04x faster                                                       |
| pycparser               | 1.67 sec                                                     | 1.61 sec: 1.04x faster                                                     |
| crypto_pyaes            | 119 ms                                                       | 115 ms: 1.04x faster                                                       |
| scimark_lu              | 167 ms                                                       | 161 ms: 1.03x faster                                                       |
| chaos                   | 109 ms                                                       | 105 ms: 1.03x faster                                                       |
| bench_thread_pool       | 1.14 ms                                                      | 1.10 ms: 1.03x faster                                                      |
| aiohttp                 | 1.19 ms                                                      | 1.15 ms: 1.03x faster                                                      |
| dask                    | 472 ms                                                       | 459 ms: 1.03x faster                                                       |
| gunicorn                | 1.16 ms                                                      | 1.13 ms: 1.03x faster                                                      |
| nqueens                 | 115 ms                                                       | 112 ms: 1.02x faster                                                       |
| scimark_sor             | 180 ms                                                       | 176 ms: 1.02x faster                                                       |
| pickle_list             | 4.12 us                                                      | 4.04 us: 1.02x faster                                                      |
| spectral_norm           | 139 ms                                                       | 137 ms: 1.02x faster                                                       |
| sqlglot_optimize        | 70.1 ms                                                      | 69.1 ms: 1.02x faster                                                      |
| pathlib                 | 21.4 ms                                                      | 21.0 ms: 1.01x faster                                                      |
| pprint_safe_repr        | 1.05 sec                                                     | 1.03 sec: 1.01x faster                                                     |
| fannkuch                | 483 ms                                                       | 477 ms: 1.01x faster                                                       |
| flaskblogging           | 4.39 ms                                                      | 4.33 ms: 1.01x faster                                                      |
| xml_etree_iterparse     | 110 ms                                                       | 109 ms: 1.01x faster                                                       |
| dulwich_log             | 81.1 ms                                                      | 80.1 ms: 1.01x faster                                                      |
| regex_dna               | 261 ms                                                       | 259 ms: 1.01x faster                                                       |
| logging_silent          | 167 ns                                                       | 166 ns: 1.01x faster                                                       |
| telco                   | 7.23 ms                                                      | 7.16 ms: 1.01x faster                                                      |
| float                   | 111 ms                                                       | 110 ms: 1.01x faster                                                       |
| sqlite_synth            | 2.99 us                                                      | 2.97 us: 1.01x faster                                                      |
| async_generators        | 421 ms                                                       | 418 ms: 1.01x faster                                                       |
| deltablue               | 7.50 ms                                                      | 7.44 ms: 1.01x faster                                                      |
| sqlalchemy_declarative  | 190 ms                                                       | 188 ms: 1.01x faster                                                       |
| unpickle_list           | 4.65 us                                                      | 4.61 us: 1.01x faster                                                      |
| logging_format          | 9.64 us                                                      | 9.57 us: 1.01x faster                                                      |
| json_loads              | 30.3 us                                                      | 30.2 us: 1.00x faster                                                      |
| pprint_pformat          | 2.15 sec                                                     | 2.14 sec: 1.00x faster                                                     |
| coroutines              | 30.3 ms                                                      | 30.2 ms: 1.00x faster                                                      |
| chameleon               | 9.44 ms                                                      | 9.41 ms: 1.00x faster                                                      |
| regex_v8                | 27.2 ms                                                      | 27.1 ms: 1.00x faster                                                      |
| 2to3                    | 350 ms                                                       | 350 ms: 1.00x faster                                                       |
| pidigits                | 271 ms                                                       | 271 ms: 1.00x slower                                                       |
| asyncio_tcp             | 779 ms                                                       | 781 ms: 1.00x slower                                                       |
| docutils                | 3.41 sec                                                     | 3.42 sec: 1.00x slower                                                     |
| python_startup_no_site  | 7.33 ms                                                      | 7.35 ms: 1.00x slower                                                      |
| python_startup          | 11.5 ms                                                      | 11.5 ms: 1.00x slower                                                      |
| coverage                | 63.3 ms                                                      | 63.5 ms: 1.00x slower                                                      |
| sqlglot_normalize       | 144 ms                                                       | 144 ms: 1.00x slower                                                       |
| xml_etree_generate      | 92.3 ms                                                      | 92.8 ms: 1.01x slower                                                      |
| async_tree_io           | 1.60 sec                                                     | 1.61 sec: 1.01x slower                                                     |
| xml_etree_process       | 75.9 ms                                                      | 76.5 ms: 1.01x slower                                                      |
| regex_compile           | 190 ms                                                       | 191 ms: 1.01x slower                                                       |
| sqlglot_parse           | 2.24 ms                                                      | 2.26 ms: 1.01x slower                                                      |
| generators              | 57.3 ms                                                      | 57.8 ms: 1.01x slower                                                      |
| genshi_text             | 31.4 ms                                                      | 31.7 ms: 1.01x slower                                                      |
| sympy_integrate         | 28.2 ms                                                      | 28.4 ms: 1.01x slower                                                      |
| async_tree_memoization  | 819 ms                                                       | 827 ms: 1.01x slower                                                       |
| go                      | 262 ms                                                       | 264 ms: 1.01x slower                                                       |
| pylint                  | 566 ms                                                       | 572 ms: 1.01x slower                                                       |
| sqlalchemy_imperative   | 22.7 ms                                                      | 23.0 ms: 1.01x slower                                                      |
| mako                    | 14.7 ms                                                      | 14.9 ms: 1.01x slower                                                      |
| comprehensions          | 26.7 us                                                      | 27.1 us: 1.01x slower                                                      |
| async_tree_cpu_io_mixed | 936 ms                                                       | 952 ms: 1.02x slower                                                       |
| json                    | 5.86 ms                                                      | 5.97 ms: 1.02x slower                                                      |
| sympy_str               | 360 ms                                                       | 366 ms: 1.02x slower                                                       |
| nbody                   | 134 ms                                                       | 137 ms: 1.02x slower                                                       |
| pickle                  | 9.89 us                                                      | 10.1 us: 1.02x slower                                                      |
| sympy_expand            | 600 ms                                                       | 615 ms: 1.03x slower                                                       |
| deepcopy_memo           | 49.8 us                                                      | 51.1 us: 1.03x slower                                                      |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 5.22 ms: 1.03x slower                                                      |
| scimark_monte_carlo     | 107 ms                                                       | 110 ms: 1.03x slower                                                       |
| sympy_sum               | 193 ms                                                       | 199 ms: 1.03x slower                                                       |
| create_gc_cycles        | 1.76 ms                                                      | 1.82 ms: 1.03x slower                                                      |
| mdp                     | 3.01 sec                                                     | 3.12 sec: 1.04x slower                                                     |
| unpickle                | 13.5 us                                                      | 14.1 us: 1.04x slower                                                      |
| regex_effbot            | 3.09 ms                                                      | 3.25 ms: 1.05x slower                                                      |
| pickle_dict             | 29.5 us                                                      | 31.1 us: 1.05x slower                                                      |
| django_template         | 50.2 ms                                                      | 53.2 ms: 1.06x slower                                                      |
| bench_mp_pool           | 6.37 ms                                                      | 6.82 ms: 1.07x slower                                                      |
| gc_traversal            | 3.42 ms                                                      | 3.68 ms: 1.08x slower                                                      |
| Geometric mean          | (ref)                                                        | 1.00x slower                                                               |

Benchmark hidden because not significant (18): html5lib, unpack_sequence, richards, thrift, deepcopy, json_dumps, deepcopy_reduce, scimark_fft, xml_etree_parse, pickle_pure_python, hexiom, meteor_contest, sqlglot_transpile, unpickle_pure_python, raytrace, async_tree_none, genshi_xml, logging_simple
Ignored benchmarks (6) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 64.62% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.02x