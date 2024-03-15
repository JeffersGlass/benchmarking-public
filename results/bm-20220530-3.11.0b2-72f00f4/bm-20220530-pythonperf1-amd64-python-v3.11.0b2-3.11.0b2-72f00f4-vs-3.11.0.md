
# Results vs. 3.11.0

- fork: python
- ref: v3.11.0b2
- machine: windows-amd64
- commit hash: 72f00f4
- commit date: 2022-05-30
- overall geometric mean: 1.03x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 211 ms: 1.01x faster                                            |
| chameleon      | 5.26 ms                                                     | 5.59 ms: 1.06x slower                                           |
| docutils       | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                          |
| html5lib       | 38.9 ms                                                     | 41.4 ms: 1.07x slower                                           |
| tornado_http   | 92.8 ms                                                     | 95.3 ms: 1.03x slower                                           |
| Geometric mean | (ref)                                                       | 1.03x slower                                                    |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 530 ms                                                      | 520 ms: 1.02x faster                                            |
| async_tree_io           | 808 ms                                                      | 794 ms: 1.02x faster                                            |
| async_tree_none         | 332 ms                                                      | 336 ms: 1.01x slower                                            |
| Geometric mean          | (ref)                                                       | 1.01x faster                                                    |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 153 ms: 1.02x slower                                            |
| Geometric mean | (ref)                                                       | 1.01x slower                                                    |

Benchmark hidden because not significant (2): nbody, float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_effbot   | 1.50 ms                                                     | 1.39 ms: 1.08x faster                                           |
| regex_v8       | 14.2 ms                                                     | 14.4 ms: 1.02x slower                                           |
| regex_dna      | 116 ms                                                      | 120 ms: 1.03x slower                                            |
| regex_compile  | 91.0 ms                                                     | 97.0 ms: 1.07x slower                                           |
| Geometric mean | (ref)                                                       | 1.01x slower                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle_dict          | 18.5 us                                                     | 17.4 us: 1.06x faster                                           |
| xml_etree_iterparse  | 65.6 ms                                                     | 62.0 ms: 1.06x faster                                           |
| pickle_list          | 2.70 us                                                     | 2.64 us: 1.02x faster                                           |
| json_dumps           | 8.09 ms                                                     | 8.21 ms: 1.01x slower                                           |
| pickle               | 6.64 us                                                     | 6.74 us: 1.02x slower                                           |
| xml_etree_generate   | 52.5 ms                                                     | 54.1 ms: 1.03x slower                                           |
| pickle_pure_python   | 208 us                                                      | 216 us: 1.04x slower                                            |
| unpickle_pure_python | 157 us                                                      | 164 us: 1.05x slower                                            |
| xml_etree_process    | 37.2 ms                                                     | 39.1 ms: 1.05x slower                                           |
| unpickle             | 7.57 us                                                     | 8.07 us: 1.07x slower                                           |
| unpickle_list        | 2.59 us                                                     | 2.76 us: 1.07x slower                                           |
| json_loads           | 13.0 us                                                     | 14.1 us: 1.08x slower                                           |
| Geometric mean       | (ref)                                                       | 1.02x slower                                                    |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.8 ms: 1.06x faster                                           |
| python_startup         | 19.8 ms                                                     | 19.0 ms: 1.04x faster                                           |
| Geometric mean         | (ref)                                                       | 1.05x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 17.9 ms: 1.03x faster                                           |
| django_template | 24.4 ms                                                     | 25.1 ms: 1.03x slower                                           |
| Geometric mean  | (ref)                                                       | 1.00x slower                                                    |

Benchmark hidden because not significant (2): mako, genshi_xml

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| logging_simple          | 6.86 us                                                     | 5.94 us: 1.16x faster                                           |
| logging_format          | 7.16 us                                                     | 6.39 us: 1.12x faster                                           |
| regex_effbot            | 1.50 ms                                                     | 1.39 ms: 1.08x faster                                           |
| pickle_dict             | 18.5 us                                                     | 17.4 us: 1.06x faster                                           |
| python_startup_no_site  | 16.8 ms                                                     | 15.8 ms: 1.06x faster                                           |
| unpack_sequence         | 46.9 ns                                                     | 44.3 ns: 1.06x faster                                           |
| xml_etree_iterparse     | 65.6 ms                                                     | 62.0 ms: 1.06x faster                                           |
| create_gc_cycles        | 713 us                                                      | 675 us: 1.06x faster                                            |
| python_startup          | 19.8 ms                                                     | 19.0 ms: 1.04x faster                                           |
| sqlite_synth            | 1.77 us                                                     | 1.71 us: 1.03x faster                                           |
| genshi_text             | 18.4 ms                                                     | 17.9 ms: 1.03x faster                                           |
| sqlalchemy_declarative  | 85.6 ms                                                     | 83.2 ms: 1.03x faster                                           |
| gc_traversal            | 1.49 ms                                                     | 1.46 ms: 1.03x faster                                           |
| pickle_list             | 2.70 us                                                     | 2.64 us: 1.02x faster                                           |
| async_tree_cpu_io_mixed | 530 ms                                                      | 520 ms: 1.02x faster                                            |
| async_tree_io           | 808 ms                                                      | 794 ms: 1.02x faster                                            |
| 2to3                    | 214 ms                                                      | 211 ms: 1.01x faster                                            |
| go                      | 101 ms                                                      | 100 ms: 1.01x faster                                            |
| dulwich_log             | 46.4 ms                                                     | 46.1 ms: 1.01x faster                                           |
| telco                   | 4.06 ms                                                     | 4.05 ms: 1.00x faster                                           |
| pyflate                 | 312 ms                                                      | 314 ms: 1.01x slower                                            |
| logging_silent          | 71.8 ns                                                     | 72.2 ns: 1.01x slower                                           |
| nqueens                 | 68.3 ms                                                     | 68.9 ms: 1.01x slower                                           |
| deltablue               | 2.70 ms                                                     | 2.72 ms: 1.01x slower                                           |
| docutils                | 1.64 sec                                                    | 1.66 sec: 1.01x slower                                          |
| async_tree_none         | 332 ms                                                      | 336 ms: 1.01x slower                                            |
| sympy_integrate         | 14.0 ms                                                     | 14.2 ms: 1.01x slower                                           |
| json_dumps              | 8.09 ms                                                     | 8.21 ms: 1.01x slower                                           |
| pickle                  | 6.64 us                                                     | 6.74 us: 1.02x slower                                           |
| scimark_monte_carlo     | 45.3 ms                                                     | 46.0 ms: 1.02x slower                                           |
| regex_v8                | 14.2 ms                                                     | 14.4 ms: 1.02x slower                                           |
| bench_thread_pool       | 872 us                                                      | 889 us: 1.02x slower                                            |
| pidigits                | 150 ms                                                      | 153 ms: 1.02x slower                                            |
| pylint                  | 323 ms                                                      | 331 ms: 1.02x slower                                            |
| pprint_pformat          | 1.09 sec                                                    | 1.11 sec: 1.02x slower                                          |
| scimark_sor             | 78.1 ms                                                     | 80.0 ms: 1.02x slower                                           |
| sympy_str               | 185 ms                                                      | 190 ms: 1.03x slower                                            |
| django_template         | 24.4 ms                                                     | 25.1 ms: 1.03x slower                                           |
| sympy_sum               | 100 ms                                                      | 103 ms: 1.03x slower                                            |
| tornado_http            | 92.8 ms                                                     | 95.3 ms: 1.03x slower                                           |
| dask                    | 273 ms                                                      | 280 ms: 1.03x slower                                            |
| scimark_lu              | 62.8 ms                                                     | 64.6 ms: 1.03x slower                                           |
| regex_dna               | 116 ms                                                      | 120 ms: 1.03x slower                                            |
| xml_etree_generate      | 52.5 ms                                                     | 54.1 ms: 1.03x slower                                           |
| spectral_norm           | 68.3 ms                                                     | 70.6 ms: 1.03x slower                                           |
| pprint_safe_repr        | 529 ms                                                      | 548 ms: 1.03x slower                                            |
| pickle_pure_python      | 208 us                                                      | 216 us: 1.04x slower                                            |
| pycparser               | 720 ms                                                      | 750 ms: 1.04x slower                                            |
| coroutines              | 15.0 ms                                                     | 15.6 ms: 1.04x slower                                           |
| aiohttp                 | 883 us                                                      | 921 us: 1.04x slower                                            |
| thrift                  | 494 us                                                      | 516 us: 1.04x slower                                            |
| sympy_expand            | 299 ms                                                      | 312 ms: 1.04x slower                                            |
| unpickle_pure_python    | 157 us                                                      | 164 us: 1.05x slower                                            |
| meteor_contest          | 75.2 ms                                                     | 78.7 ms: 1.05x slower                                           |
| fannkuch                | 253 ms                                                      | 266 ms: 1.05x slower                                            |
| xml_etree_process       | 37.2 ms                                                     | 39.1 ms: 1.05x slower                                           |
| generators              | 34.0 ms                                                     | 35.7 ms: 1.05x slower                                           |
| pathlib                 | 70.9 ms                                                     | 74.8 ms: 1.06x slower                                           |
| async_generators        | 177 ms                                                      | 187 ms: 1.06x slower                                            |
| deepcopy                | 246 us                                                      | 261 us: 1.06x slower                                            |
| crypto_pyaes            | 48.9 ms                                                     | 51.8 ms: 1.06x slower                                           |
| chameleon               | 5.26 ms                                                     | 5.59 ms: 1.06x slower                                           |
| hexiom                  | 4.55 ms                                                     | 4.84 ms: 1.06x slower                                           |
| scimark_fft             | 179 ms                                                      | 191 ms: 1.06x slower                                            |
| sqlglot_normalize       | 190 ms                                                      | 203 ms: 1.06x slower                                            |
| deepcopy_reduce         | 2.06 us                                                     | 2.19 us: 1.06x slower                                           |
| unpickle                | 7.57 us                                                     | 8.07 us: 1.07x slower                                           |
| html5lib                | 38.9 ms                                                     | 41.4 ms: 1.07x slower                                           |
| regex_compile           | 91.0 ms                                                     | 97.0 ms: 1.07x slower                                           |
| unpickle_list           | 2.59 us                                                     | 2.76 us: 1.07x slower                                           |
| chaos                   | 48.4 ms                                                     | 51.8 ms: 1.07x slower                                           |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.77 ms: 1.08x slower                                           |
| json_loads              | 13.0 us                                                     | 14.1 us: 1.08x slower                                           |
| sqlglot_optimize        | 34.5 ms                                                     | 37.5 ms: 1.08x slower                                           |
| json                    | 2.98 ms                                                     | 3.23 ms: 1.09x slower                                           |
| mdp                     | 1.59 sec                                                    | 1.75 sec: 1.10x slower                                          |
| comprehensions          | 15.6 us                                                     | 18.2 us: 1.16x slower                                           |
| sqlglot_transpile       | 1.16 ms                                                     | 1.42 ms: 1.22x slower                                           |
| sqlglot_parse           | 953 us                                                      | 1.21 ms: 1.26x slower                                           |
| coverage                | 43.4 ms                                                     | 106 ms: 2.43x slower                                            |
| Geometric mean          | (ref)                                                       | 1.03x slower                                                    |

Benchmark hidden because not significant (12): xml_etree_parse, nbody, raytrace, bench_mp_pool, async_tree_memoization, sqlalchemy_imperative, float, mako, deepcopy_memo, richards, genshi_xml, asyncio_tcp
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: unknown