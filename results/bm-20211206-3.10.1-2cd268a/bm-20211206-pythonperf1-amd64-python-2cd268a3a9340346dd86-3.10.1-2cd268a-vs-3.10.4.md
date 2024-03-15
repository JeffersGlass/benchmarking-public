
# Results vs. 3.10.4

- fork: python
- ref: 2cd268a3a9340346dd86
- machine: windows-amd64
- commit hash: 2cd268a
- commit date: 2021-12-06
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.95%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 232 ms: 1.06x faster                                                     |
| chameleon      | 5.79 ms                                                     | 5.89 ms: 1.02x slower                                                    |
| docutils       | 1.92 sec                                                    | 1.88 sec: 1.02x faster                                                   |
| html5lib       | 51.0 ms                                                     | 48.7 ms: 1.05x faster                                                    |
| Geometric mean | (ref)                                                       | 1.02x faster                                                             |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_memoization  | 526 ms                                                      | 484 ms: 1.09x faster                                                     |
| async_tree_io           | 1.11 sec                                                    | 1.03 sec: 1.08x faster                                                   |
| async_tree_none         | 435 ms                                                      | 417 ms: 1.04x faster                                                     |
| async_tree_cpu_io_mixed | 638 ms                                                      | 615 ms: 1.04x faster                                                     |
| Geometric mean          | (ref)                                                       | 1.06x faster                                                             |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| nbody          | 71.3 ms                                                     | 77.2 ms: 1.08x slower                                                    |
| Geometric mean | (ref)                                                       | 1.03x slower                                                             |

Benchmark hidden because not significant (2): pidigits, float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 129 ms: 1.05x faster                                                     |
| regex_v8       | 15.4 ms                                                     | 15.0 ms: 1.03x faster                                                    |
| regex_compile  | 106 ms                                                      | 103 ms: 1.03x faster                                                     |
| regex_effbot   | 1.66 ms                                                     | 1.74 ms: 1.05x slower                                                    |
| Geometric mean | (ref)                                                       | 1.02x faster                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| unpickle             | 9.09 us                                                     | 8.17 us: 1.11x faster                                                    |
| json_dumps           | 9.16 ms                                                     | 8.45 ms: 1.08x faster                                                    |
| unpickle_pure_python | 183 us                                                      | 177 us: 1.04x faster                                                     |
| unpickle_list        | 2.71 us                                                     | 2.64 us: 1.03x faster                                                    |
| pickle_list          | 2.75 us                                                     | 2.70 us: 1.02x faster                                                    |
| pickle_dict          | 17.2 us                                                     | 17.0 us: 1.01x faster                                                    |
| xml_etree_generate   | 55.5 ms                                                     | 55.0 ms: 1.01x faster                                                    |
| pickle_pure_python   | 270 us                                                      | 267 us: 1.01x faster                                                     |
| xml_etree_process    | 44.5 ms                                                     | 44.0 ms: 1.01x faster                                                    |
| xml_etree_parse      | 96.8 ms                                                     | 98.0 ms: 1.01x slower                                                    |
| json_loads           | 14.0 us                                                     | 15.0 us: 1.07x slower                                                    |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                             |

Benchmark hidden because not significant (2): xml_etree_iterparse, pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.7 ms: 1.05x faster                                                    |
| python_startup_no_site | 15.5 ms                                                     | 15.1 ms: 1.03x faster                                                    |
| Geometric mean         | (ref)                                                       | 1.04x faster                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|-----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 8.56 ms: 1.06x faster                                                    |
| django_template | 28.9 ms                                                     | 29.2 ms: 1.01x slower                                                    |
| Geometric mean  | (ref)                                                       | 1.02x faster                                                             |

Benchmark hidden because not significant (2): genshi_text, genshi_xml

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| unpickle                | 9.09 us                                                     | 8.17 us: 1.11x faster                                                    |
| async_tree_memoization  | 526 ms                                                      | 484 ms: 1.09x faster                                                     |
| json_dumps              | 9.16 ms                                                     | 8.45 ms: 1.08x faster                                                    |
| pycparser               | 930 ms                                                      | 861 ms: 1.08x faster                                                     |
| async_tree_io           | 1.11 sec                                                    | 1.03 sec: 1.08x faster                                                   |
| hexiom                  | 5.74 ms                                                     | 5.42 ms: 1.06x faster                                                    |
| 2to3                    | 246 ms                                                      | 232 ms: 1.06x faster                                                     |
| mako                    | 9.03 ms                                                     | 8.56 ms: 1.06x faster                                                    |
| generators              | 32.4 ms                                                     | 30.7 ms: 1.05x faster                                                    |
| regex_dna               | 136 ms                                                      | 129 ms: 1.05x faster                                                     |
| sqlalchemy_declarative  | 103 ms                                                      | 98.4 ms: 1.05x faster                                                    |
| html5lib                | 51.0 ms                                                     | 48.7 ms: 1.05x faster                                                    |
| python_startup          | 20.6 ms                                                     | 19.7 ms: 1.05x faster                                                    |
| async_tree_none         | 435 ms                                                      | 417 ms: 1.04x faster                                                     |
| comprehensions          | 16.5 us                                                     | 15.8 us: 1.04x faster                                                    |
| chaos                   | 61.7 ms                                                     | 59.4 ms: 1.04x faster                                                    |
| create_gc_cycles        | 800 us                                                      | 770 us: 1.04x faster                                                     |
| richards                | 42.4 ms                                                     | 40.9 ms: 1.04x faster                                                    |
| meteor_contest          | 75.9 ms                                                     | 73.2 ms: 1.04x faster                                                    |
| dulwich_log             | 50.5 ms                                                     | 48.7 ms: 1.04x faster                                                    |
| pyflate                 | 409 ms                                                      | 394 ms: 1.04x faster                                                     |
| async_tree_cpu_io_mixed | 638 ms                                                      | 615 ms: 1.04x faster                                                     |
| unpickle_pure_python    | 183 us                                                      | 177 us: 1.04x faster                                                     |
| mdp                     | 1.78 sec                                                    | 1.72 sec: 1.03x faster                                                   |
| sqlite_synth            | 1.91 us                                                     | 1.85 us: 1.03x faster                                                    |
| regex_v8                | 15.4 ms                                                     | 15.0 ms: 1.03x faster                                                    |
| regex_compile           | 106 ms                                                      | 103 ms: 1.03x faster                                                     |
| scimark_lu              | 85.8 ms                                                     | 83.4 ms: 1.03x faster                                                    |
| unpickle_list           | 2.71 us                                                     | 2.64 us: 1.03x faster                                                    |
| bench_mp_pool           | 62.0 ms                                                     | 60.4 ms: 1.03x faster                                                    |
| sympy_integrate         | 15.3 ms                                                     | 14.9 ms: 1.03x faster                                                    |
| gc_traversal            | 1.41 ms                                                     | 1.37 ms: 1.03x faster                                                    |
| python_startup_no_site  | 15.5 ms                                                     | 15.1 ms: 1.03x faster                                                    |
| sympy_sum               | 107 ms                                                      | 104 ms: 1.03x faster                                                     |
| deepcopy_reduce         | 2.20 us                                                     | 2.15 us: 1.02x faster                                                    |
| docutils                | 1.92 sec                                                    | 1.88 sec: 1.02x faster                                                   |
| pylint                  | 350 ms                                                      | 343 ms: 1.02x faster                                                     |
| telco                   | 3.94 ms                                                     | 3.86 ms: 1.02x faster                                                    |
| pickle_list             | 2.75 us                                                     | 2.70 us: 1.02x faster                                                    |
| sqlglot_transpile       | 1.48 ms                                                     | 1.45 ms: 1.02x faster                                                    |
| sympy_str               | 194 ms                                                      | 191 ms: 1.02x faster                                                     |
| nqueens                 | 66.6 ms                                                     | 65.5 ms: 1.02x faster                                                    |
| sqlglot_optimize        | 39.8 ms                                                     | 39.2 ms: 1.02x faster                                                    |
| deltablue               | 4.19 ms                                                     | 4.13 ms: 1.01x faster                                                    |
| pickle_dict             | 17.2 us                                                     | 17.0 us: 1.01x faster                                                    |
| sqlglot_normalize       | 205 ms                                                      | 203 ms: 1.01x faster                                                     |
| go                      | 139 ms                                                      | 137 ms: 1.01x faster                                                     |
| xml_etree_generate      | 55.5 ms                                                     | 55.0 ms: 1.01x faster                                                    |
| pickle_pure_python      | 270 us                                                      | 267 us: 1.01x faster                                                     |
| xml_etree_process       | 44.5 ms                                                     | 44.0 ms: 1.01x faster                                                    |
| scimark_monte_carlo     | 57.3 ms                                                     | 56.9 ms: 1.01x faster                                                    |
| sqlglot_parse           | 1.22 ms                                                     | 1.21 ms: 1.01x faster                                                    |
| coverage                | 39.0 ms                                                     | 38.8 ms: 1.00x faster                                                    |
| sympy_expand            | 314 ms                                                      | 316 ms: 1.00x slower                                                     |
| flaskblogging           | 2.03 sec                                                    | 2.04 sec: 1.01x slower                                                   |
| async_generators        | 222 ms                                                      | 224 ms: 1.01x slower                                                     |
| django_template         | 28.9 ms                                                     | 29.2 ms: 1.01x slower                                                    |
| thrift                  | 617 us                                                      | 625 us: 1.01x slower                                                     |
| xml_etree_parse         | 96.8 ms                                                     | 98.0 ms: 1.01x slower                                                    |
| pprint_safe_repr        | 592 ms                                                      | 601 ms: 1.02x slower                                                     |
| chameleon               | 5.79 ms                                                     | 5.89 ms: 1.02x slower                                                    |
| dask                    | 313 ms                                                      | 319 ms: 1.02x slower                                                     |
| pprint_pformat          | 1.22 sec                                                    | 1.24 sec: 1.02x slower                                                   |
| unpack_sequence         | 39.6 ns                                                     | 40.5 ns: 1.02x slower                                                    |
| spectral_norm           | 77.3 ms                                                     | 79.4 ms: 1.03x slower                                                    |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.80 ms: 1.03x slower                                                    |
| logging_silent          | 94.6 ns                                                     | 98.0 ns: 1.04x slower                                                    |
| fannkuch                | 256 ms                                                      | 266 ms: 1.04x slower                                                     |
| scimark_fft             | 187 ms                                                      | 195 ms: 1.04x slower                                                     |
| crypto_pyaes            | 62.5 ms                                                     | 65.5 ms: 1.05x slower                                                    |
| regex_effbot            | 1.66 ms                                                     | 1.74 ms: 1.05x slower                                                    |
| json_loads              | 14.0 us                                                     | 15.0 us: 1.07x slower                                                    |
| nbody                   | 71.3 ms                                                     | 77.2 ms: 1.08x slower                                                    |
| Geometric mean          | (ref)                                                       | 1.01x faster                                                             |

Benchmark hidden because not significant (20): asyncio_tcp, genshi_text, coroutines, xml_etree_iterparse, logging_format, aiohttp, genshi_xml, deepcopy, sqlalchemy_imperative, scimark_sor, json, raytrace, deepcopy_memo, pickle, pidigits, float, logging_simple, pathlib, bench_thread_pool, tornado_http
Ignored benchmarks (5) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 99.95% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown