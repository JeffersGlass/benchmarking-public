
# Results vs. 3.11.0

- fork: python
- ref: v3.11.4
- machine: windows-amd64
- commit hash: d2340ef
- commit date: 2023-06-06
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.32%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 221 ms: 1.03x slower                                        |
| chameleon      | 5.26 ms                                                     | 5.44 ms: 1.03x slower                                       |
| docutils       | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                      |
| html5lib       | 38.9 ms                                                     | 39.4 ms: 1.01x slower                                       |
| tornado_http   | 92.8 ms                                                     | 103 ms: 1.11x slower                                        |
| Geometric mean | (ref)                                                       | 1.04x slower                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_memoization | 399 ms                                                      | 392 ms: 1.02x faster                                        |
| Geometric mean         | (ref)                                                       | 1.00x faster                                                |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_io, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 151 ms: 1.01x slower                                        |
| float          | 54.4 ms                                                     | 56.7 ms: 1.04x slower                                       |
| Geometric mean | (ref)                                                       | 1.02x slower                                                |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                       |
| regex_effbot   | 1.50 ms                                                     | 1.52 ms: 1.01x slower                                       |
| regex_compile  | 91.0 ms                                                     | 92.8 ms: 1.02x slower                                       |
| regex_dna      | 116 ms                                                      | 120 ms: 1.03x slower                                        |
| Geometric mean | (ref)                                                       | 1.01x slower                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle_pure_python   | 208 us                                                      | 201 us: 1.04x faster                                        |
| unpickle_pure_python | 157 us                                                      | 153 us: 1.03x faster                                        |
| json_dumps           | 8.09 ms                                                     | 7.92 ms: 1.02x faster                                       |
| tomli_loads          | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                      |
| xml_etree_parse      | 97.6 ms                                                     | 96.4 ms: 1.01x faster                                       |
| pickle               | 6.64 us                                                     | 6.74 us: 1.02x slower                                       |
| pickle_dict          | 18.5 us                                                     | 18.8 us: 1.02x slower                                       |
| xml_etree_process    | 37.2 ms                                                     | 37.9 ms: 1.02x slower                                       |
| json_loads           | 13.0 us                                                     | 13.3 us: 1.02x slower                                       |
| xml_etree_generate   | 52.5 ms                                                     | 53.8 ms: 1.02x slower                                       |
| pickle_list          | 2.70 us                                                     | 2.78 us: 1.03x slower                                       |
| unpickle_list        | 2.59 us                                                     | 2.73 us: 1.05x slower                                       |
| unpickle             | 7.57 us                                                     | 8.15 us: 1.08x slower                                       |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 17.5 ms: 1.04x slower                                       |
| python_startup         | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                       |
| Geometric mean         | (ref)                                                       | 1.04x slower                                                |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| genshi_text    | 18.4 ms                                                     | 17.8 ms: 1.04x faster                                       |
| genshi_xml     | 39.9 ms                                                     | 38.6 ms: 1.04x faster                                       |
| mako           | 7.58 ms                                                     | 7.67 ms: 1.01x slower                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| nqueens                 | 68.3 ms                                                     | 65.1 ms: 1.05x faster                                       |
| genshi_text             | 18.4 ms                                                     | 17.8 ms: 1.04x faster                                       |
| pickle_pure_python      | 208 us                                                      | 201 us: 1.04x faster                                        |
| genshi_xml              | 39.9 ms                                                     | 38.6 ms: 1.04x faster                                       |
| sqlalchemy_declarative  | 85.6 ms                                                     | 82.7 ms: 1.04x faster                                       |
| pprint_pformat          | 1.09 sec                                                    | 1.05 sec: 1.03x faster                                      |
| pprint_safe_repr        | 529 ms                                                      | 513 ms: 1.03x faster                                        |
| raytrace                | 213 ms                                                      | 208 ms: 1.03x faster                                        |
| unpickle_pure_python    | 157 us                                                      | 153 us: 1.03x faster                                        |
| logging_simple          | 6.86 us                                                     | 6.71 us: 1.02x faster                                       |
| json_dumps              | 8.09 ms                                                     | 7.92 ms: 1.02x faster                                       |
| sqlglot_parse           | 953 us                                                      | 936 us: 1.02x faster                                        |
| regex_v8                | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                       |
| async_tree_memoization  | 399 ms                                                      | 392 ms: 1.02x faster                                        |
| thrift                  | 494 us                                                      | 486 us: 1.02x faster                                        |
| scimark_sor             | 78.1 ms                                                     | 76.9 ms: 1.02x faster                                       |
| tomli_loads             | 1.46 sec                                                    | 1.43 sec: 1.02x faster                                      |
| telco                   | 4.06 ms                                                     | 4.00 ms: 1.02x faster                                       |
| deepcopy_memo           | 26.0 us                                                     | 25.6 us: 1.02x faster                                       |
| sqlglot_transpile       | 1.16 ms                                                     | 1.15 ms: 1.02x faster                                       |
| richards                | 31.4 ms                                                     | 31.0 ms: 1.01x faster                                       |
| xml_etree_parse         | 97.6 ms                                                     | 96.4 ms: 1.01x faster                                       |
| coroutines              | 15.0 ms                                                     | 14.8 ms: 1.01x faster                                       |
| sympy_integrate         | 14.0 ms                                                     | 13.9 ms: 1.01x faster                                       |
| pyflate                 | 312 ms                                                      | 310 ms: 1.01x faster                                        |
| go                      | 101 ms                                                      | 100 ms: 1.01x faster                                        |
| scimark_monte_carlo     | 45.3 ms                                                     | 45.1 ms: 1.01x faster                                       |
| sqlite_synth            | 1.77 us                                                     | 1.76 us: 1.01x faster                                       |
| deltablue               | 2.70 ms                                                     | 2.71 ms: 1.00x slower                                       |
| pidigits                | 150 ms                                                      | 151 ms: 1.01x slower                                        |
| chaos                   | 48.4 ms                                                     | 48.8 ms: 1.01x slower                                       |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                      |
| scimark_lu              | 62.8 ms                                                     | 63.4 ms: 1.01x slower                                       |
| sympy_str               | 185 ms                                                      | 187 ms: 1.01x slower                                        |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.60 ms: 1.01x slower                                       |
| regex_effbot            | 1.50 ms                                                     | 1.52 ms: 1.01x slower                                       |
| docutils                | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                      |
| mako                    | 7.58 ms                                                     | 7.67 ms: 1.01x slower                                       |
| sqlglot_normalize       | 190 ms                                                      | 193 ms: 1.01x slower                                        |
| logging_format          | 7.16 us                                                     | 7.26 us: 1.01x slower                                       |
| html5lib                | 38.9 ms                                                     | 39.4 ms: 1.01x slower                                       |
| deepcopy_reduce         | 2.06 us                                                     | 2.09 us: 1.01x slower                                       |
| generators              | 34.0 ms                                                     | 34.5 ms: 1.02x slower                                       |
| pickle                  | 6.64 us                                                     | 6.74 us: 1.02x slower                                       |
| pickle_dict             | 18.5 us                                                     | 18.8 us: 1.02x slower                                       |
| crypto_pyaes            | 48.9 ms                                                     | 49.7 ms: 1.02x slower                                       |
| gc_traversal            | 1.49 ms                                                     | 1.52 ms: 1.02x slower                                       |
| xml_etree_process       | 37.2 ms                                                     | 37.9 ms: 1.02x slower                                       |
| regex_compile           | 91.0 ms                                                     | 92.8 ms: 1.02x slower                                       |
| sqlglot_optimize        | 34.5 ms                                                     | 35.2 ms: 1.02x slower                                       |
| json_loads              | 13.0 us                                                     | 13.3 us: 1.02x slower                                       |
| scimark_fft             | 179 ms                                                      | 184 ms: 1.02x slower                                        |
| xml_etree_generate      | 52.5 ms                                                     | 53.8 ms: 1.02x slower                                       |
| pylint                  | 323 ms                                                      | 331 ms: 1.03x slower                                        |
| unpack_sequence         | 46.9 ns                                                     | 48.1 ns: 1.03x slower                                       |
| sympy_sum               | 100 ms                                                      | 103 ms: 1.03x slower                                        |
| meteor_contest          | 75.2 ms                                                     | 77.4 ms: 1.03x slower                                       |
| regex_dna               | 116 ms                                                      | 120 ms: 1.03x slower                                        |
| pickle_list             | 2.70 us                                                     | 2.78 us: 1.03x slower                                       |
| chameleon               | 5.26 ms                                                     | 5.44 ms: 1.03x slower                                       |
| 2to3                    | 214 ms                                                      | 221 ms: 1.03x slower                                        |
| create_gc_cycles        | 713 us                                                      | 740 us: 1.04x slower                                        |
| fannkuch                | 253 ms                                                      | 263 ms: 1.04x slower                                        |
| python_startup_no_site  | 16.8 ms                                                     | 17.5 ms: 1.04x slower                                       |
| async_generators        | 177 ms                                                      | 184 ms: 1.04x slower                                        |
| float                   | 54.4 ms                                                     | 56.7 ms: 1.04x slower                                       |
| python_startup          | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                       |
| bench_mp_pool           | 63.2 ms                                                     | 66.1 ms: 1.04x slower                                       |
| dask                    | 273 ms                                                      | 287 ms: 1.05x slower                                        |
| unpickle_list           | 2.59 us                                                     | 2.73 us: 1.05x slower                                       |
| aiohttp                 | 883 us                                                      | 936 us: 1.06x slower                                        |
| unpickle                | 7.57 us                                                     | 8.15 us: 1.08x slower                                       |
| bench_thread_pool       | 872 us                                                      | 941 us: 1.08x slower                                        |
| pathlib                 | 70.9 ms                                                     | 77.5 ms: 1.09x slower                                       |
| spectral_norm           | 68.3 ms                                                     | 74.7 ms: 1.09x slower                                       |
| mdp                     | 1.59 sec                                                    | 1.76 sec: 1.10x slower                                      |
| tornado_http            | 92.8 ms                                                     | 103 ms: 1.11x slower                                        |
| json                    | 2.98 ms                                                     | 3.51 ms: 1.18x slower                                       |
| asyncio_tcp_ssl         | 2.03 sec                                                    | 2.41 sec: 1.19x slower                                      |
| coverage                | 43.4 ms                                                     | 55.6 ms: 1.28x slower                                       |
| asyncio_tcp             | 726 ms                                                      | 932 ms: 1.28x slower                                        |
| Geometric mean          | (ref)                                                       | 1.02x slower                                                |

Benchmark hidden because not significant (16): async_tree_cpu_io_mixed, xml_etree_iterparse, deepcopy, richards_super, sqlalchemy_imperative, hexiom, comprehensions, dulwich_log, typing_runtime_protocols, django_template, nbody, sympy_expand, logging_silent, async_tree_io, async_tree_none, pycparser
Ignored benchmarks (5) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, mypy2


# HPT report

- Reliability score: 99.32% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown