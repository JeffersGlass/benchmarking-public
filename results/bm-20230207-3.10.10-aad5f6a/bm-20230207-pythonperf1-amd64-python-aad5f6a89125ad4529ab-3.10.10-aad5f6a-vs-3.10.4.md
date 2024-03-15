
# Results vs. 3.10.4

- fork: python
- ref: aad5f6a89125ad4529ab
- machine: windows-amd64
- commit hash: aad5f6a
- commit date: 2023-02-07
- overall geometric mean: 1.01x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 231 ms: 1.06x faster                                                      |
| chameleon      | 5.79 ms                                                     | 5.49 ms: 1.05x faster                                                     |
| docutils       | 1.92 sec                                                    | 1.84 sec: 1.04x faster                                                    |
| html5lib       | 51.0 ms                                                     | 48.2 ms: 1.06x faster                                                     |
| Geometric mean | (ref)                                                       | 1.04x faster                                                              |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_memoization  | 526 ms                                                      | 490 ms: 1.07x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 1.05 sec: 1.06x faster                                                    |
| async_tree_none         | 435 ms                                                      | 417 ms: 1.04x faster                                                      |
| async_tree_cpu_io_mixed | 638 ms                                                      | 615 ms: 1.04x faster                                                      |
| Geometric mean          | (ref)                                                       | 1.05x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 60.6 ms: 1.02x faster                                                     |
| pidigits       | 149 ms                                                      | 148 ms: 1.01x faster                                                      |
| nbody          | 71.3 ms                                                     | 71.9 ms: 1.01x slower                                                     |
| Geometric mean | (ref)                                                       | 1.01x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 132 ms: 1.03x faster                                                      |
| regex_v8       | 15.4 ms                                                     | 15.0 ms: 1.03x faster                                                     |
| regex_compile  | 106 ms                                                      | 103 ms: 1.03x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.81 ms: 1.09x slower                                                     |
| Geometric mean | (ref)                                                       | 1.00x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| xml_etree_process    | 44.5 ms                                                     | 42.7 ms: 1.04x faster                                                     |
| xml_etree_generate   | 55.5 ms                                                     | 53.3 ms: 1.04x faster                                                     |
| json_dumps           | 9.16 ms                                                     | 8.93 ms: 1.03x faster                                                     |
| unpickle_pure_python | 183 us                                                      | 180 us: 1.02x faster                                                      |
| xml_etree_iterparse  | 65.0 ms                                                     | 64.4 ms: 1.01x faster                                                     |
| pickle_pure_python   | 270 us                                                      | 267 us: 1.01x faster                                                      |
| json_loads           | 14.0 us                                                     | 14.2 us: 1.01x slower                                                     |
| pickle               | 6.85 us                                                     | 7.00 us: 1.02x slower                                                     |
| pickle_list          | 2.75 us                                                     | 2.91 us: 1.06x slower                                                     |
| pickle_dict          | 17.2 us                                                     | 19.1 us: 1.11x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.00x slower                                                              |

Benchmark hidden because not significant (3): unpickle, xml_etree_parse, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.8 ms: 1.04x faster                                                     |
| python_startup_no_site | 15.5 ms                                                     | 15.0 ms: 1.03x faster                                                     |
| Geometric mean         | (ref)                                                       | 1.04x faster                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| genshi_text     | 19.8 ms                                                     | 18.3 ms: 1.08x faster                                                     |
| genshi_xml      | 41.0 ms                                                     | 39.0 ms: 1.05x faster                                                     |
| mako            | 9.03 ms                                                     | 8.84 ms: 1.02x faster                                                     |
| django_template | 28.9 ms                                                     | 29.2 ms: 1.01x slower                                                     |
| Geometric mean  | (ref)                                                       | 1.04x faster                                                              |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pycparser               | 930 ms                                                      | 855 ms: 1.09x faster                                                      |
| genshi_text             | 19.8 ms                                                     | 18.3 ms: 1.08x faster                                                     |
| asyncio_tcp             | 732 ms                                                      | 678 ms: 1.08x faster                                                      |
| async_tree_memoization  | 526 ms                                                      | 490 ms: 1.07x faster                                                      |
| hexiom                  | 5.74 ms                                                     | 5.38 ms: 1.07x faster                                                     |
| sqlalchemy_declarative  | 103 ms                                                      | 97.2 ms: 1.06x faster                                                     |
| 2to3                    | 246 ms                                                      | 231 ms: 1.06x faster                                                      |
| chaos                   | 61.7 ms                                                     | 58.2 ms: 1.06x faster                                                     |
| async_tree_io           | 1.11 sec                                                    | 1.05 sec: 1.06x faster                                                    |
| html5lib                | 51.0 ms                                                     | 48.2 ms: 1.06x faster                                                     |
| chameleon               | 5.79 ms                                                     | 5.49 ms: 1.05x faster                                                     |
| comprehensions          | 16.5 us                                                     | 15.7 us: 1.05x faster                                                     |
| genshi_xml              | 41.0 ms                                                     | 39.0 ms: 1.05x faster                                                     |
| async_tree_none         | 435 ms                                                      | 417 ms: 1.04x faster                                                      |
| sympy_integrate         | 15.3 ms                                                     | 14.6 ms: 1.04x faster                                                     |
| meteor_contest          | 75.9 ms                                                     | 72.9 ms: 1.04x faster                                                     |
| mdp                     | 1.78 sec                                                    | 1.71 sec: 1.04x faster                                                    |
| docutils                | 1.92 sec                                                    | 1.84 sec: 1.04x faster                                                    |
| xml_etree_process       | 44.5 ms                                                     | 42.7 ms: 1.04x faster                                                     |
| xml_etree_generate      | 55.5 ms                                                     | 53.3 ms: 1.04x faster                                                     |
| python_startup          | 20.6 ms                                                     | 19.8 ms: 1.04x faster                                                     |
| pyflate                 | 409 ms                                                      | 393 ms: 1.04x faster                                                      |
| scimark_monte_carlo     | 57.3 ms                                                     | 55.2 ms: 1.04x faster                                                     |
| async_tree_cpu_io_mixed | 638 ms                                                      | 615 ms: 1.04x faster                                                      |
| sqlglot_optimize        | 39.8 ms                                                     | 38.5 ms: 1.04x faster                                                     |
| bench_mp_pool           | 62.0 ms                                                     | 60.0 ms: 1.03x faster                                                     |
| pprint_pformat          | 1.22 sec                                                    | 1.18 sec: 1.03x faster                                                    |
| regex_dna               | 136 ms                                                      | 132 ms: 1.03x faster                                                      |
| scimark_lu              | 85.8 ms                                                     | 83.2 ms: 1.03x faster                                                     |
| python_startup_no_site  | 15.5 ms                                                     | 15.0 ms: 1.03x faster                                                     |
| create_gc_cycles        | 800 us                                                      | 776 us: 1.03x faster                                                      |
| dulwich_log             | 50.5 ms                                                     | 49.0 ms: 1.03x faster                                                     |
| regex_v8                | 15.4 ms                                                     | 15.0 ms: 1.03x faster                                                     |
| sqlite_synth            | 1.91 us                                                     | 1.86 us: 1.03x faster                                                     |
| pylint                  | 350 ms                                                      | 340 ms: 1.03x faster                                                      |
| deepcopy_reduce         | 2.20 us                                                     | 2.14 us: 1.03x faster                                                     |
| pprint_safe_repr        | 592 ms                                                      | 576 ms: 1.03x faster                                                      |
| raytrace                | 273 ms                                                      | 266 ms: 1.03x faster                                                      |
| regex_compile           | 106 ms                                                      | 103 ms: 1.03x faster                                                      |
| json_dumps              | 9.16 ms                                                     | 8.93 ms: 1.03x faster                                                     |
| json                    | 3.14 ms                                                     | 3.06 ms: 1.02x faster                                                     |
| mako                    | 9.03 ms                                                     | 8.84 ms: 1.02x faster                                                     |
| nqueens                 | 66.6 ms                                                     | 65.3 ms: 1.02x faster                                                     |
| scimark_sor             | 106 ms                                                      | 104 ms: 1.02x faster                                                      |
| thrift                  | 617 us                                                      | 605 us: 1.02x faster                                                      |
| sympy_str               | 194 ms                                                      | 191 ms: 1.02x faster                                                      |
| float                   | 61.7 ms                                                     | 60.6 ms: 1.02x faster                                                     |
| sqlglot_transpile       | 1.48 ms                                                     | 1.45 ms: 1.02x faster                                                     |
| telco                   | 3.94 ms                                                     | 3.88 ms: 1.02x faster                                                     |
| unpickle_pure_python    | 183 us                                                      | 180 us: 1.02x faster                                                      |
| aiohttp                 | 995 us                                                      | 980 us: 1.02x faster                                                      |
| sqlglot_normalize       | 205 ms                                                      | 202 ms: 1.02x faster                                                      |
| gc_traversal            | 1.41 ms                                                     | 1.40 ms: 1.01x faster                                                     |
| pathlib                 | 75.7 ms                                                     | 75.0 ms: 1.01x faster                                                     |
| xml_etree_iterparse     | 65.0 ms                                                     | 64.4 ms: 1.01x faster                                                     |
| pidigits                | 149 ms                                                      | 148 ms: 1.01x faster                                                      |
| pickle_pure_python      | 270 us                                                      | 267 us: 1.01x faster                                                      |
| coroutines              | 16.0 ms                                                     | 15.9 ms: 1.01x faster                                                     |
| sympy_sum               | 107 ms                                                      | 106 ms: 1.01x faster                                                      |
| go                      | 139 ms                                                      | 138 ms: 1.00x faster                                                      |
| sqlalchemy_imperative   | 11.4 ms                                                     | 11.5 ms: 1.01x slower                                                     |
| logging_format          | 6.76 us                                                     | 6.81 us: 1.01x slower                                                     |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                    |
| nbody                   | 71.3 ms                                                     | 71.9 ms: 1.01x slower                                                     |
| crypto_pyaes            | 62.5 ms                                                     | 63.1 ms: 1.01x slower                                                     |
| deepcopy_memo           | 28.8 us                                                     | 29.1 us: 1.01x slower                                                     |
| json_loads              | 14.0 us                                                     | 14.2 us: 1.01x slower                                                     |
| deepcopy                | 255 us                                                      | 258 us: 1.01x slower                                                      |
| django_template         | 28.9 ms                                                     | 29.2 ms: 1.01x slower                                                     |
| sqlglot_parse           | 1.22 ms                                                     | 1.23 ms: 1.01x slower                                                     |
| fannkuch                | 256 ms                                                      | 259 ms: 1.01x slower                                                      |
| pickle                  | 6.85 us                                                     | 7.00 us: 1.02x slower                                                     |
| async_generators        | 222 ms                                                      | 227 ms: 1.02x slower                                                      |
| coverage                | 39.0 ms                                                     | 40.0 ms: 1.03x slower                                                     |
| unpack_sequence         | 39.6 ns                                                     | 40.8 ns: 1.03x slower                                                     |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.82 ms: 1.04x slower                                                     |
| scimark_fft             | 187 ms                                                      | 194 ms: 1.04x slower                                                      |
| logging_simple          | 6.22 us                                                     | 6.45 us: 1.04x slower                                                     |
| logging_silent          | 94.6 ns                                                     | 99.1 ns: 1.05x slower                                                     |
| pickle_list             | 2.75 us                                                     | 2.91 us: 1.06x slower                                                     |
| spectral_norm           | 77.3 ms                                                     | 82.5 ms: 1.07x slower                                                     |
| regex_effbot            | 1.66 ms                                                     | 1.81 ms: 1.09x slower                                                     |
| pickle_dict             | 17.2 us                                                     | 19.1 us: 1.11x slower                                                     |
| Geometric mean          | (ref)                                                       | 1.01x faster                                                              |

Benchmark hidden because not significant (10): bench_thread_pool, deltablue, unpickle, richards, sympy_expand, xml_etree_parse, generators, unpickle_list, dask, tornado_http
Ignored benchmarks (5) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown