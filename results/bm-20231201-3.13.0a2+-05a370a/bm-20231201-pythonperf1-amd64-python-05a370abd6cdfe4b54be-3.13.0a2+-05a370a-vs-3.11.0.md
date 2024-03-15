
# Results vs. 3.11.0

- fork: python
- ref: 05a370abd6cdfe4b54be
- machine: windows-amd64
- commit hash: 05a370a
- commit date: 2023-12-01
- overall geometric mean: 1.06x faster
- HPT reliability: 99.69%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 218 ms: 1.02x slower                                                        |
| chameleon      | 5.26 ms                                                     | 5.21 ms: 1.01x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 88.4 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 276 ms: 1.20x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 465 ms: 1.14x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 352 ms: 1.13x faster                                                        |
| async_tree_io              | 808 ms                                                      | 743 ms: 1.09x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 376 ms: 1.08x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 287 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 488 ms: 1.07x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 781 ms: 1.06x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.11x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| nbody          | 70.3 ms                                                     | 75.8 ms: 1.08x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x slower                                                                |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 86.6 ms: 1.05x faster                                                       |
| regex_dna      | 116 ms                                                      | 120 ms: 1.03x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 14.7 ms: 1.04x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.58 ms: 1.06x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.86 ms: 1.38x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 142 us: 1.10x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 195 us: 1.07x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 94.7 ms: 1.03x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.2 us: 1.01x faster                                                       |
| unpickle_list        | 2.59 us                                                     | 2.66 us: 1.03x slower                                                       |
| pickle               | 6.64 us                                                     | 6.84 us: 1.03x slower                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.51 sec: 1.04x slower                                                      |
| pickle_list          | 2.70 us                                                     | 2.81 us: 1.04x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.05x slower                                                       |
| xml_etree_process    | 37.2 ms                                                     | 39.9 ms: 1.07x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 57.8 ms: 1.10x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.44 us: 1.11x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.3 ms: 1.02x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.2 ms: 1.08x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.07 ms: 1.07x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 80.1 us: 4.07x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 480 ms: 1.51x faster                                                        |
| generators                 | 34.0 ms                                                     | 23.3 ms: 1.46x faster                                                       |
| comprehensions             | 15.6 us                                                     | 11.2 us: 1.40x faster                                                       |
| json_dumps                 | 8.09 ms                                                     | 5.86 ms: 1.38x faster                                                       |
| raytrace                   | 213 ms                                                      | 173 ms: 1.23x faster                                                        |
| unpack_sequence            | 46.9 ns                                                     | 38.5 ns: 1.22x faster                                                       |
| async_tree_none            | 332 ms                                                      | 276 ms: 1.20x faster                                                        |
| deltablue                  | 2.70 ms                                                     | 2.25 ms: 1.20x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 85.1 ms: 1.18x faster                                                       |
| chaos                      | 48.4 ms                                                     | 41.3 ms: 1.17x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.38 sec: 1.16x faster                                                      |
| sqlglot_parse              | 953 us                                                      | 824 us: 1.16x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 465 ms: 1.14x faster                                                        |
| logging_silent             | 71.8 ns                                                     | 63.1 ns: 1.14x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 352 ms: 1.13x faster                                                        |
| sympy_str                  | 185 ms                                                      | 163 ms: 1.13x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.57 us: 1.13x faster                                                       |
| richards_super             | 38.7 ms                                                     | 34.7 ms: 1.12x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.05 ms: 1.11x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 142 us: 1.10x faster                                                        |
| go                         | 101 ms                                                      | 92.1 ms: 1.10x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 12.8 ms: 1.09x faster                                                       |
| async_tree_io              | 808 ms                                                      | 743 ms: 1.09x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 63.1 ms: 1.08x faster                                                       |
| mypy2                      | 459 ms                                                      | 426 ms: 1.08x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 376 ms: 1.08x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 287 ms: 1.08x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 43.2 ms: 1.07x faster                                                       |
| mako                       | 7.58 ms                                                     | 7.07 ms: 1.07x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 488 ms: 1.07x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 195 us: 1.07x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 45.8 ms: 1.07x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.90 sec: 1.07x faster                                                      |
| sympy_expand               | 299 ms                                                      | 281 ms: 1.06x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 781 ms: 1.06x faster                                                        |
| logging_simple             | 6.86 us                                                     | 6.47 us: 1.06x faster                                                       |
| hexiom                     | 4.55 ms                                                     | 4.29 ms: 1.06x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 86.6 ms: 1.05x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 88.4 ms: 1.05x faster                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 43.3 ms: 1.05x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.88 us: 1.04x faster                                                       |
| spectral_norm              | 68.3 ms                                                     | 65.6 ms: 1.04x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                                      |
| dask                       | 273 ms                                                      | 264 ms: 1.03x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 25.2 us: 1.03x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 94.7 ms: 1.03x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 61.0 ms: 1.03x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 14.6 ms: 1.02x faster                                                       |
| pyflate                    | 312 ms                                                      | 306 ms: 1.02x faster                                                        |
| pidigits                   | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| richards                   | 31.4 ms                                                     | 30.9 ms: 1.02x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 18.2 us: 1.01x faster                                                       |
| deepcopy                   | 246 us                                                      | 244 us: 1.01x faster                                                        |
| gc_traversal               | 1.49 ms                                                     | 1.48 ms: 1.01x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 188 ms: 1.01x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 5.21 ms: 1.01x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.09 sec: 1.01x slower                                                      |
| pprint_safe_repr           | 529 ms                                                      | 535 ms: 1.01x slower                                                        |
| meteor_contest             | 75.2 ms                                                     | 76.1 ms: 1.01x slower                                                       |
| 2to3                       | 214 ms                                                      | 218 ms: 1.02x slower                                                        |
| bench_mp_pool              | 63.2 ms                                                     | 64.7 ms: 1.02x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 35.4 ms: 1.02x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.3 ms: 1.02x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.66 us: 1.03x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 733 us: 1.03x slower                                                        |
| regex_dna                  | 116 ms                                                      | 120 ms: 1.03x slower                                                        |
| pickle                     | 6.64 us                                                     | 6.84 us: 1.03x slower                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 2.13 us: 1.03x slower                                                       |
| scimark_fft                | 179 ms                                                      | 186 ms: 1.04x slower                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.51 sec: 1.04x slower                                                      |
| regex_v8                   | 14.2 ms                                                     | 14.7 ms: 1.04x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.81 us: 1.04x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.6 us: 1.05x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 82.0 ms: 1.05x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.58 ms: 1.06x slower                                                       |
| coverage                   | 43.4 ms                                                     | 46.0 ms: 1.06x slower                                                       |
| xml_etree_process          | 37.2 ms                                                     | 39.9 ms: 1.07x slower                                                       |
| nbody                      | 70.3 ms                                                     | 75.8 ms: 1.08x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.2 ms: 1.08x slower                                                       |
| fannkuch                   | 253 ms                                                      | 275 ms: 1.09x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 57.8 ms: 1.10x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.44 us: 1.11x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 80.6 ms: 1.14x slower                                                       |
| pycparser                  | 720 ms                                                      | 836 ms: 1.16x slower                                                        |
| telco                      | 4.06 ms                                                     | 5.01 ms: 1.23x slower                                                       |
| async_generators           | 177 ms                                                      | 236 ms: 1.34x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                |

Benchmark hidden because not significant (5): bench_thread_pool, float, xml_etree_iterparse, scimark_sparse_mat_mult, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.69% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown