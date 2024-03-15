
# Results vs. 3.10.4

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: windows-amd64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.02x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 233 ms: 1.06x faster                                                      |
| chameleon      | 5.79 ms                                                     | 5.67 ms: 1.02x faster                                                     |
| docutils       | 1.92 sec                                                    | 1.82 sec: 1.05x faster                                                    |
| html5lib       | 51.0 ms                                                     | 45.8 ms: 1.12x faster                                                     |
| Geometric mean | (ref)                                                       | 1.05x faster                                                              |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_memoization  | 526 ms                                                      | 481 ms: 1.09x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 1.04 sec: 1.07x faster                                                    |
| async_tree_cpu_io_mixed | 638 ms                                                      | 598 ms: 1.07x faster                                                      |
| async_tree_none         | 435 ms                                                      | 414 ms: 1.05x faster                                                      |
| Geometric mean          | (ref)                                                       | 1.07x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pidigits       | 149 ms                                                      | 147 ms: 1.02x faster                                                      |
| float          | 61.7 ms                                                     | 60.7 ms: 1.02x faster                                                     |
| nbody          | 71.3 ms                                                     | 75.5 ms: 1.06x slower                                                     |
| Geometric mean | (ref)                                                       | 1.01x slower                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 129 ms: 1.06x faster                                                      |
| regex_v8       | 15.4 ms                                                     | 14.6 ms: 1.05x faster                                                     |
| regex_compile  | 106 ms                                                      | 102 ms: 1.04x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.60 ms: 1.03x faster                                                     |
| Geometric mean | (ref)                                                       | 1.05x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpickle_pure_python | 183 us                                                      | 177 us: 1.04x faster                                                      |
| json_dumps           | 9.16 ms                                                     | 8.90 ms: 1.03x faster                                                     |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.4 ms: 1.02x faster                                                     |
| xml_etree_generate   | 55.5 ms                                                     | 54.3 ms: 1.02x faster                                                     |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.02x faster                                                     |
| xml_etree_process    | 44.5 ms                                                     | 43.5 ms: 1.02x faster                                                     |
| unpickle_list        | 2.71 us                                                     | 2.66 us: 1.02x faster                                                     |
| pickle_pure_python   | 270 us                                                      | 266 us: 1.01x faster                                                      |
| pickle_list          | 2.75 us                                                     | 2.86 us: 1.04x slower                                                     |
| pickle               | 6.85 us                                                     | 7.34 us: 1.07x slower                                                     |
| pickle_dict          | 17.2 us                                                     | 18.7 us: 1.09x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.00x slower                                                              |

Benchmark hidden because not significant (2): xml_etree_parse, unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup | 20.6 ms                                                     | 21.1 ms: 1.02x slower                                                     |
| Geometric mean | (ref)                                                       | 1.01x slower                                                              |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| genshi_text    | 19.8 ms                                                     | 18.8 ms: 1.05x faster                                                     |
| genshi_xml     | 41.0 ms                                                     | 39.1 ms: 1.05x faster                                                     |
| mako           | 9.03 ms                                                     | 8.76 ms: 1.03x faster                                                     |
| Geometric mean | (ref)                                                       | 1.03x faster                                                              |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| html5lib                | 51.0 ms                                                     | 45.8 ms: 1.12x faster                                                     |
| pycparser               | 930 ms                                                      | 839 ms: 1.11x faster                                                      |
| async_tree_memoization  | 526 ms                                                      | 481 ms: 1.09x faster                                                      |
| sqlalchemy_declarative  | 103 ms                                                      | 95.8 ms: 1.08x faster                                                     |
| async_tree_io           | 1.11 sec                                                    | 1.04 sec: 1.07x faster                                                    |
| async_tree_cpu_io_mixed | 638 ms                                                      | 598 ms: 1.07x faster                                                      |
| hexiom                  | 5.74 ms                                                     | 5.40 ms: 1.06x faster                                                     |
| dulwich_log             | 50.5 ms                                                     | 47.6 ms: 1.06x faster                                                     |
| comprehensions          | 16.5 us                                                     | 15.6 us: 1.06x faster                                                     |
| regex_dna               | 136 ms                                                      | 129 ms: 1.06x faster                                                      |
| 2to3                    | 246 ms                                                      | 233 ms: 1.06x faster                                                      |
| regex_v8                | 15.4 ms                                                     | 14.6 ms: 1.05x faster                                                     |
| meteor_contest          | 75.9 ms                                                     | 72.1 ms: 1.05x faster                                                     |
| docutils                | 1.92 sec                                                    | 1.82 sec: 1.05x faster                                                    |
| genshi_text             | 19.8 ms                                                     | 18.8 ms: 1.05x faster                                                     |
| async_tree_none         | 435 ms                                                      | 414 ms: 1.05x faster                                                      |
| genshi_xml              | 41.0 ms                                                     | 39.1 ms: 1.05x faster                                                     |
| pyflate                 | 409 ms                                                      | 391 ms: 1.05x faster                                                      |
| chaos                   | 61.7 ms                                                     | 59.2 ms: 1.04x faster                                                     |
| mdp                     | 1.78 sec                                                    | 1.71 sec: 1.04x faster                                                    |
| regex_compile           | 106 ms                                                      | 102 ms: 1.04x faster                                                      |
| sqlglot_transpile       | 1.48 ms                                                     | 1.42 ms: 1.04x faster                                                     |
| richards                | 42.4 ms                                                     | 40.9 ms: 1.04x faster                                                     |
| json                    | 3.14 ms                                                     | 3.02 ms: 1.04x faster                                                     |
| sqlite_synth            | 1.91 us                                                     | 1.84 us: 1.04x faster                                                     |
| unpickle_pure_python    | 183 us                                                      | 177 us: 1.04x faster                                                      |
| aiohttp                 | 995 us                                                      | 962 us: 1.04x faster                                                      |
| sympy_integrate         | 15.3 ms                                                     | 14.8 ms: 1.03x faster                                                     |
| sqlglot_optimize        | 39.8 ms                                                     | 38.5 ms: 1.03x faster                                                     |
| regex_effbot            | 1.66 ms                                                     | 1.60 ms: 1.03x faster                                                     |
| dask                    | 313 ms                                                      | 303 ms: 1.03x faster                                                      |
| deepcopy_reduce         | 2.20 us                                                     | 2.13 us: 1.03x faster                                                     |
| sympy_str               | 194 ms                                                      | 188 ms: 1.03x faster                                                      |
| mako                    | 9.03 ms                                                     | 8.76 ms: 1.03x faster                                                     |
| bench_thread_pool       | 958 us                                                      | 928 us: 1.03x faster                                                      |
| create_gc_cycles        | 800 us                                                      | 777 us: 1.03x faster                                                      |
| json_dumps              | 9.16 ms                                                     | 8.90 ms: 1.03x faster                                                     |
| pylint                  | 350 ms                                                      | 341 ms: 1.03x faster                                                      |
| bench_mp_pool           | 62.0 ms                                                     | 60.4 ms: 1.03x faster                                                     |
| xml_etree_iterparse     | 65.0 ms                                                     | 63.4 ms: 1.02x faster                                                     |
| sqlglot_parse           | 1.22 ms                                                     | 1.19 ms: 1.02x faster                                                     |
| sympy_sum               | 107 ms                                                      | 105 ms: 1.02x faster                                                      |
| xml_etree_generate      | 55.5 ms                                                     | 54.3 ms: 1.02x faster                                                     |
| json_loads              | 14.0 us                                                     | 13.7 us: 1.02x faster                                                     |
| sqlalchemy_imperative   | 11.4 ms                                                     | 11.1 ms: 1.02x faster                                                     |
| chameleon               | 5.79 ms                                                     | 5.67 ms: 1.02x faster                                                     |
| xml_etree_process       | 44.5 ms                                                     | 43.5 ms: 1.02x faster                                                     |
| pprint_pformat          | 1.22 sec                                                    | 1.19 sec: 1.02x faster                                                    |
| unpickle_list           | 2.71 us                                                     | 2.66 us: 1.02x faster                                                     |
| coroutines              | 16.0 ms                                                     | 15.7 ms: 1.02x faster                                                     |
| deltablue               | 4.19 ms                                                     | 4.11 ms: 1.02x faster                                                     |
| sqlglot_normalize       | 205 ms                                                      | 202 ms: 1.02x faster                                                      |
| pidigits                | 149 ms                                                      | 147 ms: 1.02x faster                                                      |
| pathlib                 | 75.7 ms                                                     | 74.4 ms: 1.02x faster                                                     |
| async_generators        | 222 ms                                                      | 218 ms: 1.02x faster                                                      |
| float                   | 61.7 ms                                                     | 60.7 ms: 1.02x faster                                                     |
| scimark_lu              | 85.8 ms                                                     | 84.5 ms: 1.02x faster                                                     |
| go                      | 139 ms                                                      | 137 ms: 1.01x faster                                                      |
| pickle_pure_python      | 270 us                                                      | 266 us: 1.01x faster                                                      |
| pprint_safe_repr        | 592 ms                                                      | 584 ms: 1.01x faster                                                      |
| raytrace                | 273 ms                                                      | 271 ms: 1.01x faster                                                      |
| generators              | 32.4 ms                                                     | 32.1 ms: 1.01x faster                                                     |
| deepcopy_memo           | 28.8 us                                                     | 28.6 us: 1.01x faster                                                     |
| sympy_expand            | 314 ms                                                      | 312 ms: 1.01x faster                                                      |
| gc_traversal            | 1.41 ms                                                     | 1.42 ms: 1.00x slower                                                     |
| logging_simple          | 6.22 us                                                     | 6.28 us: 1.01x slower                                                     |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                    |
| crypto_pyaes            | 62.5 ms                                                     | 63.2 ms: 1.01x slower                                                     |
| scimark_sor             | 106 ms                                                      | 107 ms: 1.01x slower                                                      |
| nqueens                 | 66.6 ms                                                     | 67.5 ms: 1.01x slower                                                     |
| thrift                  | 617 us                                                      | 629 us: 1.02x slower                                                      |
| deepcopy                | 255 us                                                      | 260 us: 1.02x slower                                                      |
| python_startup          | 20.6 ms                                                     | 21.1 ms: 1.02x slower                                                     |
| logging_silent          | 94.6 ns                                                     | 97.2 ns: 1.03x slower                                                     |
| scimark_monte_carlo     | 57.3 ms                                                     | 58.9 ms: 1.03x slower                                                     |
| pickle_list             | 2.75 us                                                     | 2.86 us: 1.04x slower                                                     |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.83 ms: 1.04x slower                                                     |
| spectral_norm           | 77.3 ms                                                     | 81.4 ms: 1.05x slower                                                     |
| nbody                   | 71.3 ms                                                     | 75.5 ms: 1.06x slower                                                     |
| unpack_sequence         | 39.6 ns                                                     | 42.1 ns: 1.06x slower                                                     |
| pickle                  | 6.85 us                                                     | 7.34 us: 1.07x slower                                                     |
| fannkuch                | 256 ms                                                      | 276 ms: 1.08x slower                                                      |
| scimark_fft             | 187 ms                                                      | 203 ms: 1.08x slower                                                      |
| pickle_dict             | 17.2 us                                                     | 18.7 us: 1.09x slower                                                     |
| Geometric mean          | (ref)                                                       | 1.02x faster                                                              |

Benchmark hidden because not significant (9): xml_etree_parse, telco, tornado_http, logging_format, django_template, coverage, python_startup_no_site, unpickle, asyncio_tcp
Ignored benchmarks (5) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown